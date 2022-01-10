---
title: "createObject"
description: "Use the method to create a new subscription for a notification.  This method is the entry method to the notification sys... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Notification"
classes:
    - "SoftLayer_Notification_User_Subscriber_Mobile"
aliases:
    - "/reference/services/softlayer_notification_user_subscriber_mobile/createObject"
---
# [SoftLayer_Notification_User_Subscriber_Mobile](/reference/services/SoftLayer_Notification_User_Subscriber_Mobile)::createObject


Create a new notification subscriber.


## Overview 
Use the method to create a new subscription for a notification.  This method is the entry method to the notification system. Certain properties are required to create a subscription while others are optional. 

The required property is the resourceRecord property which is type SoftLayer_Notification_User_Subscriber_Resource.  For the resourceRecord property, the only property that needs to be populated is the resourceTableId.  The resourceTableId is the unique identifier of a SoftLayer service to create the subscription for.  For example, the unique identifier of the Storage Evault service to create the subscription on. 

Optional properties that can be set is the preferences property.  The preference property is an array SoftLayer_Notification_User_Subscriber_Preference. By default, the system will populate the preferences with the default values if no preferences are passed in.  The preferences passed in must be the preferences related to the notification subscribing to.  The notification preferences and preference details (such as minimum and maximum values) can be retrieved using the SoftLayer_Notification service.  The properties that need to be populated for preferences are the notificationPreferenceId and value. 

For example to create a subscriber for a Storage EVault service to be notified 15 times during a billing cycle and to be notified when the vault usage reaches 85% of its allowed capacity use the following structure: 


*userRecordId = 1111
*notificationId = 3
*resourceRecord
**resourceTableId = 1234
*preferences[1]
**notificationPreferenceId = 2
**value = 85
*preference[2]
**notificationPreferenceId = 3
**value = 15



-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|templateObject| <a href='/reference/datatypes/SoftLayer_Notification_User_Subscriber_Mobile'>SoftLayer_Notification_User_Subscriber_Mobile </a>| The SoftLayer_Notification_User_Subscriber_Mobile object that you wish to create.|


### Required Headers
* authenticate


### Return Values
* boolean




