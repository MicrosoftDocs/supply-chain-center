---
title: WarehouseItemSafetyStock
description: This article provides information about the WarehouseItemSafetyStock entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# WarehouseItemSafetyStock

A quantity of an Item within a Warehouse that is planned to be in inventory to protect against fluctuations in demand and/or supply. Safety stock also protects against inaccuracies in inventory.

The stock is held to protect against the differences between forecast and actual consumption, and between expected and actual delivery times of procurement orders, to protect against stockouts during the replenishment cycle. In calculating safety stock, account is taken of such factors as service level, expected fluctuations of demand and likely variations in lead time.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| WarehouseItemSafetyStock | Timestamp | yes | timestamp | 14 | The timestamp that the associated information is reported, recorded or effective as-of. |
| WarehouseItemSafetyStock | ItemSku | yes | string | 20 | The Stock Keeping Unit identifier, which is typically used for inventory-related activities. |
| WarehouseItemSafetyStock | WarehouseId | yes | string | 36 | The unique identifier of a Warehouse. |
| WarehouseItemSafetyStock | ActualSafetyStockItemQuantity | no | decimal | 9 | The quantity of Item that was actually on-hand at the Warehouse functioning as safety stock for the associated period. |
| WarehouseItemSafetyStock | PlannedSafetyStockItemQuantity | no | decimal | 9 | The quantity of Item that is planned to be on-hand at the Warehouse functioning as safety stock for the associated period. |
