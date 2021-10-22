---
title: "inviteUserToLinkOpenIdConnect"
description: "Send email invitation to a user to join a SoftLayer account and authenticate with OpenIdConnect. Throws an exception on... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "User"
classes:
    - "SoftLayer_User_Customer_OpenIdConnect_TrustedProfile"
aliases:
    - "/reference/services/softlayer_user_customer_openidconnect_trustedprofile/inviteUserToLinkOpenIdConnect"
---
# [SoftLayer_User_Customer_OpenIdConnect_TrustedProfile](/reference/services/SoftLayer_User_Customer_OpenIdConnect_TrustedProfile)::inviteUserToLinkOpenIdConnect

Send email invitation to a user to join a SoftLayer account and authenticate with OpenIdConnect.


## Overview 
Send email invitation to a user to join a SoftLayer account and authenticate with OpenIdConnect. Throws an exception on error. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|providerType| string| A value representing the OpenID Connect provider type. Currently "IBMid" is the only supported provider.|


### Required Headers
* authenticate
* SoftLayer_User_Customer_OpenIdConnect_TrustedProfileInitParameters


### Return Values
* void




