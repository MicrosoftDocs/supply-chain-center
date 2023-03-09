---
title: ShipmentLocation
description: This article provides information about the ShipmentLocation entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# ShipmentLocation

A location of a shipment.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ShipmentLocation | PeriodStartTimestamp | yes | timestamp | 14 | The period start timestamp that the shipment was at the shipping location. |
| ShipmentLocation | ShipmentId | yes | string | 36 | The unique identifier of a Shipment. |
| ShipmentLocation | ShippingLocationId | no | string | 36 | The unique identifier of a Shipping Location. |
| ShipmentLocation | LocationId | no | string | 36 | The unique identifier of a Location. |
| ShipmentLocation | ShipmentLegNumber | no | integer | 9 | The unique identifier of the Shipment Leg Number, which equals the shipment leg 'sequence number'. |
| ShipmentLocation | ShipmentLocationGpsLatitudePosition | no | decimal | 14 | The GPS position of the Shipment Location. expressed in latitude. This may be an in-transit location.</br></br>For example:GPS Coords (Ex= 39deg 58.589min) - seconds are converted to decimal format. |
| ShipmentLocation | PeriodEndTimestamp | no | timestamp | 14 | The period end timestamp that the shipment was at the shipping location. |
| ShipmentLocation | VendorId | no | string | 36 | The unique identifier of a Vendor. |
| ShipmentLocation | ShipmentLocationGpsLongitudePosition | no | decimal | 14 | The GPS position of the Shipment expressed in longitude. This may be an in-transit location.</br></br>For example: GPS Coords (Ex= 39deg 58.589min) - seconds are converted to decimal format.. |
