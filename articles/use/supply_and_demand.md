---
title: Supply & demand analytics overview
description: This article provides information about Microsoft Supply Chain Center's Supply & demand analytics features.
author: 
ms.author: 
ms.reviewer: johnmichalak
ms.service: 
ms.topic: 
ms.date: 11/3/2023
ms.custom:
---

# Supply & demand analytics overview

Microsoft Supply Chain Center’s Supply & demand home page presents five key supply chain performance metrics for inbound orders (procurement). The dashboard helps you monitor the general health of your inbound supply chain, identifies potential risks, and monitors performance.

The **On time in full** (**OTIF**) and **Commitment shortage** metrics measure the performance of vendors (suppliers), and the general trend of their performance is visualized in the line chart. **OTIF** shows how often the suppliers are delivering the purchase orders in full and on time as requested.

The **Supply coverage** and **Inventory turnover rate** (**ITR**) metrics focus primarily on inventory levels at a facility or across facilities to help you balance demand and inventory.

**Projected inventory** on the landing page is the aggregated view of supply and demand across all facilities and items, and the general trend that is projected for on-hand stock over demand.

The visualizations on the landing page are aggregations of data across multiple facilities and items by all suppliers.

Users can set target rates or goals for **OTIF**, **Commitment shortage**, **Supply coverage**, and **ITR**. The target settings let users benchmark or measure performance against set goals. For more details about how to set target values for these metrics, see the supply and demand settings in the Admin Center.

## On time in full

**OTIF** is a measure of a supplier’s ability to fulfill an order in full and deliver it on time, based on the original requested delivery date. **OTIF** is a key supply chain metric that is used to measure a supplier’s performance. It’s sometimes referred to as **Perfect Order**.

**OTIF** is calculated as a percentage, by using the following formula:

OTIF = (_All order lines delivered in full and on time in a month_ ÷ _All order lines for that month_) × 100

