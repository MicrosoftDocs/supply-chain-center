---
title: BuildPlan
description: This article provides information about BuildPlan entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# BuildPlan

A Build Plan is the break down, usually by a specific Item, to accomplish the Master Schedule or Material Requirements Planning (Demand)

 The Master Schedule-Product Build is the product building plan that is used by manufacturers to build products or items via one or more individual Build Plans. A Master Schedule is a schedule to build several item(s) over a specific period. A Master Schedule may identify one or more Items to build. A Build Plan is the breakdown, usually by a specific Item, to accomplish the Master Schedule.
 A Run is the actual order to manufacture, or build a set number of Items on a date and/or time.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| BuildPlan | BuildPlanId | yes | string | 36 | The unique identifier of a Build Plan. |
| BuildPlan | BuildPlanPriorityId | no | string | 36 | The unique identifier of a Build Plan Priority. |
| BuildPlan | BuildPlanPeriodEndDate | no | date | 8 | The date that the Build Plan Period ended. |
| BuildPlan | BuildPlanPeriodStartDate | no | date | 8 | The date that the Build Plan Period started. |
| BuildPlan | BuildPlanStatusId | no | string | 36 | The unique identifier of a Build Plan Status. |
| BuildPlan | ManufacturerId | no | string | 36 | Manufacturer ID is the supplier ID or manufacturing location ID who will fulfill the demand |
| BuildPlan | ManufacturerFacilityId | no | string | 36 | Manufacturing facility ID is the warehouse ID or plant ID where the demand is needed to required |
| BuildPlan | ItemSku | no | string | 20 | The Stock Keeping Unit identifier, which is typically used for inventory-related activities. |
| BuildPlan | MasterScheduleId | no | string | 36 | The unique identifier of a Master Schedule. |
| BuildPlan | BuildPlanName | no | string | 128 | The name of the Build Plan. |
| BuildPlan | BuildPlanCreatedDate | no | date | 8 | The date that the Build Plan was created. |
| BuildPlan | BuildPlanItemUnitQuantity | no | decimal | 8,2 | The total number of item(s) to be built under the associated Build Plan. |

EOF