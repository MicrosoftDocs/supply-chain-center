---
title: TransferOrder
description: This is about TransferOrder entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **TransferOrder**

|	EntityAttribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	Company	|	string	|	256	|	No	|	Company	|
|	ContactEmail	|	string	|	256	|	No	|	contact email	|
|	ContactName	|	string	|	256	|	No	|	Contact name	|
|	DeliveryTerm	|	string	|	256	|	No	|	Delivery term	|
|	FormattedReceivingAddress	|	string	|	256	|	No	|	Formatted receiving address	|
|	FormattedShippingAddress	|	string	|	256	|	No	|	Formatted shipping address	|
|	FromWarehouseId	|	string	|	36	|	No	|	From warehouse Id of the transfer order	|
|	FromWarehouseNumber	|	string	|	256	|	No	|	From warehouse number of the transfer order	|
|	Name	|	string	|	256	|	No	|	Name of the transfer order	|
|	ReceiveDate	|	date	|		|	No	|	Receive date of the transfer order	|
|	ReceivingAddress1	|	string	|	256	|	No	|	Street address 1 of the receiving location	|
|	ReceivingAddress2	|	string	|	256	|	No	|	Street address 2 of the receiving location	|
|	ReceivingAddressCity	|	string	|	256	|	No	|	City of the receiving address	|
|	ReceivingAddressCountryRegionId	|	string	|	256	|	No	|	Country region Id of the receiving address	|
|	ReceivingAddressCountyId	|	string	|	256	|	No	|	County Id of the receiving address	|
|	ReceivingAddressDescription	|	string	|	4000	|	No	|	Description of the receiving address	|
|	ReceivingAddressDistrictName	|	string	|	256	|	No	|	District name of the receiving address	|
|	ReceivingAddressDunsNumber	|	string	|	256	|	No	|	Duns number of the receiving address	|
|	ReceivingAddressLatitude	|	decimal	|		|	No	|	Latitude of thereceiving address	|
|	ReceivingAddressLocationId	|	string	|	256	|	No	|	Location Id of the receiing addres	|
|	ReceivingAddressLongitude	|	decimal	|		|	No	|	Longitude of the receiving address	|
|	ReceivingAddressName	|	string	|	256	|	No	|	Name of the receiving address	|
|	ReceivingAddressPostalCode	|	string	|	256	|	No	|	Postal code of the receiving address	|
|	ReceivingAddressPostBox	|	string	|	256	|	No	|	Post box of the receiving address	|
|	ReceivingAddressStateOrProvince	|	string	|	256	|	No	|	State or province of the receiving address	|
|	ReceivingAddressTimezone	|	string	|	256	|	No	|	Time zone of the receiving address	|
|	ReceivingContactPersonnelNumber	|	string	|	256	|	No	|	Receiving contact personnel number	|
|	ShipDate	|	date	|		|	No	|	Ship date of the transfer order	|
|	ShippingAddress1	|	string	|	256	|	No	|	Shipping address 1 	|
|	ShippingAddress2	|	string	|	256	|	No	|	Shipping address 2	|
|	ShippingAddressCity	|	string	|	256	|	No	|	City of the shipping address	|
|	ShippingAddressCountryRegionId	|	string	|	256	|	No	|	Country of the shipping address	|
|	ShippingAddressCountyId	|	string	|	256	|	No	|	County Id of the shipping address	|
|	ShippingAddressDescription	|	string	|	4000	|	No	|	Description of the shipping address	|
|	ShippingAddressDistrictName	|	string	|	256	|	No	|	District name of the shipping address	|
|	ShippingAddressDunsNumber	|	string	|	256	|	No	|	Duns number of the shipping address	|
|	ShippingAddressLatitude	|	decimal	|		|	No	|	Latitude of the shipping address	|
|	ShippingAddressLocationId	|	string	|	256	|	No	|	Location Id of the shipping address	|
|	ShippingAddressLongitude	|	decimal	|		|	No	|	Longitude of the shipping address	|
|	ShippingAddressName	|	string	|	256	|	No	|	Name of the shipping address	|
|	ShippingAddressPostalCode	|	string	|	256	|	No	|	Postal code of the shipping address	|
|	ShippingAddressPostBox	|	string	|	256	|	No	|	Post box of the shipping address	|
|	ShippingAddressStateOrProvince	|	string	|	256	|	No	|	State or province of the shipping address	|
|	ShippingAddressTimezone	|	string	|	256	|	No	|	Time zone of the shipping address	|
|	ShippingContactPersonnelNumber	|	string	|	256	|	No	|	Shipping contact personnel number	|
|	ShippingService	|	string	|	256	|	No	|	Shipping service of the transfer order	|
|	ToWarehouseId	|	string	|	36	|	No	|	To warehouse Id of the transfer order	|
|	ToWarehouseNumber	|	string	|	256	|	No	|	To warehouse number of the transfer order	|
|	TransferOrderId	|	string	|	36	|	Yes	|	The unique Id of the transfer order	|
|	TransferOrderNumber	|	string	|	256	|	Yes	|	The unique number of the transfer order	|
|	TransferStatus	|	string	|	4000	|	No	|	Status of the transfer order	|
|	TransitWarehouseId	|	string	|	36	|	No	|	The Id of the transit warehouse	|
|	TransitWarehouseNumber	|	string	|	256	|	No	|	Transit warehouse number	|
