---
title: "SoftLayer_Billing_Order"
description: "The SoftLayer_Billing_Order service controls the orders that are created whenever a SoftLayer customer's places a purcha... "
date: "2018-02-12"
layout: "service"
tags:
    - "service"
    - "sldn"
    - "Billing"
classes:
    - "SoftLayer_Billing_Order"
---
# SoftLayer_Billing_Order
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
    <li id='service'> <a href='/reference/services/SoftLayer_Billing_Order' >Service</a></li>    <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Billing_Order' >Datatype</a></li>
    </ul>
</div>

## Description


The SoftLayer_Billing_Order service controls the orders that are created whenever a SoftLayer customer's places a purchase. Orders exist in several states. The ones of concern are: 
*'''QUOTE_PENDING''': Orders which have not been paid yet. Orders pending approval from a Softlayer customer.


Once an order is paid it moves from QUOTE_PENDING to PENDING_APPROVAL state. 

Orders are created with contact information duplicated from the [SoftLayer_Account]({{<ref "reference/datatypes/SoftLayer_Account">}}) or by manual entry. We do this in order to maintain a history of an account's contact information as orders are generated. 

Query the [SoftLayer_Account]({{<ref "reference/datatypes/SoftLayer_Account">}}) service to get a list of orders for your account. 


### associatedMethods

*  [SoftLayer_Account::getBalance](/reference/services/SoftLayer_Account/getBalance )
*  [SoftLayer_Account::getInvoices](/reference/services/SoftLayer_Account/getInvoices )



        
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

#### [approveModifiedOrder](/reference/services/SoftLayer_Billing_Order/approveModifiedOrder)
Approve the changes of a modified order

</div>

<div class="method-row">

#### [getAccount](/reference/services/SoftLayer_Billing_Order/getAccount)
Retrieve the [SoftLayer_Account]({{<ref "reference/datatypes/SoftLayer_Account">}}) to which an order belongs.

</div>

<div class="method-row">

#### [getAllObjects](/reference/services/SoftLayer_Billing_Order/getAllObjects)
Get all billing orders for your account

</div>

<div class="method-row">

#### [getBrand](/reference/services/SoftLayer_Billing_Order/getBrand)


</div>

<div class="method-row">

#### [getCart](/reference/services/SoftLayer_Billing_Order/getCart)
Retrieve a cart is similar to a quote, except that it can be continually modified by the customer and does not have locked-in prices. Not all orders will have a cart associated with them. See [SoftLayer_Billing_Order_Cart]({{<ref "reference/datatypes/SoftLayer_Billing_Order_Cart">}}) for more information.

</div>

<div class="method-row">

#### [getCoreRestrictedItems](/reference/services/SoftLayer_Billing_Order/getCoreRestrictedItems)
Retrieve the [SoftLayer_Billing_Order_Item]({{<ref "reference/datatypes/SoftLayer_Billing_Order_Item">}}) that are core restricted

</div>

<div class="method-row">

#### [getCreditCardTransactions](/reference/services/SoftLayer_Billing_Order/getCreditCardTransactions)
Retrieve all credit card transactions associated with this order. If this order was not placed with a credit card, this will be empty.

</div>

<div class="method-row">

#### [getExchangeRate](/reference/services/SoftLayer_Billing_Order/getExchangeRate)


</div>

<div class="method-row">

#### [getInitialInvoice](/reference/services/SoftLayer_Billing_Order/getInitialInvoice)


</div>

<div class="method-row">

#### [getItems](/reference/services/SoftLayer_Billing_Order/getItems)
Retrieve the SoftLayer_Billing_Order_items included in an order.

</div>

<div class="method-row">

#### [getObject](/reference/services/SoftLayer_Billing_Order/getObject)
Retrieve a SoftLayer_Billing_Order record.

</div>

<div class="method-row">

#### [getOrderApprovalDate](/reference/services/SoftLayer_Billing_Order/getOrderApprovalDate)


</div>

<div class="method-row">

#### [getOrderNonServerMonthlyAmount](/reference/services/SoftLayer_Billing_Order/getOrderNonServerMonthlyAmount)
Retrieve an order's non-server items total monthly fee.

</div>

<div class="method-row">

#### [getOrderServerMonthlyAmount](/reference/services/SoftLayer_Billing_Order/getOrderServerMonthlyAmount)
Retrieve an order's server items total monthly fee.

</div>

<div class="method-row">

#### [getOrderStatuses](/reference/services/SoftLayer_Billing_Order/getOrderStatuses)
Get a list of SoftLayer_Container_Billing_Order_Status objects.

</div>

<div class="method-row">

#### [getOrderTopLevelItems](/reference/services/SoftLayer_Billing_Order/getOrderTopLevelItems)
Retrieve an order's top level items. This normally includes the server line item and any non-server additional services such as NAS or ISCSI.

