---
title: "placeQuote"
description: "Use this method for placing server quotes and additional services quotes. The same applies for this as with verifyOrder.... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Billing"
classes:
    - "SoftLayer_Billing_Order_Quote"
aliases:
    - "/reference/services/softlayer_billing_order_quote/placeQuote"
---
# [SoftLayer_Billing_Order_Quote](/reference/services/SoftLayer_Billing_Order_Quote)::placeQuote


Saves changes to a quote


## Overview 
Use this method for placing server quotes and additional services quotes. The same applies for this as with verifyOrder. Send in the SoftLayer_Container_Product_Order_Hardware_Server for server quotes. In addition to verifying the quote, placeQuote() also makes an initial authorization on the SoftLayer_Account tied to this order, if a credit card is on file. If the account tied to this order is a paypal customer, an URL will also be returned to the customer. After placing the order, you must go to this URL to finish the authorization process. This tells paypal that you indeed want to place the order. After going to this URL, it will direct you back to a SoftLayer webpage that tells us you have finished the process. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|orderData| <a href='/reference/datatypes/SoftLayer_Container_Product_Order'>SoftLayer_Container_Product_Order </a>| Details required to order.|


### Required Headers
* authenticate
* SoftLayer_Billing_Order_QuoteInitParameters


### Return Values
* <a href='/reference/datatypes/SoftLayer_Container_Product_Order'>SoftLayer_Container_Product_Order </a>




