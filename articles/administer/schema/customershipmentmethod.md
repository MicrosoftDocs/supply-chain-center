---
title: CustomerShipmentMethod
description: This article provides information about the CustomerShipmentMethod entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# CustomerShipmentMethod

"The customer shipment parameters associated with a customer for the indicated period defined by: Shipment Method, Carrier "

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| CustomerShipmentMethod | CarrierId | yes | string | 36 | The unique identifier of a Carrier. |
| CustomerShipmentMethod | ShipmentMethodName | yes | string | 256 | The unique identifier of a Shipment Method. |
| CustomerShipmentMethod | PeriodStartDate | yes | date | 8 | The period start date for which the associated customer shipment method information is defined. |
| CustomerShipmentMethod | CustomerId | yes | string | 36 | The unique identifier of a Customer. |
| CustomerShipmentMethod | CustomerShipmentMethodNote | no | string | 1024 | A note, comment or additional information regarding the associated customer shipment method. |
| CustomerShipmentMethod | PreferenceId | no | string | 36 | The unique identifier of a Preference. |
| CustomerShipmentMethod | PeriodEndDate | no | date | 8 | The period end date for which the associated customer shipment method information is defined.  |
