---
title: "getUtilizedIpAddressCount"
description: "Retrieve provides the total number of utilized IP addresses on this subnet. The primary consumer of IP addresses are com... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Subnet"
aliases:
    - "/reference/services/softlayer_network_subnet/getUtilizedIpAddressCount"
---
# [SoftLayer_Network_Subnet](/reference/services/SoftLayer_Network_Subnet)::getUtilizedIpAddressCount


Retrieve provides the total number of utilized IP addresses on this subnet. The primary consumer of IP addresses are compute resources, which can consume more than one address. This value is only supported for primary subnet types.


## Overview 
Retrieve provides the total number of utilized IP addresses on this subnet. The primary consumer of IP addresses are compute resources, which can consume more than one address. This value is only supported for primary subnet types.

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* SoftLayer_Network_SubnetInitParameters
* authenticate


### Optional Headers
* SoftLayer_Network_SubnetObjectMask
* SoftLayer_Network_SubnetObjectFilter
* SoftLayer_ObjectMask

### Return Values
* unsigned integer




