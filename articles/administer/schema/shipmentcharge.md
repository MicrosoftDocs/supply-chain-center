---
title: ShipmentCharge
description: This article provides information about the ShipmentCharge entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **ShipmentCharge**

[!INCLUDE[banner](../../includes/banner.md)]

The shipment charge entity refers to the applicable fee or charges incurred by the account for a shipment. 


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	ChargeByPartyId	|	string	|	256	|	No	|	The unique identifier of a Party.	|
|	ChargeByPartyNumber	|	string	|	256	|	No	|	Shipment charge by party number	|
|	ShipmentChargeAmount	|	decimal	|		|	No	|	The amount of the shipment charge.	|
|	ShipmentChargeId	|	string	|	36	|	Yes	|	Shipment charge Id	|
|	ShipmentChargeNumber	|	string	|	256	|	Yes	|	Shipment charge number 	|
|	ShipmentChargePaidTimestamp	|	timestamp	|		|	No	|	The timestamp that the shipment charge was paid.	|
|	ShipmentChargeTimestamp	|	timestamp	|		|	No	|	The timestamp of the shipment charge.	|
|	ShipmentChargeTypeId	|	string	|	256	|	No	|	The unique identifier of a shipment charge type.	|
|	ShipmentChargeTypeNumber	|	string	|	256	|	No	|	Type of shipment charge number	|
|	ShipmentId	|	string	|	36	|	No	|	The unique identifier of a Shipment.	|
|	ShipmentLegNumber	|	string	|	256	|	No	|	The unique identifier of the Shipment Leg Number, which equals the shipment leg 'sequence number'.	|
|	ShipmentNumber	|	string	|	256	|	No	|	Number of the shipment	|
