---
title: "Endurance Storage Replication"
description: "Examples on ordering, snapshots, and replication for endurance storage. "
date: "2017-02-21"
classes: 
    - "SoftLayer_Network_Storage"
tags:
    - "endurance"
    - "replication"
    - "snapshot"
    - "storage"
    - "objectfilter"
    - "objectmask"
    - "enablesnapshots"
---

Some good starting reading.

* https://knowledgelayer.softlayer.com/procedure/endurance-replication
* https://knowledgelayer.softlayer.com/procedure/endurance-snapshots
* http://sldn.softlayer.com/reference/services/SoftLayer_Network_Storage/enableSnapshots

For more information on the magic of storage ordering see the following

* https://github.com/softlayer/softlayer-python/blob/master/SoftLayer/managers/file.py
* https://github.com/softlayer/softlayer-python/blob/master/SoftLayer/managers/storage_utils.py

This example should touch on all the basics of dealing with endurance storage replication volumes. This example uses the SoftLayer-python File manager a little bit for ordering

TO authorize hosts that are NOT virtual guests, see the allowAccessFrom* methods in 

* http://sldn.softlayer.com/reference/services/SoftLayer_Network_Storage/ 

Graceful vs Immediate failover

* http://sldn.softlayer.com/reference/services/SoftLayer_Network_Storage/immediateFailoverToReplicant
* http://sldn.softlayer.com/reference/services/SoftLayer_Network_Storage/failoverToReplicant

Failback is always immediate.

