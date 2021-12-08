---
title: "getObject"
description: "Each product item category must be tied to a category group. These category groups describe how a particular product ite... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Product"
classes:
    - "SoftLayer_Product_Item_Category_Group"
aliases:
    - "/reference/services/softlayer_product_item_category_group/getObject"
---
# [SoftLayer_Product_Item_Category_Group](/reference/services/SoftLayer_Product_Item_Category_Group)::getObject


Retrieve a SoftLayer_Product_Item_Category_Group record.


## Overview 
Each product item category must be tied to a category group. These category groups describe how a particular product item category is categorized. For example, the disk0, disk1, ... disk11 can be categorized as Server and Attached Services. There are different groups for each of this product item category depending on the function of the item product in the subject category. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* SoftLayer_Product_Item_Category_GroupInitParameters
* authenticate


### Optional Headers
* SoftLayer_Product_Item_Category_GroupObjectMask
* SoftLayer_Product_Item_Category_GroupObjectFilter
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Product_Item_Category_Group'>SoftLayer_Product_Item_Category_Group </a>




