---
title: "getObject"
description: "getObject retrieves the SoftLayer_Billing_Item object whose ID number corresponds to the ID number of the init parameter... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Billing"
classes:
    - "SoftLayer_Billing_Order_Item"
aliases:
    - "/reference/services/softlayer_billing_order_item/getObject"
---
# [SoftLayer_Billing_Order_Item](/reference/services/SoftLayer_Billing_Order_Item)::getObject


Retrieve a SoftLayer_Billing_Order_Item record.


## Overview 
getObject retrieves the SoftLayer_Billing_Item object whose ID number corresponds to the ID number of the init parameter passed to the SoftLayer_Billing_Item service. You can only retrieve billing items tied to the account that your portal user is assigned to. Billing items are an account's items of billable items. There are "parent" billing items and "child" billing items. The server billing item is generally referred to as a parent billing item. The items tied to a server, such as ram, harddrives, and operating systems are considered "child" billing items. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* SoftLayer_Billing_Order_ItemInitParameters
* authenticate


### Optional Headers
* SoftLayer_Billing_Order_ItemObjectMask
* SoftLayer_Billing_Order_ItemObjectFilter
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Billing_Order_Item'>SoftLayer_Billing_Order_Item </a>




