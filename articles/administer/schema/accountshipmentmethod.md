---
title: AccountShipmentMethod
description: This is about AccountShipmentMethod entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **AccountShipmentMethod**

The account shipment method refers to the process or means by which products or goods are delivered to the account. There are various shipment methods available, and the choice of method often depends on factors such as the nature of the product, customer preferences, geographical location, and time constraints. This entity records an accounts default preference related to shipping. The default preference can be overwritten at the time of placing the order. 



|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountId	|	string	|	256	|	No	|	The unique Id of the account. This is an internal system generated Id by D365 applications	|
|	AccountNumber	|	string	|	256	|	No	|	Number or code for the account to quickly search and identify the account in system views.	|
|	AccountShipmentMethodId	|	string	|	36	|	Yes	|	Unique Preferred shipment method by the account	|
|	AccountShipmentMethodNote	|	string	|	4000	|	No	|	A note, comment or additional information regarding the associated customer shipment method.	|
|	AccountShipmentMethodNumber	|	string	|	256	|	Yes	|	Unique preferred shipment method number of the account	|
|	AccountTypeCode	|	string	|	256	|	No	|	Account type code indicates the type of account. An account could be Vendor, Customer etc.	|
|	CarrierId	|	string	|	36	|	No	|	Unique Id of the carrier. This is an internal carrier Id of the number	|
|	CarrierNumber	|	string	|	256	|	No	|	Unique carrier number. This is the searchable external carrier Id. From your ERP map the Carrier Id to this attribute	|
|	PeriodEndDate	|	date	|		|	No	|	The validity or expirty date of this record	|
|	PeriodStartDate	|	date	|		|	No	|	The beginning or effective start date of this record	|
|	PreferenceNumber	|	string	|	256	|	No	|	The unique shipment preference number of the account	|
|	ShipmentMethodName	|	string	|	256	|	No	|	The unique name identifier of a Shipment Method.	|
