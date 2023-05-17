---
title: CarrierRouteAccountTariffSchedule
description: This article provides information about the CarrierRouteAccountTariffSchedule entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **CarrierRouteAccountTariffSchedule**

Carrier route account tariff schedule refers to the published rates and fees charged by shipping carriers for their services. These tariffs outline the costs associated with various shipping options, such as domestic or international shipping, different delivery speeds, origin and destination (carrier route id) package sizes, and additional services like tracking or insurance.

The tariffs usually include:

**Base Rates**: The standard rates charged for shipping based on factors like package weight, dimensions, and destination.

**Surcharges**: Additional fees applied under specific circumstances, such as fuel surcharges or residential delivery surcharges.

**Accessorial Charges**: Extra services like signature confirmation, insurance, or special handling that incur additional fees.

**Specialized Services**: Tariffs may outline rates for specialized services like overnight or express delivery, international shipping, or freight services.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountId	|	string	|	36	|	No	|	The unique Id of the account	|
|	AccountNumber	|	string	|	256	|	Yes	|	Number or code for the account to quickly search and identify the account in system views.	|
|	AccountTypeCode	|	string	|	256	|	No	|	Account type code indicates the type of account. An account could be Vendor, Customer etc.	|
|	CargoTypeId	|	string	|	36	|	No	|	Unique Id of the cargo type	|
|	CargoTypeNumber	|	string	|	256	|	Yes	|	Unique number of the cargo type	|
|	CarrierId	|	string	|	36	|	No	|	The unique Id of the carrier	|
|	CarrierNumber	|	string	|	256	|	Yes	|	The unique number of the carrier	|
|	CarrierRouteId	|	string	|	36	|	No	|	The unique Id of the carrier route	|
|	CarrierRouteNumber	|	string	|	256	|	Yes	|	The unique number of the carrier route	|
|	ContractId	|	string	|	36	|	No	|	Unique Id of the contract with carrier	|
|	ContractNumber	|	string	|	256	|	Yes	|	contract number with the carrier	|
|	InsuranceOptionId	|	string	|	36	|	No	|	Type of insurance option for this tariff schedule	|
|	InsuranceOptionNumber	|	string	|	256	|	Yes	|	Insurance option number of the tariff schedule	|
|	IsoCurrencyCode	|	string	|	256	|	Yes	|	Iso currency code for this tariff	|
|	MaximumUnitsOfMeasure	|	decimal	|		|	Yes	|	Maximum units of measure Id or number	|
|	MinimumShipmentChargeAmount	|	decimal	|		|	No	|	Minimum shipment charge amount	|
|	MinimumUnitsOfMeasure	|	decimal	|		|	Yes	|	Minimum units of measure Id or number	|
|	PackagingTypeId	|	string	|	36	|	No	|	Id of the packaging type. This is an auto generated internal number of D365 applications	|
|	PackagingTypeNumber	|	string	|	256	|	Yes	|	The number of the packaging type. This is an external number	|
|	PeriodEndTimeStamp	|	timestamp	|		|	No	|	Validity end date of this record	|
|	PeriodStartTimeStamp	|	timestamp	|		|	No	|	Validity start date of this record	|
|	PerUnitOfMeasureShippingChargeAmount	|	decimal	|		|	No	|	Shipping charges or amount, Price per unit of measure. Example $3 per mile	|
|	ShipmentMethodId	|	string	|	36	|	No	|	Unique Id of the shipment method for this tariff schedule	|
|	ShipmentMethodNumber	|	string	|	256	|	Yes	|	Unique number of the shipment method for this tariff schedule	|
|	ShipmentServiceTypeId	|	string	|	36	|	No	|	Type of shipment service	|
|	ShipmentServiceTypeNumber	|	string	|	256	|	No	|	Unique number of the shipment service type	|
|	ShipmentTermId	|	string	|	36	|	No	|	Unique Id of the freight or shipment terms	|
|	ShipmentTermNumber	|	string	|	256	|	Yes	|	Unique number of the freight or shipment terms	|
|	UnitOfMeasureId	|	string	|	36	|	No	|	Unit of measure Id	|
|	UnitOfMeasureNumber	|	string	|	256	|	Yes	|	Unit of measure number	|
