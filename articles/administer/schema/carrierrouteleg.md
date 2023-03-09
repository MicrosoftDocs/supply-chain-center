---
title: CarrierRouteLeg
description: This article provides information about the CarrierRouteLeg entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# CarrierRouteLeg

The one or more locations that comprise a route in the associated sequence.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| CarrierRouteLeg | CarrierRouteId | yes | string | 36 | The unique identifier of a Carrier Route. |
| CarrierRouteLeg | CarrierRouteLegNumber | yes | integer | 8 | The assigned to the Carrier Route Leg. |
| CarrierRouteLeg | CarrierId | yes | string | 36 | The unique identifier of a Carrier. |
| CarrierRouteLeg | FromLocationId | no | string | 36 | The unique identifier of a Shipping Location. |
| CarrierRouteLeg | ShipmentMethodName | no | string | 256 | The unique identifier of a Shipment Method. |
| CarrierRouteLeg | PlannedRouteLegTransitTime | no | string | 256 | The planned transit time for completion of the leg in hours. |
| CarrierRouteLeg | PlannedRouteLegDistance | no | integer | 8 | The planned route leg distance in miles. |
| CarrierRouteLeg | ToLocationId | no | string | 36 | The unique identifier of a Shipping Location. |

EOF