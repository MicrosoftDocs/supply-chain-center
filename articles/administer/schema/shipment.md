---
title: Shipment
description: This article provides information about the Shipment entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# Shipment

A quantity of items, goods or bulk cargo that are shipped together.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| Shipment | ShipmentId | yes | string | 36 | The unique identifier of a Shipment. |
| Shipment | ChannelId | no | string | 36 | The unique identifier of a Channel. |
| Shipment | RequestedCarrierId | no | string | 36 | The unique identifier of a Carrier. |
| Shipment | PalletTypeId | no | string | 36 | The unique identifier of a Pallet Type. |
| Shipment | ContainerId | no | string | 36 | The unique identifier of the container.</br></br> This would be the 'serial number' of the container if it is serialized. |
| Shipment | CarrierId | no | string | 36 | The unique identifier of a Carrier. |
| Shipment | ShipmentTypeId | no | string | 36 | The unique identifier of a Shipment Type. |
| Shipment | PackingTypeId | no | string | 36 | The unique identifier of a Packing Type. |
| Shipment | ShipmentMethodName | no | string | 256 | The unique identifier of a Shipment Method. |
| Shipment | WarehouseId | no | string | 36 | The unique identifier of a Warehouse. |
| Shipment | IncotermId | no | string | 36 | The unique identifier of a Incoterm. |
| Shipment | OriginationWarehouseId | no | string | 36 | The unique identifier of a Warehouse. |
| Shipment | VolumeUnitOfMeasureId | no | string | 36 | Note: A temporary divider header that is used to separate and organize information for the viewer.</br></br> This column is marked 'Logical Only' and is therefore 'for presentation only' and will not be used when generating DDL. |
| Shipment | ShipmentVolume | no | decimal | 9 | The volume of the shipment. |
| Shipment | LengthWidthHeightUnitOfMeasureId | no | string | 36 | The unique identifier of a Unit Of Measure. |
| Shipment | TimeSpentAtDeliveryLocation | no | string | 256 | The amount of time spent at the ship-to address to deliver the shipment. |
| Shipment | WeightUnitOfMeasureId | no | string | 36 | The unique identifier of a Unit Of Measure. |
| Shipment | ShipmentHeight | no | decimal | 9 | The height of the Shipment. |
| Shipment | DestinationWarehouseId | no | string | 36 | The unique identifier of a Warehouse. |
| Shipment | ShipmentWidth | no | decimal | 9 | The width of the Shipment. |
| Shipment | ShipmentNetWeight | no | decimal | 9 | The weight of the Shipment. |
| Shipment | ShipmentLength | no | decimal | 9 | The length of the Shipment. |
| Shipment | ShipmentFromName | no | string | 128 | The name of the ship-from party. |
| Shipment | ActualShipTimestamp | no | timestamp | 14 | The actual shipment date. |
| Shipment | ShipmentFromLocationId | no | string | 36 | The unique identifier of a Location. |
| Shipment | MasterShipmentNumber | no | integer | 9 | A master shipment number is used to tie multiple shipments together. It is typically used when one or more shipments are to be considered to be a single shipment for billing purposes. |
| Shipment | ShipmentToName | no | string | 128 | The name of the ship-to party. |
| Shipment | ShipmentTotalNetWeight | no | decimal | 9 | Net Weight - The total weight of a shipment less the weight of containers, pallets, nets or straps. |
| Shipment | ShipmentToLocationId | no | string | 36 | The unique identifier of a Location. |
| Shipment | ShipmentTotalGrossWeight | no | decimal | 9 | The full weight of a shipment including goods and packaging.</br></br> The weight of the shipment including all packing, blocking, platforms, special bracing, etc., if required. (includes weight of unit load device, when applicable.) |
| Shipment | PlannedShipTimestamp | no | timestamp | 14 | The planned date of shipment. |
| Shipment | PlannedLatestDeliveryTimestamp | no | timestamp | 14 | The latest that the shipment can be delivered. |
| Shipment | TrackingIdentifier | no | string | 1024 | A tracking identifier is a number or alphanumeric string consisting of a series of numbers and letters, used to uniquely identify a handling unit associated with a shipment. |
| Shipment | PlannedLatestPickUpTimestamp | no | timestamp | 14 | The latest that the shipment can be picked-up. |
| Shipment | PlannedEarliestPickUpTimestamp | no | timestamp | 14 | The earliest that the shipment can be picked up. |
| Shipment | PlannedEarliestDeliveryTimestamp | no | timestamp | 14 | The earliest that the shipment can be delivered. |
| Shipment | ShipmentDeliveryTimestamp | no | timestamp | 14 | The timestamp that the shipment was received or delivered at the ship-to address. |
| Shipment | EstimatedDeliveryTimestamp | no | timestamp | 14 | Estimated delivery timestamp. |
| Shipment | GlobalShipmentIdentificationNumber | no | decimal | 13 | The Global Shipment Identification Number (GSIN) is part of the GS1 system of standards. It is used to identify shipments.</br></br> A shipment, which may be comprised of one or more logistic units, is intended to be delivered together. The logistic units belonging to a particular shipment keep the same GSIN during all transport stages, from origin to final destination. |
| Shipment | ShipmentBookingNumber | no | integer | 10 | Reservation number used to secure equipment and act as a control number prior to completion of a B/L. |
| Shipment | ShipmentOrderId | no | string | 36 | The unique number that identifies an Order. |
| Shipment | EstimatedNumberDeliveryDays | no | integer | 9 | The estimated number of days to deliver the Shipment. |
| Shipment | ShipmentOrderLineNumber | no | integer | 9 | The number that identifies the Order Line Item. |
