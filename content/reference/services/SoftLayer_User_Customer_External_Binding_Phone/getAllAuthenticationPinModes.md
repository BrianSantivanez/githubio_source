---
title: "getAllAuthenticationPinModes"
description: "This service returns key names of all available authentication modes. Refer to [SoftLayer_User_Customer_External_Binding... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "User"
classes:
    - "SoftLayer_User_Customer_External_Binding_Phone"
aliases:
    - "/reference/services/softlayer_user_customer_external_binding_phone/getAllAuthenticationPinModes"
---
# [SoftLayer_User_Customer_External_Binding_Phone](/reference/services/SoftLayer_User_Customer_External_Binding_Phone)::getAllAuthenticationPinModes


Returns available authentication pin modes


## Overview 
This service returns key names of all available authentication modes. Refer to [SoftLayer_User_Customer_External_Binding_Phone::getAllAuthenticationModes]({{<ref "reference/services/SoftLayer_User_Customer_External_Binding_Phone/getAllAuthenticationModes">}}) to retrieve authentication mode key names. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|authenticationModeKeyName| string| |


### Required Headers
* authenticate
* SoftLayer_User_Customer_External_Binding_PhoneInitParameters


### Return Values
* array of strings




