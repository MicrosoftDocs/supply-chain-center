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

|	EntityAttribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	CarrierId	|	string	|	36	|	No	|	Unique Id of the carrier. This is an internal carrier Id of the number	|
|	CarrierNumber	|	string	|	256	|	No	|	Unique number of the carrier. 	|
|	CarrierServiceCode	|	string	|	256	|	No	|	The carrier service code	|
|	CarrierServiceId	|	string	|	36	|	Yes	|	The unique Id of the service the carrier provides	|
|	CarrierServiceNumber	|	string	|	256	|	Yes	|	The unique number of the service the carrier provides. Map your service Id in your ERP to this field	|
|	DeliveryMethodCode	|	string	|	256	|	No	|	The delivery method of the carrier	|
|	DeliveryMethodName	|	string	|	256	|	No	|	The name of the delivery method	|
|	DeliveryModeName	|	string	|	256	|	No	|	The delivery mode of the carrier	|
