---
title: InventoryTransactionUnserializedItem
description: This article provides information about the InventoryTransactionUnserializedItem entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# InventoryTransactionUnserializedItem

The unserialized Item(s) involved in the Inventory Transaction.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| InventoryTransactionUnserializedItem | ItemSku | yes | string | 20 | The Stock Keeping Unit identifier, which is typically used for inventory-related activities. |
| InventoryTransactionUnserializedItem | TransactionId | yes | string | 36 | The unique identifier of a Transaction. |
| InventoryTransactionUnserializedItem | Quantity | no | decimal | 0 | The quantity of Item involved in the transaction. |
| InventoryTransactionUnserializedItem | UnitOfMeasureId | no | string | 36 | The unique identifier of a Unit Of Measure.. |
