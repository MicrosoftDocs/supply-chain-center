---
title: SubscriptionOrder
description: This article provides information about the SubscriptionOrder entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **SubscriptionOrder**

A subscription order entity refers to a specific type of entity or object in a business or e-commerce system that represents a customer's subscription order.

When a customer subscribes to a product or service on a recurring basis, such as a magazine, a software license, or a streaming service, their subscription order is typically managed through an entity specifically designed to handle the details of the subscription. This entity contains information about the customer, the subscription plan, the billing details, and any additional parameters related to the subscription.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	BillingFrequency	|	string	|	256	|	No	|	#N/A	|
|	CurrentSubscription	|	string	|	256	|	No	|	#N/A	|
|	CustomerNumber	|	string	|	256	|	No	|	#N/A	|
|	CustomerTypeCode	|	string	|	256	|	No	|	#N/A	|
|	DeliveryChoice	|	string	|	256	|	No	|	#N/A	|
|	DiscountAmount	|	decimal	|		|	No	|	#N/A	|
|	DiscountAmountBase	|	decimal	|		|	No	|	#N/A	|
|	EmailAddress	|	string	|	256	|	No	|	#N/A	|
|	ExchangeRate	|	string	|	256	|	No	|	#N/A	|
|	FreightTermsCode	|	string	|	256	|	No	|	#N/A	|
|	FulfillmentFrequency	|	string	|	256	|	No	|	#N/A	|
|	LastFulfillmentDate	|	date	|		|	No	|	#N/A	|
|	MonthlyInstallment	|	string	|	256	|	No	|	#N/A	|
|	MonthlyInstallmentBase	|	string	|	256	|	No	|	#N/A	|
|	Name	|	string	|	256	|	No	|	#N/A	|
|	OrderNumber	|	string	|	256	|	Yes	|	#N/A	|
|	PriceLevelId	|	string	|	256	|	No	|	#N/A	|
|	SalesOrderOriginNumber	|	string	|	256	|	No	|	#N/A	|
|	SalesOriginOrderId	|	string	|	36	|	No	|	#N/A	|
|	ShipmentAmount	|	decimal	|		|	No	|	#N/A	|
|	ShipmentAmountBase	|	decimal	|		|	No	|	#N/A	|
|	ShippingMethodCode	|	string	|	256	|	No	|	#N/A	|
|	ShipToCity	|	string	|	256	|	No	|	#N/A	|
|	ShipToContactName	|	string	|	256	|	No	|	#N/A	|
|	ShipToCountry	|	string	|	256	|	No	|	#N/A	|
|	ShipToLine1	|	string	|	256	|	No	|	#N/A	|
|	ShipToLine2	|	string	|	256	|	No	|	#N/A	|
|	ShipToLine3	|	string	|	256	|	No	|	#N/A	|
|	ShipToPostalCode	|	string	|	256	|	No	|	#N/A	|
|	ShipToStateOrProvince	|	string	|	256	|	No	|	#N/A	|
|	SubscriptionEndDate	|	date	|		|	No	|	The validity or expirty date of this record	|
|	SubscriptionOrderId	|	string	|	36	|	Yes	|	#N/A	|
|	SubscriptionOrderNumber	|	string	|	256	|	Yes	|	#N/A	|
|	SubscriptionStartDate	|	date	|		|	No	|	The beginning or effective start date of this record	|
|	TransactionCurrencyId	|	string	|	256	|	No	|	#N/A	|