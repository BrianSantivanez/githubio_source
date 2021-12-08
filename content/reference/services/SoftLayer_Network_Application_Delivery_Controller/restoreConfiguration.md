---
title: "restoreConfiguration"
description: "Restore an application delivery controller's configuration state."
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Application_Delivery_Controller"
aliases:
    - "/reference/services/softlayer_network_application_delivery_controller/restoreConfiguration"
---
# [SoftLayer_Network_Application_Delivery_Controller](/reference/services/SoftLayer_Network_Application_Delivery_Controller)::restoreConfiguration


Restore an application delivery controller's configuration state.


## Overview 
Restore an application delivery controller's configuration state. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|configurationHistoryId| integer| The id of a SoftLayer_Network_Application_Delivery_Controller_Configuration_History record to restore.|


### Required Headers
* authenticate
* SoftLayer_Network_Application_Delivery_ControllerInitParameters


### Return Values
* boolean


### Associated Methods

*  [SoftLayer_Network_Application_Delivery_Controller::getConfigurationHistory](/reference/services/SoftLayer_Network_Application_Delivery_Controller/getConfigurationHistory )
*  [SoftLayer_Network_Application_Delivery_Controller::saveCurrentConfiguration](/reference/services/SoftLayer_Network_Application_Delivery_Controller/saveCurrentConfiguration )
*  [SoftLayer_Network_Application_Delivery_Controller::restoreBaseConfiguration](/reference/services/SoftLayer_Network_Application_Delivery_Controller/restoreBaseConfiguration )




