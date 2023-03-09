---
title: ItemVendorSupplyPlan
description: This article provides information about the ItemVendorSupplyPlan entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# ItemVendorSupplyPlan

A supply plan that a vendor makes for an item.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ItemVendorSupplyPlan | ItemVendorSupplyPlanId | yes | string | 36 | Unique Id of the item vendor supply plan. |
| ItemVendorSupplyPlan | ItemSku | yes | string | 20 | Unique Id of the item. |
| ItemVendorSupplyPlan | ItemSupplyPlanName | no | string | 256 | Name of the item supply plan. |
| ItemVendorSupplyPlan | ItemVendorSupplyPlanNote | no | string | 1024 | Note for item vendor supply plan. |
| ItemVendorSupplyPlan | VendorId | no | string | 36 | Unique Id of the supplier or vendor. |
| ItemVendorSupplyPlan | SupplierPartNumber | no | string | 256 | Unique Id of the supplier's item. |
| ItemVendorSupplyPlan | MRPPlanner | no | string | 256 | MRP planner associated with vendor supply plan. |
| ItemVendorSupplyPlan | UnitOfMeasureId | no | string | 36 | Unit of measure Id for the supply plan quantity. |
| ItemVendorSupplyPlan | FromLocationId | no | string | 36 | Vendor supply plan for from location Id. |
| ItemVendorSupplyPlan | ItemVendorSupplyPlanEndDate | no | timestamp | 0 | End date of the item vendor supply plan |
| ItemVendorSupplyPlan | ToWarehouseId | no | string | 36 | Vendor supply plan for the To location Id. |
| ItemVendorSupplyPlan | ItemVendorSupplyPlanQuantity | no | decimal | 0 | Item vendor supply plan quantity. |
| ItemVendorSupplyPlan | ItemVendorSupplyPlanStartDate | no | timestamp | 0 | Start date of the item vendor supply plan. |

EOF