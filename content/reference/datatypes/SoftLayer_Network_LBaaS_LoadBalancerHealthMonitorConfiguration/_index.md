---
title: "SoftLayer_Network_LBaaS_LoadBalancerHealthMonitorConfiguration"
description: "SoftLayer_Network_LBaaS_LoadBalancerHealthMonitorConfiguration specifies the check method to be used for health monitori... "
layout: "datatype"
tags:
    - "datatype"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_LBaaS_LoadBalancerHealthMonitorConfiguration"
---

# SoftLayer_Network_LBaaS_LoadBalancerHealthMonitorConfiguration
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
        <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Network_LBaaS_LoadBalancerHealthMonitorConfiguration' >Datatype</a></li>
    </ul>
</div>

## Description 


SoftLayer_Network_LBaaS_LoadBalancerHealthMonitorConfiguration specifies the check method to be used for health monitoring backend members. 





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
[backendPort]: #backendport
#### [backendPort]
Backends port  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[backendProtocol]: #backendprotocol
#### [backendProtocol]
Backends protocol. Valid values are "TCP", "HTTP"   
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[healthMonitorUuid]: #healthmonitoruuid
#### [healthMonitorUuid]
Health Monitor UUID, required for update only  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[interval]: #interval
#### [interval]
<<< EOT Interval in seconds to perform  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[maxRetries]: #maxretries
#### [maxRetries]
Max number of retries until the member is considered as DOWN   
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[timeout]: #timeout
#### [timeout]
Health check methods timeout in  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[urlPath]: #urlpath
#### [urlPath]
If monitor is "HTTP", this specifies URL path  
<span class="type-label">Type: </span>**string**  



</div>
</div>
<!-- LOCAL PROPERTY END -->

</div>


