---
title: "getLoadBalancerVirtualIpAddresses"
description: "Retrieve the load balancers virtual IP addresses currently associated with the certificate."
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Security"
classes:
    - "SoftLayer_Security_Certificate"
aliases:
    - "/reference/services/softlayer_security_certificate/getLoadBalancerVirtualIpAddresses"
---
# [SoftLayer_Security_Certificate](/reference/services/SoftLayer_Security_Certificate)::getLoadBalancerVirtualIpAddresses


Retrieve the load balancers virtual IP addresses currently associated with the certificate.


## Overview 
Retrieve the load balancers virtual IP addresses currently associated with the certificate.

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* SoftLayer_Security_CertificateInitParameters
* authenticate


### Optional Headers
* SoftLayer_Security_CertificateObjectMask
* SoftLayer_Security_CertificateObjectFilter
* resultLimit
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress'>SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress[] </a>




