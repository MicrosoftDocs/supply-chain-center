---
title: App Browser
description: This article provides information about Microsoft Supply Chain Center's App Browser.
author: derekkwan
ms.author: derekkwan
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: how-to
ms.date: 07/18/23
ms.custom: bap-template
---

# App Browser

Companies can customize Supply Chain Center to meet their unique business requiements and goals by connecting various first and third party supply chain applications. Supply Chain Center provides an easy-to-use App Browser to search through a comprehensive list of applications and ability to get started with them quickly. 

Applications are categorized as:

- **Modules**: Modules are feature rich applications that provide an interface to perform tasks and view information. For example, Inetlligent Order Management, Smart News, Overhaul, and CH Robinson.
 **Providers**: Providers are applications that transform data from another source to be used by Supply Chain Center or first party modules on Supply Chain Center. For example, FedEx, SAP, and Big Commerce.
- **Connectors**: Connectors are applications that provide a connection to another source. For examples, Snowflake, SQL, Azure Blob, and SAP Hana database.

Applications need to be approved and installed by your administrator before it is made accessible to you and the rest of your organization. Administrators can install and manage apps from the [App Management page](appmanagement.md).

# Finding and using apps

:::image type="content" source="media/app_browser.png" alt-text="Screenshot of the App Browser":::

You can access the App Browser by selecting the **Apps** icon in the left menu. 

The App Browser page has two tabs: **Installed** and **All**. **Installed** is the default view, and contains all of the apps that have been installed for you by your administrator. The **All** tab has all of the available apps for Supply Chain Center. If you see an app that you're interested in but has not been installed for you yet, contact your administrator.

The App Browser has two sections: **Modules** and **Providers and connectors**. On top of each section in the upper right is a filter control. Modules can be filtered by publisher or domain. Providers and connectors have more filters, such as which modules they connect to, or are already connected with, and status.

Modules can be opened with the **Open** button on the tile. Opened modules appear in the left navigation as an **Active** app. Right click the app in the left navigation to pin the app to the menu for quick access (or unpin if you no longer want the app there). 

You can see details of all apps by selecting the **Details** button. **Details** provides a description, screenshots or videos, licensing and support links, and more.

Select the **Manage** button on any tile to open the **App management** area to manage that app. You will need administrator rights to manage apps.

Some apps can't be used unless a dependent app is enabled. For example, FedEx connects with Intellegent Order Management and can't be activated until the Intelligent Order Mangement module is activated.

To use any third party apps on Supply Chain Center, you need a license and credentials with that third party. Please contact the third party company directly to get an account.
