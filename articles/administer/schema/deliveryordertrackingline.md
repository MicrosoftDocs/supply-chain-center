---
title: DeliveryOrderTrackingLine
description: This is about DeliveryOrderTrackingLine entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **DeliveryOrderTrackingLine**

The delivery order tracking line entity refers to the details of the tracking associated with the delivery order.


|	EntityAttribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	DeliveryOrderLineId	|	string	|	256	|	No	|	Delivery order line Id	|
|	DeliveryOrderLineNumber	|	string	|	256	|	No	|	Delivery order line number	|
|	DeliveryOrderQuantity	|	decimal	|		|	No	|	Delivery order quantity	|
|	DeliveryOrderTrackingId	|	string	|	36	|	No	|	Unique tracking Id for the delivery order line, this is system generated	|
|	DeliveryOrderTrackingLineId	|	string	|	36	|	Yes	|	Unique Id of the tracking order line	|
|	DeliveryOrderTrackingLineNumber	|	string	|	256	|	Yes	|	Unique tracking line number for the delivery order, 	|
|	DeliveryOrderTrackingNumber	|	string	|	256	|	No	|	Tracking number of the delivery order line	|
|	Name	|	string	|	256	|	No	|	Name of the delivery order tracking line	|
