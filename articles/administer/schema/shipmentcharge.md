---
title: ShipmentCharge
description: This article provides information about the ShipmentCharge entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# ShipmentCharge

A charge or fee incurred by the shipment by the indicated party.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ShipmentCharge | ShipmentChargeTimestamp | yes | timestamp | 14 | The timestamp of the shipment charge. |
| ShipmentCharge | ShipmentChargeTypeId | yes | string | 36 | The unique identifier of a shipment charge type. |
| ShipmentCharge | ShipmentId | yes | string | 36 | The unique identifier of a Shipment. |
| ShipmentCharge | ShipmentChargePaidTimestamp | no | timestamp | 14 | The timestamp that the shipment charge was paid. |
| ShipmentCharge | ChargeByPartyId | no | string | 36 | The unique identifier of a Party. |
| ShipmentCharge | ShipmentLegNumber | no | integer | 9 | The unique identifier of the Shipment Leg Number, which equals the shipment leg 'sequence number'. |
| ShipmentCharge | ShipmentChargeAmount | no | decimal | 9 | The amount of the shipment charge. |
