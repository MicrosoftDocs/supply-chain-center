---
title: Bring your own apps
description: This article provides information about how to bring your own apps to Microsoft Supply Chain Center's App management.
author: derekkwan
ms.author: derekkwan
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: how-to
ms.date: 07/18/2023
ms.custom: bap-template
---

# Bring your own apps

By connecting different first-party and third-party supply chain applications, companies can customize Microsoft Supply Chain Center to meet their unique business requirements and goals. Supply Chain Center provides an easy-to-use App management experience that lets administrators search through a comprehensive list of apps, and install and configure them for their organization.

Apps are categorized in the following ways:

- **Modules** – Feature-rich apps that provide an interface for performing tasks and viewing information. Examples of modules include Intelligent Order Management, Smart News, Overhaul, and CH Robinson.
- **Providers** – Apps that transform data from another source so that it can be used by Supply Chain Center or first-party modules in Supply Chain Center. Examples of providers include FedEx, SAP, and Big Commerce.
- **Connectors** – Apps that provide a connection to another source. Examples of connectors include Snowflake, SQL, Azure Blob, and SAP Hana database.

Supply Chain Center might not currently have all the modules that you need. However, thanks to its tight integration with [Power Apps](/power-apps/maker/), you can create new apps or bring existing apps to Supply Chain Center.

> [!NOTE]
> Currently, you can bring only [model-driven apps](/power-apps/maker/model-driven-apps/) to Supply Chain Center. Support for canvas apps will be provided in the future.

In the **Modules** section of the **App management** page, select **Link Power App** to bring your own apps to Supply Chain Center.

:::image type="content" source="media/byopa.png" alt-text="Screenshot of the Link Power App dialog box on the App management page.":::

The **Link Power App** dialog box provides a list of current apps in your Power Apps environment. You can use the search field above the list to search for specific apps by name. After you find the app that you want to bring over, you can select it in the list and then select **Next** at the bottom of the dialog box.

You can select a domain for your app, so that it can be categorized in Supply Chain Center. If no appropriate domain is listed, select **Unspecified**.

The app is brought to Supply Chain Center in an **Enabled** state. Therefore, it's immediately made available to all users in your organization. If you want to bring an app to Supply Chain Center, but you don't want users to access it, set the **Availability** option to **Disabled**.

The grid on the **App management** page shows the app that you just brought over. If you set the app to an **Enabled** state, it appears on the **Installed** tab of the [App Browser](../use/appbrowser.md) and is accessible to all users in your organization.

> [!NOTE]
> If the list in the **Link Power App** dialog box doesn't include one of your apps, it might be in a different environment. To switch environments, close the dialog box by selecting the **Close** button (**X**) in the upper-right corner. Then tap or click in the environment switcher at the top of the Supply Chain Center page to open a dialog box where you can switch environments.
>
> :::image type="content" source="media/envswitcher.png" alt-text="Screenshot of the Select environment dialog box.":::

If Supply Chain Center or your environment doesn't have the app that you need, you can create it for yourself. In the **Link Power App** dialog box, select **Create Power App** to open the [Power Apps maker portal](/power-apps/maker/model-driven-apps/build-app-three-steps), where you can create your own app. Many customers partner with independent software vendors (ISVs) who have some expertise in Power Apps to help them create new apps.
