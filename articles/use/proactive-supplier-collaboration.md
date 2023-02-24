--- 

title: Proactive Supplier Collaboration

description: This article provides information about Microsoft Supply Chain Center's Proactive Supplier Collaboration capability.

author: algiddin

ms.author: algiddin

ms.reviewer: johnmichalak 

ms.service: supply-chain-center 

ms.topic: conceptual 

ms.date: 02/24/2023

ms.custom: bap-template 

--- 

# Proactive Supplier Collaboration

Proactive Supplier Collaboration drafts e-mails to supply chain vendors based on a user-selected topic and news article. If the topic is to follow-up on purchase orders, then open purchase order Ids with that vendor are included in the mail. Proactive Supplier Collaboration leverages generative AI to draft the e-mail and subject line.

# Prerequisites

You need to have the news module installed. For more information, see [News](news.md) 

# Functionality

To get started with proactive supplier collaboration, you just need to add vendors through data management in the admin center of MSCC. 

Then, you can see news articles about your vendors in the news feed. 

You can select an article to view the detail page. Here, you can select a partner to contact.    

Then, select a message type for what you want to communicate. 

Finally, you will see a draft e-mail that you can review and then select create draft to open the mail in your default mail client.

# What are Proactive Supplier Collaboration’s capabilities? 
Proactive Supplier Collaboration uses text-davinci-003 generative AI model to draft the e-mail. It leverages Azure Open AI’s Content Moderator to help validate the response, along with an NGram-based relevance filter to ensure response is on-topic.

# What is Proactive Supplier Collaboration’s intended use?
The intended use of Proactive Supplier Collaboration is to provide a way for business users to more quickly and efficiently follow-up with their partners on supply chain disruptions in the news.

# How was Proactive Supplier Collaboration evaluated? What metrics are used to measure performance?
Proactive Supplier Collaboration was evaluated with human judgment on a random sample of drafted e-mails from a random selection of news articles. To evaluate the system, our metrics included if the e-mail contained false information, if the e-mail content was relevant and actionable, if the e-mail was syntactically correct, if the topic was correctly incorporated into the e-mail, and the amount of editing needed before sending.

# What are the limitations of Proactive Supplier Collaboration? How can users minimize the impact of Proactive Supplier Collaboration’s limitations when using it?
Proactive Supplier Collaboration today only supports drafting e-mails in the English language. The e-mail draft is generated one time, and there is not additional support for editing the draft. As we are not able to test for every possible news situation, it is possible some generated e-mails may be of lower quality than the e-mails that we tested. This can be mitigated by always reviewing the draft e-mail before sending.

# What operational factors and settings allow for effective and responsible use of Proactive Supplier Collaboration?
The selection you make for the news article to e-mail about, and the topic of the e-mail, will have significant influence on the generated e-mail. The generated e-mail should mention the impact on supply chain from the news article, and ask the partner about the selected topic.

# Learn More

Link to future blog post (WIP)
