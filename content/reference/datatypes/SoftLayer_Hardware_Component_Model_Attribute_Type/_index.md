---
title: "SoftLayer_Hardware_Component_Model_Attribute_Type"
description: "The SoftLayer_Hardware_Component_Model_Attribute_Type data type contains general information for the type of an attribut... "
layout: "datatype"
tags:
    - "datatype"
    - "sldn"
    - "Hardware"
classes:
    - "SoftLayer_Hardware_Component_Model_Attribute_Type"
---

# SoftLayer_Hardware_Component_Model_Attribute_Type
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
        <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Hardware_Component_Model_Attribute_Type' >Datatype</a></li>
    </ul>
</div>

## Description 


The SoftLayer_Hardware_Component_Model_Attribute_Type data type contains general information for the type of an attribute for a hardware component model. 





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
[description]: #description
#### [description]
The description for the data that a hardware component model type's [SoftLayer_Hardware_Component_Model_Attribute]({{<ref "reference/datatypes/SoftLayer_Hardware_Component_Model_Attribute">}}) contains.  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[id]: #id
#### [id]
A hardware component model attribute type's Id.  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[keyName]: #keyname
#### [keyName]
A hardware component model attribute type's unique name.  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[name]: #name
#### [name]
A hardware component model attribute type's name.  
<span class="type-label">Type: </span>**string**  



</div>
</div>
<!-- LOCAL PROPERTY END -->

<div id="relationalProperties"  class="prop-content" >

## Relational
<div class="prop-row">

-----
[validComponentTypes]: #validcomponenttypes
#### [validComponentTypes]
  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Hardware_Component_Type'>SoftLayer_Hardware_Component_Type[] </a>**  



</div>

## Count
<div class="prop-row">

-----
[validComponentTypeCount]: #validcomponenttypecount
#### [validComponentTypeCount]
A count of    
<span class="type-label">Type: </span>**unsigned long**  



</div>
</div>


