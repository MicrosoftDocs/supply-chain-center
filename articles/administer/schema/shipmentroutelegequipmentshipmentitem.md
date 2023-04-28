---
title: ShipmentRouteLegEquipmentShipmentItem
description: This is about ShipmentRouteLegEquipmentShipmentItem entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **ShipmentRouteLegEquipmentShipmentItem**

|	EntityAttribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	ShipmentId	|	string	|	36	|	No	|	The unique identifier of a Shipment.	|
|	ShipmentItemDeconsolidationNumber	|	string	|	256	|	No	|	A portion (breakdown / deconsolidation) of the a shipment item into smaller parts for the purpose of transport.	|
|	ShipmentItemId	|	string	|	36	|	Yes	|	Shipment item Id associated with the shipment route leg	|
|	ShipmentItemNumber	|	string	|	256	|	Yes	|	The shipment line number.	|
|	ShipmentNumber	|	string	|	256	|	No	|	Shipment number associated with shipment route leg	|
|	ShipmentRouteLegEquipmentShipmentItemId	|	string	|	36	|	Yes	|	The unique Id of the shipment route leg equipment shipment item	|
|	ShipmentRouteLegEquipmentShipmentItemNote	|	string	|	4000	|	No	|	A note, comment or additional information regarding the shipment route leg equipment shipment item.	|
|	ShipmentRouteLegEquipmentShipmentItemNumber	|	string	|	256	|	Yes	|	The unique number of the shipment route leg equipment shipment item	|
|	ShipmentRouteLegId	|	string	|	256	|	No	|	Route leg Id of the shipment route leg	|
|	ShipmentRouteLegNumber	|	string	|	256	|	No	|	Route leg number of the shipment route leg	|
|	SRLEquipmentSequenceNumber	|	string	|	256	|	No	|	The sequence number associated with the shipment route/leg equipment.	|
