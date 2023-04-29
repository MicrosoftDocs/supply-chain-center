---
title: KPIs
description: This article provides information about Microsoft Supply Chain Center's KPIs feature.
author: itayhi
ms.author: itayh
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 4/29/2023
ms.custom: bap-template
---


# KPIs

## What are KPIs?
KPIs, or Key Performance Indicators, are measurable values that help organizations, teams, or individuals assess their progress towards achieving specific objectives or goals. These quantifiable metrics are used to evaluate the effectiveness of processes, projects, or initiatives, and to track performance over time. Managing the use of KPIs includes setting a target (the desired level of performance), tracking progress against those targets and taking corrective actions.

## Create a new KPI
**Prerequisite**
In order to create a KPI, you must first create or import Calculations. 
**Create a new KPI**
To create a KPI, sign into Microsoft Supply Chain Center, and then select Analytics.  Then, select KPIs on the left navigation bar. 
 
Then, select create to start the KPI creation wizard.
-	**Details**:
 -	Enter the general details of the KPI: Name, description, categories, start date, end date, parent. 
 -	The Start Date and End Date represent the period over which the KPI will be tracked.
 -	Categories can be used to group KPIs together. 
 -	If you already have an existing KPI, then you can assign it as a parent to the new KPI. This is useful for showing the relationship between different KPIs.   
-	**Measure**
 -	**Select**: Select the Calculation you would like to use for measuring the KPI. Only calculations that were successfully refreshed can be selected.
 - **Map**: Select the measure value and date columns in your Calculation you would like to use for tracking the KPI. A measure value is the value that will be tracked over time as the KPI. Date column will be used as the time series data over which the KPI is measured and evaluated. Then, enter the Units which the KPI is measured in, for example: USD, EUR, Lb, KG, pallets, cases. 
-	**Target**: Set your target value for the KPI. The target value will be used to calculate the KPI progress. 
-	**Threshold**: A KPI is required to have at least one rule. A rule consists of a set of conditions and actions. Added to actions will be performed when the a condition is met. In addition, you can change the status of the KPI when the rule is met.. For example if you are making  an On Time In Full KPI, you can setup a threshold for when the value is less than 95% that will set the KPI status to “At risk” and trigger a Power Automate Flow. KPI rules are evaluated periodically, according to the data refresh rate set in the Supply and demand insights section in Settings. 
-	**Summary**: Review the details of the KPI you are creating. You can edit any of the information on the previous steps.
 
## Edit or Delete an Existing KPI
Currently, apart from modifying its Parent or Child KPIs,  an existing KPI cannot be edited. To delete a KPI, select the KPI you wish to delete and then select “Delete KPI”.

## View a KPI
In the KPIs page, you can view different KPIs by their Name, Description, Status, Value, Units, Progress, Start Date, End Date, Owner and Categories. You may filter by Status by selecting the different Status labels on the top of the page.
 
To view the details of a KPI, click on its name. In this screen, you can view the KPI’s performance over time, its value history, any Parent or Child KPIs it is related to, and other details. 
 
## Best Practices 

1.	Best practices for creating calculations to be used by KPI 
a.	Include a measure and date column in your calculation: 
When creating a calculation for use in a KPI, it's important to include both a measure (or an aggregation) and a date column. The measure should represent the data that you want to track, such as revenue or customer satisfaction. The date column should represent the time period over which you want to track the data, such as days, weeks, or months. 
b.	Sort date columns in descending order: 
To ensure that your KPI accurately reflects historical trends, it is important to sort your date columns in descending order. This way, the most recent data will be displayed first, allowing you to quickly see if there are any changes or trends over time. 
c.	Refresh calculations: 
Calculations used in KPIs should be successfully refreshed to ensure that they are up to date and accurate.  
d.	Use the appropriate level of aggregation: 
When creating calculations for use in KPIs, it's important to measure the smallest possible unit to a high level of aggregation. This means that you should create calculations that represent the data at different levels, from the most granular (such as individual transactions) to the most aggregated (such as total revenue). For example, if you want to track revenue growth for a company by region, you should create separate calculations for each region, as well as a calculation for the company as a whole. The most aggregated calculation can be used in parent KPIs and most granular level in children KPIs. 
 
2.	Best practices for creating KPIs 
a.	Use a calculation that fulfills all the above criteria: 
To ensure that your KPI accurately reflects the data you want to track, it's important to use a calculation that meets all the criteria outlined in the above section. This includes having a measure and date column, sorting date columns in descending order, refreshing calculations regularly, and using the appropriate level of aggregation. 
b.	Keep in mind the start date when evaluating progress: 
When evaluating progress for a KPI, it's important to keep in mind that the progress is with respect to the start date of the KPI and does not take into account historical data.  
c.	A KPI target cannot have a negative value.
d.	Child KPIs do not roll up to Parent KPIs: 
Each KPI tracks its own progress and does not roll up the progress from its child KPIs. This allows you to track progress at different levels of aggregation and identify areas that may require further analysis. 

