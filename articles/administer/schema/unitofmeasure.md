---
title: UnitOfMeasure
description: This article provides information about the UnitOfMeasure entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# UnitOfMeasure

A standard of measurement for an item as to how it is stocked in the warehouse, priced, sold or procured.

For example: Soap powder in a box may be sold as 1 EA but it may be priced based on its weight.

Examples of Unit Of Measure are EA (eaches), Pack, LB (Pounds), KG (Kilograms), Ton, Cubic Litre, Cubic Foot, Box, Cartons etc.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| UnitOfMeasure | UnitOfMeasureId | yes | string | 36 | The unique identifier of a Unit Of Measure. |
| UnitOfMeasure | UnitOfMeasureAbbreviation | no | string | 3 | The abbreviation assigned to the Unit Of Measure. |
| UnitOfMeasure | UnitOfMeasureTypeId | no | integer | 9 | The unique identifier of a Unit Of Measure Type. |
| UnitOfMeasure | UnitOfMeasureName | no | string | 128 | The name of a Unit Of Measure. |
| UnitOfMeasure | UnitOfMeasureDescription | no | string | 512 | The description of a Unit Of Measure.. |
