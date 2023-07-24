---
title: Use App management to ingest data
description: This article provides information about using App management to ingest data with providers and connectors
author: mkannapiran
ms.author: Kannapiran.Manickavasagam
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: how-to
ms.date: 7/11/2023
ms.custom: bap-template
---

# Use App management to ingest data

App management in Microsoft Supply Chain Center is the process of overseeing the lifecycle of data ingestion. It includes two main categories of data ingestion through the concept of providers and connectors. Providers and connectors are the key functionalities that are composed on two main systems, Power Automate Flows (Transactional) and Power Platform Dataflows (Analytical scenarios). 

Providers provide default data mapping and transformation functionalities that enable simple click features for data ingestion. You have the convenience to accept these default mappings or edit or modify the mappings to suit your requirements.

Connectors

Transactional providers are enabled in supply chain center for Microsoft Intelligent Order Management. There are out of the box transactional providers like SAP ERP, UPS, Flexe, Shipstation, FedEx, Orderful, Avalara, Amazon, Narvar, Uber Freight, and Big commerce. 

Analytical providers are enabled in supply chain center for lighting up out of the box capabilities like Supply Demand Insights (SDI), Calculation table, or KPI features. Currently SAP ERP is the out of the box analytical provider.

![A screenshot of the installed modules and the Providers and Connectors that are available.](media/app-management.png)


## Set up providers

Providers implement default data mapping and transformation functionalities enabling simple click features for data ingestion. You have the convenience to accept these default mappings or edit or modify the mappings to suit your requirements. 

### How to create new instance of provider in Supply Chain Center

To create a new instance of a provider and enable the enable **SAP ERP** provider, follow these steps.

1. From...
1. Search for available providers by typing the provider name in the search bar on the **Providers and connectors** page. You can select the **Type** column to sort by providers or connectors. This example is a step-by-step process to enable **SAP ERP** provider in supply chain center. The steps remain the same for any of the out of the box providers.
1. Hovers over the provider name. You have two options available; open the provider or create a new instance. 
1. Select the plus sign to create a new instance of the provider. 
1. Select the module for which the SAP ERP provider instance is created, and then select **Next**.
1. Accept the terms and conditions, and then select **Next**.
1. Select **New connection** to establish connection between SAP ERP and Supply Chain Center. The SAP ERP connection requires the SAP connection string and login credentials. 

   ![A screenshot of a sample SAP system connection string.](media/sap-erp-provider-connection-string.png)

 1. Enter the connection string details. SAP system connection string, Data gateway, Username and Password are mandatory when creating the connection. 

   Sample connection string

   ``` text
   {"AppServerHost": "sap.xxxxxx.com", "Client": "XXX", "SystemNumber": "XX", "LogonType": "ApplicationServer"}
   ```
1. Select **Save** to establish connection with SAP, and then select **Next**.
1. The **Data transformations** page shows the list of entities available to be mapped from SAP to Supply Chain Center. From the **Sync** column for each entity, select active to synchronize the selected entity. The mapping for each of these entities is auto populated and then you can choose to change those mappings by selecting the pencil icon.
1. From the menu bar, select the **Advance editor** to modify the mappings as required.

   ![A screenshot of the Custom mapping page.](media/sap-erp-mapping.png)

1. On the **Refresh settings** page, select the refresh settings to set up the frequency of data ingestion. You can either set up manual refresh or set up automatic refresh at regular intervals. 
1. Select **Finish setup** to complete setting up SAP ERP provider.

## Connectors

Power Query connectors are Microsoft’s data connectivity and data preparation technologies that let you seamlessly access data stored in hundreds of sources and reshape it to fit your needs—all with an easy to use, engaging, no-code experience. For more information about connectors, see the [Power Query documentation](/power-query/).

In Supply chain center users can use the connectors experience to create instances of data flow. 

### How to create new instance of connector in supply chain center

To create new instance of connector for a SQL Server database, follow these steps.

1. From ...
1. Search for available connectors by typing the connector name in the search bar on the **Providers and connectors** page. You can select the **Type** column to sort by providers or connectors. This example is a step-by-step process to enable the connector experience in Supply Chain Center using the SQL Server database connector. The steps remain the same for any of the out of the box connectors.
1. Choose **SQL Server database**, and the select the plus icon to create a new instance.
1. Select **Next**.
1. Choose the **Ingestion based** scenario, and then select **Next**. 
1. Select the tables or entities, and then select **Next**.
1. Select **Edit** to begin establishing connection with the source.
1. Enter the connection string details. Server, database and user credentials for authentication.

   ![A screenshot of the Connect to data source page.](media/connector-sql-connection.png)

1. Select **Next** to connect to the source.
1. Choose the source entity, and the select **Next**.

![A screenshot of Purchase Order entity selected.](media/connector-table-choose.png)

1. Select **"Map to entity"**.
1. Select **Finish configuration** to complete mapping source data to destination data.

![A screenshot of Purchase Order entity with Map to entity CDM highlighted in red.](media/connector-mapping.png)

1. On the **Refresh settings** page, select the refresh settings to set up the frequency of data ingestion. You can either set up manual refresh or set up automatic refresh at regular intervals. 
1. Select **Save** to save the connector.
