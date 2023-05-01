---
title: CarrierDeliveryService
description: This is about CarrierDeliveryService entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **CarrierDeliveryService**

Carrier service refers to the transportation and delivery of goods or items from one location to another by a carrier or shipping company. It involves the process of moving packages, parcels, or freight using various modes of transportation such as trucks, ships, airplanes, or trains.
Carriers offer different type of delivery service. Some of the various delivery services are shown below. 

Express Shipping: This type of service offers the fastest delivery times, often within one to two days. Express shipping is typically used for urgent or time-sensitive shipments. Some of express shipping are same day delivery or overnight delivery

Standard Shipping: Standard shipping is the most common and affordable option for shipping packages. It usually takes a few days to a week for the shipment to reach its destination.

International Shipping: International shipping allows you to send packages or goods across borders to different countries. It involves additional documentation, customs clearance, and compliance with international regulations.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	CarrierId	|	string	|	36	|	No	|	Unique Id of the carrier. This is an internal carrier Id of the number	|
|	CarrierNumber	|	string	|	256	|	No	|	Unique number of the carrier. 	|
|	CarrierServiceCode	|	string	|	256	|	No	|	The carrier service code	|
|	CarrierServiceId	|	string	|	36	|	Yes	|	The unique Id of the service the carrier provides	|
|	CarrierServiceNumber	|	string	|	256	|	Yes	|	The unique number of the service the carrier provides. Map your service Id in your ERP to this field	|
|	DeliveryMethodCode	|	string	|	256	|	No	|	The delivery method of the carrier	|
|	DeliveryMethodName	|	string	|	256	|	No	|	The name of the delivery method	|
|	DeliveryModeName	|	string	|	256	|	No	|	The delivery mode of the carrier	|
