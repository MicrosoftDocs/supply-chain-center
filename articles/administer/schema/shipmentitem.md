---
title: ShipmentItem
description: This is about ShipmentItem entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **ShipmentItem**

|	EntityAttribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	ActualGrossShipmentWeight	|	decimal	|		|	No	|	The weight of the shipment including all packing, blocking, platforms, special bracing, etc., if required. (includes weight of unit load device, when applicable.)	|
|	CargoTypeId	|	string	|	256	|	No	|	The unique identifier of a Cargo Type.	|
|	CargoTypeNumber	|	string	|	256	|	No	|	The cargo type number of the shipment	|
|	DangerousGoodsIndicator	|	string	|	256	|	No	|	Items capable of presenting a risk to the health or safety of people or property when shipped.

The term used by I.M.C.O. for hazardous materials which are capable of posing a significant risk to health, safety or property while being transported.

The United Nation's official term for Hazardous Materials.  Articles or substances which are capable of posing a significant risk to the health or safety of the general public when transported by air and which are classified according to the most current editions of the ICAO Technical Instructions for the Safe Transport of Dangerous Goods by Air and the IATA Dangerous Goods Regulations.  See Hazardous Materials.	|
|	HandlingInstructions	|	string	|	256	|	No	|	Written instructions provided by the shipper/manufacturer and designed to
ensure proper handling of the cargo. This can be in the form of marks (see Cautionary Markings) on the cargo or packaging itself or in a separate document such as the bill of lading.	|
|	HazardousMaterialHazmatIndicator	|	string	|	256	|	No	|	Hazardous materials (Hazmat)    The U.S. Government's official term for Dangerous Goods.  Items of freight that are inherently harmful and classified under Title 49, Code of Federal Regulations (CFR).  Hazardous Materials may only be transported under certain conditions relative to packaging, quantity carried, airplane type, location on board the airplane, etc., and in conformance with applicable rules.  Also see Dangerous Goods.	|
|	IncotermId	|	string	|	256	|	No	|	The unique identifier of a Incoterm.	|
|	IncotermNumber	|	string	|	256	|	No	|	The Incoterms of the shipment 	|
|	ItemSku	|	string	|	256	|	No	|	The Stock Keeping Unit identifier, which is typically used for inventory-related activities.	|
|	OrderId	|	string	|	36	|	No	|	The unique number that identifies an Order.	|
|	OrderLineId	|	string	|	36	|	No	|	Order line Id on the shipment	|
|	PackingInstructions	|	string	|	256	|	No	|	Packing instructions for the associated shipped item.	|
|	PerItemDimensionalWeight	|	decimal	|		|	No	|	The per item dimensional weight, which is the conversion of the cubic space of a shipment into pounds. Commonly referred to as dim weight. The international term is volume weight.	|
|	PerItemPackagedWeight	|	decimal	|		|	No	|	The weight of each item packaged for shipment.	|
|	PerItemWeight	|	decimal	|		|	No	|	The individual or per item weight of an item.	|
|	ProductHeight	|	decimal	|		|	No	|	Height of the product on the shipment	|
|	ProductId	|	string	|	36	|	No	|	The product Id of the shipment 	|
|	ProductLength	|	decimal	|		|	No	|	Length of the product on the shipment	|
|	ProductNetWeight	|	decimal	|		|	No	|	Net weight of the product that is shipped in this shipment	|
|	ProductWidth	|	decimal	|		|	No	|	Product width of the product of the shipment item	|
|	PurchaseOrderId	|	string	|	36	|	No	|	The purchase order line Id on the shipment	|
|	PurchaseOrderLineId	|	string	|	36	|	No	|	The purchase order Id on the shipment	|
|	PurchaseOrderLineNumber	|	string	|	256	|	No	|	Purchase Order Line number that was shipped on this shipment	|
|	PurchaseOrderNumber	|	string	|	256	|	No	|	Purchase order that was shipped on this shipment	|
|	SalesOrderDetailLineNumber	|	string	|	256	|	No	|	Sales order line that was shipped on this shipment	|
|	SalesOrderNumber	|	string	|	256	|	No	|	Sales order that was shipped on this shipment	|
|	ShipmentId	|	string	|	36	|	No	|	The unique identifier of a Shipment.	|
|	ShipmentItemId	|	string	|	36	|	Yes	|	The unique Id of the shipment item	|
|	ShipmentItemNumber	|	string	|	256	|	Yes	|	The shipment line number.	|
|	ShipmentNumber	|	string	|	256	|	No	|	Shipment number for this shipment item	|
|	ShipmentProductNetWeight	|	decimal	|		|	No	|	Net weight of the product that is shipped in this shipment	|
|	ShippedProductQuantity	|	decimal	|		|	No	|	Shipped quantity of the shipment	|
|	TotalProductChargeableWeight	|	decimal	|		|	No	|	Total product chargeable weight	|
|	TotalProductDensity	|	string	|	256	|	No	|	Total product density of the shipment line	|
|	TotalQuantityDimensionalWeight	|	decimal	|		|	No	|	The dimensional weight of all items, which is the conversion of the cubic space of a shipment into pounds. Commonly referred to as dim weight. T	|
|	TotalQuantityPackagedWeight	|	decimal	|		|	No	|	The total weight of all items packaged for shipment.	|
|	TotalQuantityProductWeight	|	decimal	|		|	No	|	Total product weight of the shipment line	|
|	UoMId	|	string	|	36	|	No	|	Unit of measure Id	|
|	UoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
|	Volume	|	decimal	|		|	No	|	The volume of the shipment item.	|
|	VolumeUoMId	|	string	|	36	|	No	|	Unit of measure Id	|
|	VolumeUoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
|	WeightUoMId	|	string	|	36	|	No	|	Unit of measure Id	|
|	WeightUoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
