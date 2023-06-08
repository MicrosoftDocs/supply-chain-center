---
title: SalesOrderScheduleLine
description: This article provides information about the SalesOrderScheduleLine entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **SalesOrderScheduleLine**

THe sales order schedule line entity refers to sales order confirmation details. If the order line has multiple partial confirmations then the schedule contains details of the line with multiple delivery times and corresponding quantities.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	CommitmentItemSku	|	string	|	256	|	No	|	The product number of the sales order line	|
|	CommitmentProductId	|	string	|	36	|	No	|	The product ID of the sales order line	|
|	CommitmentQuantity	|	decimal	|		|	No	|	Confirmed or committed quantity of the sales order schedule	|
|	CommittedDeliveryDate	|	date	|		|	No	|	Estimated or committed delivery date of the sales order schedule	|
|	CommittedShipDate	|	date	|		|	No	|	Confirmed or committed ship date of the sales order schedule	|
|	FromWarehouseId	|	string	|	36	|	No	|	Fulfillment warehouse or From warehouse ID of the sales order schedule	|
|	FromWarehouseNumber	|	string	|	256	|	No	|	Fulfillment warehouse or From warehouse number of the sales order schedule	|
|	PlannedRouteId	|	string	|	256	|	No	|	Planned route ID of the sales order schedule	|
|	PlannedRouteNumber	|	string	|	256	|	No	|	Planned route number of the sales order schedule	|
|	SalesOrderId	|	string	|	36	|	No	|	Sales order ID of the schedule	|
|	SalesOrderLineId	|	string	|	36	|	No	|	Sales order line ID of the schedule	|
|	SalesOrderLineNumber	|	string	|	256	|	No	|	Sales order line number of the sales order	|
|	SalesOrderNumber	|	string	|	256	|	No	|	Sales order number of the schedule	|
|	SalesOrderScheduleLineId	|	string	|	36	|	Yes	|	The unique ID of the sales order schedule	|
|	SalesOrderScheduleLineNumber	|	string	|	256	|	Yes	|	The unique number of the sales order schedule	|
|	SequenceNumber	|	string	|	256	|	No	|	Sequence number of the sales order schedule	|
|	ShipMethod	|	string	|	256	|	No	|	The shipment method of the schedule line	|
