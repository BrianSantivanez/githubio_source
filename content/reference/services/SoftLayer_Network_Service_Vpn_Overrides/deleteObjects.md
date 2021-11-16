---
title: "deleteObjects"
description: "Use this method to delete a collection of SoftLayer portal VPN user subnet overrides."
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Service_Vpn_Overrides"
aliases:
    - "/reference/services/softlayer_network_service_vpn_overrides/deleteObjects"
---
# [SoftLayer_Network_Service_Vpn_Overrides](/reference/services/SoftLayer_Network_Service_Vpn_Overrides)::deleteObjects


Delete multiple entries in the overrides 'white list' for a SoftLayer portal VPN user.


## Overview 
Use this method to delete a collection of SoftLayer portal VPN user subnet overrides. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|templateObjects| <a href='/reference/datatypes/SoftLayer_Network_Service_Vpn_Overrides'>SoftLayer_Network_Service_Vpn_Overrides[] </a>| An array of skeleton SoftLayer_Network_Service_Vpn_Overrides objects that you wish to delete. Each object in the array must have at least their id properties defined.|


### Required Headers
* authenticate


### Return Values
* boolean


### Associated Methods

*  [SoftLayer_Network_Service_Vpn_Overrides::deleteObject](/reference/services/SoftLayer_Network_Service_Vpn_Overrides/deleteObject )




