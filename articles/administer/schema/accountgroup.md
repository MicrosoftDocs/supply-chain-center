---
title: AccountGroup
description: This is about AccountGroup entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **AccountGroup**

Account group entity defines the group or classification an account belongs. Account group is a categorization or segmentation of accounts based on certain criteria or characteristics. Account groups are used to group accountss together for various purposes,business processes and relations such as sales and marketing activities, pricing and discount management, analytics, market segmentation etc.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountGroupDescription	|	string	|	4000	|	No	|	Description of the account group	|
|	AccountGroupId	|	string	|	36	|	Yes	|	Unique Id of the account group	|
|	AccountGroupNumber	|	string	|	256	|	Yes	|	Unique number of the account group	|
|	AccountPaymentTermId	|	string	|	36	|	No	|	Account payment terms Id	|
|	ClearingPeriodPaymentTermName	|	string	|	256	|	No	|	Clearing period payment term name	|
|	GroupNumber	|	string	|	36	|	Yes	|	Group number of the account	|
|	WriteOffCompany	|	string	|	256	|	No	|	Write off company name	|
|	WriteOffReason	|	string	|	4000	|	No	|	Write off reason	|
