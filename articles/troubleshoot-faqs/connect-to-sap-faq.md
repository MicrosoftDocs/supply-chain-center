---
title: Connect your SAP data to Supply Chain Center FAQ
description: This article provides answers to frequently asked questions about connecting your SAP data to Microsoft Supply Chain Center
author: mkannapiran 
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: faq
ms.date: 03/30/2023
ms.custom: bap-template
---

# Connect your SAP data to Supply Chain Center FAQ

[!INCLUDE[banner](../includes/banner.md)]

This article provides answers to frequently asked questions about connecting your SAP data to Microsoft Supply Chain Center.

### The SAP ERP Beta connector is labeled as 3rd Party, is this connector not created or managed by Microsoft?

Microsoft creates and manages the SAP ERP Beta connector. As a beta connector, it has a “3rd party” label until it becomes generally available.  

### I'm getting the following error when attempting to connect “The given data source kind isn't supported Data source kind SAPERP”, how do I address it?  

As a custom connector we default save the connection in your [System Drive]\Windows\ServiceProfiles\PBIEqwService\Documents\Power BI Desktop\Custom Connectors folder. If this folder doesn't exist, or if the gateway is configured to use a different custom connector folder, you'll see the error. To remediate, the user will need to copy the SAPERP.mez connector file from [System Drive]\Windows\ServiceProfiles\PBIEqwService\Documents\Power BI Desktop\Custom Connectors, and copy it into the folder that you configured in your gateway.  

### Do I always need to identify a Data gateway in connection settings?

As part of connection setting, you must identify a Data gateway in order to successfully connect through the SAP ERP connector. 

### My connection continues to fail, what can I do to remediate? 

Make sure to check that the installers described above are up-to-date and current. Reinstalling drivers may solve your connection issues.  

