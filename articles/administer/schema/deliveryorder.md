---
title: DeliveryOrder
description: This is about DeliveryOrder entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **DeliveryOrder**

A delivery order refers to the document created or issued by a supplier to the customer acknowledging delivery of goods or services. It serves as an official confirmation and instruction for the shipment of products or provision of services to a specified location.

A delivery order typically contains the following information:

Order details: This includes the order number, date, and any specific reference numbers or codes associated with the order.

Supplier information: The name, address, and contact details of the supplier or shipping company responsible for delivering the goods or services.

Customer information: The name, address, and contact details of the customer or recipient who requested the delivery.

Delivery instructions: Any specific instructions or requirements for the delivery, such as the delivery date, preferred time, or special handling instructions.

Billing and payment details: If applicable, the delivery order may include information regarding the payment terms, such as the total amount due, payment method, and any other relevant billing details.

Terms and conditions: This section outlines the terms and conditions of the delivery, including liability, warranties, and any other relevant contractual agreements.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountNumber	|	string	|	256	|	No	|	Number or code for the account to quickly search and identify the account in system views.	|
|	AccountTypeCode	|	string	|	256	|	No	|	Account type code indicates the type of account. An account could be Vendor, Customer etc.	|
|	CustomerId	|	string	|	256	|	No	|	Account Id of the account for which this delivery order is created	|
|	DeliveryNotes	|	string	|	4000	|	No	|	Notes or comments for this delivery order	|
|	DeliveryOrderNumber	|	string	|	256	|	Yes	|	The unique number of the delivery order	|
|	DeliveryOrderNumberId	|	string	|	36	|	Yes	|	The unique Id of the delivery order	|
|	DeliveryOrderPlan	|	string	|	256	|	No	|	Plan for this delivery order	|
|	DeliveryOrderSourceId	|	string	|	36	|	No	|	Source Id for this delivery order	|
|	DeliveryOrderSourceNumber	|	string	|	256	|	No	|	Source number for this delivery order	|
|	DeliveryOrderWillCall	|	string	|	256	|	No	|	Delivery order will call	|
|	EmailAddress	|	string	|	256	|	No	|	Email address for the delivery order	|
|	ExchangeRate	|	string	|	256	|	No	|	Exchange rate for this delivery order	|
|	FulfillmentPlanNumber	|	string	|	256	|	No	|	Fulfillment plan number for this delivery order	|
|	OrderSourceId	|	string	|	36	|	No	|	Order source Id	|
|	OrderSourceNumber	|	string	|	256	|	No	|	Order source number	|
|	PlannedDeliveryDate	|	date	|		|	No	|	Planned delivery date	|
|	PlannedShippingDate	|	date	|		|	No	|	Planned shipping date	|
|	SalesOrderOriginId	|	string	|	36	|	No	|	Sales order origin Id for this delivery order	|
|	SalesOrderOriginNumber	|	string	|	256	|	No	|	Sales order origin number for this delivery order	|
|	ShipmentBookingAmount	|	decimal	|		|	No	|	Freight booking amount for the delivery order	|
|	ShipmentBookingAmountBase	|	decimal	|		|	No	|	Base amount of shipment booking for this delivery order	|
|	ShippingQuoteAmount	|	decimal	|		|	No	|	Amount for freight quote	|
|	ShippingQuoteAmountBase	|	decimal	|		|	No	|	Base amount for freight quote	|
|	ShipToCity	|	string	|	256	|	No	|	Ship to city	|
|	ShipToContactName	|	string	|	256	|	No	|	Ship to contact name	|
|	ShipToCountry	|	string	|	256	|	No	|	Ship to country	|
|	ShipToFax	|	string	|	256	|	No	|	Ship to fax number	|
|	ShipToLine1	|	string	|	256	|	No	|	Ship to line1	|
|	ShipToLine2	|	string	|	256	|	No	|	Ship to line2	|
|	ShipToLine3	|	string	|	256	|	No	|	Ship to line3	|
|	ShipToLocationId	|	string	|	256	|	No	|	Ship to location Id	|
|	ShipToLocationNumber	|	string	|	256	|	No	|	Ship to location number	|
|	ShipToPostalCode	|	string	|	256	|	No	|	Ship to postal code	|
|	ShipToState	|	string	|	256	|	No	|	Ship to state	|
|	ShipToTelephone	|	string	|	256	|	No	|	Ship to telephone	|
