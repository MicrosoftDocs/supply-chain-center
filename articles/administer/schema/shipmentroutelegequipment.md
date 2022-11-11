---
title: ShipmentRouteLegEquipment
description: This article provides information about the ShipmentRouteLegEquipment entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# ShipmentRouteLegEquipment

The shipment mode(s) being utilized for the shipment route leg.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ShipmentRouteLegEquipment | SRLEquipmentSequenceNumber | yes | integer | 10 | The sequence number associated with the shipment route/leg equipment. |
| ShipmentRouteLegEquipment | ShipmentLegNumber | yes | integer | 9 | The unique identifier of the Shipment Leg Number, which equals the shipment leg 'sequence number'. |
| ShipmentRouteLegEquipment | ShipmentId | yes | string | 36 | The unique identifier of a Shipment. |
| ShipmentRouteLegEquipment | TrailerId | no | string | 36 | The unique identifier of a trailer. |
| ShipmentRouteLegEquipment | EngineId | no | string | 36 | The unique identifier of an engine. |
| ShipmentRouteLegEquipment | BargeId | no | string | 36 | The unique identifier of a Barge instance. |
| ShipmentRouteLegEquipment | VehicleId | no | string | 36 | The unique identifier of a Vehicle. |
| ShipmentRouteLegEquipment | ContainerId | no | string | 36 | The unique identifier of the container.</br></br> This would be the 'serial number' of the container if it is serialized. |
| ShipmentRouteLegEquipment | StorageContainerId | no | string | 36 | The unique identifier of a Storage Container. |
| ShipmentRouteLegEquipment | RailcarId | no | string | 36 | The unique identifier of a Railcar instance. |
| ShipmentRouteLegEquipment | PipelineStationId | no | string | 36 | The unique identifier of a Pipeline Station. |
| ShipmentRouteLegEquipment | ShipmentLegFromLocationId | no | string | 36 | The unique identifier of the From-Location. |
| ShipmentRouteLegEquipment | ShipmentLegToLocationId | no | string | 36 | The unique identifier of the To-Location. |
| ShipmentRouteLegEquipment | PeriodStartTimestamp | no | timestamp | 14 | The period start timestamp associated with the shipment route/leg shipment mode. |
| ShipmentRouteLegEquipment | PeriodEndTimestamp | no | timestamp | 14 | The period end timestamp associated with the shipment route/leg shipment mode. |
| ShipmentRouteLegEquipment | VesselId | no | string | 36 | The unique identifier of a vessel/ship. |
| ShipmentRouteLegEquipment | TowboatId | no | string | 36 | The unique identifier of a towboat. |
| ShipmentRouteLegEquipment | InterlineCargoTransferLocationIndicator | no | boolean | 14 | Indicates that the cargo is arriving at a point by one carrier and continuing its journey through another carrier. |
| ShipmentRouteLegEquipment | AircraftId | no | string | 36 | The unique identifier of an Aircraft. |
