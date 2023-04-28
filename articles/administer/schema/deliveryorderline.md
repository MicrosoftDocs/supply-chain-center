---
title: DeliveryOrderLine
description: This is about DeliveryOrderLine entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **DeliveryOrderLine**

|	EntityAttribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	ActualShipDate	|	date	|		|	No	|	Actual ship date of the delivery order line	|
|	CarrierDeliveryService	|	string	|	256	|	No	|	Carrier delivery service	|
|	CarrierId	|	string	|	36	|	No	|	Carrier Id for the delivery order line	|
|	CarrierNumber	|	string	|	256	|	No	|	Carrier number for the delivery order line	|
|	CarrierServiceNumber	|	string	|	256	|	No	|	Carrier service number	|
|	DeliveryDate	|	date	|		|	No	|	Delivery date of the delivery order	|
|	DeliveryOrderId	|	string	|	36	|	No	|	Delivery order iD	|
|	DeliveryOrderLineId	|	string	|	36	|	Yes	|	The unique line Id of the delivery order	|
|	DeliveryOrderLineNumber	|	string	|	256	|	Yes	|	The unique line number of the delivery order	|
|	DeliveryOrderName	|	string	|	256	|	No	|	Name of the delivery order	|
|	DeliveryOrderNumber	|	string	|	256	|	No	|	Delivery order number	|
|	DeliveryOrderOpenQuantity	|	string	|	256	|	No	|	Delivery order open quantity	|
|	DeliveryOrderPickedQuantity	|	decimal	|		|	No	|	Picked quantity for the delivery order line	|
|	DeliveryOrderQuantity	|	decimal	|		|	No	|	Delivery order quantity	|
|	InvoiceQuantity	|	decimal	|		|	No	|	Invoice quantity of the delivery order line	|
|	IomReadOnly	|	string	|	256	|	No	|	Delivery order line IOM read only	|
|	IomState	|	string	|	256	|	No	|	Delivery order line IOM state	|
|	IomStateReason	|	string	|	4000	|	No	|	Delivery order IOM state reason	|
|	IsProductOverridden	|	boolean	|		|	No	|	Is this product overridden	|
|	ItemSku	|	string	|	256	|	No	|	The stock keeping unit of the product	|
|	LineNumber	|	string	|	256	|	Yes	|	Line number of the delivery order line	|
|	OpenInvoiceQuantity	|	decimal	|		|	No	|	Open invoice quantity for the delivery order line	|
|	PlannedShippingDate	|	date	|		|	No	|	Planned shipping date for the delivery order line	|
|	ProductCategoryId	|	string	|	36	|	No	|	Product category Id of the product in the delivery order	|
|	ProductCategoryNumber	|	string	|	256	|	No	|	Product category number	|
|	ProductDescription	|	string	|	4000	|	No	|	Description of the product	|
|	ProductId	|	string	|	256	|	No	|	The unique Id of the product	|
|	ProductReservationNumber	|	string	|	256	|	No	|	Product reservation number	|
|	ProductReservationQuantity	|	decimal	|		|	No	|	Product reservation quantity	|
|	ReferenceOrderQuantity	|	decimal	|		|	No	|	Reference order quantity for the delivery order line	|
|	SalesLineId	|	string	|	256	|	No	|	Sales order line id of the sales order	|
|	SalesOrderLineNumber	|	string	|	256	|	No	|	Sales order line number of the sales order	|
|	SalesUnitOfMeasure	|	string	|	256	|	No	|	Sales unit of measure of the delivery order line quantity	|
|	UoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
