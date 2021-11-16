---
title: "getPublicVlanByFqdn"
description: "Retrieve the VLAN that belongs to a server's public network interface, as described by a server's fully-qualified domain... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Vlan"
aliases:
    - "/reference/services/softlayer_network_vlan/getPublicVlanByFqdn"
---
# [SoftLayer_Network_Vlan](/reference/services/SoftLayer_Network_Vlan)::getPublicVlanByFqdn


Retrieve a server's public VLAN based on it's fully-qualified domain name


## Overview 
Retrieve the VLAN that belongs to a server's public network interface, as described by a server's fully-qualified domain name. A server's ''FQDN'' is it's hostname, followed by a period then it's domain name. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|fqdn| string| The fully-qualified domain name of the server you wish to search for. This follows the naming convention "{hostname}.{domain}".|


### Required Headers
* authenticate


### Optional Headers
* SoftLayer_Network_VlanObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Network_Vlan'>SoftLayer_Network_Vlan </a>

### External Links


* [Fully qualified domain name at Wikipedia](http://en.wikipedia.org/wiki/Fully_qualified_domain_name)




### Error Handling

* SoftLayer_Exception 

> Throw the exception "You must supply a valid fully-qualified domain name, for example www.example.org" if the ''fqdn'' parameter is not a valid fully-qualified domain name with at least two periods in it. 

* SoftLayer_Exception 

> Throw the exception "Unable to find hardware with the fully-qualified domain name of '{fqdn}'" if the API is unable to locate a server with that fully-qualified domain name under your account. 



