---
title: Warehouse
description: This article provides information about the Warehouse entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# Warehouse

A structure designated for storage of things or items

A warehouse is synonymous with a stockroom

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| Warehouse | WarehouseId | yes | string | 36 | The unique identifier of a Warehouse. |
| Warehouse | LocationId | no | string | 36 | The unique identifier of a Location. |
| Warehouse | WarehouseOrderCutoffTime | no | string | 256 | The latest time each day that new orders will be accepted for delivery for the next scheduled delivery day. |
| Warehouse | PickAndPackLeadTime | no | string | 256 | The default time required to pick and pack an item at a warehouse. |
| Warehouse | WarehouseName | no | string | 128 | The name of the Warehouse. |

EOF