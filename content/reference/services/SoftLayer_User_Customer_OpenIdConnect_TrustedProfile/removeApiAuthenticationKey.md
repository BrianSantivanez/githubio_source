---
title: "removeApiAuthenticationKey"
description: "Remove a user's API authentication key, removing that user's access to query the SoftLayer API."
layout: "method"
tags:
    - "method"
    - "sldn"
    - "User"
classes:
    - "SoftLayer_User_Customer_OpenIdConnect_TrustedProfile"
aliases:
    - "/reference/services/softlayer_user_customer_openidconnect_trustedprofile/removeApiAuthenticationKey"
---
# [SoftLayer_User_Customer_OpenIdConnect_TrustedProfile](/reference/services/SoftLayer_User_Customer_OpenIdConnect_TrustedProfile)::removeApiAuthenticationKey

Remove a user's API authentication key.


## Overview 
Remove a user's API authentication key, removing that user's access to query the SoftLayer API. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|keyId| integer| The identifier of the API authentication key you wish to remove.|


### Required Headers
* authenticate


### Return Values
* boolean


### Associated Methods

*  [SoftLayer_User_Customer::addApiAuthenticationKey](/reference/services/SoftLayer_User_Customer/addApiAuthenticationKey )



### Error Handling

* SoftLayer_Exception_Public 

> Throws the exception "Please provide an API Authentication key ID." when not passing or passing an invalid API authentication key ID. 



