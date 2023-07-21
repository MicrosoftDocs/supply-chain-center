---
title: Extend the Data schema in Microsoft Supply Chain Center
description: This article provides information about how to extend or modify the structure of a schema in a database or data model.
author: mkannapiran
ms.author: mkannapiran
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: how-to
ms.date: 7/11/2023
ms.custom: bap-template
---

# Extend the Data schema in Microsoft Supply Chain Center

Supply chain center allows users to extend or modify the structure of a schema in a database or data model. Schema extensibility is particularly useful in scenarios where the data requirements are subject to frequent changes or where the system needs to accommodate user-defined scenarios or customizable data structures. Schema extensibility promotes flexibility, scalability, and adaptability in data models, and enables customization and personalization of data models. This level of customizability empowers you to adapt the data model to your unique business scenarios, workflows and preferences. Extending the schema can enhance data analysis capabilities, connect to external risk signals and enable risk analysis, impact analysis and mitigation capabilities in Supply Chain Center.

## **How to define new schema**

To define a new schema, follow these steps.

1. In Supply Chain Center, select **Admin settings**, and then select **App management**.
1. Choose one of the connectors, and then select **New instance**.
1. Choose the scenario for which you would like to add these new entities.  

   > [!NOTE]
   > Even if the entities are not for any specific scenario, choose one of the scenario as shown in screenshot below.

   ![A screenshot of App management feature.](media/schema-scenario-select.png)

1. Select **Next**.
1. Select **Import custom data table**. 

   ![A screenshot of App management feature.](media/schema-import-custom-table.png)

   Depending on the connector the next page varies. In this example, because the connector is a SQL Server Database, the connector expects connection and authentication related information to connect to source. 

   ![A screenshot of App management feature.](media/schema-connector.png)

1. Select the entities that need to be created in Supply Chain Center. You can choose one or more of the entities, and you cane use the power of Power Query to define an entity that is combination of all the entities.

   ![A screenshot of App management feature.](media/schema-table-choose.png)

1. Select **Next**. You can change the title of the column name by double clicking on the title of the column. You can also change the data type by selecting the left corner of each column header to change the data type of the column if required. By default, Power query determines the data type based on the source.
1. Select **Next**, and define the name of the entity, primary keys of the entity and define length of the field.

   ![A screenshot of App management feature.](media/schema-define-table.png)

1. Select **Create** to create the new custom entity.
