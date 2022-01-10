---
title: "findByIpAddress"
description: "The '''findByIpAddress''' method finds hardware using its primary public or private IP address. IP addresses that have a... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Hardware"
classes:
    - "SoftLayer_Hardware_Server"
aliases:
    - "/reference/services/softlayer_hardware_server/findByIpAddress"
---
# [SoftLayer_Hardware_Server](/reference/services/SoftLayer_Hardware_Server)::findByIpAddress


Find hardware by its primary public or private IP (ipv4) address.


## Overview 
The '''findByIpAddress''' method finds hardware using its primary public or private IP address. IP addresses that have a secondary subnet tied to the hardware will not return the hardware. If no hardware is found, no errors are generated and no data is returned. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|ipAddress| string| An IP (ipv4) address by which to search for hardware|


### Required Headers
* authenticate


### Optional Headers
* SoftLayer_Hardware_ServerObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Hardware_Server'>SoftLayer_Hardware_Server </a>



### Error Handling

* SoftLayer_Exception 

> "Invalid IP address of [ip address] defined." 



