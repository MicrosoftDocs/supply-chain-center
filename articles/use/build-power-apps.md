---
title: Build own Power Apps
description: This article describes the process to Build Own Power Apps in Microsoft Supply Chain Center.
author: mkannapiran
ms.author: mkannapiran
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: overview
ms.date: 7/11/2023
ms.custom: bap-template
---

# **Build Own Power Apps**

Microsoft Supply Chain Center supports user to build their own Power Apps. Power Apps is a suite of apps, services, and connectors, as well as a data platform, that provides a rapid development environment to build custom apps for your business needs. Using Power Apps, you can quickly build custom business apps that connect to your data stored either in the underlying data platform (Microsoft Dataverse) or in various online and on-premises data sources (such as SharePoint, Microsoft 365, Dynamics 365, SQL Server, and so on). 

Apps built using Power Apps provide rich business logic and workflow capabilities to transform your manual business operations into digital, automated processes. What's more, apps built using Power Apps have a responsive design and can run seamlessly in browser and on mobile devices (phone or tablet). Power Apps "democratizes" the business-app-building experience by enabling users to create feature-rich, custom business apps without writing code.

Power Apps also provides an extensible platform that lets pro developers programmatically interact with data and metadata, apply business logic, create custom connectors, and integrate with external data.

For more information on how to build power apss visit https://learn.microsoft.com/en-us/power-apps/maker/ 

## **How to build Power Apps in Supply Chain Center**

Microsoft Supply Chain Center's underlying data platform is Microsoft Dataverse. Data ingested in Microsoft Supply Chain Center for analytical purposes lands in Managed Data Lake (MDL). To build Power Apps, the data has to be available in Dataverse to build Power Apps. For this to happen the data has to be hydrated from MDL to Dataverse. 

To build Power Apps visit https://make.powerapps.com/

The following entities are currently available from MDL to Dataverse.

| **Entity Name**                          | **Alias or Display Name**          |
|------------------------------------------|------------------------------------|
| msdyn_accountproductleadtime             | AccountProductLeadTime             |
| msdyn_accountproductprice                | AccountProductPrice                |
| msdyn_accountproductstatus               | AccountProductStatus               |
| msdyn_materialresourceplanningschedule   | ProductResourcePlanningSchedule    |
| msdyn_productaccountdemandforecast       | ProductAccountDemandForecast       |
| msdyn_productaccountsupplyplan           | ProductAccountSupplyPlan           |
| msdyn_productinventory                   | WarehouseProductAvailableStock     |
| msdyn_purchaseorder                      | PurchaseOrder                      |
| msdyn_purchaseorderproduct               | PurchaseOrderLine                  |
| msdyn_shipment                           | Shipment                           |
| msdyn_shipmentproduct                    | ShipmentProduct                    |
| msdyn_shipmentrouteleg                   | ShipmentRouteLeg                   |
| msdyn_shippingcarrier                    | Carrier                            |
| msdyn_shippingcarrierroute               | CarrierRoute                       |
| msdyn_warehouse                          | Warehouse                          |
| msdyn_carrierroutecustomertariffschedule | CarrierRouteCustomerTariffSchedule |
| product                                  | Product                            |
| salesorder                               | SalesOrder                         |
| salesorderdetail                         | SalesOrderDetail                   |


If any of the entities needed to build Power Apps are not in the list of entities from above, please reach out to Microsoft Supply Chain Center communities forum by clicking this link https://community.dynamics.com/forums/thread/?partialUrl=microsoft-supply-chain-center or write an email to mscc_support@microsoft.com
