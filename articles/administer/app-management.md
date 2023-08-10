---
title: Use App management to ingest data
description: This article provides information about how to use App management to ingest data through providers and connectors.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: how-to
ms.date: 7/11/2023
ms.custom: bap-template
---

# Use App management to ingest data

App management in Microsoft Supply Chain Center is the process of overseeing the lifecycle of data ingestion. It includes two main categories of data ingestion through the concepts of providers and connectors. Providers and connectors are the key functionalities that are composed in two main systems: Power Automate flows (transactional scenarios) and Microsoft Power Platform dataflows (analytical scenarios).

Providers implement default data mapping and transformation functionalities that enable simple click features for data ingestion. You can accept the default mappings for the sake of convenience, or you can edit or modify them to suit your requirements.

Transactional providers are enabled in Supply Chain Center for Dynamics 365 Intelligent Order Management. Out-of-box transactional providers include SAP ERP, UPS, Flexe, Shipstation, FedEx, Orderful, Avalara, Amazon, Narvar, Uber Freight, and Big commerce.

Analytical providers that are enabled in Supply Chain Center to light up out-of-box capabilities such as Supply & demand insights, calculation table, and key performance indicator (KPI) features. Currently, SAP ERP is the only out-of-box analytical provider.

:::image type="content" source="media/app-management.png" alt-text="Screenshot that shows the installed modules and the providers and connectors that are available."::: 

## Set up providers

Providers implement default data mapping and transformation functionalities that enable simple click features for data ingestion. You can accept the default mappings for the sake of convenience, or you can edit or modify them to suit your requirements.

### Create a new instance of a provider in Supply Chain Center

To create and enable a new instance of a provider, follow these steps. This procedure uses the SAP ERP provider as an example, but the basic steps are the same for any other out-of-box provider.

1. In Supply Chain Center, select **Admin Settings** on the left menu.
1. Select **App management**.
1. Search for available providers by entering the provider name in the search bar on the **Providers and connectors** page. You can select the **Type** column to sort by providers or connectors.
1. Select the **SAP ERP** provider.
1. Hover over the provider name. You have two options: open the provider, or create a new instance of it.
1. Select the plus sign (**\+**) to create a new instance of the provider.
1. Select the module to create the instance of the SAP ERP provider for, and then select **Next**.
1. Accept the terms and conditions, and then select **Next**.
1. Select **New connection** to establish a connection between SAP ERP and Supply Chain Center.
1. The SAP ERP connection requires the SAP system connection string and sign-in credentials. On the **Connection settings** page, enter the connection string, data gateway, user name, and password. Here's an example of a connection string:

    `{"AppServerHost": "sap.xxxxxx.com", "Client": "XXX", "SystemNumber": "XX", "LogonType": "ApplicationServer"}`

    :::image type="content" source="media/sap-erp-provider-connection-string.png" alt-text="Screenshot that shows an example of a sample SAP system connection string.":::

1. Select **Save** to establish a connection with SAP, and then select **Next**.
1. The **Data transformations** page shows the list of entities that are available to be mapped from SAP to Supply Chain Center. In the **Sync** column for each entity, select **active** to synchronize the entity. The mapping for each of the entities is automatically filled in. However, you can change the mappings by selecting the pencil symbol.
1. On the menu bar, select **Advance editor** to modify the mappings as you require.

    :::image type="content" source="media/sap-erp-mapping.png" alt-text="Screenshot of the Custom mapping page.":::

1. On the **Refresh settings** page, select the refresh settings to set up the frequency of data ingestion. You can set up either manual refreshes or automatic refreshes at regular intervals.
1. Select **Finish setup** to finish setting up the SAP ERP provider.

## Set up connectors

Power Query connectors are Microsoft data connectivity and data preparation technologies. They let you seamlessly access data that's stored in hundreds of sources and reshape it to fit your needs through an easy-to-use, engaging, no-code experience. For more information about connectors, see the [Power Query documentation](/power-query/).

In Supply Chain Center, users can use the connector experience to create instances of dataflows.

### Create a new instance of a connector in Supply Chain Center

To create a new instance of a connector, follow these steps. This procedure uses the SQL Server database connector as an example, but the basic steps are the same for any other out-of-box connector.

1. In Supply Chain Center, select **Admin Settings** on the left menu.
1. Select **App management**.
1. Search for available connectors by entering the connector name in the search bar on the **Providers and connectors** page. You can select the **Type** column to sort by providers or connectors.
1. Select the **SQL Server database** connector, and then select the plus sign (**\+**) to create a new instance of it.
1. Select **Next**.
1. Select the **Ingestion based** scenario, and then select **Next**.
1. Select the tables or entities, and then select **Next**.
1. Select **Edit** to start to establish a connection with the source.
1. Enter the connection string details, server, database, and user credentials for authentication.

    :::image type="content" source="media/connector-sql-connection.png" alt-text="Screenshot of the Connect to data source page.":::

1. Select **Next** to connect to the source.
1. Select the source entity, and the select **Next**.

    :::image type="content" source="media/connector-table-choose.png" alt-text="Screenshot that shows the Purchase Order entity selected.":::

1. Select **Map to entity**.
1. Select **Finish configuration** to finish mapping source data to destination data.

    :::image type="content" source="media/connector-mapping.png" alt-text="Screenshot that shows the Purchase Order entity, with the Map to entity CDM button highlighted in red.":::

1. On the **Refresh settings** page, select the refresh settings to set up the frequency of data ingestion. You can set up either manual refreshes or automatic refreshes at regular intervals.
1. Select **Save** to save the connector.
