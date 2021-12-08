---
title: "createObjects"
description: "Create a new shipment tracking data. The ''shipmentId'', ''sequence'', and ''trackingData'' properties of each templateO... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Account"
classes:
    - "SoftLayer_Account_Shipment_Tracking_Data"
aliases:
    - "/reference/services/softlayer_account_shipment_tracking_data/createObjects"
---
# [SoftLayer_Account_Shipment_Tracking_Data](/reference/services/SoftLayer_Account_Shipment_Tracking_Data)::createObjects


Create multiple tracking data records.


## Overview 
Create a new shipment tracking data. The ''shipmentId'', ''sequence'', and ''trackingData'' properties of each templateObject in the templateObjects array are required parameters to create a tracking data record. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|templateObjects| <a href='/reference/datatypes/SoftLayer_Account_Shipment_Tracking_Data'>SoftLayer_Account_Shipment_Tracking_Data[] </a>| An array of SoftLayer_Account_Shipment_Tracking_Data objects that you wish to create.|


### Required Headers
* authenticate


### Optional Headers
* SoftLayer_Account_Shipment_Tracking_DataObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Account_Shipment_Tracking_Data'>SoftLayer_Account_Shipment_Tracking_Data[] </a>


### Associated Methods

*  [SoftLayer_Account_Shipment_Tracking_Data::createObject](/reference/services/SoftLayer_Account_Shipment_Tracking_Data/createObject )




