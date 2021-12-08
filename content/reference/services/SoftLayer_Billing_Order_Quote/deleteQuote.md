---
title: "deleteQuote"
description: "Account master users and sub-users in the SoftLayer customer portal can delete the quote of an order."
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Billing"
classes:
    - "SoftLayer_Billing_Order_Quote"
aliases:
    - "/reference/services/softlayer_billing_order_quote/deleteQuote"
---
# [SoftLayer_Billing_Order_Quote](/reference/services/SoftLayer_Billing_Order_Quote)::deleteQuote


Delete the quote of an order


## Overview 
Account master users and sub-users in the SoftLayer customer portal can delete the quote of an order. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* authenticate
* SoftLayer_Billing_Order_QuoteInitParameters


### Optional Headers
* SoftLayer_Billing_Order_QuoteObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Billing_Order_Quote'>SoftLayer_Billing_Order_Quote </a>


### Associated Methods

*  [SoftLayer_Billing_Order_Quote::deleteQuote](/reference/services/SoftLayer_Billing_Order_Quote/deleteQuote )
*  [SoftLayer_Billing_Order_Quote::saveQuote](/reference/services/SoftLayer_Billing_Order_Quote/saveQuote )



### Error Handling

* SoftLayer_Exception_Public 

> Throws the exception 'You cannot delete a deleted quote.' 



