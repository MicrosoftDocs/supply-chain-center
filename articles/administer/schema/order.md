---
title: Order
description: This article provides information about the Order entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# Order

A document or commission by the customer to order products.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| Order | OrderId | yes | string | 36 | The unique number that identifies an Order. |
| Order | ShipmentToLocationId | no | string | 36 | The unique identifier of a Location. |
| Order | ShipmentToName | no | string | 128 | The name of the ship-to party. |
| Order | OrderTotalRetailPriceAmount | no | decimal | 9 | The total list price value of the ordered products = (list price per unit product price)x(quantity ordered) for each line item. |
| Order | CarrierId | no | string | 36 | The unique identifier of a Carrier. |
| Order | OrderTotalAmount | no | decimal | 9 | The total value of the Order including Adjustment(s). |
| Order | OrderTotalActualSalesPriceAmount | no | decimal | 9 | The total actual price value of the ordered products = (actual selling price per unit product price)x(quantity ordered) for each line item. |
| Order | OrderReturnedDate | no | date | 8 | The date that the Order was returned. |
| Order | OrderCancellationDate | no | date | 8 | The date that the Order was cancelled. |
| Order | ShipmentMethodName | no | string | 256 | The unique identifier of a Shipment Method. |
| Order | OrderProcessingStatusId | no | string | 36 | The unique identifier of an Order Processing Status. |
| Order | RejectionReasonId | no | string | 36 | The unique identifier of a Rejection Reason. |
| Order | VendorId | no | string | 36 | The unique identifier of a Vendor. |
| Order | IsoCurrencyCode | no | string | 3 | The ISO 4217 currency code. |
| Order | OrderTypeId | no | string | 36 | The unique identifier of an Order Type. |
| Order | WeightUomId | no | string | 36 | The unique identifier of a Unit Of Measure. |
| Order | TotalOrderWeight | no | decimal | 9 | The total weight of the Order. |
| Order | DistributionChannelId | no | integer | 9 | The unique identifier of a Channel. |
| Order | SalesChannelId | no | integer | 9 | The unique identifier of a Channel. |
| Order | ProductOrderIndicator | no | boolean | 9 | Indicates that the Order is for Products. |
| Order | LatestDeliveryWindowTimestamp | no | timestamp | 8 | The latest timestamp that the order should be made available for delivery. |
| Order | WarehouseId | no | string | 36 | The unique identifier of a Warehouse. |
| Order | CustomerAccountId | no | string | 36 | The unique identifier of a Customer Account. |
| Order | EarliestDeliveryWindowTimestamp | no | timestamp | 8 | The earliest timestamp that the order should be made available for delivery. |
| Order | StoreId | no | string | 36 | The unique identifier of a Store. |
| Order | OrderDeliveryInstructions | no | string | 2048 | Instructions related to the delivery of the Order. |
| Order | PoNumber | no | string | 36 | The unique identifier of a Purchase Order. |
| Order | CustomerIdentificationMethodId | no | string | 36 | The unique identifier of a customer identification method. |
| Order | OrderCommittedDeliveryDate | no | date | 8 | The date committed to the Customer/Customer Account for delivery of the Order. |
| Order | OrderRequestedDeliveryDate | no | date | 8 | The date that the Customer/Customer Account requested delivery of the Order. |
| Order | OrderActualDeliveryTimestamp | no | timestamp | 8 | The actual timestamp of delivery of the Order to the Customer/Customer Account. |
| Order | ShipmentConfirmationTimestamp | no | timestamp | 8 | The timestamp that confirmation of the Shipment was made to the Customer/Customer Account. |
| Order | OrderEntryTimestamp | no | timestamp | 8 | The date that the Order was entered into the order entry system. |
| Order | OrderConfirmationNumber | no | string | 16 | The order confirmation number provided to the Customer/Customer Account. |
| Order | CustomerId | no | string | 36 | The unique identifier of a customer. |
| Order | OrderReceivedTimestamp | no | timestamp | 8 | The timestamp that the Order was received from the Customer/Customer Account. |
| Order | OrderEnteredByEmployeeId | no | string | 36 | The employee ID of the employee entering the Order into the order entry system.. |
