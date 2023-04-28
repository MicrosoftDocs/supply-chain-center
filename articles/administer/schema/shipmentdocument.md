---
title: ShipmentDocument
description: This is about ShipmentDocument entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **ShipmentDocument**

|	EntityAttribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	IsoCurrencyCode	|	string	|	256	|	No	|	The ISO 4217 currency code.	|
|	ShipmentDocumentId	|	string	|	36	|	Yes	|	The unique Id of the shipment document	|
|	ShipmentDocumentIssuedTimestamp	|	timestamp	|		|	No	|	The timestamp when the shipment document was issued.	|
|	ShipmentDocumentNumber	|	string	|	256	|	Yes	|	The unique number of the shipment document	|
|	ShipmentDocumentTypeId	|	string	|	256	|	No	|	The unique Id of the shipment document type	|
|	ShipmentDocumentTypeNumber	|	string	|	256	|	No	|	The unique number of the shipment document type	|
|	ShipmentId	|	string	|	36	|	No	|	The unique identifier of a Shipment.	|
|	ShipmentNumber	|	string	|	256	|	No	|	Shipment number of the shipment document	|
