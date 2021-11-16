---
title: "findAllSubnetsAndActiveSwipTransactionStatus"
description: "***DEPRECATED***
Retrieve a list of a SoftLayer customer's subnets along with their SWIP transaction statuses. This is a... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Subnet"
aliases:
    - "/reference/services/softlayer_network_subnet/findAllSubnetsAndActiveSwipTransactionStatus"
---
# [SoftLayer_Network_Subnet](/reference/services/SoftLayer_Network_Subnet)::findAllSubnetsAndActiveSwipTransactionStatus

<div class="deprecated"><span class="deprecation-label">Deprecated </span></div>

Retrieve a list of subnets along with their SWIP transaction statuses.


## Overview 

***DEPRECATED***
Retrieve a list of a SoftLayer customer's subnets along with their SWIP transaction statuses. This is a shortcut method that combines the SoftLayer_Network_Subnet retrieval methods along with [[object masks]] to retrieve their subnets' associated SWIP transactions as well. 

This is a special function built for SoftLayer's use on the SWIP section of the customer portal, but may also be useful for API users looking for the same data. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* authenticate


### Optional Headers
* SoftLayer_Network_SubnetObjectMask
* SoftLayer_ObjectMask
* SoftLayer_Network_SubnetObjectFilter
* resultLimit

### Return Values
* <a href='/reference/datatypes/SoftLayer_Network_Subnet'>SoftLayer_Network_Subnet[] </a>




