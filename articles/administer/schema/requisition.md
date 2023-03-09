---
title: Requisition
description: This article provides information about the Requisition entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# Requisition

A Requisition is an internal document prepared to detail funding and authorization to procure Item(s) via the forthcoming Purchase Order, PO.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| Requisition | RequisitionId | yes | string | 36 | The unique identifier of a Requisition. |
| Requisition | PartyId | no | string | 36 | The unique identifier of a Party. |
| Requisition | DocumentId | no | string | 36 | The unique identifier of a Document. |
| Requisition | RequisitionSubmittedDate | no | date | 8 | The date that the Requisition was submitted for approval/fulfillment. |
| Requisition | RequisitionSubmittedByName | no | string | 128 | The name of the person submitting the Requisition. |

EOF