---
title: CarrierLocation
description: This article provides information about the CarrierLocation entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# CarrierLocation

The carrier location(s) of the associated Location Type for the indicated period.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| CarrierLocation | PeriodStartTimestamp | yes | timestamp | 8 | The period start timestamp associated with the information. |
| CarrierLocation | LocationTypeId | yes | string | 36 | The unique identifier of a Location Type. |
| CarrierLocation | LocationId | yes | string | 36 | The unique identifier of a Location. |
| CarrierLocation | CarrierId | yes | string | 36 | The unique identifier of a Carrier. |
| CarrierLocation | PreferenceId | no | string | 36 | The unique identifier of a Preference. |
| CarrierLocation | CarrierLocationNote | no | string | 1024 | A note, comment or additional information regarding a Carrier Location. |
| CarrierLocation | GlobalLocationNumber | no | decimal | 16 | The Global Location Number (GLN) is a simple tool used to uniquely identify locations. It can be used to identify physical locations such as a warehouse, legal entities, or a function / department within a legal entity. The GLN is part of the GS1 system of standards. |
| CarrierLocation | PeriodEndTimestamp | no | timestamp | 8 | The period end timestamp associated with the information. |

EOF