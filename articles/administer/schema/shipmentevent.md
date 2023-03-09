---
title: ShipmentEvent
description: This article provides information about the ShipmentEvent entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# ShipmentEvent

An event that is associated with a Shipment to track its progress or status as it is shipped, stored, in customs etc.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ShipmentEvent | ShipmentEventStartTimestamp | yes | timestamp | 14 | The start timestamp of the associated Shipment Event. |
| ShipmentEvent | ShipmentEventTypeId | yes | string | 36 | The unique identifier of a Shipment Event Type. |
| ShipmentEvent | ShipmentId | yes | string | 36 | The unique identifier of a Shipment. |
| ShipmentEvent | Sequence | no | string | 256 | Sequence number of the event |
| ShipmentEvent | ExceptionInitiatedBy | no | string | 256 | Event initiator |
| ShipmentEvent | ShipmentEventStatus | no | string | 256 | Shipment event status |
| ShipmentEvent | LoadNumber | no | string | 256 | Load number of the shipment |
| ShipmentEvent | CustomAttributes | no | string | 4000 | Custom attributes |
| ShipmentEvent | ExpectedDeliveryDateTimestamp | no | string | 256 | Expected delivery date time stamp |
| ShipmentEvent | ShipmentEventTypeDescription | no | string | 256 | Shipment event type |
| ShipmentEvent | ShippingLocationId | no | string | 36 | The unique identifier of a Shipping Location. |
| ShipmentEvent | ShipmentEventStatusId | no | string | 36 | The unique identifier of a Shipment Event Status. |
| ShipmentEvent | ShipmentEventEndTimestamp | no | timestamp | 14 | The end timestamp of the associated Shipment Event. |
| ShipmentEvent | ShipmentReferenceNumber | no | string | 256 | Reference number of the shipment |
| ShipmentEvent | ShipmentEventTypeName | no | string | 256 | Name of the shipment event |
| ShipmentEvent | TrackingIdentifier | no | string | 256 | Tracking number of the shipment |
| ShipmentEvent | ShipmentReferenceNumberTypeName | no | string | 256 | Name of the shipment reference number type |

EOF