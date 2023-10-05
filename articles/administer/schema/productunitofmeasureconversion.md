---
title: ProductUnitOfMeasureConversion
description: This article provides information about the ProductUnitOfMeasureConversion entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **ProductUnitOfMeasureConversion**

[!INCLUDE[banner](../../includes/banner.md)]

The product unit of measure conversion entity refers to the various selling or buying unit of measure of product and the conversion factor between those unit of measure vis-a-vis the product. For example if product A is sold in eaches and packs and if a pack contains 6 eaches, this entity will hold the conversion relationship between packs and eaches for product A.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	Denominator	|	string	|	256	|	No	|	Denominator	|
|	Factor	|	string	|	256	|	No	|	Factor for unit of measure conversion	|
|	FromUnit	|	string	|	256	|	No	|	Unit of measure from which the conversion is applicable	|
|	ItemSku	|	string	|	256	|	No	|	Stock keeping unit of the product	|
|	Numerator	|	string	|	256	|	No	|	Numerator	|
|	ProductNumber	|	string	|	256	|	No	|	Product number	|
|	ProductUnitOfMeasureConversionId	|	string	|	36	|	Yes	|	The unique ID for product unit of measure	|
|	ProductUnitOfMeasureConversionNumber	|	string	|	256	|	Yes	|	The unique number for product unit of measure	|
|	Rounding	|	string	|	256	|	No	|	Rounding 	|
|	ToUnit	|	string	|	256	|	No	|	Unit of measure to which the conversion is applicable	|
