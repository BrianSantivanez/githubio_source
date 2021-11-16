---
title: "removeAccessToReplicantFromVirtualGuestList"
description: "This method is used to modify the access control list for this Storage replica volume.  The SoftLayer_Virtual_Guest obje... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Storage_Iscsi"
aliases:
    - "/reference/services/softlayer_network_storage_iscsi/removeAccessToReplicantFromVirtualGuestList"
---
# [SoftLayer_Network_Storage_Iscsi](/reference/services/SoftLayer_Network_Storage_Iscsi)::removeAccessToReplicantFromVirtualGuestList


Remove access to this replica volume from multiple SoftLayer_Virtual_Guest objects.


## Overview 
This method is used to modify the access control list for this Storage replica volume.  The SoftLayer_Virtual_Guest objects which have been allowed access to this storage will be listed in the allowedVirtualGuests property of this storage replica volume. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|virtualGuestObjectTemplates| <a href='/reference/datatypes/SoftLayer_Virtual_Guest'>SoftLayer_Virtual_Guest[] </a>| |


### Required Headers
* authenticate
* SoftLayer_Network_Storage_IscsiInitParameters


### Return Values
* boolean




