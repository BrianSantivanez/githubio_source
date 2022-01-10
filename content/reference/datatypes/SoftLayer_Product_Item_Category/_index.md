---
title: "SoftLayer_Product_Item_Category"
description: "The SoftLayer_Product_Item_Category data type contains general category information for prices."
layout: "datatype"
tags:
    - "datatype"
    - "sldn"
    - "Product"
classes:
    - "SoftLayer_Product_Item_Category"
---

# SoftLayer_Product_Item_Category
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
    <li id='service'> <a href='/reference/services/SoftLayer_Product_Item_Category' >Service</a></li>    <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Product_Item_Category' >Datatype</a></li>
    </ul>
</div>

## Description 


The SoftLayer_Product_Item_Category data type contains general category information for prices. 





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
[categoryCode]: #categorycode
#### [categoryCode]
The code used to identify this category.  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[id]: #id
#### [id]
identifier for category.  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[name]: #name
#### [name]
The friendly, descriptive name of the category as seen on the order forms and on invoices.  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[quantityLimit]: #quantitylimit
#### [quantityLimit]
Quantity that can be ordered. If 0, it will inherit the quantity from the server quantity ordered. Otherwise it can be specified with the order separately  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[sortOrder]: #sortorder
#### [sortOrder]
The sort order of the category. It may be used to affect the order in which the category may appear in lists (on order forms and invoices).  
<span class="type-label">Type: </span>**integer**  



</div>
</div>
<!-- LOCAL PROPERTY END -->

<div id="relationalProperties"  class="prop-content" >

## Relational
<div class="prop-row">

-----
[billingItems]: #billingitems
#### [billingItems]
The billing items associated with an account that share a category code with an item category's category code.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Billing_Item'>SoftLayer_Billing_Item[] </a>**  



</div>
<div class="prop-row">

-----
[group]: #group
#### [group]
This invoice item's "item category group".   
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Product_Item_Category_Group'>SoftLayer_Product_Item_Category_Group </a>**  



</div>
<div class="prop-row">

-----
[groups]: #groups
#### [groups]
A collection of service offering category groups. Each group contains a collection of items associated with this category.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Product_Package_Item_Category_Group'>SoftLayer_Product_Package_Item_Category_Group[] </a>**  



</div>
<div class="prop-row">

-----
[orderOptions]: #orderoptions
#### [orderOptions]
Any unique options associated with an item category.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Product_Item_Category_Order_Option_Type'>SoftLayer_Product_Item_Category_Order_Option_Type[] </a>**  



</div>
<div class="prop-row">

-----
[packageConfigurations]: #packageconfigurations
#### [packageConfigurations]
A list of configuration available in this category.'  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Product_Package_Order_Configuration'>SoftLayer_Product_Package_Order_Configuration[] </a>**  



</div>
<div class="prop-row">

-----
[presetConfigurations]: #presetconfigurations
#### [presetConfigurations]
A list of preset configurations this category is used in.'  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Product_Package_Preset_Configuration'>SoftLayer_Product_Package_Preset_Configuration[] </a>**  



</div>
<div class="prop-row">

-----
[questionReferences]: #questionreferences
#### [questionReferences]
The question references that are associated with an item category.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Product_Item_Category_Question_Xref'>SoftLayer_Product_Item_Category_Question_Xref[] </a>**  



</div>
<div class="prop-row">

-----
[questions]: #questions
#### [questions]
The questions that are associated with an item category.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Product_Item_Category_Question'>SoftLayer_Product_Item_Category_Question[] </a>**  



</div>

## Count
<div class="prop-row">

-----
[billingItemCount]: #billingitemcount
#### [billingItemCount]
A count of the billing items associated with an account that share a category code with an item category's category code.   
<span class="type-label">Type: </span>**unsigned long**  



</div>
<div class="prop-row">

-----
[groupCount]: #groupcount
#### [groupCount]
A count of a collection of service offering category groups. Each group contains a collection of items associated with this category.   
<span class="type-label">Type: </span>**unsigned long**  



</div>
<div class="prop-row">

-----
[orderOptionCount]: #orderoptioncount
#### [orderOptionCount]
A count of any unique options associated with an item category.   
<span class="type-label">Type: </span>**unsigned long**  



</div>
<div class="prop-row">

-----
[packageConfigurationCount]: #packageconfigurationcount
#### [packageConfigurationCount]
A count of a list of configuration available in this category.'   
<span class="type-label">Type: </span>**unsigned long**  



</div>
<div class="prop-row">

-----
[presetConfigurationCount]: #presetconfigurationcount
#### [presetConfigurationCount]
A count of a list of preset configurations this category is used in.'   
<span class="type-label">Type: </span>**unsigned long**  



</div>
<div class="prop-row">

-----
[questionCount]: #questioncount
#### [questionCount]
A count of the questions that are associated with an item category.   
<span class="type-label">Type: </span>**unsigned long**  



</div>
<div class="prop-row">

-----
[questionReferenceCount]: #questionreferencecount
#### [questionReferenceCount]
A count of the question references that are associated with an item category.   
<span class="type-label">Type: </span>**unsigned long**  



</div>
</div>


