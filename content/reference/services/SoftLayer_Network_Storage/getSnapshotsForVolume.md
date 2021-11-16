---
title: "getSnapshotsForVolume"
description: "Retrieves a list of snapshots for this SoftLayer_Network_Storage volume. This method works with the result limits and of... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Storage"
aliases:
    - "/reference/services/softlayer_network_storage/getSnapshotsForVolume"
---
# [SoftLayer_Network_Storage](/reference/services/SoftLayer_Network_Storage)::getSnapshotsForVolume


Retrieves a list oƒf snapshots for a given volume.


## Overview 
Retrieves a list of snapshots for this SoftLayer_Network_Storage volume. This method works with the result limits and offset to support pagination. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* authenticate
* SoftLayer_Network_StorageInitParameters


### Optional Headers
* SoftLayer_Network_StorageObjectMask
* SoftLayer_ObjectMask
* resultLimit

### Return Values
* <a href='/reference/datatypes/SoftLayer_Network_Storage'>SoftLayer_Network_Storage[] </a>




