---
title: "findByIpv4Address"
description: "Search for an IP address record by IPv4 address."
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Subnet_IpAddress"
aliases:
    - "/reference/services/softlayer_network_subnet_ipaddress/findByIpv4Address"
---
# [SoftLayer_Network_Subnet_IpAddress](/reference/services/SoftLayer_Network_Subnet_IpAddress)::findByIpv4Address


Search for an IP address record by IPv4 address.


## Overview 
Search for an IP address record by IPv4 address.

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|ipAddress| string| The IP address to search for|


### Required Headers
* authenticate


### Optional Headers
* SoftLayer_Network_Subnet_IpAddressObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Network_Subnet_IpAddress'>SoftLayer_Network_Subnet_IpAddress </a>



### Error Handling

* SoftLayer_Exception_Public 

> Throw the exception "The IP address provided (ipAddress) is not a valid IPv4 address." if the ipAddress parameter is not a valid IPv4 address. 



