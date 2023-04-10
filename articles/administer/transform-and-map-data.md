---
title: Transform and map the data according to your desired entity
description: This article provides information about transforming and mapping the data according to your desired entity
author: johnmichalak
ms.author: johnmichalak
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: how-to
ms.date: 11/3/2022
ms.custom: bap-template
---

# Transform and map the data according to your desired entity

The next step in the ingestion process is to transform and map your data. First, transform your data into the required [Supply Chain Center data schema](data-schema.md).

You can use the Power Query editor to transform your data into a single query that has one table that contains all attributes of an entity. Transformation and mapping of your data have to be done only once for an entity, provided that you don't change the data sources.

![A screenshot of the Power Query interface.](media/ingest-data-power-query.png)

After you've created a single query that has the table that contains the data that you want to import, map your table columns into the Supply Chain Center entities attributes, so that your data can be analyzed and made available for the different Supply Chain Center modules. You can view the required and optional attributes for the entity on the right side of the page.

![A screenshot of Power Query's auto map feature.](media/ingest-data-auto-map.png)

To map your table columns to the Supply Chain Center entity attributes, follow these steps.

1. Select **Map to entity** in the upper right.
1. In the **Map to CDM entity** dialog box, select the entity in the left column, and then select **Auto map**. Supply Chain Center will use the column headers of the query table to determine which column represents which attribute.
1. To ensure that automatic mapping is run correctly, select the **Mapped attributes** column together with the **Data preview** table at the bottom of the page. If an error occurs, or if you prefer to do the mapping manually, select the option for the required attribute in the **Mapped attributes** column, and then select the appropriate column header name.
1. When you've finished, select **Done**.

> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE5cnCu]
