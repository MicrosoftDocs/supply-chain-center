---
title: Product
description: This is about Product entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **Product**

The product entity refers to the stock keeping unit of the goods that is purchased or sold. The product entity contains the base unit of measure, weight, volume and product related. Base price and cost of the product. The product entity has references to product category and the product family. 


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AllowedSubscriptionFrequency	|	string	|	256	|	No	|	Subscription frequency allowed	|
|	CompanyId	|	string	|	256	|	No	|	Company of the product	|
|	CurrentCost	|	decimal	|		|	No	|	Current cost	|
|	CurrentCost_Base	|	decimal	|		|	No	|	Current base cost	|
|	DefaultUoMId	|	string	|	36	|	No	|	Unit of measure Id	|
|	DefaultUoMScheduleId	|	string	|	36	|	No	|	Default UoM schedule Id	|
|	DefaultUoMScheduleNumber	|	string	|	256	|	No	|	Default UoM schedule number	|
|	Description	|	string	|	4000	|	No	|	Description of the product	|
|	EntityImage	|	string	|	256	|	No	|	Image of the product	|
|	EntityImageId	|	string	|	256	|	No	|	Image id of the product	|
|	ExchangeRate	|	string	|	256	|	No	|	Exchange rate for this product	|
|	FieldServiceProductType	|	string	|	256	|	No	|	Product type from Field Service	|
|	GDPROptout	|	string	|	256	|	No	|	Opt out of GDPR	|
|	IsCatchWeight	|	boolean	|		|	No	|	Is catch weight	|
|	IsInventoryAllocation	|	boolean	|		|	No	|	Is on product allocation	|
|	IsKit	|	string	|	256	|	No	|	Is kit item (Bill of material)	|
|	IsStockedProduct	|	boolean	|		|	No	|	Is stocked product	|
|	IsStockItem	|	boolean	|		|	No	|	Is stock item	|
|	ItemNumber	|	string	|	256	|	No	|	Item number of the product	|
|	ItemSku	|	string	|	256	|	Yes	|	The Stock Keeping Unit identifier, which is typically used for inventory-related activities.	|
|	LaunchDate	|	date	|		|	No	|	Launch date	|
|	LotSizeQuantity	|	decimal	|		|	No	|	Lot size quantity	|
|	MinimumOrderQuantity	|	decimal	|		|	No	|	Minimum order quantity	|
|	Name	|	string	|	256	|	No	|	Name of the product	|
|	NumberOfDaysToReplace	|	integer	|		|	No	|	Number of days to replace	|
|	ParentProductId	|	string	|	256	|	No	|	Parent product Id	|
|	ParentProductNumber	|	string	|	256	|	No	|	Parent product number	|
|	PreorderEligible	|	string	|	256	|	No	|	Preorder eligible	|
|	Price	|	decimal	|		|	No	|	Price of the product	|
|	Price_Base	|	decimal	|		|	No	|	Base price of the product	|
|	PriceLevelId	|	string	|	256	|	No	|	The unique Id of the price level	|
|	ProcessId	|	string	|	256	|	No	|	Process Id	|
|	ProductCategoryHierarchyId	|	string	|	36	|	No	|	Product category hierarchy Id	|
|	ProductCategoryHierarchyNumber	|	string	|	256	|	No	|	Product category hierarchy number	|
|	ProductCategoryId	|	string	|	36	|	No	|	Product category Id of the product	|
|	ProductCategoryNumber	|	string	|	256	|	No	|	Product category number	|
|	ProductColor	|	string	|	256	|	No	|	Product color	|
|	ProductConfiguration	|	string	|	256	|	No	|	Product configuration	|
|	ProductId	|	string	|	256	|	Yes	|	The unique identifier of a Product.	|
|	ProductNumber	|	string	|	256	|	No	|	Product number	|
|	ProductSize	|	string	|	256	|	No	|	Prodcut size	|
|	ProductStructure	|	string	|	256	|	No	|	Product structure	|
|	ProductStyle	|	string	|	256	|	No	|	Product style 	|
|	ProductTypeCode	|	string	|	256	|	No	|	Product type code	|
|	ProductURL	|	string	|	256	|	No	|	URL for the product	|
|	QuantityDecimal	|	decimal	|		|	No	|	Decimal quantity	|
|	QuantityOnHand	|	decimal	|		|	No	|	Quantity on hand	|
|	SharedProductDetailId	|	string	|	256	|	No	|	Shared product detail Id	|
|	Size	|	string	|	256	|	No	|	Size of the product	|
|	StageId	|	string	|	256	|	No	|	Stage Id of the product	|
|	StandardCost	|	decimal	|		|	No	|	Standard cost of the product	|
|	StandardCost_Base	|	decimal	|		|	No	|	Standard base cost of the product	|
|	StockDimensionUnit	|	string	|	256	|	No	|	Product stock dimensional unit	|
|	StockGrossWeight	|	decimal	|		|	No	|	Product stock gross weight	|
|	StockHeight	|	decimal	|		|	No	|	Product stock height	|
|	StockLength	|	decimal	|		|	No	|	Product stock length	|
|	StockNetWeight	|	decimal	|		|	No	|	Stock net weight	|
|	StockVolume	|	decimal	|		|	No	|	Stock volume	|
|	StockWeight	|	decimal	|		|	No	|	Stock weight	|
|	StockWeightUnit	|	string	|	256	|	No	|	Stock weight unit	|
|	StockWidth	|	decimal	|		|	No	|	Stock width	|
|	SubjectId	|	string	|	256	|	No	|	Subject Id of the product	|
|	SupplierName	|	string	|	256	|	No	|	Name of the vendor or supplier	|
|	Taxable	|	string	|	256	|	No	|	Product taxable	|
|	TransactionCurrencyId	|	string	|	256	|	No	|	Transaction currency	|
|	TraversedPath	|	string	|	256	|	No	|	Traversed path of the product	|
|	UoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
|	ValidFromDate	|	date	|		|	No	|	The date by which this product becomes active. 	|
|	ValidToDate	|	date	|		|	No	|	The validity or expirty date of this record	|
|	VendorId	|	string	|	256	|	No	|	The unique Id of the vendor or supplier	|
|	VendorName	|	string	|	256	|	No	|	Name of the vendor or supplier	|
|	VendorNumber	|	string	|	256	|	No	|	The unique number of the vendor or supplier	|
|	VendorPartNumber	|	string	|	256	|	No	|	Vendor or supplier part number	|
