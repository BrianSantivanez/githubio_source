---
title: "addPortalPermission"
description: "Add a permission to a portal user's permission set. [SoftLayer_User_Customer_CustomerPermission_Permission](/reference/datatypes/SoftLayer_User_Customer_CustomerPermission_Permission) control which features in the SoftLayer customer portal and API a user may use. If the user already has the permission you're attempting to add then addPortalPermission() returns true. 

Users can assign permissions to their child users, but not to themselves. An account's master has all portal permissions and can set permissions for any of the other users on their account. 

Use the [SoftLayer_User_Customer_CustomerPermission_Permission::getAllObjects](/reference/datatypes/$1/#$2) method to retrieve a list of all permissions available in the SoftLayer customer portal and API. Permissions are added based on the keyName property of the permission parameter. "
date: "2018-02-12"
tags:
    - "method"
    - "sldn"
    - "User"
classes:
    - "SoftLayer_User_Customer_OpenIdConnect"
type: "reference"
layout: "method"
mainService : "SoftLayer_User_Customer_OpenIdConnect"
---
