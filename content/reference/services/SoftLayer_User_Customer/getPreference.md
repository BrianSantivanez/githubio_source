---
title: "getPreference"
description: "Select a type of preference you would like to get using [SoftLayer_User_Customer::getPreferenceTypes]({{<ref 'reference/... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "User"
classes:
    - "SoftLayer_User_Customer"
aliases:
    - "/reference/services/softlayer_user_customer/getPreference"
---
# [SoftLayer_User_Customer](/reference/services/SoftLayer_User_Customer)::getPreference


Get a preference value for the current user


## Overview 
Select a type of preference you would like to get using [SoftLayer_User_Customer::getPreferenceTypes]({{<ref "reference/services/SoftLayer_User_Customer/getPreferenceTypes">}}) and invoke this method using that preference type key name. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|preferenceTypeKeyName| string| The preference type key name from SoftLayer_User_Preference_Type.|


### Required Headers
* authenticate
* SoftLayer_User_CustomerInitParameters


### Optional Headers
* SoftLayer_User_CustomerObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_User_Preference'>SoftLayer_User_Preference </a>




