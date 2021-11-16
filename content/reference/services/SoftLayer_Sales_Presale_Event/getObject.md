---
title: "getObject"
description: "'''getObject''' retrieves the [SoftLayer_Sales_Presale_Event]({{<ref 'reference/datatypes/SoftLayer_Sales_Presale_Event'... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Sales"
classes:
    - "SoftLayer_Sales_Presale_Event"
aliases:
    - "/reference/services/softlayer_sales_presale_event/getObject"
---
# [SoftLayer_Sales_Presale_Event](/reference/services/SoftLayer_Sales_Presale_Event)::getObject


Retrieve a SoftLayer_Sales_Presale_Event record.


## Overview 
'''getObject''' retrieves the [SoftLayer_Sales_Presale_Event]({{<ref "reference/datatypes/SoftLayer_Sales_Presale_Event">}}) object whose id number corresponds to the id number of the init parameter passed to the SoftLayer_Sales_Presale_Event service. Customers may only retrieve presale events that are currently active. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* SoftLayer_Sales_Presale_EventInitParameters
* authenticate


### Optional Headers
* SoftLayer_Sales_Presale_EventObjectMask
* SoftLayer_Sales_Presale_EventObjectFilter
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Sales_Presale_Event'>SoftLayer_Sales_Presale_Event </a>




