---
title: CarrierLocationCutoffTime
description: This article provides information about the CarrierLocationCutoffTime entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# CarrierLocationCutoffTime

The last time for which the identified shipment service type is offered by the carrier at a particular location on a particular day.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| CarrierLocationCutoffTime | DayOfWeekId | yes | integer | 3 | The unique identifier of a Day Of Week. |
| CarrierLocationCutoffTime | ShipmentServiceTypeId | yes | string | 36 | The unique identifier of a Shipment Service Type. |
| CarrierLocationCutoffTime | LocationId | yes | string | 36 | The unique identifier of a Location. |
| CarrierLocationCutoffTime | CarrierId | yes | string | 36 | The unique identifier of a Carrier. |
| CarrierLocationCutoffTime | PeriodStartTimestamp | yes | timestamp | 8 | The period start timestamp associated with the information. |
| CarrierLocationCutoffTime | CarrierLocationCutoffTime | no | timestamp | 8 | The last time for which the identified shipment service type is offered by the carrier on a particular day. |
| CarrierLocationCutoffTime | PeriodEndTimestamp | no | timestamp | 8 | The period end timestamp associated with the information.. |
