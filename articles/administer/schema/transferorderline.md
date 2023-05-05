---
title: TransferOrderLine
description: This is about TransferOrderLine entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **TransferOrderLine**

A transfer order entity typically refers to a document or record that facilitates the movement of goods or products from one location to another within an organization. It is commonly used in logistics and supply chain management systems to initiate and track the transfer of inventory products.

A transfer order entity contains information such as the source location (where the goods are currently located), the destination location (where the goods should be transferred to), the quantity of items to be transferred, and any other relevant details specific to the organization's requirements.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AllowedOverDeliveryPercentage	|	string	|	256	|	No	|	Allowed over delivery percentage	|
|	AllowedUnderDeliveryPercentage	|	string	|	256	|	No	|	Allowed under weight percentage	|
|	CatchWeightQuantity	|	decimal	|		|	No	|	Catch weight quantity	|
|	CatchWeightQuantityReceived	|	decimal	|		|	No	|	Catch weight of the quantity received	|
|	CatchWeightQuantityScrapped	|	decimal	|		|	No	|	Catch weight of the quantity scrapped	|
|	CatchWeightQuantityShipped	|	decimal	|		|	No	|	Catch weight of the quantity shipped	|
|	Company	|	string	|	256	|	No	|	Company	|
|	ItemSku	|	string	|	256	|	No	|	Stock keeping unit of the product	|
|	LineOrder	|	string	|	256	|	Yes	|	Line order	|
|	LineStatus	|	string	|	4000	|	No	|	Transfer order line status	|
|	Name	|	string	|	256	|	No	|	Name of the product	|
|	ProductId	|	string	|	36	|	No	|	Product Id	|
|	Quantity	|	decimal	|		|	No	|	Transfer order quantity	|
|	QuantityReceived	|	decimal	|		|	No	|	Received quantity	|
|	QuantityScrapped	|	decimal	|		|	No	|	Scrapped quantity 	|
|	QuantityShipped	|	decimal	|		|	No	|	Shipped quantity of the transfer order line	|
|	ReceiveDate	|	date	|		|	No	|	Receive date of the transfer order	|
|	ShipDate	|	date	|		|	No	|	Ship date of the transfer order	|
|	ShippingSite	|	string	|	256	|	No	|	Shipping site of the transfer order line	|
|	ShippingWarehouseId	|	string	|	36	|	No	|	Shipping warehouse Id of the transfer order line	|
|	ShippingWarehouseNumber	|	string	|	256	|	No	|	Shipping warehouse number of the transfer order line	|
|	TransferOrderId	|	string	|	36	|	No	|	Unique Id of the transfer order	|
|	TransferOrderLineId	|	string	|	36	|	Yes	|	Transfer Order Line Id	|
|	TransferOrderLineNumber	|	string	|	256	|	Yes	|	Transfer order line number	|
|	TransferOrderNumber	|	string	|	256	|	Yes	|	Transfer order number	|
|	UnitId	|	string	|	256	|	No	|	Unit Id of the transfer order line	|
|	UnitNumber	|	string	|	256	|	No	|	Unit number of thetransfer order line	|
