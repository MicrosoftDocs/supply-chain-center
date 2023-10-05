---
title: ShipmentQuote
description: This article provides information about the ShipmentQuote entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **ShipmentQuote**

[!INCLUDE[banner](../../includes/banner.md)]

The shipment quote entity refers to the freight quote by the shipping carrier.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	BookingAmount	|	decimal	|		|	No	|	Booking amount	|
|	BookingAmountBase	|	decimal	|		|	No	|	Base amount of the booking	|
|	BookingId	|	string	|	256	|	No	|	Booking reference of the shipment quote	|
|	ExchangeRate	|	string	|	256	|	No	|	Exchange rate applied for the quote	|
|	Fulfillment	|	string	|	256	|	No	|	Fulfillment of the shipment quote	|
|	Name	|	string	|	256	|	No	|	Name of the shipment quote	|
|	QuoteAmount	|	decimal	|		|	No	|	Amount quoted in the quote	|
|	QuoteAmountBase	|	decimal	|		|	No	|	Base amount of the quote	|
|	QuoteId	|	string	|	256	|	Yes	|	The unique ID of the quote	|
|	ShipmentQuoteId	|	string	|	36	|	Yes	|	The unique ID of the shipment quote. 	|
|	ShipmentQuoteNumber	|	string	|	256	|	Yes	|	The unique number of the shipment quote	|
|	TransactionCurrencyId	|	string	|	256	|	No	|	Currency of the shipment quote	|
