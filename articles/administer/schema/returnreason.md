---
title: ReturnReason
description: This article provides information about the ReturnReason entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **ReturnReason**

The return reason entity refers to the return reason code for return, repair and exchange process. The return reason is typically documented at the time of creating the return order.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	Company	|	string	|	256	|	No	|	Company	|
|	Description	|	string	|	4000	|	No	|	Description of the return reason	|
|	DisplayOrderRank	|	string	|	256	|	No	|	Display order rank of the return reason	|
|	IsCommentsRequired	|	boolean	|		|	No	|	Is comments required for this reason number	|
|	IsReplaceEligible	|	boolean	|		|	No	|	Is this return reason replacement eligible	|
|	Name	|	string	|	256	|	No	|	Name of the return reason number	|
|	ReasonGroup	|	string	|	256	|	No	|	The reason group of this return reason 	|
|	ReturnReasonId	|	string	|	36	|	Yes	|	The unique ID of the return reason 	|
|	ReturnReasonNumber	|	string	|	256	|	Yes	|	The unique number of the return reason 	|
