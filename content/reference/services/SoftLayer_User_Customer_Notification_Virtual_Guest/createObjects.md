---
title: "createObjects"
description: "Passing in a collection of unsaved instances of SoftLayer_Customer_Notification_Virtual_Guest objects into this function... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "User"
classes:
    - "SoftLayer_User_Customer_Notification_Virtual_Guest"
aliases:
    - "/reference/services/softlayer_user_customer_notification_virtual_guest/createObjects"
---
# [SoftLayer_User_Customer_Notification_Virtual_Guest](/reference/services/SoftLayer_User_Customer_Notification_Virtual_Guest)::createObjects


Create multiple user Virtual Guest notification entries at once


## Overview 
Passing in a collection of unsaved instances of SoftLayer_Customer_Notification_Virtual_Guest objects into this function will create all objects and return the results to the user. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|templateObjects| <a href='/reference/datatypes/SoftLayer_User_Customer_Notification_Virtual_Guest'>SoftLayer_User_Customer_Notification_Virtual_Guest[] </a>| An array of SoftLayer_User_Customer_Notification_Virtual_Guest objects that you wish to create.|


### Required Headers
* authenticate


### Optional Headers
* SoftLayer_User_Customer_Notification_Virtual_GuestObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_User_Customer_Notification_Virtual_Guest'>SoftLayer_User_Customer_Notification_Virtual_Guest[] </a>