![A screenshot of the On time in full report chart.](//:0)

To determine whether an order is fulfilled in full, the system compares the purchase order quantity against the line item (Purchase Order Line table) with the quantity of all shipments that are in transit and the quantity that has been received against that line item of the Purchase Order.

Determination of on time is calculated by looking at Date Required attribute of a Purchase Order Line entity or table, and then comparing it with the EstimatedDeliveryTimestamp attribute in a shipment that is in transit shipments or comparing it with the ShipmentDeliveryTimestamp attribute for shipments that have been delivered. If either of those dates are beyond the Date Required attribute, then the order was not delivered on time.

Higher OTIF indicates better performance. Target levels above 90% are considered preferred in the current competitive market demands

OTIF has filters for the visualizations on the page. Filters are Goods receipt date, Time grain, Vendor & Facility, and Item. The filters enable search and multiselection capabilities. For example, by selecting the **Item** filter and using the search field on the drop-down menu, you can search the items. You can then use the checkboxes to select multiple items in the search results, as shown in the following illustration.

![A screenshot of the available filters.](//:0)

To enable OTIF, the following entities or tables are required:
- Item
- Vendors
- Warehouse
- Purchase Order
- Purchase Order Line
- Shipment
- Shipment Item
- Inventory Transaction
- Inventory Transaction Shipment
- Inventory Transaction Unserialized Item

To return to the Supply & demand home page, select **Supply & demand mismatch** at the top of the page, as shown in the following illustration.

![A screenshot of the breadcrumbs Supply & demand insights > Ontime in full.](//:0)

## In-transit shipments

In-transit shipments are shipments that have been shipped by a supplier and are on their way to their final destination. The **Shipments in transit** report shows the original requested delivery date and the actual ship date, together with the original order quantity and the actual delivery quantity.

![A screenshot of the shipments in transit report.](//:0)

You can download the report as an Excel file by selecting the **More options** button (three dots) in the upper-right corner of the report and then selecting **Export data** on the menu. The menu also includes options that let you sort the report in different ways. For example, to sort the report by a specific column, select **Sort by** to get additional sort options.

![A screenshot with Export data and Sort by highlighted.](//:0)

## Inventory turnover rate

**ITR** is a measure of the number of times that goods have turned over relative to their consumption. In other words, it’s a measure, by the company, of the number of days that are required to consume an item that was procured. **ITR** is indicative of the financial investment health of a company.

**ITR** is calculated as the ratio of goods consumed in one month to the average inventory for that month. The following formula is used:

ITR = _Goods sold or consumed in a month_ ÷ _Average inventory for the month_

Consumption of an item during each month is determined from Inventory Transaction entities. Average inventory during each month is determined from the Warehouse Item Available Stock entity.

A higher **ITR** value indicates better inventory management. In general, an **ITR** value above 2 is recommended.

![A screenshot of the Inventory turnover rate chart.](//:0)

**ITR** has the following filters for the visualizations on the page: **Goods receipt date**, **Time grain**, **Facility**, and **Item**. The filters enable search and multi-selection capabilities. For example, by selecting the **Item** filter and using the search field on the drop-down menu, you can search the items. You can then use the checkboxes to select multiple items in the search results, as shown in the following illustration.

![A screenshot of the available filters.](//:0)

To enable **ITR**, the following entities or tables are required:

- Item
- Vendors
- Warehouse
- Purchase Order
- Purchase Order Line
- Shipment
- Shipment Item
- Inventory Transaction
- Inventory Transaction Shipment
- Inventory Transaction Unserialized Item
- Warehouse Item Available Stock

To return to the Supply & demand home page, select **Supply & demand mismatch** at the top of the page, as shown in the following illustration.

![A screenshot of the breadcrumbs Supply & demand insights > inventory turnover rate.](//:0)

## Supply coverage

**Supply coverage** is a measure of supply that meets demand. It’s expressed as a percentage. **Supply coverage** helps you determine whether the on-hand inventory and the expected supply that is in transit for a period will meet the demand for that period. A higher percentage indicates better supply coverage. A lower percentage indicates supply shortfalls and potential risks to meeting demand.

**Supply coverage** is calculated as the ratio of demand and supply. The following formula is used:

Supply coverage = \[(_Sum of all supply for a period_) ÷ (_Sum of all demand for the period_)\] × 100

Supply consists of both on-hand inventory and inventory for shipments that are in transit. On-hand inventory is available in the Warehouse Item Available Stock entity. In-transit shipments are determined by using the Shipment and Shipment Item entities.

Demand is available through the Build Plan entity, which holds the materials requirement planning for the item during the period.

In the upper-right corner of the **Supply coverage** page is the supply coverage slider. You can use percent to slider to filter the visualization, the inventory projection, and the **Open orders** report on the page. By defaulpercent tohe slider is set to 0-percent supply coverage. You can adjust both ends of the slider to view data that falls within the specified range, as shown in the following illustration.

![A screenshot of the supply coverage data ranges.](//:0)

Options at the top of the supplier coverage visualization let you apply the following additional filters: **Goods receipt date**, **Time grain**, **Facility**, and **Item**. The filters enable search and multiselection capabilities. For example, by selecting the **Item** filter and using the search field on the drop-down menu, you can search the items. You can then use the checkboxes to select multiple items in the search results, as shown in the following illustration.

![A screenshot of the available filters.](//:0)

The filters on the page let you slice and dice the **Supply coverage** metric in different ways. The changes affect the supply coverage visualization, and also the inventory projection and the **Open orders** report at the bottom of the page.

  

To enable **Supply coverage**, the following entities or tables are required:

- Build Plan
- Inventory Transaction
- Inventory Transaction Shipment
- Inventory Transaction Unserialized Item
- Item
- Item Unit Of Measure Conversion
- Location
- Purchase Order
- Purchase Order Line
- Shipment
- Shipment Item
- Shipment Location
- Shipment Route Leg
- Shipment Route Leg Equipment
- Shipment Route Leg Equipment Shipment Item
- Shipment Route Leg IOT
- Vendor
- Vendor Item Leadtime
- Vendor Item Status
- Vendor Location
- Warehouse Item Available Stock

## Open orders

The **Open orders** report shows all purchase order lines that no shipment has yet been planned for. It includes partially fulfilled orders, backordered orders, and future orders that don’t yet have planned shipments.

![A screenshot of the open orders report](//:0)

You can download the report as an Excel file by selecting the **More options** button (three dots) in the upper-right corner of the report and then selecting **Export data** on the menu. The menu also includes options that let you sort the report in different ways. For example, to sort the report by a specific column, select **Sort by** to get additional sort options.

![A screenshot with Export data and Sort by highlighted.](//:0)

To return to the Supply & demand home page, select **Supply & demand mismatch** at the top of the page, as shown in the following illustration. To return to the Supply & demand home page, select **Supply & demand mismatch** at the top of the page, as shown in the following illustration.

![A screenshot of the breadcrumbs Supply & demand insights > supply coverage.](//:0)

## Commitment shortage

**Commitment shortage** is a measure of a supplier’s forecasted commitments and its ability to meet those commitments. It’s expressed as a percentage. This metric is an important KPI that is used to evaluate a supplier’s commitments.

**Commitment shortage** is calculated by comparing the original promise and the actual delivery. It’s the ratio of the supplier’s forecast that is shared in weekly or daily buckets to the shipments that are received for that period. The following formula is used:

Commitment shortage = (_Quantity not delivered by the supplier for a period_ ÷ _Commitment quantity by the supplier for the period_) × 100

The supplier’s commitment quantity for the period is derived from the ItemCustomerSupplyPlan table.

A low percentage indicates reliable performance (better commitment by the supplier), and a high percentage indicates a potentially unreliable supplier.

To enable **Commitment shortage**, the following entities or tables are required:

- Item
- Vendors
- Warehouse
- Purchase Order
- Purchase Order Line
- Shipment
- Shipment Item
- Inventory Transaction
- Inventory Transaction Shipment
- Item Customer Supply Plan
- Vendor Location
- Location
- Inventory Transaction Unserialized Item

## Projected inventory

**Projected inventory** is the quantity of an item that is a shortfall or surplus for the on-hand demand. It’s calculated as the difference between supply and firm demand. Supply consists of both what is available on hand and what is expected to be received (in-transit shipments). The following formula is used:

Projected inventory = _On-hand inventory_ + _In-transit shipments_ – _Firm demand_

![Chart, bar chart
Projected Inventory](//:0)

To enable **Projected inventory**, the following entities or tables are required:

- Item
- Vendors
- Warehouse
- Purchase Order
- Purchase Order Line
- Shipment
- Shipment Item
- Build Plan

To return to the Supply & demand home page, select **Supply & demand mismatch** at the top of the page, as shown in the following illustration.

![A screenshot of the breadcrumbs Supply & demand insights > projected inventory.](//:0)

## Restock quantity (Restock recommendations)

Supply Chain Center has AI-driven optimal inventory. You can access it by selecting **Restock recommendations** at the top of the page,as shown in the following illustration.

![A screenshot of the breadcrumbs Supply & demand insights > projected inventory. Restock recommendation is highlighted.](//:0)

**Restock recommendations** shows the reorder quantity by facility and item. It also shows the recommended safety stock for the combination of a facility and an item. You can download this recommendation as an Excel file. For more information, see the [Configure and review restock recommendations](https://microsoft-my.sharepoint.com/personal/johnmichalak_microsoft_com/Documents/Documents/Windblade%20Conversion/Supply%20and%20demand.docx#_Configure_and_review) section.

You can download the report as an Excel file by selecting the **More options** button (three dots) in the upper-right corner of the report and then selecting **Export data** on the menu. Then menu also includes options that let you sort the report in different ways. For example, to sort the report by a specific column, select **Sort by** to get additional sort options.

![A screenshot with Export data and Sort by highlighted.](//:0)
