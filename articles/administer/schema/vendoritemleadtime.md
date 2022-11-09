---
title: VendorItemLeadtime
description: This article provides information about the VendorItemLeadtime entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# VendorItemLeadtime

The leadtime expressed in days required to get the associated Item from the Vendor.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| VendorItemLeadtime | VendorId | yes | string | 36 | The unique identifier of a Vendor. |
| VendorItemLeadtime | ItemSku | yes | string | 20 | The Stock Keeping Unit identifier, which is typically used for inventory-related activities. |
| VendorItemLeadtime | PeriodStartDate | yes | date | 14 | The period start date. |
| VendorItemLeadtime | AverageLeadTimeDays | no | integer | 9 | The lead time expressed in days that it takes to get the associated Item from the Vendor. |
| VendorItemLeadtime | NegotiatedLeadTimeDays | no | integer | 9 | The negotiated lead time expressed in days agreed by the vendor/supplier to provide the associated Item. |
| VendorItemLeadtime | PeriodEndDate | no | date | 14 | The period end date. |
