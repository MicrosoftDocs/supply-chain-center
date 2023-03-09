---
title: PurchaseOrder
description: This article provides information about the PurchaseOrder entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# PurchaseOrder

Purchase orders are used in relatively simple transactions where minimal negotiations are required between the buyer and seller or where an existing agreement is in place. The seller states that products can be ordered with a purchase order. The Purchase Order is an offer to the seller to contract on the terms offered and any such offer specifically limits acceptance by seller to the terms defined.

A Purchase Order is a contract between the buyer and seller that specifies the items to be purchased, price and date that the goods or services will be delivered. The PO may also contain terms of purchase (STANDARD TERMS & CONDITIONS), specifications and quality levels. It is the legal agreement between the buyer and supplier and the reference point for measuring supplier performance. Changes to the Purchase Order may be made several points, PO Change Order (PURCHASING), and must be maintained for audit purposes.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| PurchaseOrder | PoNumber | yes | string | 36 | The unique identifier of a Purchase Order. |
| PurchaseOrder | PurchaseOrderTypeId | no | string | 36 | The unique identifier of a Purchase Order Type. |
| PurchaseOrder | RequisitionId | no | string | 36 | The unique identifier of the Requisition. |
| PurchaseOrder | PurchaseOrderStatusTypeId | no | string | 36 | The unique identifier of the PO Status. |
| PurchaseOrder | DocumentId | no | string | 36 | The unique identifier of a Document. |
| PurchaseOrder | CustomerId | no | string | 36 | The unique identifier of a Customer. |
| PurchaseOrder | VendorId | no | string | 36 | The unique identifier of a Vendor. |
| PurchaseOrder | ShipToLocationId | no | string | 36 | The unique identifier of a Location. |
| PurchaseOrder | PoAmount | no | decimal | 9 | The total amount of products that the Purchase Order authorizes purchase of. |
| PurchaseOrder | PoAcknowledgementDate | no | date | 8 | The date that acceptance of a purchase order was received, which verifies the cost, description, quantity and ship date of goods ordered as well as special terms or conditions. |
| PurchaseOrder | PoIssuedDate | no | date | 8 | The date that the Purchase Order was issued. |
| PurchaseOrder | ShipToName | no | string | 128 | The name of the person or organization that the PO items are to be shipped to (if different from the buyers). |
| PurchaseOrder | PoFreightAmount | no | decimal | 9 | The total amount of freight due for the PO items. |
| PurchaseOrder | PoProductAmount | no | decimal | 9 | The total product value of the PO exclusive of taxes, freight and any other costs.. |
