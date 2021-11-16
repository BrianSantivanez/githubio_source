---
title: "SoftLayer_Container_Network_Storage_Evault_WebCc_JobDetails"
description: "The SoftLayer_Container_Network_Storage_Evault_WebCc_JobDetails will contain basic details for all backup and restore jo... "
layout: "datatype"
tags:
    - "datatype"
    - "sldn"
    - "Container"
classes:
    - "SoftLayer_Container_Network_Storage_Evault_WebCc_JobDetails"
---

# SoftLayer_Container_Network_Storage_Evault_WebCc_JobDetails
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
        <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Container_Network_Storage_Evault_WebCc_JobDetails' >Datatype</a></li>
    </ul>
</div>

## Description 


The SoftLayer_Container_Network_Storage_Evault_WebCc_JobDetails will contain basic details for all backup and restore jobs performed by the StorageLayer EVault service offering. 


### associatedMethods

*  [SoftLayer_Network_Storage_Backup_Evault::getAgentStatuses](/reference/services/SoftLayer_Network_Storage_Backup_Evault/getAgentStatuses )
*  [SoftLayer_Network_Storage_Backup_Evault::getTasks](/reference/services/SoftLayer_Network_Storage_Backup_Evault/getTasks )





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
[bytesUsed]: #bytesused
#### [bytesUsed]
The number of bytes currently used by the backup job. (provided only for backup jobs)  
<span class="type-label">Type: </span>**unsigned long**  



</div>
<div class="prop-row">

-----
[description]: #description
#### [description]
Description of the backup/restore job  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[hardwareId]: #hardwareid
#### [hardwareId]
hardware id  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[lastRunDate]: #lastrundate
#### [lastRunDate]
Date of the last jobrun.  
<span class="type-label">Type: </span>**dateTime**  



</div>
<div class="prop-row">

-----
[name]: #name
#### [name]
Name of the backup/restore job  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[originalSize]: #originalsize
#### [originalSize]
Size of backup job when it was first run. (provided only for backup jobs)  
<span class="type-label">Type: </span>**unsigned long**  



</div>
<div class="prop-row">

-----
[percentageOfTotalUsage]: #percentageoftotalusage
#### [percentageOfTotalUsage]
Percentage of overall used space allocated by the job. (provided only for backup jobs)  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[result]: #result
#### [result]
Result of the latest jobrun.  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[virtualGuestId]: #virtualguestid
#### [virtualGuestId]
virtual guest id  
<span class="type-label">Type: </span>**integer**  



</div>
</div>
<!-- LOCAL PROPERTY END -->

</div>


