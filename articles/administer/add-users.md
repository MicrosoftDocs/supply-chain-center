---
title: Add users
description: This article provides information about how to add users to Microsoft Supply Chain Center.
author: 
ms.author: 
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: how-to
ms.date: 11/3/2022
ms.custom:
---

# Add users

The process of adding users to Supply Chain Center consists of three steps. 

1. Ensure that the user is added in Microsoft Azure Active Directory (Azure AD). 
1. Assign a Supply Chain Center license to the user in Microsoft Azure Active Directory (Azure AD).
1. Add the user to your Microsoft Dataverse environment.

## Add users to your Azure AD tenant

To add users to your Azure AD tenant, follow these steps. This step _can be skipped_ if the user you want to add to Supply Chain Center is already added to your Azure AD tenant.

1. Go to the Microsoft [Azure portal](https://portal.azure.com/), and sign in.
1. Search for and select **Azure Active Directory**. The **Overview** page of your Azure AD tenant appears.
1. Confirm that you're in the same Azure AD tenant that is being used for Supply Chain Center. You can change the tenant by selecting **Manage tenants** and then selecting the desired tenant.
1. To add a user to the Azure AD tenant, on the **Overview** page, select **Add**, and then **select User on the drop-down menu. Please note that the user’s Usage Location must be set to the United States**.
1. Enter the new user's information, and then select **Create**.

## Assign a Supply Chain Center license to the user

To Assign a Supply Chain Center license to the user, follow these steps.

1. Go to the Microsoft [Azure portal](https://portal.azure.com/), and sign in.
1. Search for and select **Azure Active Directory**. The **Overview** page of your Azure AD tenant appears.
1. Confirm that you're in the same Azure AD tenant that is being used for Supply Chain Center. You can change the tenant by selecting **Manage tenants**, and then select the desired tenant.
1. After you are on the correct tenant overview page, select **Licenses** from the left navigation, and then select **All Products**. 
1. Select the **Dynamics 365 Supply Chain Insights Preview** product and assign it to the user you would like to add to Supply Chain Center. 

## Add users to your Dataverse environment

To add users to your Dataverse environment, follow these steps.

1. Go to the [Power Platform admin center](https://admin.powerplatform.microsoft.com/), and sign in.
1. Open the Environments page and select the environment that you want to add users to.
1. In the Access section, under Users, select See all. You should see a list of all users that have been added to your environment.
1. Select the name of the user that you want to grant access to Supply Chain Center, and then select Manage roles.

Assign the user to the System Administrator role, and then select Save.

## Troubleshooting

If you experience issues, please check the following: 

1. Go to the [Azure portal](https://portal.azure.com/), and check that the user’s usage location is set to the United States.
1. Go to the [Azure portal](https://portal.azure.com/), and check that the user has been assigned a Supply Chain Center license. 
1. Go to the [Power Platform admin center](https://admin.powerplatform.microsoft.com/) and ensure the user has been added to the correct Dataverse environment and assigned the System Administrator role.
