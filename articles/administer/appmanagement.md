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

Companies can customize Supply Chain Center to meet their unique business requirements and goals by connecting various first and third party supply chain applications. Supply Chain Center provides administrators an easy-to-use App management experience to search through a comprehensive list of applications and install and configure those apps for their organizations. 

Applications are categorized as:

- **Modules**: Modules are feature rich applications that provide an interface to perform tasks and view information. For example, Intelligent Order Management, Smart News, Overhaul, and CH Robinson.
 **Providers**: Providers are applications that transform data from another source to be used by Supply Chain Center or first party modules on Supply Chain Center. For example, FedEx, SAP, and Big Commerce.
- **Connectors**: Connectors are applications that provide a connection to another source. For examples, Snowflake, SQL, Azure Blob, and SAP Hana database.

Apps that are installed by your administrators appear in the **Installed** tab in the [App Browser](../use/appbrowser.md).

## Find apps
 
:::image type="content" source="media/appmanagement.png" alt-text="A screenshot of the App management page"::: 

To access App management, in Supply Chain Center, select select **Admin Settings** in the left menu, then select **App management**.

The App management page is split into two sections: **Modules** and **Providers and connectors**. You can filter each section to find what you need. You can filter modules by publisher or domain. Providers and connectors have more filters, such as which modules they connect to, or are already connected with, and status. You can use the search box to search for an app by name.

Each column can be sorted to help group the apps for easier discovery. Select name of any module, provider, or connector and the **App information** page appears. The **App information** page provides a description, screenshots or videos, licensing and support links, and more.

The **Providers and connectors** list on the **App management** page has columns for **Connected with** and **Connects to**. The **Connected with** column shows which apps a current app is already connected with. For example, FedEx connected with IIntelligent Order Management. The **Connects to** column lets you know which apps a given app connects to. For example, UPS connects to only Intelligent Order Management, and not any other apps, while SQL Server DB connects to both Supply and Demand Insights and Smart News.   

## Install and manage apps

The **Modules** list appears at the top of the **App management** page. For each module, the **Status** column lets you install or update settings. **Install** displays if the module hasn't been installed, and leads you to an easy-to-use wizard to set up the module. For modules that are already installed, **Update settings** lets you update your settings for that module. You need administrator rights to install and manage modules.

Each module may have slightly different installation steps. Some modules may require you to install a package from [AppSource](https://appsource.microsoft.com/home) to your environment before adding it to Supply Chain Center. Other modules, like first party modules, can be set up directly in Supply Chain Center without installing a package. Some modules, such as Intelligent Order Management, need data mappings to complete set up. Each step of the wizard provides context and instructions on what needs to be done. 
When you select **Update settings**, that specific module's settings page appears so you can manage its settings. For example, Inetllegien Order Management's settings lets you configure data mappings, orchestrations, orders, and more.

The **Aavailability** column has a toggle to enabled or disabled the module. Apps can remain disabled even after they're installed. Disabled prevents your organization from using it. Leaving a module in the disabled state prevents it from appearing in the **Installed** tab in the **App browser**. After installing a module, you're prompted to either enable or disable the module. You can also change the availability directly in the list with the toggle.

In the **Providers and connectors** section, the control on top of the page is **New instance**. The first time you set up an instance for a provider or connector, that provider or connector becomes active. After itis active, you may add more instances of that provider or connector. You can add new instances for different purposes. For example, you can use new instances for different geographies or teams. Here are examples of setting up [Big Commerce](/dynamics365/intelligent-order-management/set-up-bigcommerce-provider) and the [FedEx](/dynamics365/intelligent-order-management/set-up-fedex-provider) for Intelligent Order Management.

If you don't see a provider you're looking for, you can create your own provider by selecting **Custom provider** at the top of the **Provider and connectors** list. 

> [!NOTE]
> Currently, you can only create custom providers for Intelligent Order Management. For more information, see [Create a new provider](/dynamics365/intelligent-order-management/create-new-provider). 

Some apps can't be used unless a dependent app is enabled. For example, FedEx connects with Intelligent Order Management and can't be activated until the Intelligent Order Management module is activated.

To use any third party apps on Supply Chain Center, you need a license and credentials with that third party. Contact the third party company directly to get an account.
