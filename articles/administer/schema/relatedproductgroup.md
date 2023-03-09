---
title: RelatedProductGroup
description: This article provides information about the RelatedProductGroup entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# RelatedProductGroup

The relationship of two or more Product Groups.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| RelatedProductGroup | ProductGroupRelationshipTypeId | yes | string | 36 | The unique identifier of a Product Group Relationship Type. |
| RelatedProductGroup | PeriodStartDate | yes | date | 8 | The period start date of the product relationship. |
| RelatedProductGroup | ProductGroupId | yes | string | 36 | The unique identifier of a Product Group. |
| RelatedProductGroup | RelatedProductGroupId | yes | string | 36 | The unique identifier of a Product Group. |
| RelatedProductGroup | ProductGroupRelationshipNote | no | string | 1024 | A note, comment or additional information regarding the product group relationship. |
| RelatedProductGroup | PeriodEndDate | no | date | 8 | The period end date of the product relationship.. |
