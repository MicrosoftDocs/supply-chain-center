---
title: PurchaseOrderRelatedParty
description: This article provides information about the PurchaseOrderRelatedParty entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# PurchaseOrderRelatedParty

The Party(s) related to the Purchase Order.

For example:

- PO issued to Vendor Party
- Ship-To Party
- PO Created-by Party
- PO Notify Party
- Responsible Employee
- Buy Team Member

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| PurchaseOrderRelatedParty | PurchasingPartyRelTypeId | yes | string | 36 | The unique identifier of a Purchasing Party Relationship Type. |
| PurchaseOrderRelatedParty | PurchaseOrderRelatedPartyStartDate | yes | date | 8 | The start date of the Purchase Order Party Relationship. |
| PurchaseOrderRelatedParty | PoNumber | yes | string | 36 | The unique identifier of a Purchase Order. |
| PurchaseOrderRelatedParty | PartyId | yes | string | 36 | The unique identifier of a Party. |
| PurchaseOrderRelatedParty | PurchaseOrderRelatedPartyNote | no | string | 1024 | A note, comment or additional information regarding the Purchase Order Party Relationship. |
| PurchaseOrderRelatedParty | PurchaseOrderRelatedPartyEndDate | no | date | 8 | The end date of the Purchase Order Party Relationship. |
