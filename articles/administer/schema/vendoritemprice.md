---
title: VendorItemPrice
description: This article provides information about the VendorItemPrice entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# VendorItemPrice

The price set by the vendor for the minimum purchase quantity of the item for the specified period.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| VendorItemPrice | MinimumPurchaseQuantity | yes | decimal | 9 | The minimum number of units that must be purchased for the price to be effective. |
| VendorItemPrice | PeriodStartDate | yes | date | 14 | The period start date. |
| VendorItemPrice | VendorId | yes | string | 36 | The unique identifier of a Vendor. |
| VendorItemPrice | ItemSku | yes | string | 20 | The Stock Keeping Unit identifier, which is typically used for inventory-related activities. |
| VendorItemPrice | VendorItemPriceNote | no | string | 1024 | A note, comment or additional information regarding the vendor item price. |
| VendorItemPrice | VendorItemPrice | no | decimal | 9 | The price set by the vendor for the minimum purchase quantity of the item. |
| VendorItemPrice | PeriodEndDate | no | date | 14 | The period end date. |

EOF