</div>

<div class="method-row">

#### [getOrderTotalAmount](/reference/services/SoftLayer_Billing_Order/getOrderTotalAmount)
Retrieve this amount represents the order's initial charge including set up fee and taxes.

</div>

<div class="method-row">

#### [getOrderTotalOneTime](/reference/services/SoftLayer_Billing_Order/getOrderTotalOneTime)
Retrieve an order's total one time amount summing all the set up fees, the labor fees and the one time fees. Taxes will be applied for non-tax-exempt. This amount represents the initial fees that will be charged.

</div>

<div class="method-row">

#### [getOrderTotalOneTimeAmount](/reference/services/SoftLayer_Billing_Order/getOrderTotalOneTimeAmount)
Retrieve an order's total one time amount. This amount represents the initial fees before tax.

</div>

<div class="method-row">

#### [getOrderTotalOneTimeTaxAmount](/reference/services/SoftLayer_Billing_Order/getOrderTotalOneTimeTaxAmount)
Retrieve an order's total one time tax amount. This amount represents the tax that will be applied to the total charge, if the SoftLayer_Account tied to a SoftLayer_Billing_Order is a taxable account.

</div>

<div class="method-row">

#### [getOrderTotalRecurring](/reference/services/SoftLayer_Billing_Order/getOrderTotalRecurring)
Retrieve an order's total recurring amount. Taxes will be applied for non-tax-exempt. This amount represents the fees that will be charged on a recurring (usually monthly) basis.

</div>

<div class="method-row">

#### [getOrderTotalRecurringAmount](/reference/services/SoftLayer_Billing_Order/getOrderTotalRecurringAmount)
Retrieve an order's total recurring amount. This amount represents the fees that will be charged on a recurring (usually monthly) basis.

</div>

<div class="method-row">

#### [getOrderTotalRecurringTaxAmount](/reference/services/SoftLayer_Billing_Order/getOrderTotalRecurringTaxAmount)
Retrieve the total tax amount of the recurring fees, if the SoftLayer_Account tied to a SoftLayer_Billing_Order is a taxable account.

</div>

<div class="method-row">

#### [getOrderTotalSetupAmount](/reference/services/SoftLayer_Billing_Order/getOrderTotalSetupAmount)
Retrieve an order's total setup fee.

</div>

<div class="method-row">

#### [getOrderType](/reference/services/SoftLayer_Billing_Order/getOrderType)
Retrieve the type of an order. This lets you know where this order was generated from.

</div>

<div class="method-row">

#### [getPaypalTransactions](/reference/services/SoftLayer_Billing_Order/getPaypalTransactions)
Retrieve all PayPal transactions associated with this order. If this order was not placed with PayPal, this will be empty.

</div>

<div class="method-row">

#### [getPdf](/reference/services/SoftLayer_Billing_Order/getPdf)
Retrieve a PDF copy of a quote.

</div>

<div class="method-row">

#### [getPdfFilename](/reference/services/SoftLayer_Billing_Order/getPdfFilename)
Retrieve the default name of the PDF

</div>

<div class="method-row">

#### [getPresaleEvent](/reference/services/SoftLayer_Billing_Order/getPresaleEvent)


</div>

<div class="method-row">

#### [getQuote](/reference/services/SoftLayer_Billing_Order/getQuote)
Retrieve the quote of an order. This quote holds information about its expiration date, creation date, name and status. This information is tied to an order having the status 'QUOTE'

</div>

<div class="method-row">

#### [getRecalculatedOrderContainer](/reference/services/SoftLayer_Billing_Order/getRecalculatedOrderContainer)
Generate an [SoftLayer_Container_Product_Order]({{<ref "reference/datatypes/SoftLayer_Container_Product_Order">}}) from a billing order. 

</div>

<div class="method-row">

#### [getReceipt](/reference/services/SoftLayer_Billing_Order/getReceipt)
Generate and return an order receipt.

</div>

<div class="method-row">

#### [getReferralPartner](/reference/services/SoftLayer_Billing_Order/getReferralPartner)
Retrieve the Referral Partner who referred this order. (Only necessary for new customer orders)

</div>

<div class="method-row">

#### [getUpgradeRequestFlag](/reference/services/SoftLayer_Billing_Order/getUpgradeRequestFlag)
Retrieve this flag indicates an order is an upgrade.

</div>

<div class="method-row">

#### [getUserRecord](/reference/services/SoftLayer_Billing_Order/getUserRecord)
Retrieve the SoftLayer_User_Customer object tied to an order.

</div>

<div class="method-row">

#### [isPendingEditApproval](/reference/services/SoftLayer_Billing_Order/isPendingEditApproval)
Determine if the existing order is pending edit approval

</div>
</div>

</div>

