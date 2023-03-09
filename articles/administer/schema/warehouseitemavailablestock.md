---
title: WarehouseItemAvailableStock
description: This article provides information about the WarehouseItemAvailableStock entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# WarehouseItemAvailableStock

The stock available to service immediate demand. The difference between the quantity of an Item that is on hand and not subject to a hold and the quantity of an Item that has been allocated to orders for a timestamp

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| WarehouseItemAvailableStock | Timestamp | yes | timestamp | 14 | The timestamp that the associated information is reported, recorded or effective as-of. |
| WarehouseItemAvailableStock | ItemSku | yes | string | 20 | The Stock Keeping Unit identifier, which is typically used for inventory-related activities. |
| WarehouseItemAvailableStock | WarehouseId | yes | string | 36 | The unique identifier of a Warehouse. |
| WarehouseItemAvailableStock | ActualItemAvailabilityQuantity | no | decimal | 9 | The quantity of available items, the quantity of an Item that is on hand and not subject to a hold and the quantity of an Item that has been allocated to orders for some period of time. |

EOF