---
title: ProductAccountSupplyPlan
description: This article provides information about the ProductAccountSupplyPlan entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **ProductAccountSupplyPlan**

The product account supply plan entity refers to the product allocation or commitment by the supplier to the customer.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountId	|	string	|	36	|	No	|	A unique identifier of an account. The account could be a customer or vendor etc. AccountId is an auto generated ID by Microsoft Dynamics 365 or Supply Chain Center. 	|
|	AccountNumber	|	string	|	256	|	No	|	Number or code for the account to quickly search and identify the account in system views.	|
|	AccountTypeCode	|	string	|	256	|	No	|	Account type code indicates the type of account. An account could be Vendor, Customer etc.	|
|	FromWarehouseId	|	string	|	256	|	No	|	The unique ID of the origin warehouse	|
|	FromWarehouseNumber	|	string	|	256	|	No	|	The origin warehouse number for the demand forecast	|
|	ItemSku	|	string	|	256	|	No	|	The stock keeping unit of the product	|
|	ProductAccountSupplyPlanId	|	string	|	36	|	Yes	|	The unique ID of the supply plan	|
|	ProductAccountSupplyPlanNote	|	string	|	4000	|	No	|	Notes or comments for supply plan	|
|	ProductAccountSupplyPlanNumber	|	string	|	256	|	Yes	|	The unique number of the account supply plan	|
|	ProductAccountSupplyPlanPeriodEndDate	|	date	|		|	No	|	The validity or expirty date of this record	|
|	ProductAccountSupplyPlanPeriodStartDate	|	date	|		|	No	|	The beginning or effective start date of this record	|
|	ProductAccountSupplyPlanQuantity	|	decimal	|		|	No	|	The supply plan quantity	|
|	ProductId	|	string	|	36	|	No	|	Product Id	|
|	ToWarehouseId	|	string	|	36	|	No	|	The unique ID of the destination warehouse	|
|	ToWarehouseNumber	|	string	|	256	|	No	|	The unique number of the destination warehouse	|
|	UoMId	|	string	|	36	|	No	|	Unit of measure Id	|
|	UoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
