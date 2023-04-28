---
title: ProductUnitOfMeasureConversion
description: This is about ProductUnitOfMeasureConversion entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **ProductUnitOfMeasureConversion**

|	EntityAttribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	Denominator	|	string	|	256	|	No	|	Denominator	|
|	Factor	|	string	|	256	|	No	|	Factor for unit of measure conversion	|
|	FromUnit	|	string	|	256	|	No	|	Unit of measure from which the conversion is applicable	|
|	ItemSku	|	string	|	256	|	No	|	Stock keeping unit of the product	|
|	Numerator	|	string	|	256	|	No	|	Numerator	|
|	ProductNumber	|	string	|	256	|	No	|	Product number	|
|	ProductUnitOfMeasureConversionId	|	string	|	36	|	Yes	|	The unique Id for product unit of measure	|
|	ProductUnitOfMeasureConversionNumber	|	string	|	256	|	Yes	|	The unique number for product unit of measure	|
|	Rounding	|	string	|	256	|	No	|	Rounding 	|
|	ToUnit	|	string	|	256	|	No	|	Unit of measure to which the conversion is applicable	|
