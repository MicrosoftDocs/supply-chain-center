---
title: ReturnReason
description: This is about ReturnReason entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **ReturnReason**

|	EntityAttribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	Company	|	string	|	256	|	No	|	Company	|
|	Description	|	string	|	4000	|	No	|	Description of the return reason	|
|	DisplayOrderRank	|	string	|	256	|	No	|	Display order rank of the return reason	|
|	IsCommentsRequired	|	boolean	|		|	No	|	Is comments required for this reason number	|
|	IsReplaceEligible	|	boolean	|		|	No	|	Is this return reason replacement eligible	|
|	Name	|	string	|	256	|	No	|	Name of the return reason number	|
|	ReasonGroup	|	string	|	256	|	No	|	The reason group of this return reason 	|
|	ReturnReasonId	|	string	|	36	|	Yes	|	The unique Id of the return reason 	|
|	ReturnReasonNumber	|	string	|	256	|	Yes	|	The unique number of the return reason 	|
