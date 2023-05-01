---
title: ShipmentEventStatus
description: This is about ShipmentEventStatus entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **ShipmentEventStatus**

The shipment event status entity refers to the status of the shipment.
For example:

planned
in process
completed
unknown

|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	ShipmentEventId	|	string	|	256	|	No	|	Shipment event Id of the shipment	|
|	ShipmentEventNumber	|	string	|	256	|	No	|	Shipment event number of the shipment	|
|	ShipmentEventStatusDescription	|	string	|	4000	|	No	|	The description of a Shipment Event Status.	|
|	ShipmentEventStatusId	|	string	|	36	|	Yes	|	The unique identifier of a Shipment Event Status.	|
|	ShipmentEventStatusName	|	string	|	256	|	No	|	The name of a Shipment Event Status.	|
|	ShipmentEventStatusNumber	|	string	|	256	|	Yes	|	Shipment event status number of the shipment	|
