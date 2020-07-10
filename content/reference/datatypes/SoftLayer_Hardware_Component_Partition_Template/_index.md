---
title: "SoftLayer_Hardware_Component_Partition_Template"
description: "The SoftLayer_Hardware_Component_Partition_Template data type contains general information relating to a single SoftLaye... "
layout: "datatype"
tags:
    - "datatype"
    - "sldn"
    - "Hardware"
classes:
    - "SoftLayer_Hardware_Component_Partition_Template"
---

# SoftLayer_Hardware_Component_Partition_Template
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
    <li id='service'> <a href='/reference/services/SoftLayer_Hardware_Component_Partition_Template' >Service</a></li>    <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Hardware_Component_Partition_Template' >Datatype</a></li>
    </ul>
</div>

## Description 
The SoftLayer_Hardware_Component_Partition_Template data type contains general information relating to a single SoftLayer partition template.  Partition templates group 1 or more partition configurations that can be used to predefine how a hard drive's partitions will be configured. 


### associatedMethods

*  [SoftLayer_Hardware_Component_Partition_Template::getData](/reference/services/SoftLayer_Hardware_Component_Partition_Template/getData )
*  [SoftLayer_Hardware_Component_Partition_Template::getPartitionTemplatePartition](/reference/services/SoftLayer_Hardware_Component_Partition_Template/getPartitionTemplatePartition )





<!-- Filer BEGIN -->
<div class="view-filters">
        <div class="clearfix">
            <div class="search-input-box">
                <input placeholder="Datatype Filter" onkeyup="titleSearch(inputId='prop-input', divId='properties', elementClass='prop-row')" 
                    type="text" id="prop-input" value="" size="30" maxlength="128" class="form-text">
            </div>
        </div>
</div>
<!-- Filer END -->

<div id="properties" class="content">
<div id="localProperties" class="prop-content" >

## Local
<div class="prop-row">

-----
[accountId]: #accountid
#### [accountId]
A partition template's owner. The [SoftLayer_Account]({{<ref "reference/datatypes/SoftLayer_Account">}}) that a template was created by.  
<span class="type-label">Type: </span>**integer**


</div>
<div class="prop-row">

-----
[description]: #description
#### [description]
A partition template's description.  
<span class="type-label">Type: </span>**string**


</div>
<div class="prop-row">

-----
[id]: #id
#### [id]
A partition template's id.  
<span class="type-label">Type: </span>**integer**


</div>
<div class="prop-row">

-----
[partitionOperatingSystemId]: #partitionoperatingsystemid
#### [partitionOperatingSystemId]
A partition template's associated [SoftLayer_Hardware_Component_Partition_OperatingSystem]({{<ref "reference/datatypes/SoftLayer_Hardware_Component_Partition_OperatingSystem">}}) Id.  
<span class="type-label">Type: </span>**integer**


</div>
<div class="prop-row">

-----
[statusCode]: #statuscode
#### [statusCode]
A partition template's status code. ACTIVE ,INACTIVE.  
<span class="type-label">Type: </span>**string**


</div>
<div class="prop-row">

-----
[templateType]: #templatetype
#### [templateType]
A partition template's Type. SYSTEM - template generated by softlayer.  CUSTOM - templates generated by SoftLayer customers.  
<span class="type-label">Type: </span>**string**


</div>
</div>
<!-- LOCAL PROPERTY END -->

<div id="relationalProperties"  class="prop-content" >

## Relational
<div class="prop-row">

-----
[account]: #account
#### [account]
A partition template's associated [SoftLayer_Account]({{<ref "reference/datatypes/SoftLayer_Account">}}).  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Account'>SoftLayer_Account </a>**


</div>
<div class="prop-row">

-----
[data]: #data
#### [data]
An individual partition for a partition template. This is identical to 'partitionTemplatePartition' except this will sort unix partitions.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Hardware_Component_Partition_Template_Partition'>SoftLayer_Hardware_Component_Partition_Template_Partition[] </a>**


</div>
<div class="prop-row">

-----
[expireDate]: #expiredate
#### [expireDate]
  
<span class="type-label">Type: </span>**string**


</div>
<div class="prop-row">

-----
[partitionOperatingSystem]: #partitionoperatingsystem
#### [partitionOperatingSystem]
A partition template's associated [SoftLayer_Hardware_Component_Partition_OperatingSystem]({{<ref "reference/datatypes/SoftLayer_Hardware_Component_Partition_OperatingSystem">}}).  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Hardware_Component_Partition_OperatingSystem'>SoftLayer_Hardware_Component_Partition_OperatingSystem </a>**


</div>
<div class="prop-row">

-----
[partitionTemplatePartition]: #partitiontemplatepartition
#### [partitionTemplatePartition]
An individual partition for a partition template.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Hardware_Component_Partition_Template_Partition'>SoftLayer_Hardware_Component_Partition_Template_Partition[] </a>**


</div>

## Count
<div class="prop-row">

-----
[dataCount]: #datacount
#### [dataCount]
A count of an individual partition for a partition template. This is identical to 'partitionTemplatePartition' except this will sort unix partitions.   
<span class="type-label">Type: </span>**unsigned long**


</div>
<div class="prop-row">

-----
[partitionTemplatePartitionCount]: #partitiontemplatepartitioncount
#### [partitionTemplatePartitionCount]
A count of an individual partition for a partition template.   
<span class="type-label">Type: </span>**unsigned long**


</div>
</div>

