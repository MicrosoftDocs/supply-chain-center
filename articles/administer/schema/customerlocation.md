---
title: CustomerLocation
description: This article provides information about the CustomerLocation entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# CustomerLocation

The customer location(s) of the associated Location Type for the indicated period.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| CustomerLocation | LocationId | yes | string | 36 | The unique identifier of a Location. |
| CustomerLocation | PeriodStartTimestamp | yes | timestamp | 8 | The period start timestamp associated with the information. |
| CustomerLocation | CustomerId | yes | string | 36 | The unique identifier of a Customer. |
| CustomerLocation | LocationTypeId | yes | string | 36 | The unique identifier of a Location Type. |
