---
title: AccountProductStatus
description: This is about AccountProductStatus entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **AccountProductStatus**

The account product status refers to the products current status. The status of the product could be active, end of life, pre-order etc. The account product status entity also has cross references between seller's product and buyer's product. The product status has a validity period defined by period start date and period end date.



|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountId	|	string	|	36	|	No	|	The unique Id of the account. This is an internal system generated Id by D365 applications	|
|	AccountNumber	|	string	|	256	|	No	|	Number or code for the account to quickly search and identify the account in system views.	|
|	AccountProductId	|	string	|	36	|	No	|	The Stock Keeping Unit of the product, which is typically used for inventory-related activities. This is the unique Id of the product managed by the account. 
For example, If the account is a customer, then this will hold the product Id the customer uses to refer the sellers product.	|
|	AccountProductNumber	|	string	|	256	|	No	|	The unique product number of the account	|
|	AccountProductStatusId	|	string	|	36	|	Yes	|	The unique Id of the account product status	|
|	AccountProductStatusNote	|	string	|	4000	|	No	|	A note, comment or additional information regarding the vendor item status.	|
|	AccountProductStatusNumber	|	string	|	256	|	Yes	|	The unique number of the account product status	|
|	AccountStatusTypeId	|	string	|	36	|	No	|	The unique identifier of a Account Status Type.	|
|	AccountTypeCode	|	string	|	256	|	No	|	Account type code indicates the type of account. An account could be Vendor, Customer etc.	|
|	ItemSku	|	string	|	256	|	No	|	The Stock Keeping Unit of the product, which is typically used for inventory-related activities. 

For example, If the account is a customer, then this will identify the product Id of the seller.|
|	PeriodEndDate	|	date	|		|	No	|	The validity or expirty date of this record	|
|	PeriodStartDate	|	date	|		|	No	|	The beginning or effective start date of this record	|
|	ProductId	|	string	|	36	|	No	|	The Stock Keeping Unit of the product, which is typically used for inventory-related activities.	|
