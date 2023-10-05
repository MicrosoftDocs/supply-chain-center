---
title: DocumentType
description: This article provides information about the DocumentType entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/30/2023
ms.custom: bap-template
---

# DocumentType

[!INCLUDE[banner](../../includes/banner.md)]

The document type entity refers to the definition of type of document.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	Description	|	string	|	4000	|	No	|	Description of the document type.	|
|	DocumentTypeId	|	string	|	36	|	Yes	|	The unique identifier of the document.	|
|	DocumentTypeName	|	string	|	256	|	No	|	Name of the document type.	|
|	DocumentTypeNumber	|	string	|	256	|	Yes	|	Number of the document type.	|
