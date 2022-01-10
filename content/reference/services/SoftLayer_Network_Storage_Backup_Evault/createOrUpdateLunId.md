---
title: "createOrUpdateLunId"
description: "The LUN ID only takes effect during the Host Authorization process. It is required to de-authorize all hosts before usin... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Storage_Backup_Evault"
aliases:
    - "/reference/services/softlayer_network_storage_backup_evault/createOrUpdateLunId"
---
# [SoftLayer_Network_Storage_Backup_Evault](/reference/services/SoftLayer_Network_Storage_Backup_Evault)::createOrUpdateLunId


Creates or updates the LUN ID property on a volume.


## Overview 
The LUN ID only takes effect during the Host Authorization process. It is required to de-authorize all hosts before using this method. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|lunId| integer| <<< EOT|


### Required Headers
* authenticate
* SoftLayer_Network_Storage_Backup_EvaultInitParameters


### Optional Headers
* SoftLayer_Network_Storage_Backup_EvaultObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Network_Storage_Property'>SoftLayer_Network_Storage_Property </a>




