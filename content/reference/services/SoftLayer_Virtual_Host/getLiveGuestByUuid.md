---
title: "getLiveGuestByUuid"
description: "Query a virtualization platform directly to retrieve details regarding a guest."
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Virtual"
classes:
    - "SoftLayer_Virtual_Host"
aliases:
    - "/reference/services/softlayer_virtual_host/getLiveGuestByUuid"
---
# [SoftLayer_Virtual_Host](/reference/services/SoftLayer_Virtual_Host)::getLiveGuestByUuid


Query a virtualization platform directly to retrieve details regarding a guest. 


## Overview 
Query a virtualization platform directly to retrieve details regarding a guest. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|uuid| string| The Universally Unique Identifier for the guest to fetch|


### Required Headers
* authenticate
* SoftLayer_Virtual_HostInitParameters


### Optional Headers
* SoftLayer_Virtual_HostObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Virtual_Guest'>SoftLayer_Virtual_Guest </a>




