---
title: "restoreFromSnapshot"
description: "Restore the volume from a snapshot that was previously taken."
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Storage_Iscsi"
aliases:
    - "/reference/services/softlayer_network_storage_iscsi/restoreFromSnapshot"
---
# [SoftLayer_Network_Storage_Iscsi](/reference/services/SoftLayer_Network_Storage_Iscsi)::restoreFromSnapshot


Restore from a volume snapshot.


## Overview 
Restore the volume from a snapshot that was previously taken. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|snapshotId| integer| Snapshot ID to restore from|


### Required Headers
* authenticate
* SoftLayer_Network_Storage_IscsiInitParameters


### Return Values
* boolean

### External Links


* [In depth details on storage snapshots at Wikipedia](http://en.wikipedia.org/wiki/Snapshot_(computer_storage))





