---
title: Bring your own Power Apps
description: This article provides information about how to bring your own Power Apps to Microsoft Supply Chain Center's App Management.
author: derekkwan
ms.author: derekkwan
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: use
ms.date: 07/18/23
ms.custom: bap-template
---

# Bring your own Power Apps

Companies can customize MSCC to meet their unique business requiements and goals by connecting various first and third party supply chain applications. MSCC provides adminsitrators an easy-to-use [App Management experience](articles/administer/appmanagement) to search through a comprehensive list of applications and install and configure those apps for their organizations. 

Applications are categorized as:

1. Modules: feature rich applications that provide an interface to perform tasks and view information (examples: IOM, Smart News, Overhaul, CH Robinson)
2. Providers: applications that transform data from another source to be used by MSCC or 1P modules on MSCC (examples: FedEx, SAP, Big Commerce)
3. Connectors: applications that provide a connection to another source (examples: Snowflake, SQL, Azue Blob, SAP Hana DB)

However, MSCC may not currently have all the modules that you need. Luckily, MSCC is integrated tightly with [Power Apps](https://learn.microsoft.com/en-us/power-apps/maker/) so you can create new apps or bring existing apps to MSCC. 
Note: you can only bring [model driven apps](https://learn.microsoft.com/en-us/power-apps/maker/model-driven-apps/) to MSCC for the time being. We will support canvas apps in the near future.

In the module section of the App Management page, you will see a control for "Link Power App". This will open up a side panel on the right where you can bring your own Power Apps to MSCC.

![Screenshot of BYOPA](articles/administer/media/byopa.png)

The side panel provides a list of current Power Apps in your Power App environment. There is a search bar on top of the list to also help you locate any specific Power Apps by name. Once you find the Power App you want to bring over, you can select it from the list, and then click "next" on the bottom of the panel. 
From here, you can select a domain for your Power App so it can be categorized in MSCC. If none of the domains fit, just choose "unspecified". The app will be brought to MSCC in "enabled" state, which means it will be immediately made available to all users in your org. If you would like to bring the app, but hold off on allowing users to access, just set the "availability" toggle to "disabled" on this step before continuing. When everything looks good, click "save".
You will be returned to the main app management area, where you can locate the app you just brought over in the list. If you set the app to "enabled", it will show up in the "installed" tab in the [App Browser](articles/use/appbrowser), and be accessible to all users in your org. 

Note: If you can't find one of the Power Apps in your environment in the list, it may be in a different environment. To switch environments, close the side panel by clicking the "x" on top of the panel, and you will see the environment switcher on top of the MSCC page. Clicking in the environment switcher will slide out a side panel where you can switch your environments. 

![Screenshot of Env Switcher](articles/administer/media/envswitcher.png)

Lastly, if MSCC does not have the app you need, and your environment also doesn't have the app you need, you can build your own. In the "Link Power App" side panel, next to the search box, is a control for "Create Power App". This will take you directly to the [Power App Maker portal](https://learn.microsoft.com/en-us/power-apps/maker/model-driven-apps/build-app-three-steps) where you can create your own. Many customers partner with ISVs who have some expertise in Power Apps to assist them with creating new apps.
