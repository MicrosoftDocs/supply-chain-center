# This file contains examples of commonly used markdown.

## Metadata example

Every article file you create in GitHub must contain the following metadata. Edit the section where indicated. Include the --- at the beginning and the end.

---
title: [Type your title here, must match your H1.]
description: [Type your description here. This will display in search results.]
author: [Type your GitHub alias here.]
ms.author: [Type your Microsoft alias.]
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: [See the Contributor guide for options]
ms.date: [date in MM/DD/YYYY format]
ms.custom: bap-template
---

## Headings

This is a level 2 heading. 

## Bold Text

From the navigation pane, select **Module library**.

## Notes

> [!NOTE]
> This feature is only available after it is enabled.
>
> To enable the feature, see…

## Images

![alt text goes here](path/filename.png)

For example, 
![Screenshot of the details for the Supply and demand insights module/](../use/media/module-library-supply-and-demand-details.png)

## Bulleted lists

This feature has the following options:
- Option 1
- Option 2
- Option 3

## Numbered lists

The process of adding users to Supply Chain Center consists of three steps.
 
1. Ensure that the user is added in Microsoft Azure Active Directory (Azure AD). 
1. Assign a Supply Chain Center license to the user in Microsoft Azure Active Directory (Azure AD).
1. Add the user to your Microsoft Dataverse environment.

## Links

[display name](URL)

Note. DO NOT put click here, here, or some other variant in the display name. As a general rule, you want to include the full title of the target page exactly as it will appear after the link is selected. Rewrite your into sentence to make it more appropriate:

DO NOTE USE: Click here for more information.
USE: For more information, see the Asure portal.

However, depending on the target for the link, you will need to make alterations to the URL.

If you are linking to an article that is in the same GitHub folder as the one you are editing, you only need to include the filename. For example,

[Azure portal](azure-portal.md)

If you are linking to an article that is in the same doc set, but in a different folder, you need to include a relative link. For example,

[Azure portal](../azure-portal.md)

If you are linking to an article that is published on learn.microsoft.com, you need to modify the URL. 

Original URL: 
https://review.learn.microsoft.com/en-us/help/contribute/metrics-content-engagement
Modified: 
[Content Engagement report](/en-us/help/contribute/metrics-content-engagement.md)

## Tables

You can do this (if it makes it easier for your to read), but it is not needed:

| **1**         | **2**         | **3**         |
| --------------|---------------|---------------|
| **row one**   | **row one**   | **row one**   |
| **row two**   | **row two**   | **row two**   |
| **row three** | **row three** | **row three** |

This is perfectly acceptable:

| **1** | **2** | **3** |
| ---|---|---|
| **row one** | **row one** | **row one** |
| **row two** | **row two** | **row two** |
| **row three** | **row three** | **row three** |

Use </br> if you need a line break within a cell.

