---
title: ItemCustomerSupplyPlan
description: This article provides information about the ItemCustomerSupplyPlan entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# ItemCustomerSupplyPlan

Supply plan quantity that is planned for a customer by the supplier.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ItemCustomerSupplyPlan | ItemCustomerSupplyPlanId | yes | string | 36 | Unique Id of the item customer supply plan. |
| ItemCustomerSupplyPlan | UnitOfMeasureId | no | string | 36 | Unit of measure for Item customer supply plan quantity. |
| ItemCustomerSupplyPlan | ItemCustomerSupplyPlanNote | no | string | 256 | Note for item customer supply plan. |
| ItemCustomerSupplyPlan | ItemSku | no | string | 20 | Unique Id of the item. |
| ItemCustomerSupplyPlan | ItemCustomerSupplyPlanDate | no | date | 0 | Item customer plan date. |
| ItemCustomerSupplyPlan | ItemCustomerSupplyPlanQuantity | no | decimal | 0 | Item customer supply plan quantity. |
