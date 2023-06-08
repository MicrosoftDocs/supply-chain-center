---
title: OrderReturns
description: This article provides information about the OrderReturns entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **OrderReturns**

The order returns entity refers to the returns order. The returns order contains the ship to address, return order id and RMA number for returns.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountNumber	|	string	|	36	|	No	|	Number or code for the account to quickly search and identify the account in system views.	|
|	AccountOrderReference	|	string	|	256	|	No	|	Order reference for the account	|
|	BillToCity	|	string	|	256	|	No	|	City of the bill to account	|
|	BillToContactName	|	string	|	256	|	No	|	Contact name of the bill to account	|
|	BillToCountry	|	string	|	256	|	No	|	Country of bill to account	|
|	BillToFax	|	string	|	256	|	No	|	Fax number of the bill to account	|
|	BillToLine1	|	string	|	256	|	No	|	Address line 1 of the bill to account	|
|	BillToLine2	|	string	|	256	|	No	|	Address line 2 of the bill to account	|
|	BillToLine3	|	string	|	256	|	No	|	Address line 3 of the bill to account	|
|	BillToName	|	string	|	256	|	No	|	Name of the bill to account	|
|	BillToPostalCode	|	string	|	256	|	No	|	Postal code of the bill to account	|
|	BillToStateOrProvince	|	string	|	256	|	No	|	State or province of the bill to account	|
|	BillToTelephone	|	string	|	256	|	No	|	Telephone of the bill to account	|
|	Company	|	string	|	256	|	No	|	Company of the returns order	|
|	ContactPerson	|	string	|	256	|	No	|	Contact person for the returns order	|
|	CustomerRequisitionNumber	|	string	|	256	|	No	|	Account requisition number	|
|	DateInitiated	|	date	|		|	No	|	Returns initiated date	|
|	DateReturnBy	|	date	|		|	No	|	Return by date	|
|	DefaultReturnSite	|	string	|	256	|	No	|	Default returns site	|
|	DefaultReturnWarehouseId	|	string	|	36	|	No	|	Default returns warehouse Id	|
|	DefaultReturnWarehouseNumber	|	string	|	256	|	No	|	Default returns warehouse number	|
|	Description	|	string	|	4000	|	No	|	Description of the returns order	|
|	DropOffCity	|	string	|	256	|	No	|	Drop off City	|
|	DropOffCountry	|	string	|	256	|	No	|	Drop off country	|
|	DropOffLine1	|	string	|	256	|	No	|	Drop off line 1	|
|	DropOffLine2	|	string	|	256	|	No	|	Drop off line 2	|
|	DropOffLine3	|	string	|	256	|	No	|	Drop off line 3	|
|	DropOffLocationName	|	string	|	256	|	No	|	Drop off location name	|
|	DropOffPostalCode	|	string	|	256	|	No	|	Drop off postal code	|
|	DropOffStateOrProvince	|	string	|	256	|	No	|	Drop off state or province	|
|	EmailAddress	|	string	|	256	|	No	|	Email address	|
|	ExchangeRate	|	string	|	256	|	No	|	Exchange rate for this returns order	|
|	FormattedReturnAddress	|	string	|	256	|	No	|	Formatted return address	|
|	IsReadyToSync	|	boolean	|		|	No	|	Is ready to sync	|
|	IsReturnAddressOrderSpecific	|	boolean	|		|	No	|	Is this return address order specific	|
|	IsReturnAddressPrivate	|	boolean	|		|	No	|	Is this a private address	|
|	IsReturnProcessingStopped	|	boolean	|		|	No	|	Is this returns order processing stopped	|
|	Language	|	string	|	256	|	No	|	Language of the returns order	|
|	Name	|	string	|	256	|	No	|	Name of the returns order	|
|	OrderReturnsId	|	string	|	36	|	Yes	|	The unique ID of the returns order	|
|	OrderReturnsNumber	|	string	|	256	|	Yes	|	The unique number of the returns order	|
|	OrderSourceId	|	string	|	36	|	No	|	Order source Id	|
|	OrderSourceNumber	|	string	|	256	|	No	|	Order source number	|
|	ReturnActionNumber	|	string	|	256	|	No	|	Return action number	|
|	ReturnAddress1	|	string	|	256	|	No	|	Street address 1 of the returns address	|
|	ReturnAddress2	|	string	|	256	|	No	|	Street address 2 of the returns address	|
|	ReturnAddressCity	|	string	|	256	|	No	|	City of the returns address	|
|	ReturnAddressCountryRegionId	|	string	|	256	|	No	|	Country of the returns address	|
|	ReturnAddressCountyId	|	string	|	256	|	No	|	County ID of the returns address	|
|	ReturnAddressDescription	|	string	|	4000	|	No	|	Description of the returns address	|
|	ReturnAddressDistrictName	|	string	|	256	|	No	|	District name of the returns address	|
|	ReturnAddressDunsNumber	|	string	|	256	|	No	|	Duns number of the returns address	|
|	ReturnAddressLatitude	|	decimal	|		|	No	|	Latitude of the location	|
|	ReturnAddressLocationId	|	string	|	36	|	No	|	Location ID of the return address	|
|	ReturnAddressLongitude	|	decimal	|		|	No	|	Longitude of the location	|
|	ReturnAddressName	|	string	|	256	|	No	|	Name on the return address	|
|	ReturnAddressPostalCode	|	string	|	256	|	No	|	Postal code of the return address	|
|	ReturnAddressPostBox	|	string	|	256	|	No	|	Post box of the return address	|
|	ReturnAddressStateOrProvince	|	string	|	256	|	No	|	Return address state or province	|
|	ReturnAddressTimezone	|	string	|	256	|	No	|	Time zone of the return address	|
|	ReturnDeadline	|	string	|	256	|	No	|	Deadline for returns order	|
|	ReturnOrderStatus	|	string	|	4000	|	No	|	Status of returns order	|
|	ReturnReasonId	|	string	|	36	|	No	|	Return reason ID for the returns order	|
|	ReturnReasonNumber	|	string	|	256	|	No	|	Return reason number for the returns order	|
|	RMANumber	|	string	|	256	|	No	|	RMA number for sales order returns	|
|	RMAStatus	|	string	|	4000	|	No	|	Status of RMA	|
|	SalesOrderNumber	|	string	|	256	|	No	|	Sales order number	|
|	SalesOrderOriginNumber	|	string	|	256	|	No	|	Origin number for sales order returns	|
|	SalesOriginOrderId	|	string	|	36	|	No	|	Origin order ID for sales order returns	|
|	TotalChargesAmount	|	decimal	|		|	No	|	Total amount for returns order	|
|	TotalChargesAmountBase	|	decimal	|		|	No	|	Total base charges amount of the returns order	|
|	TotalDetailRefundAmount	|	decimal	|		|	No	|	Total detail refund amount of the returns order	|
|	TotalDetailRefundAmountBase	|	decimal	|		|	No	|	Total base detail refund amount of the returns order	|
|	TotalDiscountAmount	|	decimal	|		|	No	|	Total discount amount of the returns order	|
|	TotalDiscountAmountBase	|	decimal	|		|	No	|	Total base discount amount of the returns order	|
|	TotalRefundAmount	|	decimal	|		|	No	|	Total refund amount of the returns order	|
|	TotalRefundAmountBase	|	decimal	|		|	No	|	Total base refund amount of the returns order	|
|	TotalShipmentAmount	|	decimal	|		|	No	|	Total freight amount of the returns order	|
|	TotalShipmentAmountBase	|	decimal	|		|	No	|	Total base freight amount of the returns order	|
|	TotalTax	|	string	|	256	|	No	|	Total tax of the returns order	|
|	TotalTaxBase	|	string	|	256	|	No	|	Tax base of the returns order	|
|	TransactionCurrencyId	|	string	|	256	|	No	|	The transaction currency of the returns order	|
