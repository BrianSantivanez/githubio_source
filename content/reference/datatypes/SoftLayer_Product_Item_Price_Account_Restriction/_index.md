---
title: "SoftLayer_Product_Item_Price_Account_Restriction"
description: "The SoftLayer_Product_Item_Price data type gives more information about the item price restrictions.  An item price may... "
layout: "datatype"
tags:
    - "datatype"
    - "sldn"
    - "Product"
classes:
    - "SoftLayer_Product_Item_Price_Account_Restriction"
---

# SoftLayer_Product_Item_Price_Account_Restriction
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
        <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Product_Item_Price_Account_Restriction' >Datatype</a></li>
    </ul>
</div>

## Description 


The SoftLayer_Product_Item_Price data type gives more information about the item price restrictions.  An item price may be restricted to one or more accounts. If the item price is restricted to an account, only that account will see the restriction details. 





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
The account id for the item price account restriction.  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[id]: #id
#### [id]
The unique identifier for the item price account restriction.  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[itemPriceId]: #itempriceid
#### [itemPriceId]
The item price id for the item price account restriction.  
<span class="type-label">Type: </span>**integer**  



</div>
</div>
<!-- LOCAL PROPERTY END -->

<div id="relationalProperties"  class="prop-content" >

## Relational
<div class="prop-row">

-----
[account]: #account
#### [account]
The account the item price is restricted to.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Account'>SoftLayer_Account </a>**  



</div>
<div class="prop-row">

-----
[itemPrice]: #itemprice
#### [itemPrice]
The item price that has the account restriction.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Product_Item_Price'>SoftLayer_Product_Item_Price </a>**  



</div>

## Count
</div>


