---
title: "createObjects"
description: "Passing in a collection of unsaved instances of Customer_Notification_Hardware objects into this function will create al... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "User"
classes:
    - "SoftLayer_User_Customer_Notification_Hardware"
aliases:
    - "/reference/services/softlayer_user_customer_notification_hardware/createObjects"
---
# [SoftLayer_User_Customer_Notification_Hardware](/reference/services/SoftLayer_User_Customer_Notification_Hardware)::createObjects

Create multiple user hardware notification entries at once


## Overview 
Passing in a collection of unsaved instances of Customer_Notification_Hardware objects into this function will create all objects and return the results to the user. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|templateObjects| <a href='/reference/datatypes/SoftLayer_User_Customer_Notification_Hardware'>SoftLayer_User_Customer_Notification_Hardware[] </a>| An array of SoftLayer_User_Customer_Notification_Hardware objects that you wish to create.|


### Required Headers
* authenticate


### Optional Headers
* SoftLayer_User_Customer_Notification_HardwareObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_User_Customer_Notification_Hardware'>SoftLayer_User_Customer_Notification_Hardware[] </a>




