---
title: DeliveryOrderSequenceNumber
description: This article provides information about the DeliveryOrderSequenceNumber entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **DeliveryOrderSequenceNumber**

Delivery order sequence entity refers to the sequencing of delivery order.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	DeliveryOrderId	|	string	|	36	|	No	|	Delivery order Id	|
|	DeliveryOrderName	|	string	|	256	|	No	|	Name of the delivery order sequence	|
|	DeliveryOrderNumber	|	string	|	256	|	No	|	Delivery order number	|
|	DeliveryOrderSequenceNumberId	|	string	|	36	|	Yes	|	Delivery order sequence Id	|
|	DeliveryOrderSequenceNumberNumber	|	string	|	256	|	Yes	|	Number of the delivery order sequence	|
|	MaximumSequenceNumber	|	string	|	256	|	No	|	Maximum sequence number	|