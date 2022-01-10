---
title: "deleteObject"
description: "Delete a network storage volume. '''This cannot be undone.''' At this time only network storage snapshots may be deleted... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Storage_Iscsi"
aliases:
    - "/reference/services/softlayer_network_storage_iscsi/deleteObject"
---
# [SoftLayer_Network_Storage_Iscsi](/reference/services/SoftLayer_Network_Storage_Iscsi)::deleteObject


Delete a network storage volume


## Overview 
Delete a network storage volume. '''This cannot be undone.''' At this time only network storage snapshots may be deleted with this method. 

''deleteObject'' returns Boolean ''true'' on successful deletion or ''false'' if it was unable to remove a volume; 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* authenticate
* SoftLayer_Network_Storage_IscsiInitParameters


### Return Values
* boolean



### Error Handling

* SoftLayer_Exception 

> Throw the exception "Only snapshots may be deleted with this method." when attempting to remove anything other than a snapshot. 



