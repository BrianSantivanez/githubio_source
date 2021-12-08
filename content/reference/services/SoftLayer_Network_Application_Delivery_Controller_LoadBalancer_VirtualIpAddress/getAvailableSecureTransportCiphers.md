---
title: "getAvailableSecureTransportCiphers"
description: "Yields a list of the SSL/TLS encryption ciphers that are currently supported on this virtual IP address instance."
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress"
aliases:
    - "/reference/services/softlayer_network_application_delivery_controller_loadbalancer_virtualipaddress/getAvailableSecureTransportCiphers"
---
# [SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress](/reference/services/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress)::getAvailableSecureTransportCiphers


Lists the SSL encryption ciphers available to this virtual IP address


## Overview 
Yields a list of the SSL/TLS encryption ciphers that are currently supported on this virtual IP address instance. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* authenticate
* SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddressInitParameters


### Return Values
* <a href='/reference/datatypes/SoftLayer_Security_SecureTransportCipher'>SoftLayer_Security_SecureTransportCipher[] </a>


### Associated Methods

*  [SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress::getAvailableSecureTransportProtocols](/reference/services/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress/getAvailableSecureTransportProtocols )




