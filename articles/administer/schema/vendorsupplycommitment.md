---
title: VendorSupplyCommitment
description: This article provides information about the VendorSupplyCommitment entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# VendorSupplyCommitment

A vendor supply commitment is essentially an acknowledgement of a purchase order line, specifying the quantities of the PO line item that the vendor commits to deliver and when. A vendor may not be able to supply the full quantity in 1 shipment or not by the requested date. This shows how much they can ship and when, so there could be multiple commitments specified per PO line.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| VendorSupplyCommitment | VendorSupplyCommitmentLineNumber | yes | integer | 9 | The line number of a Vendor Supply Commitment, which is part of the unique identifier.</br></br> The line number of a Vendor Supply Commitment, which is part of the unique identifier. |
| VendorSupplyCommitment | PoLineItemNumber | yes | integer | 9 | The unique identifier of a PO line item. |
| VendorSupplyCommitment | PoNumber | yes | string | 18 | The unique identifier of a Purchase Order. |
| VendorSupplyCommitment | ShipmentMethodName | no | string | 36 | The unique identifier of the Shipment Method that will be used to ship the goods of this commitment. |
| VendorSupplyCommitment | CarrierID | no | string | 36 | The unique identifier of a Carrier that will be used to ship the commitment |
| VendorSupplyCommitment | VendorSupplyCommitmentQuantity | no | decimal | 9 | The quantity of the item that will be fulfilled in this commitment. |
| VendorSupplyCommitment | VendorSupplyCommitmentShipmentDate | no | timestamp | 14 | The date that a vendor intends to ship a specific supply commitment. |
| VendorSupplyCommitment | VendorSupplyCommitmentDeliveryDate | no | timestamp | 14 | The date that a vendor intends to deliver a specific supply commitment. |
