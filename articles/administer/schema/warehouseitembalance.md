---
title: WarehouseItemBalance
description: This article provides information about the WarehouseItemBalance entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# WarehouseItemBalance

The on-hand balance for the associated timestamp. The quantity of an item shown in the inventory records as being physically in stock.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| WarehouseItemBalance | Timestamp | yes | timestamp | 14 | The timestamp that the associated information is reported, recorded or effective as-of. |
| WarehouseItemBalance | ItemSku | yes | string | 20 | The Stock Keeping Unit identifier, which is typically used for inventory-related activities. |
| WarehouseItemBalance | WarehouseId | yes | string | 36 | The unique identifier of a Warehouse. |
| WarehouseItemBalance | ActualItemQuantity | no | decimal | 9 | The actual Item on-hand balance for the associated period. |
| WarehouseItemBalance | PlannedItemQuantity | no | decimal | 9 | The planned Item on-hand balance for the associated period. |

EOF