---
title: InventoryTransactionShipment
description: This article provides information about the InventoryTransactionShipment entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# InventoryTransactionShipment

The shipments used to transport the items specified in the inventory transaction.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| InventoryTransactionShipment | TransactionId | yes | string | 36 | The unique identifier of a Transaction. |
| InventoryTransactionShipment | ShipmentItemNumber | yes | integer | 6 | The shipment line number. |
| InventoryTransactionShipment | ShipmentId | yes | string | 36 | The unique identifier of a Shipment. |

EOF