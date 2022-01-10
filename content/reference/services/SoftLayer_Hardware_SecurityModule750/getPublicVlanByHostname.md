---
title: "getPublicVlanByHostname"
description: "Retrieve the frontend network Vlan by searching the hostname of a server"
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Hardware"
classes:
    - "SoftLayer_Hardware_SecurityModule750"
aliases:
    - "/reference/services/softlayer_hardware_securitymodule750/getPublicVlanByHostname"
---
# [SoftLayer_Hardware_SecurityModule750](/reference/services/SoftLayer_Hardware_SecurityModule750)::getPublicVlanByHostname


Retrieve the frontend VLAN by a server's hostname.


## Overview 
Retrieve the frontend network Vlan by searching the hostname of a server 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|hostname| string| The hostname for a server, example: www.server.com|


### Required Headers
* authenticate


### Optional Headers
* SoftLayer_Hardware_SecurityModule750ObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Network_Vlan'>SoftLayer_Network_Vlan </a>



### Error Handling

* SoftLayer_Exception 

> Throw the exception "You must supply a valid hostname. Example: www.domain.com" if an invalid hostname was provided. 

* SoftLayer_Exception 

> Throw the exception "Unable to find hardware with the hostname of '{host}.{domain}'" if there is no server with the hostname provided. 



