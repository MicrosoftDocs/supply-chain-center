---
title: PurchasingPartyRelationshipType
description: This article provides information about the PurchasingPartyRelationshipType entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# PurchasingPartyRelationshipType

"he nature of the relationship between the party and the purchasing process or document.

For example:

- Vendor/Supplier
- Responsible employee
- Buy-Team member
- RFI Notice Party
- RFP Notice Party
- PO Notice Party
- Order Notice Party
- Bidder
- National Jurisdiction
- State Jurisdiction
- Provincial Jurisdiction

>[!Note]
> This is defined once and used for RFI, RFP, RFQ, ORDER etc. in place of defining a 'party relationship' for each one, which would require common data to be duplicated for each.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| PurchasingPartyRelationshipType | PurchasingPartyRelTypeId | yes | string | 36 | The unique identifier of a Purchasing Party Relationship Type. |
| PurchasingPartyRelationshipType | PurchasingPartyRelationshipTypeDescription | no | string | 512 | The description of a Purchasing Party Relationship Type. |
| PurchasingPartyRelationshipType | PurchasingPartyRelationshipTypeName | no | string | 128 | The name of a Purchasing Party Relationship Type.. |
