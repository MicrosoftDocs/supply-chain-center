---
title: ShipmentEventStatus
description: This article provides information about the ShipmentEventStatus entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# ShipmentEventStatus

The status of the Shipment Event. For example:

- planned
- in process
- completed
- unknown

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ShipmentEventStatus | ShipmentEventStatusId | yes | string | 36 | The unique identifier of a Shipment Event Status. |
| ShipmentEventStatus | ShipmentEventStatusDescription | no | string | 512 | The description of a Shipment Event Status. |
| ShipmentEventStatus | ShipmentEventStatusName | no | string | 128 | The name of a Shipment Event Status.. |
