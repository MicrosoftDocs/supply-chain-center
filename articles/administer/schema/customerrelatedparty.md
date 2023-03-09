---
title: CustomerRelatedParty
description: This article provides information about the CustomerRelatedParty entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# CustomerRelatedParty

A party that has a relationship with the customer over the indicated period.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| CustomerRelatedParty | CustomerPartyRelationshipTypeId | yes | string | 36 | The unique identifier of a customer relationship type. |
| CustomerRelatedParty | PeriodStartTimestamp | yes | timestamp | 8 | The period start timestamp for which the associated customer - party relationship is valid or in-effect. |
| CustomerRelatedParty | CustomerId | yes | string | 36 | The unique identifier of a Customer. |
| CustomerRelatedParty | PartyId | yes | string | 36 | The unique identifier of a Party. |
| CustomerRelatedParty | PeriodEndTimestamp | no | timestamp | 8 | The period end timestamp for which the associated customer - party relationship is valid or in-effect. |

EOF