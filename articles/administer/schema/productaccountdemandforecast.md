---
title: ProductAccountDemandForecast
description: This article provides information about the ProductAccountDemandForecast entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **ProductAccountDemandForecast**

The product account demand forecast refers to forecast made for a specific time period for product estimated to be in demanded by an account.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountId	|	string	|	36	|	No	|	A unique identifier of an account. The account could be a customer or vendor etc. AccountId is an auto generated Id by Microsoft D365 or Supply chain center. 	|
|	AccountNumber	|	string	|	256	|	No	|	Number or code for the account to quickly search and identify the account in system views.	|
|	ForecastAccountType	|	string	|	256	|	No	|	Account type of forecast	|
|	FromWarehouseId	|	string	|	36	|	No	|	The unique Id of warehouse	|
|	FromWarehouseNumber	|	string	|	256	|	No	|	The origin warehouse number for the demand forecast	|
|	ItemSku	|	string	|	256	|	Yes	|	The stock keeping unit of product	|
|	ProductAccountDemandForecastEndDate	|	date	|		|	No	|	The validity or expirty date of this record	|
|	ProductAccountDemandForecastId	|	string	|	36	|	Yes	|	The unique Id of the demand forecast	|
|	ProductAccountDemandForecastName	|	string	|	256	|	No	|	Name of the demand forecast	|
|	ProductAccountDemandForecastNote	|	string	|	4000	|	No	|	Notes or comments for demand forecast	|
|	ProductAccountDemandForecastNumber	|	string	|	256	|	Yes	|	The unique number of the demand forecast	|
|	ProductAccountDemandForecastQuantity	|	decimal	|		|	No	|	Demand forecast quantity	|
|	ProductAccountDemandForecastStartDate	|	date	|		|	No	|	The beginning or effective start date of this record	|
|	ProductNumber	|	string	|	256	|	No	|	Product number for demand forecast	|
|	ToWarehouseId	|	string	|	36	|	No	|	The unique Id of the destination warehouse	|
|	ToWarehouseNumber	|	string	|	256	|	No	|	The destination warehouse number for the demand forecast	|
|	UoMId	|	string	|	36	|	No	|	Unit of measure Id	|
|	UoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
