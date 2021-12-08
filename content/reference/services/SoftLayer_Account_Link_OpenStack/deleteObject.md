---
title: "deleteObject"
description: "deleteObject permanently removes an account link and all of it's associated keystone data (including users for the assoc... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Account"
classes:
    - "SoftLayer_Account_Link_OpenStack"
aliases:
    - "/reference/services/softlayer_account_link_openstack/deleteObject"
---
# [SoftLayer_Account_Link_OpenStack](/reference/services/SoftLayer_Account_Link_OpenStack)::deleteObject


Remove an account link.


## Overview 
deleteObject permanently removes an account link and all of it's associated keystone data (including users for the associated project). '''This cannot be undone.''' Be wary of running this method. If you remove an account link in error you will need to re-create it by creating a new SoftLayer_Account_Link_OpenStack object. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* authenticate
* SoftLayer_Account_Link_OpenStackInitParameters


### Return Values
* boolean




