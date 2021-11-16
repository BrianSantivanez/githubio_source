---
title: "deleteObject"
description: "Delete a secondary DNS Record. This will also remove any associated domain records and resource records on the SoftLayer... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Dns"
classes:
    - "SoftLayer_Dns_Secondary"
aliases:
    - "/reference/services/softlayer_dns_secondary/deleteObject"
---
# [SoftLayer_Dns_Secondary](/reference/services/SoftLayer_Dns_Secondary)::deleteObject


Delete a secondary DNS record


## Overview 
Delete a secondary DNS Record. This will also remove any associated domain records and resource records on the SoftLayer nameservers that were created as a result of the zone transfers. This action cannot be undone. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* authenticate
* SoftLayer_Dns_SecondaryInitParameters


### Return Values
* boolean




