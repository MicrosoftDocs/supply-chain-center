---
title: ProductCategory
description: This is about ProductCategory entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **ProductCategory**

The product category entity refers to the classification or hierarchy of the product family.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	ExternalProductCategoryId	|	string	|	256	|	No	|	External product category Id	|
|	FriendlyCategoryName	|	string	|	256	|	No	|	Friendly category name of the product category	|
|	Hierarchy	|	string	|	256	|	No	|	Hierarchy of the product category	|
|	Integrationid	|	string	|	256	|	No	|	Integration Id of the product category	|
|	IsInheritingParentCategoryAttributes	|	boolean	|		|	No	|	Is it inheriting parent category attribute	|
|	IsInheritingParentProductAttributes	|	boolean	|		|	No	|	Is it inheriting parent product attribute	|
|	IsTangibleProduct	|	boolean	|		|	No	|	Is this a tangible product	|
|	Keywords	|	string	|	256	|	No	|	Keywords of the product category	|
|	Name	|	string	|	256	|	No	|	Name of the product category	|
|	Parentproductcategory	|	string	|	256	|	No	|	Parent product category	|
|	ProductCategoryCode	|	string	|	256	|	No	|	Product category code	|
|	ProductcategoryHierarchyid	|	string	|	36	|	No	|	The unique Id of the product category hierarchy	|
|	ProductCategoryHierarchyNumber	|	string	|	256	|	No	|	Product category hierarchy number	|
|	ProductCategoryId	|	string	|	36	|	Yes	|	The unique Id of the product category	|
|	ProductCategoryNumber	|	string	|	256	|	Yes	|	The unique number of the product category	|
|	ProductCategoryOwningBusinessUnit	|	string	|	4000	|	No	|	Business unit owning the product category	|
|	ProjectCategoryName	|	string	|	256	|	No	|	Name of the product category	|
