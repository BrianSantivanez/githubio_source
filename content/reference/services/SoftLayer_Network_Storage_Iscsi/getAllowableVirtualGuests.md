---
title: "getAllowableVirtualGuests"
description: "This method retrieves a list of SoftLayer_Virtual_Guest that can be authorized to this SoftLayer_Network_Storage."
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Storage_Iscsi"
aliases:
    - "/reference/services/softlayer_network_storage_iscsi/getAllowableVirtualGuests"
---
# [SoftLayer_Network_Storage_Iscsi](/reference/services/SoftLayer_Network_Storage_Iscsi)::getAllowableVirtualGuests


Return a list of SoftLayer_Virtual_Guest that can be authorized to this volume. 


## Overview 
This method retrieves a list of SoftLayer_Virtual_Guest that can be authorized to this SoftLayer_Network_Storage. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|filterHostname| string| a string to filter the hostname by.|


### Required Headers
* authenticate
* SoftLayer_Network_Storage_IscsiInitParameters


### Optional Headers
* SoftLayer_Network_Storage_IscsiObjectMask
* SoftLayer_ObjectMask
* resultLimit

### Return Values
* <a href='/reference/datatypes/SoftLayer_Virtual_Guest'>SoftLayer_Virtual_Guest[] </a>




