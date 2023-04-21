---
title: Install the Overhaul module
description: This article describes how to set up the Overhaul module within Microsoft Supply Chain Center.
author: carylhenry
ms.author: carylhenry
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: how-to
ms.date: 4/21/2023
ms.custom: bap-template
---

# Report management

## Create new reports
### Native reports
Native reports are ones that are created within MSCC and are only visible within MSCC. To create a new, native report, go to the **Analytics module,** navigate to the **Reports tab,** and click **Create** in the top left corner. Choose a template and provide a name to create the new report. Go back to the **Reports tab** and you can now find the new report under **All reports.** 


### Connected reports
Connected reports are those you have linked from your own Power BI workspace and can be accessed in both Power BI and MSCC after connecting. 

#### Connect your Power BI workspace
Before you can connect your Power BI workspace, the following prerequisites must be met:
- You must have a Power BI Professional or Power BI Premium license
- At least one report must be available in a Power BI workspace
- You must have admin privilages for MSCC and Power BI
- A system administrator must create a security group in Microsoft Azure Active Directory (Azure AD) and add Microsoft Dynamics 365 Supply Chain Visibility as a member of the security group. See [Create a basic group and add members using Azure Active Directory](https://learn.microsoft.com/azure/active-directory/fundamentals/how-to-manage-groups) for details on how to do this.  
- A Power BI admin must add the security group mentioned previously to your Power BI service after enabling the following in the Power BI admin portal:
- [Service Principal in the Developer settings](https://learn.microsoft.com/power-bi/enterprise/service-premium-service-principal#enable-service-principals)
- [Create workspaces in the Tenant settings](https://learn.microsoft.com/power-bi/admin/service-admin-portal-workspace#create-the-new-workspaces)
- Add a security group to your Power BI service within Microsoft Azure Active Directory which contains Microsoft Dynamics 365 Supply Chain Visibility as a memember

#### Link a Power BI report
Once these prerequisites have been met, an MSCC and Power BI admin can link an existing Power BI workspace or create a new one by going into MSCC's **Admin settings > Analytics > Create or link a Power BI workspace.** Once a workspace has been linked, you can connect a report from that workspace within **Analytics > Reports > Connect.** Unlinking a workspace will remove all connected reports from the Reports tab of the **Analytics module** in MSCC, but they can still be directly accessed through Power BI.  


## Using existing reports
When selecting a report from the table on the Reports tab, you can edit, clone, rename, share, or delete it.  
- Editing a report allows you to update it. For connected reports, these edits will persist when you open the report from Power BI instead of MSCC. 
- Cloning a native report duplicates the report, creating a new one that is the exact same. Note that connected reports can’t be cloned. 
- Renaming the report lets you change the name.
- Sharing the report provides a link you can give to others so they can also view the report.
- Deleting a report will remove it from the table in the Reports tab. This will remove native reports from Power BI while connected reports will still be accessible in Power BI. 
