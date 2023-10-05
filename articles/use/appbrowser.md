---
title: App Browser overview
description: This article provides information about Microsoft Supply Chain Center's App Browser.
author: derekkwan
ms.author: derekkwan
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: overview
ms.date: 07/18/2023
ms.custom: bap-template
---

# App Browser overview

[!INCLUDE[banner](../includes/banner.md)]

By connecting different first-party and third-party supply chain applications, companies can customize Microsoft Supply Chain Center to meet their unique business requirements and goals. Supply Chain Center provides an easy-to-use App management experience that lets administrators search through a comprehensive list of apps and quickly get started with them.

Apps are categorized in the following ways:

- **Modules** – Feature-rich apps that provide an interface for performing tasks and viewing information. Examples of modules include Intelligent Order Management, Smart News, Overhaul, and CH Robinson.
- **Providers** – Apps that transform data from another source so that it can be used by Supply Chain Center or first-party modules in Supply Chain Center. Examples of providers include FedEx, SAP, and Big Commerce.
- **Connectors** – Apps that provide a connection to another source. Examples of connectors include Snowflake, SQL, Azure Blob, and SAP Hana database.

Administrators must approve and install apps before they become accessible to your organization. Administrators can install and manage apps from the [App Management page](../administer/appmanagement.md).

## Find and use apps

To access the App Browser, select **Apps** on the left menu.

:::image type="content" source="media/app_browser.png" alt-text="Screenshot of the App Browser.":::

The App Browser page has two tabs: **Installed** and **All**. By default, the **Installed** tab is selected. It shows all the apps that your administrator has installed for you. The **All** tab shows all the apps that are available for Supply Chain Center. If you see an app that you're interested in, but it hasn't yet been installed for you, contact your administrator.

Both tabs of the App Browser have two sections: **Modules** and **Providers and connectors**. Each section has a filter control. You can filter modules by publisher or domain. Providers and connectors have more filters, such as modules that they connect to, modules that they're already connected with, and status.

To open a module, select the **Open** button on the tile. Opened modules appear in the left navigation as **Active** apps. Tap and hold (or right-click) an app in the left navigation to pin the app to the menu for quick access. (If you no longer want a pinned app to appear on the menu, repeat this step to unpin it.)

To view the details of an app, select the **Details** button on the tile. Details include the description, screenshots or videos, and licensing and support links.

Select the **Manage** button on a tile to open the **App management** page, where you can manage the app. You must have administrator rights to manage apps.

Some apps can't be used unless a dependent app is enabled. For example, FedEx connects with Intelligent Order Management and can't be activated until the Intelligent Order Management module is activated.

To use any third-party apps in Supply Chain Center, you must have a license and credentials with that third party. Contact the third-party company directly to get an account.
