---
title: "editObject"
description: "The subscriber's subscription status can be 'turned off' or 'turned on' if the subscription is not required. 

Subscriber preferences may also be edited.  To edit the preferences, you must pass in the id off the preferences to edit.  Here is an example of structure to pass in.  In this example, the structure will set the subscriber status to active and the threshold preference to 90 and the limit preference to 20 


*id = 1111
*active = 1
*preferences[1]
**id = 11
**value = 90
*preference[2]
**id = 12
**value = 20"
date: "2018-02-12"
tags:
    - "method"
    - "sldn"
    - "Notification"
classes:
    - "SoftLayer_Notification_User_Subscriber_Mobile"
type: "reference"
layout: "method"
mainService : "SoftLayer_Notification_User_Subscriber_Mobile"
---
