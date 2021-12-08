---
title: "removeAccessToReplicantFromHardwareList"
description: "This method is used to modify the access control list for this Storage replica volume.  The SoftLayer_Hardware objects w... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Storage_Iscsi"
aliases:
    - "/reference/services/softlayer_network_storage_iscsi/removeAccessToReplicantFromHardwareList"
---
# [SoftLayer_Network_Storage_Iscsi](/reference/services/SoftLayer_Network_Storage_Iscsi)::removeAccessToReplicantFromHardwareList


Remove access to this volume from multiple SoftLayer_Hardware objects.


## Overview 
This method is used to modify the access control list for this Storage replica volume.  The SoftLayer_Hardware objects which have been allowed access to this storage will be listed in the allowedHardware property of this storage replica volume. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|hardwareObjectTemplates| <a href='/reference/datatypes/SoftLayer_Hardware'>SoftLayer_Hardware[] </a>| |


### Required Headers
* authenticate
* SoftLayer_Network_Storage_IscsiInitParameters


### Return Values
* boolean




