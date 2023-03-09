---
title: PurchaseOrderLine
description: This article provides information about the PurchaseOrderLine entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# PurchaseOrderLine

The specific products, goods or services that are identified on the Purchase Order.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| PurchaseOrderLine | PoLineItemNumber | yes | integer | 10 | The unique identifier of a PO line item. |
| PurchaseOrderLine | PoNumber | yes | string | 36 | The unique identifier of a Purchase Order. |
| PurchaseOrderLine | TotalLineItemAmount | no | decimal | 9 | The total value of the associated PO Line Items. |
| PurchaseOrderLine | FreightAmount | no | decimal | 9 | The amount of Freight costs authorized for the associated PO Line Item. |
| PurchaseOrderLine | OrderId | no | string | 36 | The unique number that identifies an Order. |
| PurchaseOrderLine | ItemSku | no | string | 20 | The Stock Keeping Unit identifier, which is typically used for inventory-related activities. |
| PurchaseOrderLine | NegotiatedPrice | no | decimal | 9 | The negotiated price of the associated PO Line Items. |
| PurchaseOrderLine | Quantity | no | decimal | 9 | The quantity of products to be shipped for this line item. |
| PurchaseOrderLine | OrderLineNumber | no | integer | 9 | The number that identifies the Order Line Item. |
| PurchaseOrderLine | UnitPrice | no | decimal | 9 | The unit price of the product. |
| PurchaseOrderLine | DateRequired | no | date | 8 | The date that the items are required.. |
