---
title: "initiatePortalPasswordChange"
description: "Sends password change email to the user containing url that allows the user the change their password. This is the first... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "User"
classes:
    - "SoftLayer_User_Customer"
aliases:
    - "/reference/services/softlayer_user_customer/initiatePortalPasswordChange"
---
# [SoftLayer_User_Customer](/reference/services/SoftLayer_User_Customer)::initiatePortalPasswordChange


Request email to allow user to change their password


## Overview 
Sends password change email to the user containing url that allows the user the change their password. This is the first step when a user wishes to change their password.  The url that is generated contains a one-time use token that is valid for only 24-hours. 

If this is a new master user who has never logged into the portal, then password reset will be initiated. Once a master user has logged into the portal, they must setup their security questions prior to logging out because master users are required to answer a security question during the password reset process.  Should a master user not have security questions defined and not remember their password in order to define the security questions, then they will need to contact support at live chat or Revenue Services for assistance. 

Due to security reasons, the number of reset requests per username are limited within a undisclosed timeframe. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|username| string| The username of the user who is changing their password.|


### Required Headers


### Return Values
* boolean


### Associated Methods

*  [SoftLayer_User_Customer::getUserIdForPasswordSet](/reference/services/SoftLayer_User_Customer/getUserIdForPasswordSet )
*  [SoftLayer_User_Customer::getRequirementsForPasswordSet](/reference/services/SoftLayer_User_Customer/getRequirementsForPasswordSet )
*  [SoftLayer_User_Customer::processPasswordSetRequest](/reference/services/SoftLayer_User_Customer/processPasswordSetRequest )
*  [SoftLayer_User_Customer::checkPhoneFactorAuthenticationForPasswordSet](/reference/services/SoftLayer_User_Customer/checkPhoneFactorAuthenticationForPasswordSet )



### Error Handling

* SoftLayer_Exception_InvalidValue 

> Throws the exception "Invalid value provided for Username" if no username is provided. 



