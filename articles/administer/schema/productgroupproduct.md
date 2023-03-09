---
title: ProductGroupProduct
description: This article provides information about the ProductGroupProduct entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# ProductGroupProduct

The Product(s) that comprise or are members of the associated Product Group.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ProductGroupProduct | PeriodStartDate | yes | date | 8 | The period start date of the product relationship. |
| ProductGroupProduct | ProductId | yes | string | 36 | The unique identifier of a Product. |
| ProductGroupProduct | ProductGroupId | yes | string | 36 | The unique identifier of a Product Group. |
| ProductGroupProduct | PeriodEndDate | no | date | 8 | The period end date of the product relationship.. |
