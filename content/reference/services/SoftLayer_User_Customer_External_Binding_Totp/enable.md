---
title: "enable"
description: "Enabling an external binding will activate the binding on your account and require you to authenticate with our trusted... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "User"
classes:
    - "SoftLayer_User_Customer_External_Binding_Totp"
aliases:
    - "/reference/services/softlayer_user_customer_external_binding_totp/enable"
---
# [SoftLayer_User_Customer_External_Binding_Totp](/reference/services/SoftLayer_User_Customer_External_Binding_Totp)::enable


Enable an external binding.


## Overview 
Enabling an external binding will activate the binding on your account and require you to authenticate with our trusted 3rd party 2 form factor vendor when logging into the SoftLayer customer portal. 

Please note that API access will be disabled for users that have an active external binding. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* authenticate
* SoftLayer_User_Customer_External_Binding_TotpInitParameters


### Return Values
* boolean




