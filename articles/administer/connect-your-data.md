---
title: Connect your data to Supply Chain Center
description: This article provides information about connecting your data to Microsoft Supply Chain Center
author: mkannapiran 
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: how-to
ms.date: 03/30/2023
ms.custom: bap-template
---


# Connect your data to Supply Chain Center

[!INCLUDE[banner](../includes/banner.md)]

To connect your data sources to Supply Chain Center, follow these steps.

1. Select the source where your data is stored, such as Azure SQL Database or Azure Data Lake Storage. If the data for a single entity is stored in two separate data sources, select one source to begin with. You can then add the second source later in the ingestion process.

![A screenshot of a list of data sources that are compatible with Supply Chain Center.](media/ingest-data-connectors.png)

2. Select **Next**.
3. Enter additional details, such as the source URL, credentials, and other parameters.

![A screenshot showing what credentials are required for an Azure SQL database.](media/ingest-data-credentials.png)

We recommend that your data contain all the required attributes of a given entity or have attributes that map to them, so that you can get the most value out of Supply Chain Center. However, if your data doesn't contain all the required attributes, you won't be prevented from ingesting it. After you set up the ingestion process, you can edit the configuration and perform additional transformations on your data.

> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE5aCe5]
