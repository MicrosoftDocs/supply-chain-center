--- 

title: Supplier news communication
description: This article provides information about Microsoft Supply Chain Center's Supplier news communication capability.
author: algiddin
ms.author: algiddin
ms.reviewer: johnmichalak 
ms.service: supply-chain-center 
ms.topic: conceptual 
ms.date: 06/15/2023
ms.custom: bap-template 

--- 

# Supplier news communication

Supplier news communication generates draft emails to supply chain vendors, based on user-selected topics and news articles. For example, if the topic is follow-up about purchase orders, any open purchase order IDs for that vendor are included in the email. Supplier news communication uses generative AI to create the draft email and the subject line.

## Prerequisites

- Before you can use Supplier news communication, the **News** module must be installed. For more information, see [News](news.md).
- Before you can use the Supply Chain Center native email drafting experience, you need to have your mailbox set up to send email, see [instructions](/power-platform/admin/connect-exchange-online#configure-mailboxes).

## Functionality

You can quickly get started by adding Topics with keywords having the "Vendor" type in the News module. For more information, see [News](news.md). To have news about a large number of vendors who you can then contact with Supplier News Communication, you must add vendors at [**Data management**](../administer/ingest-data.md) \> **My data** in the Microsoft Supply Chain Center Admin Center. Make sure that **News** is selected in the **Module** field. 

![Vendors entity added (successfully staged and processed) in the My data area.](media/Supplier-news-communication-data.png)

After your vendors are added (successfully staged and processed), you can view news articles about them in the **News** feed.

![Example of articles in the News feed.](media/Supplier-news-communication-news.png)

You can select an article to view the details page for it. In the **Impact** section on the details page, the grid shows a list of partners that are affected, and gives the type, ID, and contact status for each.

To contact a partner, select it in the grid, and then select **Contact partner** at the top of the page.

![Partner selected for contact in the Impact section of an article's details page.](media/Supplier-news-communication-contact-partner.png)

Next, in the **New Email** dialog box that that appears, notice that there is a copilot dialog on the right side of the page, select a message type (or suggest your own) that corresponds to the information that you want to communicate to the partner.

![Message type options in the Contact partners dialog box.](media/Supplier-news-communication-select-message-type.png)

Finally, in the **New Email** dialog box that appears, review the draft email that's shown. At the bottom of the dialog box, notice that there's an option to provide thumbs-up or thumbs-down feedback. There are also buttons for copying the draft to mail and regenerating the current draft email. If you're satisfied with the draft email, select **Copy to email** to copy the contents into the native email drafting experience inside Supply Chain Center.

![Draft email for review in the Create draft dialog box.](media/Supplier-news-communication-create-draft.png)

## How do I get access?
Sign up for a preview [here](https://aka.ms/AIwaitlist).

[!INCLUDE[supplier-news-ai-faq](../includes/supplier-news-ai-faq.md)]
