---
title: AccountShipmentMethod
description: This article provides information about the AccountShipmentMethod entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **AccountShipmentMethod**

[!INCLUDE[banner](../../includes/banner.md)]

The account shipment method refers to the process or means by which products or goods are delivered to the account. There are various shipment methods available, and the choice of method often depends on factors such as the nature of the product, customer preferences, geographical location, and time constraints. This entity records an account's default preference related to shipping. The default preference can be overwritten at the time of placing the order. 



|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountId	|	string	|	256	|	No	|	The unique ID of the account. The AccountId is an internal system generated ID by Microsoft Dynamics 365 applications.	|
|	AccountNumber	|	string	|	256	|	No	|	A number or code that is used for the account to quickly search for and identify it in system views	|
|	AccountShipmentMethodId	|	string	|	36	|	Yes	|	The unique, preferred shipment method ID by the account.	|
|	AccountShipmentMethodNote	|	string	|	4000	|	No	|	A note, comment, or additional information regarding the associated account shipment method.	|
|	AccountShipmentMethodNumber	|	string	|	256	|	Yes	|	The unique, preferred shipment method number of the account.	|
|	AccountTypeCode	|	string	|	256	|	No	|	The account type code indicates the type of account. For example, vendor or customer.	|
|	CarrierId	|	string	|	36	|	No	|	The unique ID of the carrier. The CarrierID is an internal carrier ID number.	|
|	CarrierNumber	|	string	|	256	|	No	|	Unique carrier number. The CarrierNumber is the searchable external carrier ID. From your ERP, map the Carrier ID to this attribute.	|
|	PeriodEndDate	|	date	|		|	No	|	The validity or expiry date of this record.	|
|	PeriodStartDate	|	date	|		|	No	|	The beginning or effective start date of this record.	|
|	PreferenceNumber	|	string	|	256	|	No	|	The unique shipment preference number of the account.	|
|	ShipmentMethodName	|	string	|	256	|	No	|	The unique name identifier of a Shipment Method.	|
