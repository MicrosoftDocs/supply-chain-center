---
title: Ingest data
description: This article provides information about ingesting data into Microsoft Supply Chain Center
author: johnmichalak
ms.author: johnmichalak
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: how-to
ms.date: 11/3/2022
ms.custom: bap-template
---

# Ingest data into one entity from multiple data sources

If you must add data to an existing entity from additional data sources, select **Get Data** on the **Home** tab in the upper left of the Power Query editor. You're prompted to complete the connection process again to add another source. Another query will be created that includes the data from the new source. As a result, you might have multiple queries in Supply Chain Center. You must then merge those queries or append them into one query before you map the table columns to the entity attributes.

We recommend that you delete all queries except the one where you will perform the column-to-attribute mapping. If you don't remove other existing queries, the wrong data might be uploaded. For more information about how to load and transform data by using the Power Query editor, see [Use Power Query to transform data](/power-query/power-query-ui).
