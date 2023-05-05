---
title: Create and use KPIs
description: This article provides information about creating and using KPIs in Microsoft Supply Chain Center.
author: itayhi
ms.author: itayh
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: how-to
ms.date: 4/29/2023
ms.custom: bap-template
---


# Create and use KPIs

This article provides information about creating and using KPIs in Microsoft Supply Chain Center.

## What are KPIs?

KPIs, or Key Performance Indicators, are measurable values that help organizations, teams, or individuals assess their progress towards achieving specific objectives or goals. These quantifiable metrics are used to evaluate the effectiveness of processes, projects, or initiatives, and to track performance over time. Managing the use of KPIs includes setting a target (the desired level of performance), tracking progress against those targets, and taking corrective actions.

## Create a new KPI

> [!Important]
> Before you can create a KPI, you must first create or import Calculations. For more information, see [Create and use Calculations](calculations.md)

To create a KPI, follow these steps.

1. Sign into Microsoft Supply Chain Center, and then select **Analytics**.
1. From the navigation pane, select **KPIs**. 
1. Select **Create** to start the KPI creation wizard.
1. Provide the general **Details** for the KPI:
   -	Name, description, categories, start date, end date, parent. 
   -	The Start Date and End Date represent the period over which the KPI are tracked.
   -	Categories can be used to group KPIs together. 
   -	If you already have an existing KPI, then you can assign it as a parent to the new KPI. Assigning it as a parent is useful for showing the relationship between different KPIs.   
 1. Provide the **Measure** for the KPI.
 1. Select the **Calculation** you would like to use for measuring the KPI. You can only select calculations that were successfully refreshed.
 1. **Map**: Select the measure value and date columns in your Calculation you would like to use for tracking the KPI. A measure value is the value that is tracked over time as the KPI. Date column is used as the time series data over which the KPI is measured and evaluated. Then, enter the Units that the KPI is measured in, for example: USD, EUR, Lbs, KG, pallets, cases. 
1. Set your **Target** value for the KPI. The target value is used to calculate KPI progress. 
1. Set your **Threshold** for the KPI. A KPI is required to have at least one rule. A rule consists of a set of conditions and actions. Added to actions are performed when a condition is met. In addition, you can change the status of the KPI when the rule is met. For example if you're making an On Time In Full KPI, you can set up a threshold for when the value is less than 95% that sets the KPI status to “At risk” and trigger a Power Automate Flow. KPI rules are evaluated periodically, according to the data refresh rate set in the Supply and demand insights section in Settings. 
1. Review the details of the KPI you're creating. You can edit any of the information on the previous steps.
1. Select **Submit** to create the KPI.
 
## Edit or Delete an Existing KPI

Currently, editing an existing KPI isn't available. You can modify the parent and child KPIs that are associated with a KPI. To delete a KPI, select the KPI you want to delete and then select **Delete KPI**.

## View a KPI

On the KPIs page, you can view KPIs by their **Name**, **Description**, **Status**, **Value**, **Units**, **Progress**, **Start Date**, **End Date**, **Owner**, and **Categories**. You may filter by **Status** by selecting the different status labels on the top of the page.
 
To view the details of a KPI, select its **Name**. You can view the KPI’s performance over time, its value history, any parent or child KPIs it's related to, and other details. 
 
## Best Practices 

The following sections include best practices for creating calculations and KPIs.

### Best practices for creating calculations for KPIs 

-	**Include a measure and date column in your calculation**. It's important to include both a measure (or an aggregation) and a date column. The measure should represent the data that you want to track, such as revenue or customer satisfaction. The date column should represent the time period over which you want to track the data, such as days, weeks, or months. 
-	**Sort date columns in descending order**. To ensure that your KPI accurately reflects historical trends, it's important to sort your date columns in descending order. This way, the most recent data is displayed first to allow you to quickly see if there are any changes or trends over time. 
-	**Refresh calculations**. Calculations used in KPIs should be successfully refreshed to ensure that they're up to date and accurate.  
-	**Use the appropriate level of aggregation**. When creating calculations for use in KPIs, it's important to measure the smallest possible unit to a high level of aggregation. This means that you should create calculations that represent the data at different levels, from the most granular (such as individual transactions) to the most aggregated (such as total revenue). For example, if you want to track revenue growth for a company by region, you should create separate calculations for each region, and create a calculation for the company as a whole. The most aggregated calculation can be used in parent KPIs and most granular level in children KPIs. 
 
### Best practices for creating KPIs 

-	**Use a calculation that fulfills all the above criteria**. To ensure that your KPI accurately reflects the data you want to track, it's important to use a calculation that meets all the criteria outlined in the above section. This includes having a measure and date column, sorting date columns in descending order, refreshing calculations regularly, and using the appropriate level of aggregation. 
-	**Keep in mind the start date when evaluating progress**. When evaluating progress for a KPI, it's important to keep in mind that the progress is based on the start date of the KPI and doesn't consider historical data. 
-	**A KPI target can't have a negative value**.
-	**Child KPIs don't roll up to Parent KPIs**. Each KPI tracks its own progress and doesn't roll up the progress from its child KPIs. This allows you to track progress at different levels of aggregation and identify areas that may require further analysis. 

