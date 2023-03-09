---
title: RelatedCustomer
description: This article provides information about the RelatedCustomer entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# RelatedCustomer

The relationship of two or more Customers for the associated period of time.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| RelatedCustomer | CustomerId | yes | string | 36 | The unique identifier of a Customer. |
| RelatedCustomer | RelatedCustomerId | yes | string | 36 | The unique identifier of a Customer. |
| RelatedCustomer | PeriodStartDate | yes | date | 8 | The period start date for which the customer relationship is effective. |
| RelatedCustomer | PeriodEndDate | no | date | 8 | The period end date for which the customer relationship is effective. |
| RelatedCustomer | CustomerRelationshipTypeId | no | string | 36 | The unique identifier of a Household Relationship Type. |
| RelatedCustomer | RelatedCustomerNote | no | string | 1024 | A note, comment or additional information regarding the customer relationship. |

EOF