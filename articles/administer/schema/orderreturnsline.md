---
title: OrderReturnsLine
description: This article provides information about the OrderReturnsLine entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **OrderReturnsLine**

[!INCLUDE[banner](../../includes/banner.md)]

The order returns line entity refers to the details of the returns order. The return order line typically contains the product that is being returned, quantity and reference order against which this return is initiated. 


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	ActualArrivalDate	|	date	|		|	No	|	Actual arrival date	|
|	AdditionalComments	|	string	|	256	|	No	|	Additional comments	|
|	ClosedDate	|	date	|		|	No	|	Closed date	|
|	Company	|	string	|	256	|	No	|	Company of the returns order	|
|	DeliveryOrderSource	|	string	|	256	|	No	|	Source of delivery order	|
|	Description	|	string	|	4000	|	No	|	Description	|
|	ExchangeRate	|	string	|	256	|	No	|	Exchange rate for this returns order	|
|	ExpectedArrivalDate	|	date	|		|	No	|	Expected arrival date	|
|	FormattedReturnAddress	|	string	|	256	|	No	|	Formatted return address	|
|	IsProductOverridden	|	boolean	|		|	No	|	Is product overridden	|
|	IsReadyToSync	|	boolean	|		|	No	|	Is ready to sync	|
|	IsReturnAddressOrderSpecific	|	boolean	|		|	No	|	Is this address specific to returns order	|
|	IsReturnAddressPrivate	|	boolean	|		|	No	|	Is this a private address	|
|	ItemSku	|	string	|	256	|	No	|	Stock keeping unit of the product	|
|	LineItemNumber	|	string	|	256	|	No	|	Line item number of the returns	|
|	LineStatus	|	string	|	4000	|	No	|	Status of the returns line	|
|	Name	|	string	|	256	|	No	|	Name of the returns line	|
|	OrderReturnsId	|	string	|	36	|	No	|	Order returns Id	|
|	OrderReturnsLineId	|	string	|	36	|	Yes	|	Line ID of the returns order	|
|	OrderReturnsLineNumber	|	string	|	256	|	Yes	|	Line number of the returns order	|
|	OrderReturnsNumber	|	string	|	256	|	No	|	Order returns number	|
|	OriginalOrderId	|	string	|	256	|	No	|	Original order Id	|
|	OriginalOrderLineId	|	string	|	256	|	No	|	Original order line Id	|
|	OriginalSalesOrderLineNumber	|	string	|	256	|	No	|	Origin sales order line number	|
|	OriginalSalesOrderNumber	|	string	|	256	|	No	|	Origin sales order number	|
|	PricePerUnit	|	decimal	|		|	No	|	Price per unit	|
|	PricePerUnitBase	|	decimal	|		|	No	|	Price per base unit	|
|	ProductDescription	|	string	|	4000	|	No	|	Description of the product	|
|	ProductId	|	string	|	36	|	No	|	Product ID 	|
|	ProductName	|	string	|	256	|	No	|	Name of the product of the returns order line	|
|	ProductQualityCode	|	string	|	256	|	No	|	Product quality code	|
|	ProductTypeCode	|	string	|	256	|	No	|	Product type code	|
|	Quantity	|	decimal	|		|	No	|	Returns quantity	|
|	RefundAmount	|	decimal	|		|	No	|	Refund amount	|
|	RefundAmountBase	|	decimal	|		|	No	|	Refund amount base	|
|	RefundBaseAmount	|	decimal	|		|	No	|	Refund base amount	|
|	RefundBaseAmountBase	|	decimal	|		|	No	|	Refund base amount base	|
|	RefundChargesAmount	|	decimal	|		|	No	|	Refund charges amount	|
|	RefundChargesAmountBase	|	decimal	|		|	No	|	Base amount for refund charges	|
|	RefundDiscountAmount	|	decimal	|		|	No	|	Refund discount amount	|
|	RefundDiscountAmountBase	|	decimal	|		|	No	|	Base amount for refund discount	|
|	ReplaceOrderId	|	string	|	36	|	No	|	Replace order Id	|
|	ReplaceOrderLineId	|	string	|	36	|	No	|	Replace order line Id	|
|	ReplaceOrderLineNumber	|	string	|	256	|	No	|	Replace order line number	|
|	ReplaceOrderNumber	|	string	|	256	|	No	|	Replace order number	|
|	ReturnActionId	|	string	|	36	|	No	|	Return action Id	|
|	ReturnActionNumber	|	string	|	256	|	No	|	Return action number	|
|	ReturnAddress1	|	string	|	256	|	No	|	Street address 1 of the returns address	|
|	ReturnAddress2	|	string	|	256	|	No	|	Street address 2 of the returns address	|
|	ReturnAddressCity	|	string	|	256	|	No	|	City of returns address	|
|	ReturnAddressCountryRegionId	|	string	|	256	|	No	|	Country of the returns address	|
|	ReturnAddressCountyId	|	string	|	256	|	No	|	County ID of the returns address	|
|	ReturnAddressDescription	|	string	|	4000	|	No	|	Description of the return address	|
|	ReturnAddressDistrictName	|	string	|	256	|	No	|	District name of the returns address	|
|	ReturnAddressDunsNumber	|	string	|	256	|	No	|	Duns number of the returns address	|
|	ReturnAddressLatitude	|	decimal	|		|	No	|	Latitude of the location	|
|	ReturnAddressLocationId	|	string	|	256	|	No	|	Location ID of the return address	|
|	ReturnAddressLongitude	|	decimal	|		|	No	|	Longitude of the location	|
|	ReturnAddressName	|	string	|	256	|	No	|	Name of the return address	|
|	ReturnAddressPostalCode	|	string	|	256	|	No	|	Postal code of the return address	|
|	ReturnAddressPostBox	|	string	|	256	|	No	|	Post box of the return address	|
|	ReturnAddressStateOrProvince	|	string	|	256	|	No	|	State or province of the return address	|
|	ReturnAddressTimezone	|	string	|	256	|	No	|	Time zone of the return address	|
|	ReturnedQuantity	|	decimal	|		|	No	|	Returns quantity	|
|	ReturnInventoryLotId	|	string	|	256	|	No	|	Lot ID of the returns order inventory	|
|	ReturnReason	|	string	|	4000	|	No	|	Return reason	|
|	ReturnReasonV2	|	string	|	4000	|	No	|	Return reason v2	|
|	ReturnSite	|	string	|	256	|	No	|	Returns site	|
|	ReturnWarehouseId	|	string	|	36	|	No	|	Returns warehouse Id	|
|	ReturnWarehouseNumber	|	string	|	256	|	No	|	Returns warehouse number	|
|	RMANumber	|	string	|	256	|	No	|	RMA number for sales order returns line	|
|	Tax	|	string	|	256	|	No	|	Tax of the returns order line	|
|	TaxBase	|	string	|	256	|	No	|	Tax base of the returns order line	|
|	TrackingNumber	|	string	|	256	|	No	|	Tracking number of the returns order	|
|	TransactionCurrencyId	|	string	|	256	|	No	|	Transaction currency of the returns order	|
|	UoMId	|	string	|	36	|	No	|	Unit of measure Id	|
|	UoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
