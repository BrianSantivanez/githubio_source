---
title: "allowAccessFromSubnet"
description: "This method is used to modify the access control list for this Storage volume.  The SoftLayer_Network_Subnet objects whi... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Storage_Iscsi"
aliases:
    - "/reference/services/softlayer_network_storage_iscsi/allowAccessFromSubnet"
---
# [SoftLayer_Network_Storage_Iscsi](/reference/services/SoftLayer_Network_Storage_Iscsi)::allowAccessFromSubnet


Allow access to this volume from multiple SoftLayer_Network_Subnet objects.


## Overview 
This method is used to modify the access control list for this Storage volume.  The SoftLayer_Network_Subnet objects which have been allowed access to this storage will be listed in the allowedHardware property of this storage volume. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|subnetObjectTemplate| <a href='/reference/datatypes/SoftLayer_Network_Subnet'>SoftLayer_Network_Subnet </a>| |


### Required Headers
* authenticate
* SoftLayer_Network_Storage_IscsiInitParameters


### Return Values
* boolean




