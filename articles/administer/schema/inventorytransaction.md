---
title: InventoryTransaction
description: This article provides information about the InventoryTransaction entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# InventoryTransaction

A specific Inventory Transaction that is applied to or carried out at a specific Inventory Location(s) upon the Items in those locations.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| InventoryTransaction | TransactionId | yes | string | 36 | The unique identifier of a Transaction. |
| InventoryTransaction | InventoryTransactionTypeId | no | string | 36 | The unique identifier of an Inventory Transaction Type. |
| InventoryTransaction | InventoryTransactionClassId | no | string | 36 | The unique identifier of the Inventory Transaction Class. |
| InventoryTransaction | FromWarehouseId | no | string | 36 | The unique identifier of a Warehouse. |
| InventoryTransaction | TransactionCompletedTimestamp | no | timestamp | 8 | The timestamp that the Item Inventory Location Transaction was completed. |
| InventoryTransaction | TransactionRequestedTimestamp | no | timestamp | 8 | The timestamp that the Item Inventory Location Transaction was requested. |
| InventoryTransaction | InventoryTransactionStatusId | no | string | 36 | The unique identifier of an Inventory Transaction Status. |
| InventoryTransaction | ToWarehouseId | no | string | 36 | The unique identifier of a Warehouse. |

EOF