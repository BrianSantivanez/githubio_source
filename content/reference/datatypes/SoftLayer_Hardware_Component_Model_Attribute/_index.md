---
title: "SoftLayer_Hardware_Component_Model_Attribute"
description: "The SoftLayer_Hardware_Component__Model_Attribute data type contains general information relating to a single hardware s... "
layout: "datatype"
tags:
    - "datatype"
    - "sldn"
    - "Hardware"
classes:
    - "SoftLayer_Hardware_Component_Model_Attribute"
---

# SoftLayer_Hardware_Component_Model_Attribute
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
        <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Hardware_Component_Model_Attribute' >Datatype</a></li>
    </ul>
</div>

## Description 


The SoftLayer_Hardware_Component__Model_Attribute data type contains general information relating to a single hardware setting or attribute for a component model. 





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
[attributeTypeId]: #attributetypeid
#### [attributeTypeId]
A hardware component model attribute's associated [SoftLayer_Hardware_Component_Model_Attribute_Type]({{<ref "reference/datatypes/SoftLayer_Hardware_Component_Model_Attribute_Type">}}) Id.  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[hardwareComponentModelId]: #hardwarecomponentmodelid
#### [hardwareComponentModelId]
A hardware component model attribute's associated [SoftLayer_Hardware_Component_Model]({{<ref "reference/datatypes/SoftLayer_Hardware_Component_Model">}}) Id.  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[value]: #value
#### [value]
A hardware component model attribute's value.  A value can have many different values depending on the attributes [SoftLayer_Hardware_Component_Model_Attribute_Type]({{<ref "reference/datatypes/SoftLayer_Hardware_Component_Model_Attribute_Type">}}).  
<span class="type-label">Type: </span>**string**  



</div>
</div>
<!-- LOCAL PROPERTY END -->

<div id="relationalProperties"  class="prop-content" >

## Relational
<div class="prop-row">

-----
[hardwareComponent]: #hardwarecomponent
#### [hardwareComponent]
  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Hardware_Component_Model'>SoftLayer_Hardware_Component_Model </a>**  



</div>
<div class="prop-row">

-----
[hardwareComponentAttributeType]: #hardwarecomponentattributetype
#### [hardwareComponentAttributeType]
  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Hardware_Component_Model_Attribute_Type'>SoftLayer_Hardware_Component_Model_Attribute_Type </a>**  



</div>

## Count
</div>


