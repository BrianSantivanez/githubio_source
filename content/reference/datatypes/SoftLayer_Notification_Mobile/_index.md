---
title: "SoftLayer_Notification_Mobile"
description: "This is an extension of the SoftLayer_Notification class.  These are implementation details specific to those notificati... "
layout: "datatype"
tags:
    - "datatype"
    - "sldn"
    - "Notification"
classes:
    - "SoftLayer_Notification_Mobile"
---

# SoftLayer_Notification_Mobile
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
    <li id='service'> <a href='/reference/services/SoftLayer_Notification_Mobile' >Service</a></li>    <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Notification_Mobile' >Datatype</a></li>
    </ul>
</div>

## Description 


This is an extension of the SoftLayer_Notification class.  These are implementation details specific to those notifications which can be subscribed to and received on a mobile device. 





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
Unique identifier for the notification.   
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[keyName]: #keyname
#### [keyName]
Name that can be used by external systems to refer to a notification.   
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[name]: #name
#### [name]
Friendly name for the notification.   
<span class="type-label">Type: </span>**string**  



</div>
</div>
<!-- LOCAL PROPERTY END -->

<div id="relationalProperties"  class="prop-content" >

## Relational
<div class="prop-row">

-----
[preferences]: #preferences
#### [preferences]
The preferences related to the notification. These are preferences are configurable and optional for subscribers to use.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Notification_Preference'>SoftLayer_Notification_Preference[] </a>**  



</div>
<div class="prop-row">

-----
[requiredPreferences]: #requiredpreferences
#### [requiredPreferences]
The required preferences related to the notification. While configurable, the subscriber does not have the option whether to use the preference.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Notification_Preference'>SoftLayer_Notification_Preference[] </a>**  



</div>

## Count
<div class="prop-row">

-----
[preferenceCount]: #preferencecount
#### [preferenceCount]
A count of the preferences related to the notification. These are preferences are configurable and optional for subscribers to use.   
<span class="type-label">Type: </span>**unsigned long**  



</div>
<div class="prop-row">

-----
[requiredPreferenceCount]: #requiredpreferencecount
#### [requiredPreferenceCount]
A count of the required preferences related to the notification. While configurable, the subscriber does not have the option whether to use the preference.   
<span class="type-label">Type: </span>**unsigned long**  



</div>
</div>


