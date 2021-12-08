---
title: "getDiskImages"
description: "Retrieve the [SoftLayer_Virtual_Disk_Image]({{<ref 'reference/datatypes/SoftLayer_Virtual_Disk_Image'>}}) that are in a... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Virtual"
classes:
    - "SoftLayer_Virtual_Storage_Repository"
aliases:
    - "/reference/services/softlayer_virtual_storage_repository/getDiskImages"
---
# [SoftLayer_Virtual_Storage_Repository](/reference/services/SoftLayer_Virtual_Storage_Repository)::getDiskImages


Retrieve the [SoftLayer_Virtual_Disk_Image]({{<ref "reference/datatypes/SoftLayer_Virtual_Disk_Image">}}) that are in a storage repository. Disk images are the virtual hard drives for a virtual guest.


## Overview 
Retrieve the [SoftLayer_Virtual_Disk_Image]({{<ref "reference/datatypes/SoftLayer_Virtual_Disk_Image">}}) that are in a storage repository. Disk images are the virtual hard drives for a virtual guest.

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* SoftLayer_Virtual_Storage_RepositoryInitParameters
* authenticate


### Optional Headers
* SoftLayer_Virtual_Storage_RepositoryObjectMask
* SoftLayer_Virtual_Storage_RepositoryObjectFilter
* resultLimit
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Virtual_Disk_Image'>SoftLayer_Virtual_Disk_Image[] </a>




