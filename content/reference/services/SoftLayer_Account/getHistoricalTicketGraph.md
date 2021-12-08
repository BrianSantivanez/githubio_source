---
title: "getHistoricalTicketGraph"
description: "Given the start and end dates, this method will return a pie chart of ticket statistics in the form of SoftLayer_Contain... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Account"
classes:
    - "SoftLayer_Account"
aliases:
    - "/reference/services/softlayer_account/getHistoricalTicketGraph"
---
# [SoftLayer_Account](/reference/services/SoftLayer_Account)::getHistoricalTicketGraph


This method returns a pie chart of ticket statistics for the given dates.


## Overview 
Given the start and end dates, this method will return a pie chart of ticket statistics in the form of SoftLayer_Container_Account_Graph_Outputs object with a base64 PNG string. If an error occurs the graphError parameter will be populated. Possible errors include: SoftLayer_Exception_Public Thrown if an invalid start or end date is provided. SoftLayer_Exception Thrown if there is an error connecting to HBase. SoftLayer_Exception Thrown if there is no data available for the specified date range. SoftLayer_Exception Thrown if there is an error retrieving data or generating the graph. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|startDate| dateTime| timestamp of the starting date|
|endDate| dateTime| timestamp of the ending date|


### Required Headers
* authenticate


### Return Values
* <a href='/reference/datatypes/SoftLayer_Container_Account_Graph_Outputs'>SoftLayer_Container_Account_Graph_Outputs </a>


### Associated Methods

*  [SoftLayer_Account::getCurrentTicketStatisticsGraph](/reference/services/SoftLayer_Account/getCurrentTicketStatisticsGraph )
*  [SoftLayer_Metric_Tracking_Object::getSummaryData](/reference/services/SoftLayer_Metric_Tracking_Object/getSummaryData )




