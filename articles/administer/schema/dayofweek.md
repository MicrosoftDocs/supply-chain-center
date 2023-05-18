---
title: DayOfWeek
description: This article provides information about the DayOfWeek entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **DayOfWeek**


The day of week entity refers to the specific day within a week. A week consists of days like Sunday, Monday, Tuesday, Wednesday, Thursday, Friday, and Saturday. 


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	BusinessDayIndicator	|	string	|	256	|	No	|	Indicates that the associated day is a business day.	|
|	DayOfWeekDescription	|	string	|	256	|	No	|	Description of day of the week	|
|	DayOfWeekId	|	string	|	256	|	Yes	|	The unique identifier of a Day Of Week.	|
|	DayOfWeekName	|	string	|	256	|	No	|	The name of the day of week	|
|	DayOfWeekNumber	|	string	|	256	|	Yes	|	The unique identifier of a Day Of Week.	|
|	WeekendIndicator	|	string	|	256	|	No	|	Indicates that the associated day falls on a weekend.	|
