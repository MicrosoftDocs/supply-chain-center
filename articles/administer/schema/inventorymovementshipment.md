---
title: InventoryMovementShipment
description: This article provides information about the InventoryMovementShipment entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **InventoryMovementShipment**

The inventory movement shipment entity refers to the shipments used to transport the items specified in the inventory transaction.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	InventoryMovementId	|	string	|	36	|	No	|	Inventory movement id for the inventory shipment	|
|	InventoryMovementNumber	|	string	|	256	|	No	|	Inventory movement number for the inventory shipment	|
|	InventoryMovementShipmentId	|	string	|	256	|	Yes	|	Inventory movement shipment id for the inventory shipment	|
|	InventoryMovementShipmentNumber	|	string	|	256	|	Yes	|	Inventory movement shipment number for the inventory shipment	|
|	ShipmentId	|	string	|	36	|	Yes	|	The unique identifier of a Shipment.	|
|	ShipmentItemId	|	string	|	36	|	No	|	Shipment item id for the inventory shipment	|
|	ShipmentItemNumber	|	string	|	256	|	No	|	The shipment line number.	|
|	ShipmentNumber	|	string	|	256	|	Yes	|	Shipment number for the inventory shipment	|
