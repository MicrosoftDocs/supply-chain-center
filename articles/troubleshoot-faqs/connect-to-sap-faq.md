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

This article provides answers to frequently asked questions about connecting your SAP data to Microsoft Supply Chain Center.

**Q**: The SAP ERP Beta connector is labeled as 3rd Party, is this connector not created or managed by Microsoft?
  
**A**: The connector was created by Microsoft and is managed by Microsoft. As a beta connector it will hold a “3rd party” label until it becomes generally available.  

**Q**: I am getting the following error when attempting to connect “The given data source kind is not supported Data source kind SAPERP”, how do I address?  
**A**: As a custom connector we default save the connection in your [System Drive]\Windows\ServiceProfiles\PBIEqwService\Documents\Power BI Desktop\Custom Connectors folder, if this folder does not exist or if gateway is configured to use a different custom connector folder you will see the above error. To remediate the user will need to copy the SAPERP.mez connector file from [System Drive]\Windows\ServiceProfiles\PBIEqwService\Documents\Power BI Desktop\Custom Connectors and copy in to the folder that you configured in your gateway.  

**Q**: Do I always need to identify a Data gateway in connection settings?
**A**: As part of connection setting you must identify a Data gateway in order to successfully connect through the SAP ERP connector 

**Q**: My connection continues to fail, what can I do to remediate? 
**A**: Make sure to check that installers described above are up to date and current. Reinstalling drivers may solve your connection issues.  

