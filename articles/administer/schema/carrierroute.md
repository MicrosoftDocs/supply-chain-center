---
title: CarrierRoute
description: This article provides information about the CarrierRoute entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# CarrierRoute

A carrier-defined published route to send cargo.

Example:

FED/ Route 1 = SFO to Shanghai by AIR

From: San Francisco, US , From Location = SFO

To: Shanghai, China, To Location = SHA

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| CarrierRoute | CarrierRouteId | yes | string | 36 | The unique identifier of a Carrier Route. |
| CarrierRoute | CarrierId | yes | string | 36 | The unique identifier of a Carrier. |
| CarrierRoute | ShipmentMethodName | no | string | 256 | The unique identifier of a Shipment Method. |
| CarrierRoute | PlannedRouteTransitTime | no | string | 256 | The planned route transit time to complete. |
| CarrierRoute | PlannedRouteDistance | no | integer | 8 | The planned route distance expressed in miles. |
| CarrierRoute | RouteId | no | string | 36 | The unique identifier of a route. |
| CarrierRoute | FromLocationId | no | string | 36 | The unique identifier of a Shipping Location. |
| CarrierRoute | ToLocationId | no | string | 36 | The unique identifier of a Shipping Location. |
