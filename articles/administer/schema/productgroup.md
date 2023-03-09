---
title: ProductGroup
description: This article provides information about the ProductGroup entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# ProductGroup

An arbitrary grouping of Products.

For example:

- Products
- Software Products
- Retail Products
- Appliances
- Services
- Electric services
- Gas services

Implementation Note:

The primary use of the PRODUCT GROUP entity is to provide the foundation for creating a product hierarchy. There are 3 other entities that are used to provide support for this multi-level hierarchy that also allows products to belong to more than one hierarchy: RELATED PRODUCT GROUP, PRODUCT GROUP RELATIONSHIP TYPE and PRODUCT GROUP. PRODUCT GROUP is used to detail the levels in a product hierarchy.

For example, your hierarchy may include:

- Level 1 - Region: North America, Europe, Asia, Australia, South America, Africa
- Level 2 - Channel: Online, Retail Outlet, Third Party Sales Channel
- Level 3 - Product Category: Clothing, Technology

Each of these levels would be represented by PRODUCT GROUPs for each these groups would be related by RELATED PRODUCT GROUP and finally PRODUCT GROUP RELATIONSHIP TYPE would describe the relationships between each of these related.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ProductGroup | ProductGroupId | yes | string | 36 | The unique identifier of a Product Group. |
| ProductGroup | ProductGroupDescription | no | string | 512 | The description of a Product Group. |
| ProductGroup | ProductGroupName | no | string | 128 | The name of a Product Group.. |
