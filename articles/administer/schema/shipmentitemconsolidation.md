---
title: ShipmentItemConsolidation
description: This is about ShipmentItemConsolidation entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **ShipmentItemConsolidation**

The consolidation of shipment items for transfer. Shipments Items are not breakable (SHIPMENT CONSOLIDATION). Shipment Item Consolidation deals with Shipments that can be broken at the item level.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	ConsolidatedShipmentId	|	string	|	36	|	No	|	The unique identifier of a Shipment.	|
|	ConsolidatedShipmentItemId	|	string	|	36	|	No	|	Consolidated shipment item Id of the shipment	|
|	ConsolidatedShipmentItemNumber	|	string	|	256	|	No	|	The shipment line number.	|
|	ConsolidatedShipmentNumber	|	string	|	256	|	No	|	The unique geographical location Id of the shipment	|
|	ContainerId	|	string	|	256	|	No	|	The unique identifier of the container.

This would be the 'serial number' of the container if it is serialized.	|
|	ContainerNumber	|	string	|	256	|	No	|	Container number of the shipment	|
|	PackedHeight	|	decimal	|		|	No	|	The height of the Packing Type in which the associated Lot of shipped items are packed.

Ex:
Lot 3 consisting of 35 cans are packed in a box of external length, external width and external height measurements.

This enables shipped to plan for containerizing shipped items.	|
|	PackedLength	|	decimal	|		|	No	|	The length of the Packing Type in which the associated Lot of shipped items are packed.

Ex:
Lot 3 consisting of 35 cans are packed in a box of external length, external width and external height measurements.

This enables shipped to plan for containerizing shipped items.	|
|	PackedVolume	|	decimal	|		|	No	|	The volume of the Packing Type in which the associated Lot of shipped items are packed.

Ex:
Lot 3 consisting of 35 cans are packed in a box of external length, external width and external height measurements.

This enables shipped to plan for containerizing shipped items.	|
|	PackedWeight	|	decimal	|		|	No	|	The weight of the Packing Type in which the associated Lot of shipped items are packed.

Ex:
Lot 3 consisting of 35 cans are packed in a box of external length, external width and external height measurements.

This enables shipped to plan for containerizing shipped items.	|
|	PackedWidth	|	decimal	|		|	No	|	The width of the Packing Type in which the associated Lot of shipped items are packed.

Ex:
Lot 3 consisting of 35 cans are packed in a box of external length, external width and external height measurements.

This enables shipped to plan for containerizing shipped items.	|
|	PackingTypeId	|	string	|	256	|	No	|	The unique identifier of a Packing Type.	|
|	PackingTypeNumber	|	string	|	256	|	No	|	Packing type number of the shipment	|
|	Quantity	|	decimal	|		|	No	|	The quantity of shipped items in the associated lot.	|
|	ShipmentId	|	string	|	36	|	No	|	The unique identifier of a Shipment.	|
|	ShipmentItemConsolidationId	|	string	|	36	|	Yes	|	The unique consolidation Id of the shipment	|
|	ShipmentItemConsolidationNumber	|	string	|	256	|	Yes	|	The unique consolidation number of the shipment	|
|	ShipmentItemId	|	string	|	36	|	No	|	Shipment item Id of the shipment	|
|	ShipmentItemNumber	|	string	|	256	|	No	|	The shipment line number.	|
|	ShipmentNumber	|	string	|	256	|	No	|	Shipment number of the shipment	|
|	UoMId	|	string	|	36	|	No	|	Unit of measure Id	|
|	UoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
|	VolumeUoMId	|	string	|	36	|	No	|	Unit of measure Id	|
|	VolumeUoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
|	WeightUoMId	|	string	|	36	|	No	|	Unit of measure Id	|
|	WeightUoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
