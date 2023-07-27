---
title: Extend the data schema in Supply Chain Center
description: This article provides information about how to extend or modify the structure of a schema in a database or data model.
author: mkannapiran
ms.author: mkannapiran
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: how-to
ms.date: 7/11/2023
ms.custom: bap-template
---

# Extend the data schema in Supply Chain Center

Microsoft Supply Chain Center lets users extend or modify the structure of a schema in a database or data model. Schema extensibility is useful in scenarios where the data requirements are subject to frequent changes, or where the system must accommodate user-defined scenarios or customizable data structures. Schema extensibility promotes flexibility, scalability, and adaptability in data models, and enables customization and personalization of data models. This level of customizability empowers you to adapt the data model to your unique business scenarios, workflows, and preferences. Extension of the schema can enhance data analysis capabilities, connect to external risk signals, and enable risk analysis, impact analysis, and mitigation capabilities in Supply Chain Center.

## Define a new schema

To define a new schema, follow these steps.

1. In Supply Chain Center, select **Admin Settings** on the left menu.
1. Select **App management**.
1. Select a connector, and then select **New instance**.
1. Select the scenario that you want to add the new entities for.

    > [!NOTE]
    > Even if the entities aren't for any specific scenario, select one of the scenarios.

    :::image type="content" source="media/schema-scenario-select.png" alt-text="Screenshot that shows Supply Coverage selected as the scenario.":::

1. Select **Next**.
1. Select **Import custom data table**. The next page varies, depending on the connector. In this example, because the connector is a SQL Server database, it expects connection-related and authentication-related information to connect to the source.

    :::image type="content" source="media/schema-connector.png" alt-text="Screenshot of the Connect to data source page.":::

1. Select the entities that must be created in Supply Chain Center. You can select one or more of the entities, and you can use the power of Power Query to define an entity that's a combination of all the entities.

    :::image type="content" source="media/schema-table-choose.png" alt-text="Screenshot of the Choose data page.":::

1. Select **Next**. You can change the title of a column by double-tapping (or double-clicking) the existing title. You can also change the data type of a column by selecting the left corner of the column header. By default, Power Query determines the data type based on the source.
1. Select **Next**, and define the name of the entity, primary keys of the entity, and the length of the field.

    :::image type="content" source="media/schema-define-table.png" alt-text="Screenshot of the New custom data table page, where the Name, Max length, and Primary key fields are highlighted.":::

1. Select **Create** to create the new custom entity.
