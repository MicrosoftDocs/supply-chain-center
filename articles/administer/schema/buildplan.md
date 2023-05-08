---
title: BuildPlan
description: This is about BuildPlan entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 005/05/2023
ms.custom: bap-template
---

# **BuildPlan**

A Build Plan is the break down, usually by a specific Item, to accomplish the Master Schedule or Material Requirements Planning (Demand)

The Master Schedule-Product Build is the product building plan that is used by manufacturers to build products or items via one or more individual Build Plans. A Master Schedule is a schedule to build several item(s) over a specific period. A Master Schedule may identify one or more Items to build. A Build Plan is the breakdown, usually by a specific Item, to accomplish the Master Schedule. A Run is the actual order to manufacture, or build a set number of Items on a date and/or time.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	BuildPlanCreateDate	|	date	|		|	No	|	The date the build plan was created	|
|	BuildPlanId	|	string	|	36	|	Yes	|	The unique identifier of a Build Plan.	|
|	BuildPlanName	|	string	|	256	|	No	|	The name of the Build Plan.	|
|	BuildPlanNumber	|	string	|	256	|	Yes	|	The unique identifier of a Build Plan.	|
|	BuildPlanPeriodEndDate	|	date	|		|	No	|	The validity or expirty date of this record	|
|	BuildPlanPeriodStartDate	|	date	|		|	No	|	The beginning or effective start date of this record	|
|	BuildPlanPriorityNumber	|	string	|	256	|	No	|	The priority of this build plan	|
|	BuildPlanProductUnitQuantity	|	decimal	|		|	No	|	Build plan quantity that was planned for this period or time horizon	|
|	BuildPlanStatus	|	string	|	4000	|	No	|	The status of the build plan	|
|	ItemSku	|	string	|	256	|	No	|	The Stock Keeping Unit identifier, which is typically used for inventory-related activities.	|
|	ManufacturerFacilityNumber	|	string	|	256	|	No	|	The manufacturing or receiving location number (identifier) for which this build plan was created	|
|	ManufacturerNumber	|	string	|	256	|	No	|	The unique number of the manufacturer, useful especially in a contract manufacturer scenario or retail scenario	|
|	MasterSchedule	|	string	|	256	|	No	|	The unique identifier of the master schedule	|
|	MasterScheduleNumber	|	string	|	256	|	No	|	The unique identifier of a Master Schedule.	|
|	ProductNumber	|	string	|	256	|	No	|	The product for which the build plan was created	|
|	UoMId	|	string	|	36	|	No	|	Unit of measure Id	|
|	UoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
|	WarehouseId	|	string	|	36	|	No	|	The unique Id of the warehouse	|
|	WarehouseNumber	|	string	|	256	|	No	|	The location or stock keeping location where the product will be received	|
