---
title: "SoftLayer_Notification_Occurrence_Event"
description: "The [SoftLayer_Notification_Occurrence_Event]({{<ref 'reference/datatypes/SoftLayer_Notification_Occurrence_Event'>}}) s... "
date: "2018-02-12"
layout: "service"
tags:
    - "service"
    - "sldn"
    - "Notification"
classes:
    - "SoftLayer_Notification_Occurrence_Event"
---
# SoftLayer_Notification_Occurrence_Event
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
    <li id='service'> <a href='/reference/services/SoftLayer_Notification_Occurrence_Event' >Service</a></li>    <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Notification_Occurrence_Event' >Datatype</a></li>
    </ul>
</div>

## Description


The [SoftLayer_Notification_Occurrence_Event]({{<ref "reference/datatypes/SoftLayer_Notification_Occurrence_Event">}}) service represents all events with potential to cause a disruption in service. 



        
<div id="properties" class="content service-content">

## Methods

<div class="view-filters">
    <div class="clearfix">
        <div class="search-input-box">
            <input placeholder="Method Filter" onkeyup="titleSearch(inputId='edit-combine', divId='method-div', elementClass='method-row')" 
                type="text" id="edit-combine" value="" size="30" maxlength="128" class="form-text">
        </div>
    </div>
</div>

<div id="method-div">

<div class="method-row">

#### [acknowledgeNotification](/reference/services/SoftLayer_Notification_Occurrence_Event/acknowledgeNotification)


</div>

<div class="method-row">

#### [getAcknowledgedFlag](/reference/services/SoftLayer_Notification_Occurrence_Event/getAcknowledgedFlag)
Retrieve indicates whether or not this event has been acknowledged by the user.

</div>

<div class="method-row">

#### [getAllObjects](/reference/services/SoftLayer_Notification_Occurrence_Event/getAllObjects)


</div>

<div class="method-row">

#### [getAttachedFile](/reference/services/SoftLayer_Notification_Occurrence_Event/getAttachedFile)
Retrieve a file attached to an event.

</div>

<div class="method-row">

#### [getAttachments](/reference/services/SoftLayer_Notification_Occurrence_Event/getAttachments)
Retrieve a collection of attachments for this event which provide supplementary information to impacted users some examples are RFO (Reason For Outage) and root cause analysis documents.

</div>

<div class="method-row">

#### [getFirstUpdate](/reference/services/SoftLayer_Notification_Occurrence_Event/getFirstUpdate)
Retrieve the first update for this event.

</div>

<div class="method-row">

#### [getImpactedAccountCount](/reference/services/SoftLayer_Notification_Occurrence_Event/getImpactedAccountCount)
Get the number of impacted owned accounts for the current user.

</div>

<div class="method-row">

#### [getImpactedAccounts](/reference/services/SoftLayer_Notification_Occurrence_Event/getImpactedAccounts)
Retrieve a collection of accounts impacted by this event. Each impacted account record relates directly to a [SoftLayer_Account]({{<ref "reference/datatypes/SoftLayer_Account">}}).

</div>

<div class="method-row">

#### [getImpactedDeviceCount](/reference/services/SoftLayer_Notification_Occurrence_Event/getImpactedDeviceCount)
Get the number of impacted devices.

</div>

<div class="method-row">

#### [getImpactedDevices](/reference/services/SoftLayer_Notification_Occurrence_Event/getImpactedDevices)
Get devices impacted by this event

</div>

<div class="method-row">

#### [getImpactedResources](/reference/services/SoftLayer_Notification_Occurrence_Event/getImpactedResources)
Retrieve a collection of resources impacted by this event. Each record will relate to some physical resource that the user has access to such as [SoftLayer_Hardware]({{<ref "reference/datatypes/SoftLayer_Hardware">}}) or [SoftLayer_Virtual_Guest]({{<ref "reference/datatypes/SoftLayer_Virtual_Guest">}}).

</div>

<div class="method-row">

#### [getImpactedUsers](/reference/services/SoftLayer_Notification_Occurrence_Event/getImpactedUsers)
Retrieve a collection of users impacted by this event. Each impacted user record relates directly to a [SoftLayer_User_Customer]({{<ref "reference/datatypes/SoftLayer_User_Customer">}}).

</div>

<div class="method-row">

#### [getLastUpdate](/reference/services/SoftLayer_Notification_Occurrence_Event/getLastUpdate)
Retrieve the last update for this event.

</div>

<div class="method-row">

#### [getNotificationOccurrenceEventType](/reference/services/SoftLayer_Notification_Occurrence_Event/getNotificationOccurrenceEventType)
Retrieve the type of event such as planned or unplanned maintenance.

</div>

<div class="method-row">

#### [getObject](/reference/services/SoftLayer_Notification_Occurrence_Event/getObject)
Retrieve a SoftLayer_Notification_Occurrence_Event record.

</div>

<div class="method-row">

#### [getStatusCode](/reference/services/SoftLayer_Notification_Occurrence_Event/getStatusCode)


</div>

<div class="method-row">

#### [getUpdates](/reference/services/SoftLayer_Notification_Occurrence_Event/getUpdates)
Retrieve all updates for this event.

</div>
</div>

</div>

