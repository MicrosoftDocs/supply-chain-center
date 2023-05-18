---
title: GoodsReceiptLine
description: This article provides information about the GoodsReceiptLine entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **GoodsReceiptLine**

Goods receipt line entity is the details of the goods receipt document. Goods receipt line includes information such as the date and time of receipt, the quantity and description of the received goods, the supplier or vendor from whom the goods were obtained, and any relevant purchase order or transfer order or other reference numbers.

Goods receipt line entity helps ensure transparency and accuracy in the supply chain by providing a documented record of the goods received, which aids in maintaining efficient inventory control and smooth business operations.
 

|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AssociateToWarehouseId	|	string	|	36	|	No	|	#N/A	|
|	AssociateToWarehouseNumber	|	string	|	256	|	No	|	#N/A	|
|	Company	|	string	|	256	|	No	|	#N/A	|
|	DeliveryAddressCountryRegionId	|	string	|	256	|	No	|	#N/A	|
|	DeliveryAddressCountyId	|	string	|	256	|	No	|	#N/A	|
|	DeliveryAddressStateId	|	string	|	256	|	No	|	#N/A	|
|	ExpectedDeliveryDate	|	date	|		|	No	|	#N/A	|
|	ExternalItemNumber	|	string	|	256	|	No	|	#N/A	|
|	GoodsReceiptId	|	string	|	36	|	No	|	#N/A	|
|	GoodsReceiptLineId	|	string	|	36	|	Yes	|	#N/A	|
|	GoodsReceiptLineNumber	|	string	|	256	|	Yes	|	#N/A	|
|	GoodsReceiptNumber	|	string	|	256	|	No	|	#N/A	|
|	ItemBatchNumber	|	string	|	256	|	No	|	#N/A	|
|	ItemSerialNumber	|	string	|	256	|	No	|	#N/A	|
|	ItemSku	|	string	|	256	|	No	|	#N/A	|
|	LineDescription	|	string	|	4000	|	No	|	#N/A	|
|	Name	|	string	|	256	|	No	|	#N/A	|
|	OrderedPurchaseQuantity	|	decimal	|		|	No	|	#N/A	|
|	ProcurementProductCategory	|	string	|	256	|	No	|	#N/A	|
|	ProductId	|	string	|	36	|	No	|	#N/A	|
|	ProductReceiptDate	|	date	|		|	No	|	#N/A	|
|	ProductReceiptNumber	|	string	|	256	|	No	|	#N/A	|
|	PurchaseOrderId	|	string	|	36	|	No	|	#N/A	|
|	PurchaseOrderLineId	|	string	|	36	|	No	|	#N/A	|
|	PurchaseOrderLineNumber	|	string	|	256	|	No	|	#N/A	|
|	PurchaseOrderNumber	|	string	|	256	|	No	|	#N/A	|
|	PurchasePersonnel	|	string	|	256	|	No	|	#N/A	|
|	PurchaseUnitSymbol	|	string	|	256	|	No	|	#N/A	|
|	Quantity	|	decimal	|		|	No	|	#N/A	|
|	ReceivedInventoryQuantity	|	decimal	|		|	No	|	#N/A	|
|	ReceivedInventoryStatusId	|	string	|	256	|	No	|	#N/A	|
|	ReceivingSiteId	|	string	|	256	|	No	|	#N/A	|
|	ReceivingWarehouseLocationId	|	string	|	36	|	No	|	#N/A	|
|	ReceivingWarehouseLocationNumber	|	string	|	256	|	No	|	#N/A	|
|	RecordId	|	string	|	256	|	No	|	#N/A	|
|	RemainingInventoryQuantity	|	decimal	|		|	No	|	#N/A	|
|	RemainingPurchaseQuantity	|	decimal	|		|	No	|	#N/A	|
