---
title: "getBandwidthForDateRange"
description: "Retrieve a collection of bandwidth data from an individual public or private network tracking object. Data is ideal if y... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Bandwidth_Version1_Allotment"
aliases:
    - "/reference/services/softlayer_network_bandwidth_version1_allotment/getBandwidthForDateRange"
---
# [SoftLayer_Network_Bandwidth_Version1_Allotment](/reference/services/SoftLayer_Network_Bandwidth_Version1_Allotment)::getBandwidthForDateRange


Retrieve bandwidth data from a tracking object.


## Overview 
Retrieve a collection of bandwidth data from an individual public or private network tracking object. Data is ideal if you with to employ your own traffic storage and graphing systems. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|startDate| dateTime| The starting date of the range of data you wish to collect.|
|endDate| dateTime| The ending date of the range of data you wish to collect.|


### Required Headers
* authenticate
* SoftLayer_Network_Bandwidth_Version1_AllotmentInitParameters


### Return Values
* <a href='/reference/datatypes/SoftLayer_Metric_Tracking_Object_Data'>SoftLayer_Metric_Tracking_Object_Data[] </a>




