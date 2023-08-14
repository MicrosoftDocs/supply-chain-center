---
author: johnmichalak

ms.topic: include
ms.date: 08/15/2023
ms.author: johnmichalak
---

## What are Supplier news communication's capabilities?

Supplier news communication uses a text-davinci-003 generative AI model to draft the e-mail. It uses Azure Open AI's Content Moderator to help validate the response, and an NGram-based relevance filter to ensure that the response is on topic. It takes as input the title and snippet from the news article, the user-selected topic, and up to five upcoming open purchase orders to make sure the generated e-mail includes the relevant business context.

## What is Supplier news communication's intended use?

Use Supplier news communication to enable business users to follow up with their partners more quickly and efficiently about supply chain disruptions that have been reported in the news.

## How was Supplier news communication evaluated? What metrics were used to measure performance?

Supplier news communication was evaluated through human judgment on a random sample of drafted emails from a random selection of news articles. Here are some of the metrics that were used to evaluate the system's performance:

- Does the email contain false information?
- Is the email content relevant and actionable?
- Is the email syntactically correct?
- Was the topic correctly incorporated into the email?
- How much editing was required before the email could be sent?

## What are Supplier news communication's limitations? How can users minimize the impact of those limitations when they use Supplier news communication?

Supplier news communication currently supports drafting emails only in the English language. The draft email is generated one time, and there isn't support for editing it. Because we can't test every possible news situation, some generated emails might be of lower quality than the emails that we tested. You can mitigate this limitation by reviewing every draft email before you send it.

## What operational factors and settings allow for effective and responsible use of Supplier news communication?

The news article that you select to draft an email about, and the topic of the email, will significantly influence the generated email. The generated email should mention the impact that the news article will have on the supply chain, and should ask the partner about the selected topic.

## What data has Supplier News Communication been trained on? 

The text-davinci-003 generative AI model has been trained on data on the internet with billions of parameters for tuning. It doesn’t have access to the internet, meaning that data can be stale. While we'e mitigating incorrect information with our content moderation checks, it's possible that the generated e-mail may contain false information.

## Does Supplier News Communication produce perfect emails?

It's not guaranteed to produce perfect e-mails. While we do have checks in place to reduce the frequency of offensive or false information in e-mails, you should always review the e-mail before sending.

## How does a customer get the most out of Supplier News Communication? 

A customer can get the most out of Supplier News Communication by selecting topics that are relevant for them and always reviewing the generated e-mail.

## Does Supplier News Communication produce offensive content?

While we do have checks in place to reduce the likelihood of the e-mail containing offensive content, it's not guaranteed so you should always review the e-mail before sending.


## Troubleshooting

If you find that your Supply Chain Center environment is not set up to send email, see the following [documentation](/power-platform/admin/connect-exchange-online)
