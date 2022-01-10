---
title: "SoftLayer_Monitoring_Robot_Status"
description: "DEPRECATED. Your monitoring robot will be in 'Active' status under normal circumstances. If you perform an OS reload, yo... "
layout: "datatype"
tags:
    - "datatype"
    - "sldn"
    - "Monitoring"
classes:
    - "SoftLayer_Monitoring_Robot_Status"
---

# SoftLayer_Monitoring_Robot_Status
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
        <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Monitoring_Robot_Status' >Datatype</a></li>
    </ul>
</div>

## Description 


DEPRECATED. Your monitoring robot will be in "Active" status under normal circumstances. If you perform an OS reload, your robot will be in "Reclaim" status until it's reloaded on your server or virtual server. 

Advanced monitoring system requires "Nimsoft Monitoring (Advanced)" service running and TCP ports 48000 - 48020 to be open on your server or virtual server. Monitoring agents cannot be managed nor can the usage data be updated if these ports are closed. Your monitoring robot will be in "Limited Connectivity" status if our monitoring management system cannot communicate with your system. 

See [SoftLayer_Monitoring_Robot::resetStatus]({{<ref "reference/services/SoftLayer_Monitoring_Robot/resetStatus">}}) service for more details. 





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
DEPRECATED. Monitoring robot status description  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[id]: #id
#### [id]
DEPRECATED. Internal identifier of a monitoring robot status  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[name]: #name
#### [name]
DEPRECATED. Monitoring robot status name  
<span class="type-label">Type: </span>**string**  



</div>
</div>
<!-- LOCAL PROPERTY END -->

</div>


