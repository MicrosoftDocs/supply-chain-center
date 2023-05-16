---
title: AccountProductStatus
description: This article provides information about the AccountProductStatus entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **AccountProductStatus**

The account product status refers to the products current status. The status of the product could be active, end of life, preorder etc. The account product status entity also has cross references between seller's product and buyer's product. The product status has a validity period defined by period start date and period end date.



|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountId	|	string	|	36	|	No	|	The unique ID of the account. The Account ID is an internal system generated ID by Microsoft Dynamics 365 applications.	|
|	AccountNumber	|	string	|	256	|	No	|	Number or code for the account to quickly search and identify the account in system views.	|
|	AccountProductId	|	string	|	36	|	No	|	The Stockkeeping Unit of the product, which is typically used for inventory-related activities. The unique ID of the product managed by the account. For example, if the account is a customer, then AccountProductId holds the product ID the customer uses to refer the sellers product.	|
|	AccountProductNumber	|	string	|	256	|	No	|	The unique product number for the account. If the account is a customer, then AccountProductNumber identifies the product number of the customer, or if its vendor then AccountProductNumber identifies the product number of the vendor.	|
|	AccountProductStatusId	|	string	|	36	|	Yes	|	The unique ID of the account product status	|
|	AccountProductStatusNote	|	string	|	4000	|	No	|	A note, comment or additional information regarding the vendor item status.	|
|	AccountProductStatusNumber	|	string	|	256	|	Yes	|	The unique number of the account product status	|
|	AccountStatusTypeId	|	string	|	36	|	No	|	The unique identifier of an Account Status Type.	|
|	AccountTypeCode	|	string	|	256	|	No	|	Account type code indicates the type of account. An account could be Vendor, Customer etc.	|
|	ItemSku	|	string	|	256	|	No	|	The product number of the Microsoft Supply Chain Center customer or user. The Stockkeeping Unit of the product, which is typically used for inventory-related activities. |
|	PeriodEndDate	|	date	|		|	No	|	The validity or expiry date of this record	|
|	PeriodStartDate	|	date	|		|	No	|	The beginning or effective start date of this record	|
|	ProductId	|	string	|	36	|	No	|	The Stockkeeping Unit of the product, which is typically used for inventory-related activities.	|
