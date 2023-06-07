---
title: CarrierDeliveryService
description: This article provides information about the CarrierDeliveryService entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **CarrierDeliveryService**

Carrier service refers to the transportation and delivery of goods or items from one location to another by a carrier or shipping company. It involves the process of moving packages, parcels, or freight using various modes of transportation such as trucks, ships, airplanes, or trains.

Carriers offer different types of delivery service. 
* **Express Shipping**: This type of service offers the fastest delivery times, often within one to two days. Express shipping is typically used for urgent or time-sensitive shipments. Some express shipping services provide same day delivery or overnight delivery.
* **Standard Shipping**: Standard shipping is the most common and affordable option for shipping packages. It usually takes a few days to a week for the shipment to reach its destination.
* **International Shipping**: International shipping allows you to send packages or goods across borders to different countries, and involves more documentation, customs clearance, and compliance with international regulations.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	CarrierId	|	string	|	36	|	No	|	Unique ID of the carrier. This is an internal carrier ID of the number.	|
|	CarrierNumber	|	string	|	256	|	No	|	Unique number of the carrier. 	|
|	CarrierServiceCode	|	string	|	256	|	No	|	The carrier service code.	|
|	CarrierServiceId	|	string	|	36	|	Yes	|	The unique ID of the service the carrier provides.	|
|	CarrierServiceNumber	|	string	|	256	|	Yes	|	The unique number of the service the carrier provides. Map the service ID in your ERP to this field.	|
|	DeliveryMethodCode	|	string	|	256	|	No	|	The delivery method of the carrier.	|
|	DeliveryMethodName	|	string	|	256	|	No	|	The name of the delivery method.	|
|	DeliveryModeName	|	string	|	256	|	No	|	The delivery mode of the carrier.	|