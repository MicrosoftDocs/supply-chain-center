---
title: OrderLine
description: This article provides information about the OrderLine entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# OrderLine

The customer order that contains the items, quantity and date required.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| OrderLine | OrderLineNumber | yes | integer | 10 | The number that identifies the Order Line Item. |
| OrderLine | OrderId | yes | string | 36 | The unique number that identifies an Order. |
| OrderLine | DropShipOrderLineItemIndicator | no | boolean | 6 | Indicates that the Order Line Item(s) are to be drop shipped. |
| OrderLine | ShipmentConfirmationTimestamp | no | timestamp | 8 | The timestamp that the shipment confirmation notice was sent to the Customer/Customer Account. |
| OrderLine | NetWeight | no | decimal | 9 | The weight of the line items including packaging. |
| OrderLine | WaybillNumber | no | string | 256 | The shipment waybill number. |
| OrderLine | ActualShipmentTimestamp | no | timestamp | 8 | The actual shipment timestamp of the Order Line Items. |
| OrderLine | PlannedShipmentDate | no | date | 8 | The planned shipment date of the Order Line Items. |
| OrderLine | ActualDeliveryTimestamp | no | timestamp | 8 | The actual delivery timestamp of the Order Line Items. |
| OrderLine | PlannedDeliveryDate | no | date | 8 | The planned delivery date of the Order Line Items. |
| OrderLine | ReturnToStockIndicator | no | boolean | 6 | Indicates that the Line Item(s) were returned to stock. |
| OrderLine | ReturnOrderLineNumber | no | integer | 9 | The number that identifies the Order Line Item. |
| OrderLine | RejectionReasonId | no | integer | 6 | The unique identifier of a Rejection Reason. |
| OrderLine | OrderLineTypeId | no | integer | 6 | The unique identifier of an Order Line Type. |
| OrderLine | EarliestDeliveryWindowTimestamp | no | timestamp | 8 | The earliest timestamp that the order should be made available for delivery. |
| OrderLine | WeightUomId | no | string | 36 | The unique identifier of a Unit of Measure. |
| OrderLine | ReturnOrderId | no | string | 36 | The unique number that identifies an Order. |
| OrderLine | LatestDeliveryWindowTimestamp | no | timestamp | 8 | The latest timestamp that the order should be made available for delivery. |
| OrderLine | ActualPickTimestamp | no | timestamp | 8 | The actual inventory pick timestamp for the Order Line Items. |
| OrderLine | ProductSalesPriceAmount | no | decimal | 9 | The actual per unit selling price of the Order Line-Item products. |
| OrderLine | ProductListPriceAmount | no | decimal | 9 | The current per unit list price of the Order Line-Item products. |
| OrderLine | OrderLineNote | no | string | 1024 | A note, comment, or additional information regarding the Order Line. |
| OrderLine | TotalOrderLineAmount | no | decimal | 9 | The total amount of line-item charges related to the quantity of products sold at the actual selling price less rebates and discounts. |
| OrderLine | ReturnedDate | no | date | 8 | The date that Order Line Items were returned. |
| OrderLine | ProductId | no | string | 36 | The unique identifier of a Product. |
| OrderLine | Quantity | no | decimal | 9 | The quantity of Product ordered on the order line item. |
| OrderLine | ItemSku | no | string | 20 | The Stock Keeping Unit identifier, which is typically used for inventory-related activities. |
| OrderLine | RequestedDeliveryDate | no | date | 8 | The date for delivery of the Order Line Item requested by the Customer/Customer Account. |
| OrderLine | QuantityReturned | no | decimal | 9 | The quantity of Order Line Items returned. |
| OrderLine | PlannedPickDate | no | date | 8 | The planned inventory pick date for the Order Line Items. |
| OrderLine | CommittedDeliveryDate | no | date | 8 | The date committed for delivery of the Order Line Item. |
| OrderLine | QuantityBacklog | no | decimal | 9 | The quantity on backlog. |
| OrderLine | QuantityBooked | no | decimal | 9 | The quantity of Product booked. |
| OrderLine | QuantityCancelled | no | decimal | 9 | The quantity of Order Line Items cancelled. |
| OrderLine | AcceptedQuantity | no | decimal | 9 | The quantity of Order Line Item products accepted. |

EOF