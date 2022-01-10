---
title: "SoftLayer_Product_Item_Requirement"
description: "The SoftLayer_Product_Item_Requirement data type contains information relating to what requirements, if any, exist for a... "
layout: "datatype"
tags:
    - "datatype"
    - "sldn"
    - "Product"
classes:
    - "SoftLayer_Product_Item_Requirement"
---

# SoftLayer_Product_Item_Requirement
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
        <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Product_Item_Requirement' >Datatype</a></li>
    </ul>
</div>

## Description 


The SoftLayer_Product_Item_Requirement data type contains information relating to what requirements, if any, exist for an item. The requiredItemId local property is the item id that is required. 



### seeAlso

* [SoftLayer_Product_Conflict](/reference/datatypes/SoftLayer_Product_Conflict )




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
[id]: #id
#### [id]
Identifier for this record.  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[itemId]: #itemid
#### [itemId]
This is the id of the item affected by the requirement.  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[message]: #message
#### [message]
This is a custom message to display to the user when this requirement shortfall arises.  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[requiredItemId]: #requireditemid
#### [requiredItemId]
This is the id of the item required.  
<span class="type-label">Type: </span>**integer**  



</div>
</div>
<!-- LOCAL PROPERTY END -->

<div id="relationalProperties"  class="prop-content" >

## Relational
<div class="prop-row">

-----
[item]: #item
#### [item]
Item requirement applies to.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Product_Item'>SoftLayer_Product_Item </a>**  



</div>
<div class="prop-row">

-----
[product]: #product
#### [product]
The product containing the requirement.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Product_Item'>SoftLayer_Product_Item </a>**  



</div>

## Count
</div>


