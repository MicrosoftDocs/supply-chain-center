---
title: ShipmentDocument
description: This article provides information about the ShipmentDocument entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# ShipmentDocument

A document associated with a Shipment.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ShipmentDocument | DocumentId | yes | string | 36 | The unique identifier of a Document. |
| ShipmentDocument | ShipmentId | yes | string | 36 | The unique identifier of a Shipment. |
| ShipmentDocument | IsoCurrencyCode | no | string | 3 | The ISO 4217 currency code. |
| ShipmentDocument | ShipmentDocumentIssuedTimestamp | no | timestamp | 14 | The timestamp when the shipment document was issued. |
| ShipmentDocument | ShippingDocumentTypeId | no | string | 36 | The unique identifier of a Shipping Document Type. |

EOF