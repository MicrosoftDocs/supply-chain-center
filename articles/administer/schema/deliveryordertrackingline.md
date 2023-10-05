---
title: DeliveryOrderTrackingLine
description: This article provides information about the DeliveryOrderTrackingLine entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/30/2023
ms.custom: bap-template
---

# DeliveryOrderTrackingLine

[!INCLUDE[banner](../../includes/banner.md)]

The delivery order tracking line entity refers to the details of the tracking associated with the delivery order.


|	EntityAttribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	DeliveryOrderLineId	|	string	|	256	|	No	|	Unique identifier of the delivery order line.	|
|	DeliveryOrderLineNumber	|	string	|	256	|	No	|	Delivery order line number.	|
|	DeliveryOrderQuantity	|	decimal	|		|	No	|	Delivery order quantity.	|
|	DeliveryOrderTrackingId	|	string	|	36	|	No	|	Unique, system-generated tracking ID for the delivery order line.	|
|	DeliveryOrderTrackingLineId	|	string	|	36	|	Yes	|	Unique identifier of the tracking order line.	|
|	DeliveryOrderTrackingLineNumber	|	string	|	256	|	Yes	|	Tracking line number for the delivery order. 	|
|	DeliveryOrderTrackingNumber	|	string	|	256	|	No	|	Tracking number of the delivery order line.	|
|	Name	|	string	|	256	|	No	|	Name of the delivery order tracking line.	|
