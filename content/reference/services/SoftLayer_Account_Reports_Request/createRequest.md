---
title: "createRequest"
description: ""
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Account"
classes:
    - "SoftLayer_Account_Reports_Request"
aliases:
    - "/reference/services/softlayer_account_reports_request/createRequest"
---
# [SoftLayer_Account_Reports_Request](/reference/services/SoftLayer_Account_Reports_Request)::createRequest





## Overview 


-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|recipientContact| <a href='/reference/datatypes/SoftLayer_Account_Contact'>SoftLayer_Account_Contact </a>| The external party for which the request may be created|
|reason| string| The reason the external party is requesting the report|
|reportType| string| type of the report customer is requesting|
|requestorContact| <a href='/reference/datatypes/SoftLayer_Account_Contact'>SoftLayer_Account_Contact </a>| The external party for who requested the report|


### Required Headers
* authenticate


### Optional Headers
* SoftLayer_Account_Reports_RequestObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Account_Reports_Request'>SoftLayer_Account_Reports_Request </a>




