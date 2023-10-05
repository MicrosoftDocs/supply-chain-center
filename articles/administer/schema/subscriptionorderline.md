---
title: SubscriptionOrderLine
description: This article provides information about the SubscriptionOrderLine entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **SubscriptionOrderLine**

[!INCLUDE[banner](../../includes/banner.md)]

A subscription order line entity refers to a specific type of entity or object in a business or e-commerce system that represents a customer's subscription order.

When a customer subscribes to a product or service on a recurring basis, such as a magazine, a software license, or a streaming service, their subscription order is typically managed through an entity specifically designed to handle the details of the subscription. This entity contains information about the customer, the subscription plan, the billing details, and any additional parameters related to the subscription.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	BaseAmount	|	decimal	|		|	No	|	#N/A	|
|	BaseAmountBase	|	decimal	|		|	No	|	#N/A	|
|	Description	|	string	|	4000	|	No	|	#N/A	|
|	ExchangeRate	|	string	|	256	|	No	|	#N/A	|
|	ExtendedAmount	|	decimal	|		|	No	|	#N/A	|
|	ExtendedAmountBase	|	decimal	|		|	No	|	#N/A	|
|	IsPriceOverridden	|	boolean	|		|	No	|	#N/A	|
|	ItemSku	|	string	|	256	|	No	|	#N/A	|
|	ManualDiscountAmount	|	decimal	|		|	No	|	#N/A	|
|	ManualDiscountAmountBase	|	decimal	|		|	No	|	#N/A	|
|	Name	|	string	|	256	|	No	|	#N/A	|
|	PricePerUnit	|	decimal	|		|	No	|	#N/A	|
|	PricePerUnitBase	|	decimal	|		|	No	|	#N/A	|
|	ProductDescription	|	string	|	4000	|	No	|	#N/A	|
|	ProductId	|	string	|	36	|	No	|	#N/A	|
|	Quantity	|	decimal	|		|	No	|	#N/A	|
|	ShipToFreightTermsCode	|	string	|	256	|	No	|	#N/A	|
|	SubscriptionOrderId	|	string	|	36	|	No	|	#N/A	|
|	SubscriptionOrderLineId	|	string	|	36	|	Yes	|	#N/A	|
|	SubscriptionOrderLineNumber	|	string	|	256	|	Yes	|	#N/A	|
|	SubscriptionOrderNumber	|	string	|	256	|	No	|	#N/A	|
|	Tax	|	string	|	256	|	No	|	#N/A	|
|	TaxBase	|	string	|	256	|	No	|	#N/A	|
|	TransactionCurrencyId	|	string	|	256	|	No	|	#N/A	|
|	UoMId	|	string	|	36	|	No	|	Unit of measure Id	|
|	UoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
|	VolumeDiscountAmount	|	decimal	|		|	No	|	#N/A	|
|	VolumeDiscountAmountBase	|	decimal	|		|	No	|	#N/A	|
