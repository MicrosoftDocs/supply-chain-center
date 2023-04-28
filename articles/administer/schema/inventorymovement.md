---
title: InventoryMovement
description: This is about InventoryMovement entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **InventoryMovement**

|	EntityAttribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AllocatedToWorkOrder	|	string	|	256	|	No	|	Allocated to work order for the inventory movement	|
|	FromWarehouseId	|	string	|	36	|	No	|	The unique identifier of a Warehouse.	|
|	FromWarehouseNumber	|	string	|	256	|	No	|	From warehouse number for the inventory movement	|
|	GoodsReceiptLineId	|	string	|	36	|	No	|	Goods receipt line id for the inventory movement	|
|	GoodsReceiptLineNumber	|	string	|	256	|	No	|	Goods receipt line number for the inventory movement	|
|	InventoryAdjustmentProduct	|	string	|	256	|	No	|	Inventory adjustment product for the inventory movement	|
|	InventoryMovementId	|	string	|	36	|	Yes	|	The unique identifier of a inventory movement transaction.	|
|	InventoryMovementNumber	|	string	|	256	|	Yes	|	The unique number of the inventory movement transaction	|
|	InventoryTransactionClassId	|	string	|	256	|	No	|	The unique identifier of the Inventory Transaction Class.	|
|	InventoryTransactionStatusId	|	string	|	256	|	No	|	The unique identifier of an Inventory Transaction Status.	|
|	ItemSku	|	string	|	256	|	No	|	Item sku for the inventory movement	|
|	JournalType	|	string	|	256	|	No	|	Journal type for the inventory movement	|
|	OriginatingJournal	|	string	|	256	|	No	|	Originating journal for the inventory movement	|
|	ProductId	|	string	|	36	|	No	|	Product id for the inventory movement	|
|	PurchaseOrderId	|	string	|	36	|	No	|	Purchase order id for the inventory movement	|
|	PurchaseOrderLineId	|	string	|	36	|	No	|	Purchase order line id for the inventory movement	|
|	PurchaseOrderLineNumber	|	string	|	256	|	No	|	Purchase order line number for the inventory movement	|
|	PurchaseOrderNumber	|	string	|	256	|	No	|	Purchase order number for the inventory movement	|
|	Quantity	|	decimal	|		|	No	|	Quantity for the inventory movement	|
|	Reversal	|	string	|	256	|	No	|	Reversal for the inventory movement	|
|	RMAreceiptproduct	|	string	|	256	|	No	|	RMAreceiptproduct for the inventory movement	|
|	ToWarehouseId	|	string	|	36	|	No	|	The unique identifier of a Warehouse.	|
|	ToWarehouseNumber	|	string	|	256	|	No	|	To warehouse number for the inventory movement	|
|	TransactionCompletedTimestamp	|	timestamp	|		|	No	|	The timestamp that the Item Inventory Location Transaction was completed.	|
|	TransactionRequestedTimestamp	|	timestamp	|		|	No	|	The timestamp that the Item Inventory Location Transaction was requested.	|
|	TransactionType	|	string	|	256	|	No	|	Transaction type for the inventory movement	|
|	UoMId	|	string	|	36	|	No	|	Unit of measure Id	|
|	UoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
|	WorkOrderProduct	|	string	|	256	|	No	|	Work order product for the inventory movement	|
