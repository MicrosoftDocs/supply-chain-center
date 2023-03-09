---
title: VendorItemStatus
description: This article provides information about the VendorItemStatus entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# VendorItemStatus

The status of the Vendor in regard to supplying the associated Item.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| VendorItemStatus | PeriodStartDate | yes | date | 14 | The period start date that the associated status information is effective. |
| VendorItemStatus | ItemSku | yes | string | 20 | The Stock Keeping Unit identifier, which is typically used for inventory-related activities. |
| VendorItemStatus | VendorId | yes | string | 36 | The unique identifier of a Vendor. |
| VendorItemStatus | VendorStatusTypeId | no | string | 36 | The unique identifier of a Vendor Status Type. |
| VendorItemStatus | VendorItemStatusNote | no | string | 1024 | A note, comment or additional information regarding the vendor item status. |
| VendorItemStatus | PeriodEndDate | no | date | 14 | The period end date that the associated status information is effective. |
| VendorItemStatus | VendorItemSku | no | string | 20 | The Stock Keeping Unit identifier specified by the Vendor. |
