---
title: Select the refresh schedule and complete the setup process
description: This article provides information about selecting the refresh schedule and complete the setup process
author: johnmichalak
ms.author: johnmichalak
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: how-to
ms.date: 11/3/2022
ms.custom: bap-template
---

# Select the refresh schedule and complete the setup process

To finalize the ingestion setup, the last step is to select the refresh schedule. A refresh schedule automatically updates the ingested data for a given entity, based on any changes that were made to that data in your cloud storage solution. Up-to-date data is critical for deriving recent and relevant insights.

- To perform a one-time data ingestion, select **Refresh Manually**. The data connection won't be refreshed again until you choose to do so.
- For continuous data refresh, select **Refresh Automatically**, and enter the desired schedule.
- To finish the setup and initiate the ingestion process, select **Finish setup**. If you selected **Refresh Automatically**, ingestion will begin according to the selected refresh schedule.

![A screenshot of the data refresh settings.](media/ingest-data-refresh-schedule.png)

After you've finished the ingestion setup, you can review the status of your ingested entities and apply any updates that are required. For more information, see the [Review, update, and delete your data](review-update-delete-data.md) section.

> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE5amRA]