```
"""
@package examples 
@author Christopher Gallo
"""

import SoftLayer
import logging
from pprint import pprint as pp

class example():

    def __init__(self):
        """
        If you need debugging, uncomment these. be prepared for a lot of XML
        """
        # logger = logging.getLogger()
        # logger.addHandler(logging.StreamHandler())
        # logger.setLevel(3)
        self.client = SoftLayer.Client()
        self.storage = self.client['SoftLayer_Network_Storage']
        self.mgr = SoftLayer.FileStorageManager(self.client)
        # Broken up like this to look 'good' on softlayer.github.io
        self.objectMask = "mask["
            "id, username, capacityGb, bytesUsed, serviceResource[datacenter[name]], "
            "serviceResourceBackendIpAddress, activeTransactionCount, "
            "fileNetworkMountAddress, snapshots[id,createDate], hourlySchedule, " 
            "allowedReplicationVirtualGuests[hostname], allowedVirtualGuests[hostname], "
            "replicationStatus, replicationPartners]"

    def orderStorage(self):
        """
        This will order endurance storage in HOU02 with 20G in size, and the 0.25IOPS/GB tier
        0.25, 2, 4 and 10 iops/g are tiers available. 
        """
        result = self.mgr.order_file_volume(
            storage_type="storage_service_enterprise",
            location = "hou02",
            size = 20,
            tier_level = 0.25
            )
        pp(result)

    def orderSnapshot(self, volume_id):
        result = self.mgr.order_snapshot_space(
            volume_id=volume_id,
            capacity=20,
            tier = 0.25,
            upgrade=False)
        pp(result)

    def orderReplicant(self, volume_id, schedule):
        """
        Same as other ordering methods, schedule is 
        "HOURLY", "DAILY" or "WEEKLY"
        """
        result = self.mgr.order_replicant_volume(
            volume_id=volume_id,
            snapshot_schedule=schedule,
            location = "dal06",
            tier = 0.25
        )
        pp(result)



    def listStoragePrices(self):
        """
        222 - Performance - PERFORMANCE_STORAGE_SERVICE
        240 - Endurance - CODENAME_PRIME_STORAGE
        If you feel like building the pricing object yourself, start here.
        """
        mask = "mask[items[prices[pricingLocationGroup,categories],attributes]]"
        # locations = self.client['Product_Package'].getLocations(id=package_id)
        result = self.client['Product_Package'].getObject(mask=mask,id=240)
        for item in result['items']:
            print("%s - %s - %s" % 
                (str(item['id']), item['description'], item['keyName']) 
            # pp(item)
            for prices in item['prices']:
                if prices['locationGroupId'] is  '':
                    print "\t" + str(prices['id'])
                # pp(prices)

    def listStorage(self):
    """
    Super complicated objectFilter. Mostly here as an example of how to do an IN filter.
    Returns all storage that is in DAL06, HOU02, is NOT NAS, and is Endurance_File_Storage
    """
        objectFilter = {
            'nasNetworkStorage': {
                'serviceResource': {
                    'type': {
                        'type': {'operation': '!~ NAS'}
                    },
                    'datacenter': {
                        'name': {
                            'operation': 'in',
                            'options': [{
                                'name': 'data',
                                'value': ['dal06','hou02']
                            }]
                        }
                    }
                },
                'storageType': {
                    'keyName': {'operation': 'ENDURANCE_FILE_STORAGE'}
                }
            }
        }
        result = self.client['Account'].getNasNetworkStorage(
            mask=self.objectMask,filter=objectFilter)
        pp(result)

    def authHost(self, volume_id, host_id):
    """
    each host that needs to mount the volume needs to be authorized.
    host and volume need to be in the same DC
    """
        guest = {
            'id': host_id
        }
        self.storage.allowAccessFromVirtualGuest(guest, id=volume_id)

    def authReplicant(self, volume_id, host_id):
    """
    each host that needs to mount the REPLICANT needs to be authorized.
    host and volume need to be in the same DC
    """
        guest = {
            'id': host_id
        }
        self.storage.allowAccessToReplicantFromVirtualGuest(guest, id=volume_id)

    def createSnapSchedule(self, volume_id):
        # HOURLY, 24 copies, first minute of the hour. 
        self.storage.enableSnapshots('HOURLY', 24, 1, 0, 0, id=volume_id)

    def manualSnap(self, volume_id):
        self.storage.createSnapshot('Manual SNAP', id=volume_id)

    def getReplicantId(self, volume_id):
        """
        there might be more than 1 replicant id in this list if there are more 
        than 1 replicant targets. Or none of course.
        """
        result = self.storage.getReplicationPartners(id=volume_id)
        return result[0]['id']
        

    def houIsDown(self, volume_id, now=False):

        replicate_to = main.getReplicantId(volume_id)
        if now:
            self.storage.immediateFailoverToReplicant(replicate_to, id=volume_id)
        else
            self.storage.failoverToReplicant(replicate_to, id=volume_id)

    def houIsBack(self, volume_id):
        self.storage.failbackFromReplicant(id=volume_id,now=False)

    def volumeStatus(self, volume_id):
        result = self.storage.getObject(mask=self.objectMask, id=volume_id)
        pp(result)


if __name__ == "__main__":
"""
Covers each of the steps required to create a storage volume, and then fail it over.
The ordering methods will need to be slightly modified for block storage. 
everything else should be good as is.

"""

    host_a = 25206857
    host_b = 28630647
    main = example()
    main.listStorage()
    ### First we need to order a storage volume, and get its ID.
    # main.orderStorage()
    volume_id = 20017773

    ### Then we need to order snapshot space
    # main.orderSnapshot(volume_id)

    ### Then create a snapshot schedule.
    # main.createSnapSchedule(volume_id)

    ### Then Allow our host to access the volume
    # main.authHost(volume_id, [host_a])

    ### Create a manual snapshot for fun 
    # main.manualSnap(volume_id)

    ### Order replication space.
    # main.orderReplicant(volume_id, 'HOURLY')

    ### Allow our vm to access replicant volume
    # main.authReplicant(volume_id,host_b)

    ### Failover to replicant
    # main.houIsDown(volume_id)

    ### Failback to main
    # main.houIsBack(volume_id)

    ### Get some status
    # main.volumeStatus(volume_id)

```