---
title: Build your own apps by using Power Apps
description: This article provides information about how to use Microsoft Power Apps to build your own apps in Supply Chain Center.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: overview
ms.date: 7/11/2023
ms.custom: bap-template
---

# Build your own apps by using Power Apps

[!INCLUDE[banner](../includes/banner.md)]

Microsoft Supply Chain Center supports the ability of users to build their own apps by using Power Apps. Power Apps is a suite of apps, services, and connectors, and a data platform that provides a rapid development environment where you can build custom apps that meet your business needs. By using Power Apps, you can quickly build custom business apps that connect to data that's stored in either the underlying data platform (Dataverse) or various online and on-premises data sources (such as SharePoint, Microsoft 365, Dynamics 365, or SQL Server).

Power Apps simplifies the experience of building business apps by enabling users to create feature-rich, custom business apps without writing code. Apps that you build by using Power Apps provide rich business logic and workflow capabilities to transform your manual business operations into digital, automated processes. They have a responsive design and can run seamlessly in a browser and on mobile devices (phone or tablet).

Power Apps also provides an extensible platform that lets pro developers programmatically interact with data and metadata, apply business logic, create custom connectors, and integrate with external data.

For more information about how to build apps by using Power Apps, see [Overview of creating apps in Power Apps](/power-apps/maker/).

## Build apps in Supply Chain Center

Supply Chain Center's underlying data platform is Dataverse. Data that's ingested in Supply Chain Center for analytical purposes lands in a managed data lake (MDL). To build apps by using Power Apps, you must make the data available in Dataverse by hydrating it from the MDL to Dataverse.

To build apps, open the [Power Apps maker portal](https://make.powerapps.com/).

The following entities are currently available from the MDL to Dataverse.

| Entity name                               | Alias or display name              |
|-------------------------------------------|------------------------------------|
| msdyn\_accountproductleadtime             | AccountProductLeadTime             |
| msdyn\_accountproductprice                | AccountProductPrice                |
| msdyn\_accountproductstatus               | AccountProductStatus               |
| msdyn\_materialresourceplanningschedule   | ProductResourcePlanningSchedule    |
| msdyn\_productaccountdemandforecast       | ProductAccountDemandForecast       |
| msdyn\_productaccountsupplyplan           | ProductAccountSupplyPlan           |
| msdyn\_productinventory                   | WarehouseProductAvailableStock     |
| msdyn\_purchaseorder                      | PurchaseOrder                      |
| msdyn\_purchaseorderproduct               | PurchaseOrderLine                  |
| msdyn\_shipment                           | Shipment                           |
| msdyn\_shipmentproduct                    | ShipmentProduct                    |
| msdyn\_shipmentrouteleg                   | ShipmentRouteLeg                   |
| msdyn\_shippingcarrier                    | Carrier                            |
| msdyn\_shippingcarrierroute               | CarrierRoute                       |
| msdyn\_warehouse                          | Warehouse                          |
| msdyn\_carrierroutecustomertariffschedule | CarrierRouteCustomerTariffSchedule |
| product                                   | Product                            |
| salesorder                                | SalesOrder                         |
| salesorderdetail                          | SalesOrderDetail                   |

If any of the entities that you need to build apps aren't listed, reach out to the [Supply Chain Center communities forum](https://community.dynamics.com/forums/thread/?partialUrl=microsoft-supply-chain-center), or send an email to <mscc_support@microsoft.com>.
