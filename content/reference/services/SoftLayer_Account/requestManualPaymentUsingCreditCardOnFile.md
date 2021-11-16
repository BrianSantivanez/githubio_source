---
title: "requestManualPaymentUsingCreditCardOnFile"
description: "Retrieve the record data associated with the submission of a Manual Payment Request for a manual payment using a credit... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Account"
classes:
    - "SoftLayer_Account"
aliases:
    - "/reference/services/softlayer_account/requestManualPaymentUsingCreditCardOnFile"
---
# [SoftLayer_Account](/reference/services/SoftLayer_Account)::requestManualPaymentUsingCreditCardOnFile


Retrieve the record data associated with the submission of a Manual Payment Request which charges the manual payment to a credit card already on file. 


## Overview 
Retrieve the record data associated with the submission of a Manual Payment Request for a manual payment using a credit card which is on file and does not require an approval process.  Softlayer customers are permitted to request a manual one-time payment at a minimum amount of $2.00.  Customers may use an existing Credit Card on file (Mastercard, Visa, American Express).  SoftLayer engages the credit card financial institution to submit the payment request.  The financial institution's response and other data associated with the transaction are returned to the calling function.  The applicable data generated during the request is returned to the calling function. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|amount| string| dollar amount which will be charged to the specified credit card|
|payWithAlternateCardFlag| boolean| if true, the charge will be applied to the alternate card on file|
|note| string| Optional note which will be added to the manual payment request|


### Required Headers
* authenticate


### Optional Headers
* SoftLayer_AccountObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Billing_Payment_Card_ManualPayment'>SoftLayer_Billing_Payment_Card_ManualPayment </a>




