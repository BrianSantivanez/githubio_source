---
title: "createTxtRecord"
description: "Create a TXT record on a SoftLayer domain. This is a shortcut method, meant to take the work out of creating a SoftLayer... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Dns"
classes:
    - "SoftLayer_Dns_Domain"
aliases:
    - "/reference/services/softlayer_dns_domain/createTxtRecord"
---
# [SoftLayer_Dns_Domain](/reference/services/SoftLayer_Dns_Domain)::createTxtRecord


Create a TXT record on a domain.


## Overview 
Create a TXT record on a SoftLayer domain. This is a shortcut method, meant to take the work out of creating a SoftLayer_Dns_Domain_ResourceRecord if you already have a domain record available. createARecord returns the newly created SoftLayer_Dns_Domain_ResourceRecord_TxtType. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|host| string| The resource record's name|
|data| string| The resource record's value|
|ttl| integer| The resource record's time-to-live value.|


### Required Headers
* authenticate
* SoftLayer_Dns_DomainInitParameters


### Optional Headers
* SoftLayer_Dns_DomainObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Dns_Domain_ResourceRecord_TxtType'>SoftLayer_Dns_Domain_ResourceRecord_TxtType </a>

### External Links


* [List of DNS record types at Wikipedia](http://en.wikipedia.org/wiki/List_of_DNS_record_types)


* [Sender Policy Framework](http://www.openspf.org/Project_Overview)





