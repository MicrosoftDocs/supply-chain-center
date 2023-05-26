---
title: DeliveryAttachment
description: This article provides information about the DeliveryAttachment entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **DeliveryAttachment**

Delivery attachment refers to the shipping related documents attached to the delivery order and the associated shipping tracking number.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	DeliveryAttachmentId	|	string	|	36	|	Yes	|	The unique ID of delivery attachement	|
|	DeliveryAttachmentNumber	|	string	|	256	|	Yes	|	The number of the delivery attachment on the delivery order	|
|	DeliveryName	|	string	|	256	|	No	|	Name of the delivery order	|
|	DeliveryOrderTrackingId	|	string	|	36	|	No	|	The tracking ID of the delivery order	|
|	DeliveryOrderTrackingNumber	|	string	|	256	|	No	|	The tracking number of the delivery order	|
