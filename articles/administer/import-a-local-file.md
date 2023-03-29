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

### Import a local file

An [on-premises data gateway](/data-integration/gateway/service-gateway-onprem) is required to import local files from your computer into Supply Chain Center. For information about how to install an on-premises data gateway, see [Install an on-premises data gateway](/data-integration/gateway/service-gateway-install). After you install the gateway, you must use your Supply Chain Center user credentials to sign in to the application. Then make sure that the local folder that contains the file that you want to upload is configured so that access is granted to everyone. To change this configuration, go to the folder, select and hold (or right-click) it, and then select **Give access to > Specific people**.

>[!Note]
> There are two types of on-premises data gateways: personal mode and standard gateway. Don't install the personal mode on-premises data gateway. Install the standard on-premises gateway instead.

