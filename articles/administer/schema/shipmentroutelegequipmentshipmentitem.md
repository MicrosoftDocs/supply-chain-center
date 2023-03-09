---
title: ShipmentRouteLegEquipmentShipmentItem
description: This article provides information about the ShipmentRouteLegEquipmentShipmentItem entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# ShipmentRouteLegEquipmentShipmentItem

The shipment items that are being transported on the shipment route leg shipment mode.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ShipmentRouteLegEquipmentShipmentItem | ShipmentItemNumber | yes | integer | 10 | The shipment line number. |
| ShipmentRouteLegEquipmentShipmentItem | ShipmentItemDeconsolidationNumber | yes | integer | 9 | A portion (breakdown / deconsolidation) of the a shipment item into smaller parts for the purpose of transport. |
| ShipmentRouteLegEquipmentShipmentItem | SRLEquipmentSequenceNumber | yes | integer | 9 | The sequence number associated with the shipment route/leg equipment. |
| ShipmentRouteLegEquipmentShipmentItem | ShipmentId | yes | string | 36 | The unique identifier of a Shipment. |
| ShipmentRouteLegEquipmentShipmentItem | ShipmentLegNumber | yes | integer | 9 | The unique identifier of the Shipment Leg Number, which equals the shipment leg 'sequence number'. |
| ShipmentRouteLegEquipmentShipmentItem | ShipmentRouteLegEquipmentShipmentItemNote | no | string | 1024 | A note, comment, or additional information regarding the shipment route leg equipment shipment item. |
