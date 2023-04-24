---
title: Analytics
description: This article describes the Analytics module within Microsoft Supply Chain Center.
author: carylhenry
ms.author: carylhenry
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: overview
ms.date: 4/21/2023
ms.custom: bap-template
---

# Analytics

Microsoft Supply Chain Center's Analytics module empowers you to take advantage of your supply chain data through custom visualizations. Using the Microsoft Dataverse-managed Microsoft Power BI that comes with Supply Chain Center or your own Power BI license, you can create your own dashboards to fit your own supply chain needs.

## Create new reports

Supply Chain Center supports native reports and connected reports.

### Native reports

Native reports are created within Supply Chain Center and are only visible within Supply Chain Center. To create a new, native report, go to the **Analytics module,** navigate to the **Reports tab,** and select **Create** in the top left corner. Choose a template and provide a name to create the new report. Go back to the **Reports tab** to see the new report in **All reports.** 

:::image type="content" source="media/Create_report.png" alt-text="Creating a new report from the Reports tab of the Analytics module."::: 

### Connected reports

Connected reports are linked from your own Power BI workspace and are accessed in both Power BI and Supply Chain Center once connected. 

#### Connect your Power BI workspace

Before you can connect your Power BI workspace, the following prerequisites must be met:

- You must have a Microsoft Power BI Professional or Microsoft Power BI Premium license.
- At least one report must be available in a Power BI workspace.
- You must have admin privileges for Supply Chain Center and Power BI.
- A system administrator must create a security group in Microsoft Azure Active Directory (Azure AD) and add Microsoft Dynamics 365 Supply Chain Visibility as a member of the security group. See [Create a basic group and add members using Azure Active Directory](/azure/active-directory/fundamentals/how-to-manage-groups) for details on how to do this.  
- A Power BI admin must add the security group mentioned previously to your Power BI service after enabling the [Service Principal in the Developer settings](/power-bi/enterprise/service-premium-service-principal#enable-service-principals.md) and [Create workspaces in the Tenant settings](/power-bi/admin/service-admin-portal-workspace#create-the-new-workspaces.md) within the Power BI admin portal.
- Add a security group to your Power BI service within Microsoft Azure Active Directory which contains Microsoft Dynamics 365 Supply Chain Visibility as a member.

#### Link a Power BI report

Once these prerequisites have been met, a Supply Chain Center and Power BI admin can link an existing Power BI workspace or create a new one by going into Supply Chain Center's **Admin settings > Analytics > Create or link a Power BI workspace.** Once a workspace is linked, you can connect a report from that workspace within **Analytics > Reports > Connect.** Unlinking a workspace removes all connected reports from the Reports tab of the **Analytics module** in Supply Chain Center, but they can still be directly accessed through Power BI.  

:::image type="content" source="media/Connect_report.png" alt-text="Connecting a report from the Admin settings."::: 

## Using existing reports

When selecting a report from the table on the **Reports tab**, you can edit, clone, rename, share, or delete it. 

- Editing a report allows you to update it. For connected reports, these edits will persist when you open the report from Power BI instead of Supply Chain Center. 
- Cloning a native report duplicates the report, creating a new one that is the exact same. Note that connected reports can’t be cloned. 
- Renaming the report lets you change the name.
- Sharing the report provides a link you can give to others so they can also view the report.
- Deleting a report removes it from the table in the Reports tab. This will remove native reports from Power BI while connected reports will still be accessible in Power BI. 

:::image type="content" source="media/use-reports.png" alt-text="Seeing the options after selecting a report in the Reports tab of the Analytics module."::: 
