---
title: Customer
description: This article provides information about the Customer entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# Customer

A customer is an individual or legal entity that has or has purchased a product or service.

A potential customer is an individual or legal entity that desires to acquire a product or service, the financial ability to pay for that product or service, and is located in a location in which the product or service can be delivered to them.

The definition of a customer is of critical importance for every organization.

It's the customer that is the focus of product planning, marketing, sales, service, reporting and analytics. Without a customer there would be no need for the organization to exist since its purpose is to serve the customer and profit from that interaction.

The definition of a customer must be consistent with how customers exist and interact with the organization in the real world. An artificial or conceptual definition of customer that is not consistent with these two objectives will to fail because the data won't be consistent with the definition and employees won't accept concepts or terms that aren't consistent with what they see, know and how they interact with customers on a working basis.

Microsoft defines a customer to meet these objectives. When we look out into the real world, we see two dominant types of customers: human beings and legal entities.

Human beings are individuals of various ages, gender, demographics and a variety of similar dimensions that describe and define them who purchase products, good and services.

Legal entities are those legally defined entities such as corporations, partnerships, non-profit organizations, government organizations etc. that purchase products, goods and services.

This view of a customer is consistent with the real world and consistent with how employees view and interact with customers.

That is just the start of identifying, defining and understanding each type of customer. There's a great deal of detail, complexity and related data that can be used to define each type of customer to various levels of detail and different dimensions of information.

Microsoft implements these detailed concepts and related data via two distinct business area models that expand the coverage and complexity of each type of customer:

- INDIVIDUAL CUSTOMER Business Area Model
- LEGAL ENTITY CUSTOMER Business Area Model

>[!Note]
> Each of the Microsoft models - enterprise, business area or data warehouse - have a representative level of detail for the appropriate type of customer, which is a 'subset' of the total data available in the associated INDIVIDUAL CUSTOMER or LEGAL ENTITY CUSTOMER business area models.. Reference either of those models to expand the coverage or level of detail in each respective data model.

The actual customer implemented in each model depends upon the dominant use of customer for that industry.

For example, in the pharmaceutical industry the customer is a legal entity, which represents another corporation, company, government organization etc. that purchases the pharmaceutical product and then distributes that product to the end-customer, which is an individual in a retail environment or a government-distribution scheme.

For this example, the pharmaceutical models will have the legal entity customer represented but not the individual 'end customer' since that is represented in the appropriate retail industry models, which are a different offering.

Of course, the entire set of data available for a legal entity customer is contained in the associated LEGAL ENTITY CUSTOMER Business Area Model. Reference the LEGAL ENTITY CUSTOMER Business Area Model to incorporate additional data that may be of relevance.

In many industries both types of customers are represented since a legal entity or individual can purchase products, goods or services and enter into contracts. For these industries, both types of customers are represented by some of the more significant or relevant data derived from the associated LEGAL ENTITY or INDIVIDUAL CUSTOMER business area models. These models can be used to expand the scope or level of detail in any of the enterprise, business area or data warehouse models.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| Customer | CustomerId | yes | string | 36 | The unique identifier of a Customer. |
| Customer | CustomerEstablishedDate | no | date | 8 | The date that the Customer relationship was established. |
| Customer | CustomerTypeId | no | string | 36 | The unique identifier of a Customer Type. |
| Customer | PartyId | no | string | 36 | The unique identifier of a Party.. |
