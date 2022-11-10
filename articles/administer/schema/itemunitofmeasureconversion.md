---
title: ItemUnitOfMeasureConversion
description: This article provides information about the ItemUnitOfMeasureConversion entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# ItemUnitOfMeasureConversion

Unit of measure conversion relationship between various units of measure for the item. For example, if a product is sold as Eaches and Packs. How many of each item are in a pack for this item.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ItemUnitOfMeasureConversion | ConvertToUnitOfMeasureId | yes | string | 36 | Unit of measure Id to which conversion is required. |
| ItemUnitOfMeasureConversion | ConvertFromUnitOfMeasureId | yes | string | 36 | Unit of measure Id from which conversion is required. |
| ItemUnitOfMeasureConversion | ItemSku | yes | string | 36 | Unique Id of the item. |
| ItemUnitOfMeasureConversion | ItemUnitOfMeasureConversionNote | no | string | 36 | Note for item unit of measure conversion. |
| ItemUnitOfMeasureConversion | ConversionFactor | no | string | 36 | Conversion factor for unit of measure Id between from and to unit of measure. This is a number. |
