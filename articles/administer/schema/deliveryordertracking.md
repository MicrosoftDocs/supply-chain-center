---
title: DeliveryOrderTracking
description: This is about DeliveryOrderTracking entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **DeliveryOrderTracking**

Delivery order tracking entity refers to the tracking number associated with the delivery order.


|	EntityAttribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	CarrierDeliveryServiceId	|	string	|	36	|	No	|	Service Id of the carrier	|
|	CarrierId	|	string	|	36	|	No	|	Carrier Id of the delivery order	|
|	CarrierNumber	|	string	|	256	|	No	|	Carrier number for the delivery order 	|
|	CarrierServiceNumber	|	string	|	256	|	No	|	Service number of the carrier	|
|	DeliveryDate	|	date	|		|	No	|	Delivery date of the delivery order	|
|	DeliveryOrderDetailId	|	string	|	36	|	No	|	The unique Id of the delivery order line	|
|	DeliveryOrderId	|	string	|	36	|	No	|	Delivery order Id	|
|	DeliveryOrderLineNumber	|	string	|	256	|	No	|	Delivery order line number	|
|	DeliveryOrderNumber	|	string	|	256	|	No	|	Delivery order number	|
|	DeliveryOrderTrackingId	|	string	|	36	|	Yes	|	The unique tracking Id for the delivery order	|
|	DeliveryOrderTrackingNumber	|	string	|	256	|	Yes	|	The unique tracking number for the delivery order	|
|	DeliveryWindowBegin	|	timestamp	|		|	No	|	Start date of delivery window	|
|	DeliveryWindowEnd	|	timestamp	|		|	No	|	End date of delivery window	|
|	ExchangeRate	|	string	|	256	|	No	|	Exchange rate for this delivery order	|
|	InsuranceCost	|	decimal	|		|	No	|	Cost of insurance for the delivery order	|
|	InsuranceCostBase	|	decimal	|		|	No	|	Base cost of insurance for the delivery order	|
|	Name	|	string	|	256	|	No	|	Name of the delivery order tracking	|
|	PlannedDeliveryDate	|	date	|		|	No	|	Planned delivery date	|
|	ReturnOrderId	|	string	|	36	|	No	|	The unique Id of the return order	|
|	ReturnOrderNumber	|	string	|	256	|	No	|	The unique number of the return order	|
|	ShipDate	|	date	|		|	No	|	Ship date for the delivery order	|
|	ShipmentCost	|	decimal	|		|	No	|	Freight cost for the delivery order	|
|	ShipmentCostBase	|	decimal	|		|	No	|	Base freight cost for the delivery order	|
|	ShipmentId	|	string	|	36	|	No	|	Shipment Id for the delivery order	|
|	ShipmentNumber	|	string	|	256	|	No	|	Shipment number for the delivery order	|
|	SurchageFeeBase	|	decimal	|		|	No	|	Base surcharge fee for the delivery order	|
|	SurchargeFee	|	decimal	|		|	No	|	Surcharge fee for the delivery order	|
|	Tax	|	decimal	|		|	No	|	Tax for the delivery order	|
|	TaxBase	|	decimal	|		|	No	|	Tax base of the delivery order	|
|	TrackingNumber	|	string	|	256	|	Yes	|	Tracking number of the delivery order	|
|	TrackingServiceStatus	|	string	|	4000	|	No	|	Status of tracking service	|
|	TrackingStatus	|	string	|	4000	|	No	|	Status of tracking for the delivery order	|
|	TrackingURL	|	string	|	256	|	No	|	URL for shipment or freight tracking	|
