---
title: ItemCustomerSupplyAllocation
description: This article provides information about the ItemCustomerSupplyAllocation entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# ItemCustomerSupplyAllocation

Item customer supply allocation made based on Item Customer Supply Plan and Item Customer Demand Forecast.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ItemCustomerSupplyAllocation | ItemSku | yes | string | 20 | Unique Id of the item. |
| ItemCustomerSupplyAllocation | UnitOfMeasureId | no | string | 36 | Unit of measure of the allocation quantity. |
| ItemCustomerSupplyAllocation | ItemCustomerSupplyAllocationNote | no | string | 1024 | Notes or descriptions for the customer allocation. |
| ItemCustomerSupplyAllocation | ItemSupplyAllocationQuantity | no | decimal | 9 | Item supply allocation quantity from supplier. |
| ItemCustomerSupplyAllocation | ItemCustomerSupplyPlanId | no | string | 36 | Unique Id of Item customer supply plan. |
| ItemCustomerSupplyAllocation | ItemCustomerDemandForecastId | no | string | 36 | Unique Id of customer demand forecast.. |
