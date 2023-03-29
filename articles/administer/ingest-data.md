---
title: Ingest data
description: This article provides information about ingesting data into Microsoft Supply Chain Center
author: mkannapiran 
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: how-to
ms.date: 03/30/2023
ms.custom: bap-template
---

# Ingest data

Before you can start to use the Microsoft Supply Chain Center modules, Supply Chain Center requires data that is relevant to your supply chain. That data must be brought (ingested) into the application. Supply Chain Center uses [Power Query](/power-query/power-query-what-is-power-query) to help ensure a smooth data ingestion experience.

## Prerequisites

Data is ingested into Supply Chain Center in the form of tables, according to the Supply Chain Center data schema of entities and attributes. Although it's useful if your data tables are prepared according to the required entities and attributes, you can transform your data later in the ingestion process.

Before you ingest your data, review the information in [Compliance, privacy, and security](../overview/compliance-privacy-security.md) to ensure that Supply Chain Center meets your company's expectations.

## Ingesting data for the first time

When you signed up for Supply Chain Center, some sample data was provided to help you get started. Before you ingest your own data into Supply Chain Center, we recommend that you delete the sample data from your environment.

To remove preloaded sample data, follow these steps.

1. Select **Setting** (gear icon) in the upper-right corner to access the Admin Center.
1. In the Admin Center, select **General** in the left navigation.
1. Select **Remove data**
1. Select **Remove all data**


To learn more about data deletion, see [Admin settings](admin-settings.md).

![A screenshot of the general settings within the Admin center.](media/admin-center-general-settings.png)

### Get started

To start the ingestion process, follow these steps.

1. Select **Setting** (gear icon) in the upper-right corner to access the Admin Center.
1. In the Admin center, open **Data management**
1. Select **My data** to ingest data that represents your company, or select **Partner data** to ingest data that represents your business partners, such as suppliers or customers.
1. Select the module and function that you want to ingest data for to view all required entities for your the selected module and function.
1. Select the arrow button next to the entity that you want to upload to set up data ingestion.

![A screenshot of a list of entities and their data ingestion status.](media/ingested-data.png)

The following video covers navigating to the Admin center and choosing an entity to ingest data for:

> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE5azzf]
