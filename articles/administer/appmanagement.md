---
title: App management overview
description: This article provides information about Microsoft Supply Chain Center's App management.
author: derekkwan
ms.author: derekkwan
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: overview
ms.date: 07/18/2023
ms.custom: bap-template
---

# App management overview

[!INCLUDE[banner](../includes/banner.md)]

By connecting different first-party and third-party supply chain applications, companies can customize Microsoft Supply Chain Center to meet their unique business requirements and goals. Supply Chain Center provides an easy-to-use App management experience that lets administrators search through a comprehensive list of apps, and install and configure them for their organization.

Apps are categorized in the following ways:

- **Modules** – Feature-rich apps that provide an interface for performing tasks and viewing information. Examples of modules include Intelligent Order Management, Smart News, Overhaul, and CH Robinson.
- **Providers** – Apps that transform data from another source so that it can be used by Supply Chain Center or first-party modules in Supply Chain Center. Examples of providers include FedEx, SAP, and Big Commerce.
- **Connectors** – Apps that provide a connection to another source. Examples of connectors include Snowflake, SQL, Azure Blob, and SAP Hana database.

Apps that your administrators install appear on the **Installed** tab of the [App Browser](../use/appbrowser.md).

## Find apps

To access App management, in Supply Chain Center, select **Admin Settings** on the left menu, then select **App management**.

:::image type="content" source="media/appmanagement.png" alt-text="Screenshot of the App management page.":::

The **App management** page is split into two sections: **Modules** in the upper part and **Providers and connectors** in the lower part. You can filter the grid each section to find what you need. You can filter modules by publisher or domain. Providers and connectors have more filters, such as modules that they connect to, modules that they're already connected with, and status.

Both sections include a search field that you can use to search for an app by name. You can also sort each column to group the apps and make discovery easier.

The grid in the **Providers and connectors** section includes **Connected with** and **Connects to** columns. The **Connected with** column shows which apps an app is already connected with. For example, FedEx is connected with Intelligent Order Management. The **Connects to** column shows which apps an app connects to. For example, UPS connects only to Intelligent Order Management, whereas SQL Server DB connects to both Supply and demand insights and Smart News.

Select the name of any module, provider, or connector on the **App management** page to open the **App information** page. This page provides a description, screenshots or videos, licensing and support links, and more.

## Install and manage apps

In the **Modules** section of the **App management** page, the **Status** column lets you install or update settings for each module in the grid. 

- If the module hasn't been installed, **Install** is shown. Select it to open an easy-to-use wizard where you can set up the module.

    Each module can have slightly different installation steps. Some modules might require that you install a package from [AppSource](https://appsource.microsoft.com/home) in your environment before you add it to Supply Chain Center. You can set up other modules, such as first-party modules, directly in Supply Chain Center without having to install a package. For other modules, such as Intelligent Order Management, data mappings are required to complete the setup. Each step of the wizard provides context and instructions for what has to be done.

- If the module is already installed, **Update settings** is shown. Select it to open the module's settings page appears, so that you can manage its settings. For example, for Intelligent Order Management, you can configure data mappings, orchestrations, orders, and more. You must have administrator rights to install and manage modules.

The **Availability** column includes an option that lets you enable or disable each module. Apps can remain disabled even after they're installed. By disabling an app, you prevent your organization from using it. Modules that are in a **Disabled** state don't appear on the **Installed** tab of the App Browser. When you install a module, you're prompted to either enable or disable it. Afterward, you can change the availability directly in the grid by using the option in the **Availability** column.

In the **Providers and connectors** section of the page, selecting any provider or connector displays that provider's or connector's detail page. The control at the top of the detail page is named **New instance**. The first time that you set up an instance for a provider or connector, that provider or connector becomes active. After the provider or connector is active, you can add new instances of it for different purposes. For example, you can use new instances for different geographies or teams. The documentation includes examples that show how to set up the [Big Commerce](/dynamics365/intelligent-order-management/set-up-bigcommerce-provider) and [FedEx](/dynamics365/intelligent-order-management/set-up-fedex-provider) providers for Intelligent Order Management.

If you don't see the provider that you're looking for, you can create your own by selecting **Custom provider** at the top of the **Provider and connectors** section.

> [!NOTE]
> Currently, you can create custom providers only for Intelligent Order Management. For more information, see [Create a new provider](/dynamics365/intelligent-order-management/create-new-provider).

Some apps can't be used unless a dependent app is enabled. For example, FedEx connects with Intelligent Order Management and can't be activated until the Intelligent Order Management module is activated.

To use any third-party apps in Supply Chain Center, you must have a license and credentials with that third party. Contact the third-party company directly to get an account.
