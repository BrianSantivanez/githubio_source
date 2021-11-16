---
title: "getActivePackagesByAttribute"
description: "<strong>This method is deprecated and should not be used in production code.</strong> 

This method will return the [Sof... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Account"
classes:
    - "SoftLayer_Account"
aliases:
    - "/reference/services/softlayer_account/getActivePackagesByAttribute"
---
# [SoftLayer_Account](/reference/services/SoftLayer_Account)::getActivePackagesByAttribute

<div class="deprecated"><span class="deprecation-label">Deprecated </span></div>

[<strong>DEPRECATED</strong>] Retrieve the active [SoftLayer_Product_Package]({{<ref "reference/datatypes/SoftLayer_Product_Package">}}) objects from which you can order a server, service or software filtered by an attribute type ([SoftLayer_Product_Package_Attribute_Type]({{<ref "reference/datatypes/SoftLayer_Product_Package_Attribute_Type">}})) on the package. 


## Overview 
<strong>This method is deprecated and should not be used in production code.</strong> 

This method will return the [SoftLayer_Product_Package]({{<ref "reference/datatypes/SoftLayer_Product_Package">}}) objects from which you can order a bare metal server, virtual server, service (such as CDN or Object Storage) or other software filtered by an attribute type associated with the package. Once you have the package you want to order from, you may query one of various endpoints from that package to get specific information about its products and pricing. See [SoftLayer_Product_Package::getCategories]({{<ref "reference/services/SoftLayer_Product_Package/getCategories">}}) for more information. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|attributeKeyName| string| the attribute key name|


### Required Headers
* authenticate


### Optional Headers
* SoftLayer_AccountObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Product_Package'>SoftLayer_Product_Package[] </a>


### Associated Methods

*  [SoftLayer_Product_Package::getActivePackagesByAttribute](/reference/services/SoftLayer_Product_Package/getActivePackagesByAttribute )




