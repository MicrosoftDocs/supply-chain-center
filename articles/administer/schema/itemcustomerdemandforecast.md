---
title: ItemCustomerDemandForecast
description: This article provides information about the ItemCustomerDemandForecast entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# ItemCustomerDemandForecast

Forecast made for a specific time period for an item demanded by a customer.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ItemCustomerDemandForecast | ItemSku | yes | string | 20 | Unique ID of the Item. |
| ItemCustomerDemandForecast | ItemCustomerDemandForecastId | yes | string | 36 | Unique ID of the customer demand forecast. |
| ItemCustomerDemandForecast | ItemCustomerDemandForecastNote | no | string | 1024 | Additional notes or descriptions for the customer demand forecast. |
| ItemCustomerDemandForecast | ItemCustomerDemandForecastEndDate | no | timestamp | 8 | End date of the forecast period for this customer demand forecast ID. |
| ItemCustomerDemandForecast | ItemCustomerDemandForecastStartDate | no | timestamp | 8 | Start date of the forecast period for this customer demand forecast ID. |
| ItemCustomerDemandForecast | ItemCustomerDemandForecastQuantity | no | decimal | 9 | Forecast quantity for this period. |
| ItemCustomerDemandForecast | LocationId | no | string | 36 | Location Id for which the forecast is applicable. |
| ItemCustomerDemandForecast | UnitOfMeasureId | no | string | 36 | Unit of measure of the forecast quantity. |
| ItemCustomerDemandForecast | CustomerId | no | string | 36 | Customer Id for the forecast. |
| ItemCustomerDemandForecast | ItemCustomerDemandForecastName | no | string | 256 | Name of the forecast.. |
