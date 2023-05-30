---
title: DeliveryOrderSourcePrintSpecification
description: This article provides information about the DeliveryOrderSourcePrintSpecification entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/30/2023
ms.custom: bap-template
---

# DeliveryOrderSourcePrintSpecification

Delivery order source print specification entity refers to the print specification for the delivery order.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	DeliveryOrderSourceId	|	string	|	36	|	No	|	Unique identifier of the delivery order source.	|
|	DeliveryOrderSourceNumber	|	string	|	256	|	No	|	Number of the delivery order source.	|
|	DeliveryOrderSourcePrintSpecificationId	|	string	|	36	|	Yes	|	Unique identifier of the delivery order source print specification.	|
|	DeliveryOrderSourcePrintSpecificationNumber	|	string	|	256	|	Yes	|	Unique number of the delivery order source print specification.	|
|	DocumentSpecificationId	|	string	|	36	|	No	|	Unique identifier of the document specification.	|
|	DocumentSpecificationNumber	|	string	|	256	|	No	|	Document specification number of the print specification.	|
|	DocumentTypeId	|	string	|	36	|	No	|	Unique identifier of the document type.	|
|	DocumentTypeNumber	|	string	|	256	|	No	|	Document type number of the print specification.	|
|	Name	|	string	|	256	|	No	|	Name of the print specification for delivery order source.	|
