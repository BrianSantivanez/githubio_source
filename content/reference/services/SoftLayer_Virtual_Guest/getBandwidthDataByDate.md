---
title: "getBandwidthDataByDate"
description: "Use this method when needing the metric data for bandwidth for a single guest.  It will gather the correct input paramet... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Virtual"
classes:
    - "SoftLayer_Virtual_Guest"
aliases:
    - "/reference/services/softlayer_virtual_guest/getBandwidthDataByDate"
---
# [SoftLayer_Virtual_Guest](/reference/services/SoftLayer_Virtual_Guest)::getBandwidthDataByDate


Retrieve the amount of network traffic that occurred for the specified time frame for a computing instance. 


## Overview 
Use this method when needing the metric data for bandwidth for a single guest.  It will gather the correct input parameters based on the date ranges 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|startDateTime| dateTime| datetime of the start date of the graph|
|endDateTime| dateTime| datetime of the ending date of the graph|
|networkType| string| type of the graph, either "public" or "private"|


### Required Headers
* authenticate
* SoftLayer_Virtual_GuestInitParameters


### Return Values
* <a href='/reference/datatypes/SoftLayer_Metric_Tracking_Object_Data'>SoftLayer_Metric_Tracking_Object_Data[] </a>




