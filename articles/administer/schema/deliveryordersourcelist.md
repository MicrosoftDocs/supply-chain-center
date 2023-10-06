---
title: DeliveryOrderSourceList
description: This article provides information about the DeliveryOrderSourceList entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/30/2023
ms.custom: bap-template
---

# DeliveryOrderSourceList

[!INCLUDE[banner](../../includes/banner.md)]

Delivery order source list entity refers to the list of orders related to the delivery order.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	DeliveryOrderSourceListId	|	string	|	36	|	Yes	|	Unique indentifier of the delivery order source list. 	|
|	DeliveryOrderSourceListName	|	string	|	256	|	No	|	Name of the delivery order source list.	|
|	DeliveryOrderSourceListNumber	|	string	|	256	|	Yes	|	Unique number of the delivery order source list.	|
|	Description	|	string	|	4000	|	No	|	Description of the source list.	|
