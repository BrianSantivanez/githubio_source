---
title: "requestManualPayment"
description: "Retrieve the record data associated with the submission of a Manual Payment Request. Softlayer customers are permitted t... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Account"
classes:
    - "SoftLayer_Account"
aliases:
    - "/reference/services/softlayer_account/requestManualPayment"
---
# [SoftLayer_Account](/reference/services/SoftLayer_Account)::requestManualPayment


Retrieve the record data associated with the submission of a Manual Payment Request.


## Overview 
Retrieve the record data associated with the submission of a Manual Payment Request. Softlayer customers are permitted to request a manual one-time payment at a minimum amount of $2.00. Customers may submit a Credit Card Payment (Mastercard, Visa, American Express) or a PayPal payment. For Credit Card Payments, SoftLayer engages the credit card financial institution to submit the payment request.  The financial institution's response and other data associated with the transaction are returned to the calling function.  In the case of PayPal Payments, SoftLayer engages the PayPal system to initiate the PayPal payment sequence.  The applicable data generated during the request is returned to the calling function. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|request| <a href='/reference/datatypes/SoftLayer_Billing_Payment_Card_ManualPayment'>SoftLayer_Billing_Payment_Card_ManualPayment </a>| Details required to request a manual payment.|


### Required Headers
* authenticate


### Optional Headers
* SoftLayer_AccountObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Billing_Payment_Card_ManualPayment'>SoftLayer_Billing_Payment_Card_ManualPayment </a>



### Error Handling

* SoftLayer_Exception_Billing_Payment_Card_PayerAuthenticationRequired 

> Throw the error "The customer is enrolled in payer authentication. Authenticate the cardholder before continuing with the transaction. ACSUrl={access control server url} | PAReq={payer authentication request message} | TransactionID={Transaction ID}" occurs when payer authentication is required. The error message contains additional applicable data to support continuation of authentication via Cardinal Cruise Hybrid. You must take the ACSUrl, PAReq, and TransactionID and include them in the Cardinal.continue function in order to proceed with the authentication session. NOTE: In the Cardinal.continue function, the 'Payload' field value should be populated with the data from PAReq. 



