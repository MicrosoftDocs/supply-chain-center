---
title: Product
description: This article provides information about the Product entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# Product

A product is anything that can be offered to a market that might satisfy a want or need by potential customers. That product is the sum of all physical, psychological, symbolic, and service attributes associated with it.

There are two basic types of products:

- Tangible (physical)
- Intangible (non-physical) such as services

A service is a non-material or intangible product - such as professional consultancy, maintenance service, repair service etc. Each product has its own benefits, application, brand name, and packaging that gives it its own identity and distinguishing characteristics.

Every business or organization has business rules that define precisely what a product is. While we intuitively know what a product is, we must quantify that knowledge and associated business rules with consistent definitions that can be implemented within the organization in strategies and applications. A product typically goes through five stages of development:

1. Idea Stage - involving a thorough evaluation of the potential product.
1. Concept Stage - determines customer acceptance by testing and presentation to consumers and distribution channel members. Specific aspects regarding quality, dependability, reliability, warranty, packaging, service, pricing, terms of sale, sales and distribution channels, advertising and promotions are evaluated.
1. Product Development Stage - transforms the prototype product into an actual product for mass sale. This stage requires close interaction between both marketing and manufacturing.
1. Test Marketing Stage - may or may not be used since it is an expensive and time-consuming process. Test marketing involves evaluating various product options and alternatives.
1. Commercialization - It is very expensive to launch a new product so commercialization only applies to those specific products that are actually going to be sold to the market.

Products tend to be categorized as either: Industrial goods and consumer goods. Industrial goods are used to produce other products.

Industrial goods may be further divided into:

- Raw materials.
- Equipment.
- Pre-built materials.
- Supplies.
- Consumer goods are intended for consumption by the general public.
- Consumer goods may be further divided into:
  - Durable goods.
  - Nondurable goods.
  - Packaged goods.

A product may be a member of a product family or product line.

A product family is a grouping of products or services that are related to each other by common function, functionality, design platform or similar characteristics. Members of a product family frequently have many common parts and assemblies. Product families are the highest level of grouping for forecasting, capacity planning or related functions.

For example:

The Surface family of products consists of the product lines:

- Surface Book
- Surface Laptop
- Surface Go

A product line is a grouping of products that are closely related in usage, functionality or marketing characteristics. A Product Family typically is created to address one or five functions:

1. To increase profits and not erode the sales of existing products.
1. To attract additional Markets or Market Segments.
1. To counter competitor's products.
1. To fill a gap in an existing Product Family.
1. To promote sales of other products in the family line.

Line Depth refers to the number of products in the product line. Line consistency refers to how closely related the products are that make up the product line.

Line vulnerability refers to the percentage of sales or profits that are derived from only a few products in the product line. Product width refers to the number of different product lines sold by a company. Product mix refers to the total number of products sold in all product lines. Line extension refers to the adding of a new product to a line.

Trading up or brand leveraging refers to adding a product of better quality to a product line than the other products in that line. Trading down refers to adding a product of lesser quality to a product line than the other products in that line.

If a line of products is sold with the same brand name, this is referred to as family branding. Strategy and decisions regarding a product line are usually incorporated in a high-level marketing plan addressing product line strategy, sales, channels, distribution channels, pricing and related issues. A product-line manager is responsible for a product line and supervises several product managers who are responsible for individual products within the line. Product-line managers typically have the following responsibilities:

- Expansion and composition of a product line
- Evaluate the effects of product mixes on the profitability of other items in the line
- Planning and allocation of resources to individual products in the line

A product is normally associated with a brand strategy - manufacturer, private or generic.

1. Manufacturer or national branding in which the brand is assigned by the manufacturer of the Product.
1. Private or dealer branding in which the brand is assigned by the retailer or wholesaler of the Product.
1. Generic in which the Product is not marked with any identification. Generic brands are a means for manufacturers to increase profits by saving on advertising, packaging or other costs associated with manufacturer or private branding.

A brand is name, term, sign, symbol or design or a combination of these which identify the goods or services and differentiate them from those of competitors'. A Trademark is a brand or some part of the brand that is given legal protection because it is capable of exclusive appropriation and representation. Manufacturers can use their own brands (known as Manufacturers' brands) or brands of their distributors (Distributors' brands). Manufacturers/ distributors use brand names for a variety of reasons ranging from simple identification purposes to having legal protection for unique features of the products from imitations. Brands help consumers recognize certain quality parameters. In some cases, brands are just used to endow the product with unique story and character which itself can be a basis for product differentiation. Individual brands have their own identity and the corporate or common name is not used to promote its equity. Individual branding requires more expensive advertising and brand extensive brand creation investments. By extension, each new brand does not benefit from the positive perceptions of earlier brands.

By contrast, family branding has several advantages. Each new product is quickly associated with the other products and brand in terms of quality and benefits. Reduced or eliminated time for name identification and advertising for name recognition purposes.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| Product | ProductId | yes | string | 36 | The unique identifier of a Product. |
| Product | ItemSku | no | string | 20 | The Stock Keeping Unit identifier, which is typically used for inventory-related activities. |
| Product | ProductDescription | no | string | 512 | The description of the Product. |
| Product | ProductName | no | string | 128 | The name of the Product, which normally corresponds to the 'marketing name' of the Product. |
