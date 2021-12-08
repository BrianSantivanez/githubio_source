---
title: "deleteAddressTranslation"
description: "Remove an existing address translation from a network tunnel. 

Address translations deliver packets to a destination ip... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Tunnel_Module_Context"
aliases:
    - "/reference/services/softlayer_network_tunnel_module_context/deleteAddressTranslation"
---
# [SoftLayer_Network_Tunnel_Module_Context](/reference/services/SoftLayer_Network_Tunnel_Module_Context)::deleteAddressTranslation


Delete an address translation from a network tunnel


## Overview 
Remove an existing address translation from a network tunnel. 

Address translations deliver packets to a destination ip address that is on a customer subnet (remote). 

NOTE:  A network tunnel's configurations must be applied to the network device in order for an address translation to be deleted. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|translationId| integer| The internal identifier for an address translation that needs to be removed for an IPSec network tunnel.|


### Required Headers
* authenticate
* SoftLayer_Network_Tunnel_Module_ContextInitParameters


### Return Values
* boolean


### Associated Methods

*  [SoftLayer_Network_Tunnel_Module_Context::createAddressTranslation](/reference/services/SoftLayer_Network_Tunnel_Module_Context/createAddressTranslation )
*  [SoftLayer_Network_Tunnel_Module_Context::createAddressTranslations](/reference/services/SoftLayer_Network_Tunnel_Module_Context/createAddressTranslations )
*  [SoftLayer_Network_Tunnel_Module_Context::editAddressTranslation](/reference/services/SoftLayer_Network_Tunnel_Module_Context/editAddressTranslation )
*  [SoftLayer_Network_Tunnel_Module_Context::editAddressTranslations](/reference/services/SoftLayer_Network_Tunnel_Module_Context/editAddressTranslations )
*  [SoftLayer_Network_Tunnel_Module_Context::applyConfigurationsToDevice](/reference/services/SoftLayer_Network_Tunnel_Module_Context/applyConfigurationsToDevice )
*  [SoftLayer_Network_Tunnel_Module_Context::editObject](/reference/services/SoftLayer_Network_Tunnel_Module_Context/editObject )




