---
title: Data schema
description: This article provides information about Microsoft Supply Chain Center's data schema.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: overview
ms.date: 11/3/2022
ms.custom: bap-template
---

# Data schema

Microsoft supply chain center has a few out-of-the box supply chain performance metrics for inbound orders (procurement). The supply chain performance metrics help monitor the general health of inbound supply chain and identifies potential risks and monitors performance.

These metrics are **On time in full**, **Inventory turnover rate**, **Supply coverage**, **Commitment shortage**, and **Projected inventory**. Use these metrics to visualize actionable insights and analyze trends for informed decision making. 

This section details the data schema that is needed to light up those actionable insights. The data  schema is based on the [Azure Synapse Database Templates schema](/azure/synapse-analytics/database-designer/overview-database-templates), which is a large set of schemas that span multiple industry verticals, including freight and logistics.  Supply Chain Center’s schema is a representation of all supply chain process areas like Procurement, Sales, Warehouse & Distribution, Freight & Logistics, Production or Manufacturing and Planning & Forecasting. It includes all normalized entities based on industry standards to help our customers build a powerful control tower or supply chain network.     

The entities in the data schema are described in the following sections.
