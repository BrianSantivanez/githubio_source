---
title: "allowAccessFromVirtualGuest"
description: "This method is used to modify the access control list for this Storage volume.  The SoftLayer_Virtual_Guest objects whic... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Storage_Backup_Evault"
aliases:
    - "/reference/services/softlayer_network_storage_backup_evault/allowAccessFromVirtualGuest"
---
# [SoftLayer_Network_Storage_Backup_Evault](/reference/services/SoftLayer_Network_Storage_Backup_Evault)::allowAccessFromVirtualGuest


Allow access to this volume from a specified SoftLayer_Virtual_Guest object.


## Overview 
This method is used to modify the access control list for this Storage volume.  The SoftLayer_Virtual_Guest objects which have been allowed access to this storage will be listed in the allowedVirtualGuests property of this storage volume. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|virtualGuestObjectTemplate| <a href='/reference/datatypes/SoftLayer_Virtual_Guest'>SoftLayer_Virtual_Guest </a>| |


### Required Headers
* authenticate
* SoftLayer_Network_Storage_Backup_EvaultInitParameters


### Return Values
* boolean




