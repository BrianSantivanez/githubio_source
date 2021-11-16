---
title: "getBandwidthTotal"
description: "Retrieve the total amount of bandwidth recorded by a tracking object within the given date range. This method will only... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Metric"
classes:
    - "SoftLayer_Metric_Tracking_Object"
aliases:
    - "/reference/services/softlayer_metric_tracking_object/getBandwidthTotal"
---
# [SoftLayer_Metric_Tracking_Object](/reference/services/SoftLayer_Metric_Tracking_Object)::getBandwidthTotal


Retrieve the total bandwidth used within a given time frame.


## Overview 
Retrieve the total amount of bandwidth recorded by a tracking object within the given date range. This method will only work on SoftLayer_Metric_Tracking_Object for SoftLayer_Hardware objects, and SoftLayer_Virtual_Guest objects. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|startDateTime| dateTime| The starting date of the range of data you wish to collect.|
|endDateTime| dateTime| The ending date of the range of data you wish to collect.|
|direction| string| The direction of data flow that you wish to retrieve totals for, either "in", "out", or "both".|
|type| string| The type type of the bandwidth data you wish to retrieve totals for, either "public" or "private", or "both".|


### Required Headers
* authenticate
* SoftLayer_Metric_Tracking_ObjectInitParameters


### Return Values
* unsigned long


### Associated Methods

*  [SoftLayer_Metric_Tracking_Object::getBandwidthGraph](/reference/services/SoftLayer_Metric_Tracking_Object/getBandwidthGraph )
*  [SoftLayer_Metric_Tracking_Object::getBandwidthData](/reference/services/SoftLayer_Metric_Tracking_Object/getBandwidthData )




