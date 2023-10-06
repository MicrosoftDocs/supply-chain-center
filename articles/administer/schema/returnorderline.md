---
title: ReturnOrderLine
description: This article provides information about the ReturnOrderLine entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **ReturnOrderLine**

[!INCLUDE[banner](../../includes/banner.md)]

The return order line entity refers to the details of the return order. The return order line contains the product that is returned with quantity and product quality code for returns.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	Carrier	|	string	|	256	|	No	|	Carrier of the return order line	|
|	CarrierDeliveryService	|	string	|	256	|	No	|	Carrier delivery service for return order line	|
|	CarrierNumber	|	string	|	256	|	No	|	The unique number of the carrier	|
|	CarrierServiceNumber	|	string	|	256	|	No	|	Carrier service number of the return service number	|
|	DeliveryOrderSource	|	string	|	256	|	No	|	Source for the deliveyr order	|
|	DeliveryOrderSourceNumber	|	string	|	256	|	No	|	Number of the delivery order source	|
|	InspectionCode	|	string	|	256	|	No	|	Inspection code for the return order line	|
|	IsProductOverridden	|	boolean	|		|	No	|	Is the product overridden	|
|	ItemSku	|	string	|	256	|	No	|	Product number of the return order	|
|	LineNumber	|	string	|	256	|	Yes	|	Line number of the returns order	|
|	OrderReturnsLineId	|	string	|	36	|	No	|	The unique line ID of the returns order	|
|	OrderReturnsLineNumber	|	string	|	256	|	No	|	The unique line number of the returns order	|
|	ProductCategory	|	string	|	256	|	No	|	Category of the product in return order	|
|	ProductCategoryNumber	|	string	|	256	|	No	|	Category number of the product in return order	|
|	ProductDescription	|	string	|	4000	|	No	|	Description of the product in return order	|
|	ProductId	|	string	|	256	|	No	|	The unique ID of the product in the return order	|
|	ProductQualityCode	|	string	|	256	|	No	|	Product quality code applied for the return order line	|
|	ReceivedDate	|	date	|		|	No	|	Received date	|
|	ReceivedQuantity	|	decimal	|		|	No	|	Received quantity	|
|	ReturnOrderId	|	string	|	36	|	No	|	The unique ID of the return order	|
|	ReturnOrderLineComments	|	string	|	256	|	No	|	Comments or notes for return order line	|
|	ReturnOrderLineId	|	string	|	36	|	Yes	|	The unique line ID of the return order	|
|	ReturnOrderLineNumber	|	string	|	256	|	Yes	|	The unique line number of the return order	|
|	ReturnOrderName	|	string	|	256	|	No	|	Name of the return order	|
|	ReturnOrderNumber	|	string	|	256	|	No	|	The unique number of the return order	|
|	ReturnOrderQuantity	|	decimal	|		|	No	|	The quantity that is being returned 	|
|	ReturnProductInventoryType	|	string	|	256	|	No	|	Inventory type of the return product	|
|	SerialOrupcNumber	|	string	|	256	|	No	|	The serial orupc number	|
|	UoMId	|	string	|	36	|	No	|	Unit of measure Id	|
|	UoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
