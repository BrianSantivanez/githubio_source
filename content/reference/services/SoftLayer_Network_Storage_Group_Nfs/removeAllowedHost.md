---
title: "removeAllowedHost"
description: "Use this method to remove a SoftLayer_Network_Storage_Allowed_Host object from this group.  This will automatically disa... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Storage_Group_Nfs"
aliases:
    - "/reference/services/softlayer_network_storage_group_nfs/removeAllowedHost"
---
# [SoftLayer_Network_Storage_Group_Nfs](/reference/services/SoftLayer_Network_Storage_Group_Nfs)::removeAllowedHost


Remove a SoftLayer_Network_Storage_Allowed_Host object from this group


## Overview 
Use this method to remove a SoftLayer_Network_Storage_Allowed_Host object from this group.  This will automatically disable access from this host to any SoftLayer_Network_Storage volumes currently attached to this group. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|allowedHost| <a href='/reference/datatypes/SoftLayer_Network_Storage_Allowed_Host'>SoftLayer_Network_Storage_Allowed_Host </a>| |


### Required Headers
* authenticate
* SoftLayer_Network_Storage_Group_NfsInitParameters


### Return Values
* boolean




