---
title: UnitOfMeasure
description: This article provides information about the UnitOfMeasure entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **UnitOfMeasure**

The unit of measure entity holds the various selling and buying unit of measure of the products. Example unit of measure include eaches, packs, kilograms, litre etc.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	BaseUOM	|	string	|	256	|	No	|	Base unit of measure	|
|	IsBaseUnit	|	boolean	|		|	No	|	Is this base unit of measure	|
|	IsScheduleBaseUOM	|	boolean	|		|	No	|	Is this base schedule unit of measure	|
|	Name	|	string	|	256	|	No	|	Name of unit of measure	|
|	Quantity	|	decimal	|		|	No	|	Unit of measure quantity	|
|	UnitOfMeasureGroupId	|	string	|	36	|	No	|	Id of the unit of measure group	|
|	UnitOfMeasureGroupNumber	|	string	|	256	|	No	|	Number of the unit of measure group 	|
|	UoMId	|	string	|	36	|	Yes	|	Unit of measure Id	|
|	UoMNumber	|	string	|	256	|	Yes	|	Unit of measure ISO code	|
