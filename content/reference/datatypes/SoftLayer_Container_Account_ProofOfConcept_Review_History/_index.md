---
title: "SoftLayer_Container_Account_ProofOfConcept_Review_History"
description: "Summary of review activity for a proof of concept request."
layout: "datatype"
tags:
    - "datatype"
    - "sldn"
    - "Container"
classes:
    - "SoftLayer_Container_Account_ProofOfConcept_Review_History"
---

# SoftLayer_Container_Account_ProofOfConcept_Review_History
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
        <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Container_Account_ProofOfConcept_Review_History' >Datatype</a></li>
    </ul>
</div>

## Description 


Summary of review activity for a proof of concept request. 





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
[accountCreatedFlag]: #accountcreatedflag
#### [accountCreatedFlag]
True for approved requests associated with a new account and false otherwise.  
<span class="type-label">Type: </span>**boolean**  



</div>
<div class="prop-row">

-----
[deniedFlag]: #deniedflag
#### [deniedFlag]
True for denied requests and false otherwise.  
<span class="type-label">Type: </span>**boolean**  



</div>
<div class="prop-row">

-----
[events]: #events
#### [events]
List of events occurring during the review.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Container_Account_ProofOfConcept_Review_Event'>SoftLayer_Container_Account_ProofOfConcept_Review_Event[] </a>**  



</div>
<div class="prop-row">

-----
[reviewCompleteFlag]: #reviewcompleteflag
#### [reviewCompleteFlag]
True for fully reviewed requests and false otherwise.  
<span class="type-label">Type: </span>**boolean**  



</div>
</div>
<!-- LOCAL PROPERTY END -->

</div>


