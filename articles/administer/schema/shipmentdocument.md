---
title: ShipmentDocument
description: This article provides information about the ShipmentDocument entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **ShipmentDocument**

The shipment document entity refers to the document associated with that shipment. Typical shipment documents are bill of lading, provisional invoice, customs invoice etc.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	IsoCurrencyCode	|	string	|	256	|	No	|	The ISO 4217 currency code.	|
|	ShipmentDocumentId	|	string	|	36	|	Yes	|	The unique ID of the shipment document	|
|	ShipmentDocumentIssuedTimestamp	|	timestamp	|		|	No	|	The timestamp when the shipment document was issued.	|
|	ShipmentDocumentNumber	|	string	|	256	|	Yes	|	The unique number of the shipment document	|
|	ShipmentDocumentTypeId	|	string	|	256	|	No	|	The unique ID of the shipment document type	|
|	ShipmentDocumentTypeNumber	|	string	|	256	|	No	|	The unique number of the shipment document type	|
|	ShipmentId	|	string	|	36	|	No	|	The unique identifier of a Shipment.	|
|	ShipmentNumber	|	string	|	256	|	No	|	Shipment number of the shipment document	|
