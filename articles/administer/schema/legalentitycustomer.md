---
title: LegalEntityCustomer
description: This article provides information about the LegalEntityCustomer entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# LegalEntityCustomer

A legal entity customer is one of the two types of customers upon which the Microsoft data models focus. Individual customer is the other. The definition of a customer is of critical importance for every organization. It's the customer that is the focus of product planning, marketing, sales, service, reporting and analytics. Without a customer there would be no need for the organization to exist since its purpose is to serve the customer and profit from that interaction.

The definition of a customer must be consistent with how customers exist and interact with the organization in the real world. An artificial or conceptual definition of a customer that isn't consistent with these two objectives will fail because the data won't be consistent with the definition and employees won't accept concepts or terms that aren't consistent with what they see, know and how they interact with customers on a working basis.

Microsoft defines a customer to meet these objectives. When we look out into the real world, we see two dominant types of customers: human beings (individual customers) and legal entities (legal entity customers). Legal entities are those legally defined entities such as corporations, partnerships, non-profit organizations, government organizations etc. that purchase products, goods and services. Individual customers are human beings of various ages, genders, demographics and a variety of similar dimensions that describe and define those who purchase products, good and services.

This view of a customer is consistent with the real world and consistent with how employees view and interact with customers. That is just the start of identifying, defining and understanding each corresponding type of customer. There is a great deal of detail, complexity and related data that can be used to define each type of customer to various levels of detail and different dimensions of information. Microsoft implements these detailed concepts and related data via two distinct business area models that expand the coverage and complexity of each type of customer:

LEGAL ENTITY CUSTOMER Business Area Model

INDIVIDUAL CUSTOMER Business Area Model

>[!Note]
> Each of the Microsoft models - enterprise, business area or data warehouse - have a representative level of detail for the appropriate type of customer, which is a 'subset' of the total data available in the associated INDIVIDUAL CUSTOMER or LEGAL ENTITY CUSTOMER business area models.. Reference either of those models to expand the coverage or level of detail in each respective data model.

The actual customer implemented in each model depends upon the dominant use of customer for that industry. For example, in the pharmaceutical industry, the customer is a legal entity, which represents another corporation, company, government organization etc. that purchases the pharmaceutical product and then distributes that product to the end-customer, which is an individual in a retail environment or a government-distribution scheme. For this example, the pharmaceutical models will have the legal entity customer represented but not the individual 'end customer' since that is represented in the appropriate retail industry models, which are a different offering. The entire set of data available for a legal entity customer is contained in the associated LEGAL ENTITY CUSTOMER Business Area Model. Reference the LEGAL ENTITY CUSTOMER Business Area Model to incorporate additional data that may be of relevance. In many industries both types of customers are represented since a legal entity or individual can purchase products, goods or services and enter into contracts. For these industries, both types of customers are represented by some of the more significant or relevant data derived from the associated LEGAL ENTITY or INDIVIDUAL CUSTOMER business area models. These models can be used to expand the scope or level of detail in any of the enterprise, business area or data warehouse models."

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| LegalEntityCustomer | CustomerId | yes | string | 36 | The unique identifier of a Customer. |
| LegalEntityCustomer | NaicsNationalIndustryCode | no | decimal | 9 | The unique identifier of a NAICS National Industry Code. |
| LegalEntityCustomer | DunsNumber | no | decimal | 13 | The DUNS number is a nine-digit number issued by Dun & Bradstreet and assigned to each business location in the D&B database having a unique, separate, and distinct operation to businesses for the purpose of identifying them. The number as issued is random and the digits apparently have no significance as to their issuance. |
| LegalEntityCustomer | AnzsicClassCode | no | decimal | 9 | The unique identifier of an ANZSIC Class. |
| LegalEntityCustomer | SicIndustryCode | no | decimal | 9 | The unique identifier of the SIC Industry. |
| LegalEntityCustomer | ListedSecuritySymbol | no | string | 8 | The security symbol of the Legal Entity, if any. |
| LegalEntityCustomer | StateOfLegalEntityResidence | no | string | 64 | The state in which the Legal Entity has it's primary business or official residence. |
| LegalEntityCustomer | LegalEntityName | no | string | 128 | The business name of the Legal Entity. |
| LegalEntityCustomer | FirstDateOfOperation | no | date | 8 | The first date that the Legal Entity entered into normal business operations. |
| LegalEntityCustomer | CountryOfLegalEntityResidence | no | string | 64 | The country in which the Legal Entity has its primary business or official residence. |
