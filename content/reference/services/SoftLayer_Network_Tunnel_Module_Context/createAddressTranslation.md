---
title: "createAddressTranslation"
description: "Create an address translation for a network tunnel. 

To create an address translation, ip addresses from an assigned /3... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Tunnel_Module_Context"
aliases:
    - "/reference/services/softlayer_network_tunnel_module_context/createAddressTranslation"
---
# [SoftLayer_Network_Tunnel_Module_Context](/reference/services/SoftLayer_Network_Tunnel_Module_Context)::createAddressTranslation


Create an address translation for a network tunnel


## Overview 
Create an address translation for a network tunnel. 

To create an address translation, ip addresses from an assigned /30 static route subnet are used.  Address translations deliver packets to a destination ip address that is on a customer (remote) subnet. 

NOTE:  A network tunnel's configurations must be applied to the network device in order for an address translation to be created. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|translation| <a href='/reference/datatypes/SoftLayer_Network_Tunnel_Module_Context_Address_Translation'>SoftLayer_Network_Tunnel_Module_Context_Address_Translation </a>| The address translation to create for an IPSec network tunnel.|


### Required Headers
* authenticate
* SoftLayer_Network_Tunnel_Module_ContextInitParameters


### Optional Headers
* SoftLayer_Network_Tunnel_Module_ContextObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Network_Tunnel_Module_Context_Address_Translation'>SoftLayer_Network_Tunnel_Module_Context_Address_Translation </a>


### Associated Methods

*  [SoftLayer_Network_Tunnel_Module_Context::createAddressTranslations](/reference/services/SoftLayer_Network_Tunnel_Module_Context/createAddressTranslations )
*  [SoftLayer_Network_Tunnel_Module_Context::editAddressTranslation](/reference/services/SoftLayer_Network_Tunnel_Module_Context/editAddressTranslation )
*  [SoftLayer_Network_Tunnel_Module_Context::editAddressTranslations](/reference/services/SoftLayer_Network_Tunnel_Module_Context/editAddressTranslations )
*  [SoftLayer_Network_Tunnel_Module_Context::deleteAddressTranslation](/reference/services/SoftLayer_Network_Tunnel_Module_Context/deleteAddressTranslation )
*  [SoftLayer_Network_Tunnel_Module_Context::applyConfigurationsToDevice](/reference/services/SoftLayer_Network_Tunnel_Module_Context/applyConfigurationsToDevice )




