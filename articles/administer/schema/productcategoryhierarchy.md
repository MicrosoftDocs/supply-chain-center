---
title: ProductCategoryHierarchy
description: This is about ProductCategoryHierarchy entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **ProductCategoryHierarchy**

The product category hierarchy entity refers to an organizational structure that categorizes and organizes products within a company. It establishes a hierarchical relationship between various products, enabling businesses to manage and analyze their product portfolio effectively.

The product hierarchy typically consists of multiple levels, each representing a different level of detail and specificity. The exact structure may vary depending on the company and industry, but it generally follows a top-down approach.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	ProductCategoryHierarchyId	|	string	|	36	|	Yes	|	Product category hierarchy Id	|
|	ProductCategoryHierarchyNumber	|	string	|	256	|	Yes	|	Product category hierarchy number	|
|	ProductHierarchyDescription	|	string	|	4000	|	No	|	Description of the product hierarchy	|
|	ProductHierarchyName	|	string	|	256	|	No	|	Name of the product hierarchy	|
