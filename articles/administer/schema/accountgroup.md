---
title: AccountGroup
description: This article provides information about the AccountGroup entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **AccountGroup**

The account group entity defines the group or classification an account belongs to. The account group is a categorization or segmentation of accounts that is based on certain criteria or characteristics. Account groups are used to group accounts together. They are used for various purposes, business processes, and business relations. For example, sales and marketing activities, pricing and discount management, analytics, ad market segmentation.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountGroupDescription	|	string	|	4000	|	No	|	A description of the account group.	|
|	AccountGroupId	|	string	|	36	|	Yes	|	The unique ID of the account group.	|
|	AccountGroupNumber	|	string	|	256	|	Yes	|	The unique number of the account group.	|
|	AccountPaymentTermId	|	string	|	36	|	No	|	The account payment terms ID.	|
|	ClearingPeriodPaymentTermName	|	string	|	256	|	No	|	The clearing period payment term name.	|
|	GroupNumber	|	string	|	36	|	Yes	|	The group number of the account.	|
|	WriteOffCompany	|	string	|	256	|	No	|	The write off company name.	|
|	WriteOffReason	|	string	|	4000	|	No	|	The write off reason.	|
