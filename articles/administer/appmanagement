---
title: App Management
description: This article provides information about Microsoft Supply Chain Center's App Management.
author: derekkwan
ms.author: derekkwan
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: use
ms.date: 07/18/23
ms.custom: bap-template
---

# App Management

Companies can customize MSCC to meet their unique business requiements and goals by connecting various first and third party supply chain applications. MSCC provides adminsitrators an easy-to-use App Management experience to search through a comprehensive list of applications and install and configure those apps for their organizations. 

Applications are categorized as:

1. Modules: feature rich applications that provide an interface to perform tasks and view information (examples: IOM, Smart News, Overhaul, CH Robinson)
2. Providers: applications that transform data from another source to be used by MSCC or 1P modules on MSCC (examples: FedEx, SAP, Big Commerce)
3. Connectors: applications that provide a connection to another source (examples: Snowflake, SQL, Azue Blob, SAP Hana DB)

Apps that have been installed by administrators will appear in the "installed" tab in the [App Browser](articles/use/appbrowser).

## Finding apps

![Screenshot of App Management](articles/administer/media/appmanagement.png) 

You can access the App Management area by clicking "Admin Settings" in the left menu. This will open an additional menu, which contains a link for "App management".

The app management screen is split into two sections: "Modules" and "Providers and connectors", same as in the App Browser. You can filter each section to find what you need. Modules can be filtered by publisher or domain. Providers and connectors have more filters, such as which modules they connect to, or are already connected with, and status. There is alos a search box to search for an app by name.

In the lists themselves, each column can be sorted to help group the apps for easier discovery. By clicking on the name of any module, provider, or connector, the app information page will display. This will provide info like a description, screenshots or videos, licensing and support links, and more.

You will notice a "connected with" and "connects to" columns. Connected with shows which apps a current app is already connected with (such as FedEx connected with IOM). The "connects to" column lets you know which apps a given app will connect to. For example, UPS connects to only IOM, and not any other apps, while SQL Server DB connects to both Supply and Demand Insights and Smart News.   

## Installing and managing apps

For modules, on top of the app information page is a control to either "install" or "update settings". "Install" will display if the module has not been installed yet, and will lead you to a easy-to-use wizard to set up the module. For modules already installed, the "update settings" control will allow you to update settings for that module as needed. You will need administrator rights to install and manage modules.

Each module may have slightly different installation steps. Some modules may require you to install a package from [AppSource](https://appsource.microsoft.com/en-us/home) to your environment first before adding it to MSCC. Other modules, particulalry 1P modules, can be set up directly in MSCC without installing a package. Some modules, such as IOM, will need you to do data mappings to complete set up. Each step of the wizard will provide context and instructions on what needs to be done. 
When clicking "update settings", you will be taken to that specific module's settings area, where you can manage the different parts of a given module. For example, IOM's settings allow you to configure data mappings, orchestrations, orders, and more.

You will also notice a "availability" column, with a toggle for enabled or disabled. You can keep an app disabled even after installing, if you would like to prevent your org from using it yet for any reason. Leaving a module in the disabled state will prevent it from appearing in the installed tab in the App Browser. Upon installing a module, you wil be prompted to either enable or disable the module, and you can also change the availability directly in the list with the toggle.

For providers and connectors, the control on top of the page will say "new instance". The first time you set up an instance for a provider or connector, that provider or connector will become active. After it has become active, you may add more instances of that provider or connector. Customers add new instances for a number of different purposes, such as for different geographies or teams. Here are examples of setting up [Big Commerce](https://learn.microsoft.com/en-us/dynamics365/intelligent-order-management/set-up-bigcommerce-provider) and [FedEx](https://learn.microsoft.com/en-us/dynamics365/intelligent-order-management/set-up-fedex-provider) for IOM.

If you do not see a provider you are looking for, you can create your own provider by clicking the "custom provider" control on top of the provider and connectors list. Note: you can currently only create custom providers for IOM. Instructions on how to create custome providers is [available here](https://learn.microsoft.com/en-us/dynamics365/intelligent-order-management/create-new-provider). 

Some apps cannot be used unless a dependent app is enabled. For example, Fedex "connects with" IOM. Thus, FedEx cannot be activated until the IOM module is activated.

To use any 3p apps on MSCC, you will need a license and credentials with that 3p. Please contact those 3p companies directly to get an account.
