---
title: ShippingService
description: This is about ShippingService entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **ShippingService**

The shipping service entity refers to the various shipping service associated with the carrier and shipment


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	Company	|	string	|	256	|	No	|	Company	|
|	Description	|	string	|	4000	|	No	|	Description of the shipping service	|
|	Name	|	string	|	256	|	No	|	Name of the shipping service	|
|	ShippingServiceId	|	string	|	36	|	Yes	|	The unique Id of the shipping service	|
|	ShippingServiceNumber	|	string	|	256	|	Yes	|	The unique number of the shipping service	|
