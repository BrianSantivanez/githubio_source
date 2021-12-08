---
title: "removeAssociationId"
description: "Remove the association from a billing item."
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Billing"
classes:
    - "SoftLayer_Billing_Item"
aliases:
    - "/reference/services/softlayer_billing_item/removeAssociationId"
---
# [SoftLayer_Billing_Item](/reference/services/SoftLayer_Billing_Item)::removeAssociationId


Remove an association from an orphan billing item.


## Overview 
Remove the association from a billing item. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* authenticate
* SoftLayer_Billing_ItemInitParameters


### Return Values
* boolean


### Associated Methods

*  [SoftLayer_Billing_Item::setAssociationId](/reference/services/SoftLayer_Billing_Item/setAssociationId )



### Error Handling

* SoftLayer_Exception_Public 

> Throw the exception "This billing item is not an orphan billing item." if the given billing item has a parent billing item. 



