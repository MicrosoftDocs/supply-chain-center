---
title: Location
description: This article provides information about the Location entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# MaterialResourcePlanningSchedule

Material resource planning (MRP) for an item with expected requirement date.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| MaterialResourcePlanningSchedule | PeriodStartDate | yes | timestamp | 8 | Start date of the material resource planning schedule. |
| MaterialResourcePlanningSchedule | ItemSku | yes | string | 20 | Unique Id of the item. |
| MaterialResourcePlanningSchedule | MasterScheduleId | yes | string | 36 | Unique Id of the master schedule. |
| MaterialResourcePlanningSchedule | ForecastDescription | no | string | 4000 | Forecast description. |
| MaterialResourcePlanningSchedule | PeriodEndDate | no | timestamp | 8 | End date of the material resource planning schedule. |
| MaterialResourcePlanningSchedule | VendorLocationId | no | string | 36 | Supplier location ID. |
| MaterialResourcePlanningSchedule | SupplierPartNumber | no | string | 256 | Unique Id of the supplier's item. |
| MaterialResourcePlanningSchedule | VendorId | no | string | 36 | Unique Id of the supplier or vendor. |
| MaterialResourcePlanningSchedule | MRPPlanner | no | string | 40 | MRP planner associated with Material Resource Planning (MRP). |
| MaterialResourcePlanningSchedule | UnitOfMeasureId | no | string | 36 | Unit of measure Id. |
| MaterialResourcePlanningSchedule | WarehouseName | no | string | 256 | Name of the warehouse. |
