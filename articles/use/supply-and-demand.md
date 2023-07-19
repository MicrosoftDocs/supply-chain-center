---
title: Supply & demand insights overview
description: This article provides information about Microsoft Supply Chain Center's Supply & demand insights features.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: overview
ms.date: 05/24/2023
ms.custom: bap-template
---

# Supply & demand insights overview

The Supply & demand insights home page in Microsoft Supply Chain Center presents a dashboard that shows five key performance indicators (KPIs) for inbound orders (procurement). The dashboard helps you monitor the general health of your inbound supply chain, identifies potential risks, and monitors performance. You can also create a personalized view of these KPIs through the My analytics feature. Just select **Create custom view** on the top bar in the **Supply & demand insights** module or **My analytics** in the left navigation pane.

> [!Video https://www.microsoft.com/videoplayer/embed/RE5azzg]

## Supply & demand insights landing page

The landing page for the **Supply & demand insights** module consists of favorite KPIs and supply chain maps. You can choose any three KPIs from one or more persona-specific KPI pages and add (pin) them to the landing page as favorite KPIs.

:::image type="content" source="media/SDI-Landing-Page.png" alt-text="Screenshot of the landing page for the Supply & demand insights module, showing three pinned favorite KPIs and a supply chain map."::: 

## Add favorite KPIs to the landing page

1. On the **Summary** drop-down menu, select an option to go to a persona-specific KPI page.

    :::image type="content" source="media/SDI-Persona-Dropdown.png" alt-text="Screenshot of the Summary drop-down menu for the persona-driven Supply & demand insights module."::: 

1. In the upper-right corner of the KPI card, select the pin symbol to pin that KPI to the landing page as a favorite KPI.

    :::image type="content" source="media/Pin-Favorite-KPI.png" alt-text="Screenshot of the card for the Supply coverage KPI.":::

## Available KPIs

The **On time in full** (**OTIF**) and **Commitment shortage** KPIs measure the performance of vendors (suppliers), and the general trend of their performance is visualized in the line chart. **OTIF** shows how often the suppliers are delivering the purchase orders in full and on time as requested.

The **Supply coverage** and **Inventory turnover rate** (**ITR**) KPIs focus primarily on inventory levels at a facility or across facilities, to help you balance demand and inventory.

The **Projected inventory** KPI is an aggregated view of supply and demand across all facilities and items, and the general trend that's projected for on-hand stock over demand.

The visualizations on the landing page are aggregations of data across multiple facilities and items by all suppliers.

:::image type="content" source="media/supply-and-demand-overview.png" alt-text="Screenshot of the home page for the Supply & demand insights module.":::

You can set target rates or goals for **OTIF**, **Commitment shortage**, **Supply coverage**, and **ITR**. The target settings let users benchmark or measure performance against set goals. You can also set the refresh frequency for the analytics of the **Supply & demand insights** module. In this way, you can ensure that you're accurately measuring your performance. You can find both settings in the Admin center. The following video provides more information.

> [!Video https://www.microsoft.com/videoplayer/embed/RE5cauF]

Every KPI has its own visualized report. Filters near the top of each report page can help you better understand the related KPI, because the report is updated based on the filters that you apply.

:::image type="content" source="media/supply-and-demand-OTIF-filters.png" alt-text="Screenshot with the available filters highlighted for the OTIF report.":::

### On time in full

**OTIF** is a measure of a supplier's ability to fulfill an order in full and deliver it on time, based on the original requested delivery date. It's a key supply chain metric that's used to measure a supplier's performance. It's sometimes referred to as **Perfect Order**.

**OTIF** is expressed as a percentage. The following formula is used:

OTIF = (_All order lines delivered in full and on time in a month_ &divide; _All order lines for that month_) &times; 100

:::image type="content" source="media/supply-and-demand-OTIF-overview.png" alt-text="Screenshot of an example On time in full KPI report.":::

To determine whether an order is fulfilled in full, the system compares the purchase order quantity against the line item (Purchase Order Line table) with the quantity of all shipments that are in transit and the quantity that has been received against that line item of the purchase order.

To determine whether an order was delivered on time, the system compares the **Date Required** attribute of a Purchase Order Line entity or table with either the **EstimatedDeliveryTimestamp** attribute for shipments that are in transit or the **ShipmentDeliveryTimestamp** attribute for shipments that have been delivered. If either of those dates is beyond the value of the **Date Required** attribute, the order wasn't delivered on time.

A higher **OTIF** value indicates better performance. Target levels above 90 percent are considered preferred in the current competitive market demands.

#### Required entities

To enable **OTIF**, the following entities or tables and attributes are required:

| Entity   Name              | Alias or   Display Entity Name | Attribute Name                   | Alias or   Display Attribute Name | Source  |
|----------------------------|--------------------------------|----------------------------------|-----------------------------------|---------|
| msdyn_purchaseorder        | PurchaseOrder                  | msdyn_purchaseorderkey           | PurchaseOrderNumber               | My Data |
| msdyn_purchaseorder        | PurchaseOrder                  | msdyn_accountkey                 | AccountNumber                     | My Data |
| msdyn_purchaseorder        | PurchaseOrder                  | msdyn_geolocationkey             | GeoLocationNumber                 | My Data |
|			     |				      |					 |				     |	       |
| msdyn_purchaseorderproduct | PurchaseOrderLine              | msdyn_purchaseorderkey           | PurchaseOrderNumber               | My Data |
| msdyn_purchaseorderproduct | PurchaseOrderLine              | msdyn_purchaseorderproductkey    | PoLineItemNumber                  | My Data |
| msdyn_purchaseorderproduct | PurchaseOrderLine              | msdyn_productkey                 | ProductNumber                     | My Data |
| msdyn_purchaseorderproduct | PurchaseOrderLine              | msdyn_quantity                   | Quantity                          | My Data |
| msdyn_purchaseorderproduct | PurchaseOrderLine              | msdyn_dateexpected               | DateExpected                      | My Data |
|                            |                                |                                  |                                   |         |
| msdyn_shipment             | Shipment                       | msdyn_shipmentkey                | ShipmentNumber                    | My Data |
| msdyn_shipment             | Shipment                       | msdyn_shipmentdeliverytimestamp  | ShipmentDeliveryTimestamp         | My Data |
| msdyn_shipment             | Shipment                       | msdyn_estimateddeliverytimestamp | EstimatedDeliveryTimestamp        | My Data |
| msdyn_shipment             | Shipment                       | msdyn_towarehousekey             | DestinationWarehouseNumber        | My Data |
|                            |                                |                                  |                                   |         |
| msdyn_shipmentproduct      | ShipmentProduct                | msdyn_shipmentkey,               | ShipmentNumber                    | My Data |
| msdyn_shipmentproduct      | ShipmentProduct                | msdyn_shippedproductquantity     | ShippedProductQuantity            | My Data |
| msdyn_shipmentproduct      | ShipmentProduct                | msdyn_purchaseorderkey           | PoNumber                          | My Data |
| msdyn_shipmentproduct      | ShipmentProduct                | msdyn_purchaseorderproductkey    | PoLineItemNumber                  | My Data |
|                            |                                |                                  |                                   |         |
| msdyn_warehouse            | Warehouse                      | msdyn_warehousekey               | WarehouseNumber,                  | My Data |
| msdyn_warehouse            | Warehouse                      | msdyn_name                       | Name                              | My Data |
| msdyn_warehouse            | Warehouse                      | msdyn_geolocationkey             | GeoLocationNumber                 | My Data |

> [!Video https://www.microsoft.com/videoplayer/embed/RE5cl3l]

### Inventory turnover rate

**ITR** is a measure of the number of times that goods have turned over relative to their consumption. In other words, it's a measure, by the company, of the number of days that are required to consume an item that was procured. **ITR** is indicative of the financial investment health of a company.

**ITR** is calculated as the ratio of goods that were consumed during one month to the average inventory for that month. The following formula is used:

ITR = _Goods sold or consumed in a month_ &divide; _Average inventory for the month_

Consumption of an item during each month is determined from Inventory Transaction entities. Average inventory during each month is determined from the Warehouse Item Available Stock entity.

A higher **ITR** value indicates better inventory management. In general, an **ITR** value above 2 is recommended.

:::image type="content" source="media/supply-and-demand-inventory-turnover-overview.png" alt-text="Screenshot of the Inventory turnover rate KPI report.":::

#### Required entities

To enable **ITR**, the following entities are required:

- Product
- Account
- Warehouse
- Purchase Order
- Purchase Order Line
- Shipment
- Shipment Item
- Inventory Journal
- Inventory Movement Shipment
- Warehouse Product Available Stock

> [!Video https://www.microsoft.com/videoplayer/embed/RE5cisx]

### Supply coverage


**Supply coverage** is calculated as the ratio of demand and supply, and is expressed as a percentage. The following formula is used:

Supply coverage = \[(_Sum of all supply for a period_) &divide; (_Sum of all demand for the period_)\] &times; 100

Supply consists of both on-hand inventory and inventory for shipments that are in transit. On-hand inventory is available in the Warehouse Item Available Stock entity. In-transit shipments are determined by using the Shipment and Shipment Item entities. Demand is available through the Build Plan entity, which holds the materials requirement planning for the item during the period.

A higher percentage indicates better supply coverage. A lower percentage indicates supply shortfalls and potential risks to meeting demand.

:::image type="content" source="media/supply-and-demand-supply-coverage-overview.png" alt-text="Screenshot of the Supply coverage KPI report.":::

#### Open orders

The **Open orders** chart shows all purchase order lines that no shipment has yet been planned for. It includes partially fulfilled orders, backordered orders, and future orders that don't yet have planned shipments.

#### Shipments in transit

In-transit shipments are shipments that the supplier has shipped and that are on the way to their final destination. The **Shipments in transit** report shows the original requested delivery date and the actual ship date, together with the original order quantity and the actual delivery quantity.

#### Required entities

To enable **Supply coverage**, the following entities are required:

- Build Plan
- Inventory Journal
- Inventory Movement Shipment
- Product
- Purchase Order
- Purchase Order Line
- Shipment
- Shipment Item
- Account
- Account Product Lead Time
- Account Product Status
- Warehouse Product Available Stock

> [!Video https://www.microsoft.com/videoplayer/embed/RE5cnB0]

### Commitment shortage

**Commitment shortage** is a measure of a supplier's forecasted commitments and its ability to meet those commitments. It's an important KPI that's used to evaluate a supplier's commitments.

**Commitment shortage** is the ratio of the supplier's forecast that's shared in weekly or daily buckets to the shipments that are received for that period. It's calculated by comparing the original promise and the actual delivery and is expressed as a percentage. The following formula is used:

Commitment shortage = (_Quantity not delivered by the supplier for a period_ &divide; _Commitment quantity by the supplier for the period_) &times; 100

The supplier's commitment quantity for the period is derived from the ItemCustomerSupplyPlan table.

A low percentage indicates reliable performance (better commitment by the supplier), and a high percentage indicates a potentially unreliable supplier.

:::image type="content" source="media/supply-and-demand-commitment-shortage-overview.png" alt-text="Screenshot of the Commitment shortage KPI report.":::

#### Required entities

To enable **Commitment shortage**, the following entities are required:

- Product
- Account
- Warehouse
- Purchase Order
- Purchase Order Line
- Shipment
- Shipment Item
- Inventory Journal
- Inventory Movement Shipment
- Product Account Supply Plan

> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE5cqYQ]

### Projected inventory

**Projected inventory** is the quantity of an item that's a shortfall or surplus for the on-hand demand. It's calculated as the difference between supply and firm demand. The following formula is used:

Projected inventory = _On-hand inventory_ + _In-transit shipments_ – _Firm demand_

Supply consists of both what's available on hand and what you expect to receive (in-transit shipments).

:::image type="content" source="media/supply-and-demand-projected-inventory-overview.png" alt-text="Screenshot of the Projected inventory KPI report.":::

#### Required entities

To enable **Projected inventory**, the following entities or tables are required:

- Product
- Account
- Warehouse
- Purchase Order
- Purchase Order Line
- Shipment
- Shipment Item
- Build Plan

> [!Video https://www.microsoft.com/videoplayer/embed/RE5cisz]

### Planning shortage

In supply chain management, KPIs are used to measure and evaluate the performance of different aspects of the supply chain. One important KPI that's related to planning is **Planning shortage**. This KPI measures the extent to which there's a shortage or shortfall in the planned inventory versus the planned commitment from the supplier. It's calculated as the ratio of shortfall or surplus to planned requirements.

:::image type="content" source="media/Planning-Shortage.png" alt-text="Screenshot of the Planning shortage KPI report.":::

#### Required entities

To enable **Planning shortage**, the following entities or tables are required:

- Product
- Account
- Warehouse
- Account Product Status
- Product Resource Planning Schedule (Original equipment manufacturer \[OEM\] data)
- Product Account Supply Plan (Supplier-provided data)

### Purchase order fill rate

**Purchase order fill rate** is a measure of the percentage of orders that a supplier fulfills during a specific timeframe. It indicates how well a supplier is meeting demand and fulfilling orders on time. It's often used in the context of inventory management, supply chain management, and e-commerce.

**Purchase order fill rate** is the ratio of the sum of delivered quantities on purchase order lines to the sum of ordered quantities on purchase order lines in a given period. The period is expressed in months or weeks.

A high order fill rate indicates that the supplier is meeting customer expectations and promptly fulfilling product demand. A low order fill rate indicates that the supplier is struggling to keep up with demand or is experiencing supply chain disruptions.

:::image type="content" source="media/Purchase-Order-Fill-Rate.png" alt-text="Screenshot of the Purchase order fill rate KPI report.":::

#### Required entities

To enable **Purchase order fill rate**, the following entities or tables are required:

- Product
- Account
- Warehouse
- Account Product Status
- Purchase Order
- Purchase Order Line
- Vendor Supply Commitment (Supplier-provided data)
- Shipment
- Shipment Item

### Purchase order commitment rate

**Purchase order commitment rate** is a measure of the percentage of customer orders that a supplier commits to fulfilling during a specific timeframe. This commitment might be a promise that the supplier makes to deliver goods or services to customers within a specific number of days or hours.

**Purchase order commitment rate** is an important metric for businesses to monitor because it directly affects satisfaction and loyalty. If a supplier consistently fails to meet customer expectations or consistently promises less than demand, the customer becomes dissatisfied and, more importantly, the supplier is considered unreliable.

:::image type="content" source="media/Purchase-Order-Commitment.png" alt-text="Screenshot of the Purchase order commitment rate KPI report.":::

#### Required entities

To enable **Purchase order commitment rate**, the following entities or tables are required:
- Product
- Account
- Warehouse
- Account Product Status
- Purchase Order
- Purchase Order Line
- Vendor Supply Commitment (Supplier-provided data)

### Purchase order return rate

**Purchase order return rate** is a measure of the percentage of orders that are returned to suppliers after purchase. Businesses often use this metric to track a supplier's product quality and its impact on meeting demand. It provides insight into product quality and also helps monitor a supplier's overall business performance.

A high order return rate can indicate issues with product quality, inaccurate product descriptions, or problems with the order fulfillment process. A low order return rate can indicate higher standards of quality and consistency on the part of the supplier. The ability to track order return rates over time can help customers identify areas where improvements can be made to reduce returns and improve overall supply chain reliability.

:::image type="content" source="media/Purchase-Order-Return-Rate.png" alt-text="Screenshot of the Purchase order return rate KPI report.":::

#### Required entities

To enable **Purchase order return rate**, the following entities or tables are required:

- Product
- Account
- Warehouse
- Account Product Status
- Inventory Journal
- Inventory Movement Shipment

### Weeks of supply

**Weeks of supply** measures how long a product inventory lasts before it must be replenished. It's an important metric for inventory management, production planning, and supply chain management. It calculates the number of weeks that a company or organization can continue to operate based on its current inventory levels and its current sales or consumption. Therefore, it helps companies avoid stockouts, minimize waste, and ensure that they have enough inventory to meet customer demand.

For example, if a company has 500 units of a product in stock and consumes 50 units per week on average, it has 10 weeks of supply (500 units &divide; 50 units per week). In this case, the company can continue to operate for 10 weeks before it must replenish its inventory to avoid stockouts or delays in customer order fulfillment.

**Weeks of supply** can be calculated for different types of products, including raw materials, finished goods, and supplies. 

:::image type="content" source="media/Weeks-Of-Supply.png" alt-text="Screenshot of the Weeks of supply KPI report.":::

#### Required entities

To enable **Weeks of supply**, the following entities or tables are required:

- Product
- Account
- Warehouse
- Account Product Status
- Inventory Journal
- Inventory Movement Shipment

### Purchase order cycle time

**Purchase order cycle time** is a measure of the time that's required for creation, approval, and processing of purchase order, up through final delivery of goods or services to the customer by the supplier. It's essentially the time that a purchase order takes to move from the initial request stage through delivery. It can be used to evaluate the efficiency of the procurement process and identify areas where improvements can be made to streamline the procurement process.

The **Purchase order cycle time** metric begins when the purchase request is submitted and ends when the vendor or supplier delivers goods or services.

:::image type="content" source="media/Weeks-Of-Supply.png" alt-text="Screenshot of the Weeks of supply KPI report.":::

#### Required entities

To enable **Purchase order cycle time**, the following entities or tables are required:

- Product
- Account
- Warehouse
- Account Product Status
- Purchase Order
- Purchase Order Line
- Inventory Journal
- Inventory Movement Shipment

### Purchase transit time

**Purchase Order transit time** is a measure of the time that's required to fulfill a purchase order from the moment that it's placed until the moment that it's delivered to the buyer's location. Businesses typically use this metric to track the efficiency of their procurement, shipping, and transportation processes in their supply chain. The ability to measure the purchase order transit time helps businesses identify potential bottlenecks that might affect inventory in their shipping and transportation processes.

In general, a shorter purchase order transit time is desirable because it indicates that the business can receive the products that it needs more quickly. Faster receipt of products can, in turn, help reduce lead times and improve operating margins. It also helps minimize inventory carrying costs by reducing the weeks of supply.

:::image type="content" source="media/Purchase-Transit-Time.png" alt-text="Screenshot of the Purchase transit time KPI report.":::

#### Required entities

To enable **Purchase order cycle time**, the following entities or tables are required:

- Product
- Account
- Warehouse
- Account Product Status
- Purchase Order
- Purchase Order Line
- Shipment
- Shipment Item
- Inventory Journal
- Inventory Movement Shipment

## Restock recommendations

Supply Chain Center has AI-driven optimal inventory. You can access it by selecting the **Restock recommendations** tab at the top of the page, as shown in the following illustration.

:::image type="content" source="media/supply-and-demand-supply-coverage-restock-recommendations.png" alt-text="Screenshot of the Restock recommendations tab of the Supply coverage report page.":::

The **Restock recommendations** tab shows the reorder quantity by facility and item. It also shows the recommended safety stock for the combination of a facility and an item. You can download this recommendation as an Excel file. For more information, see [Configure and review restock recommendations](restock-recommendations.md).

## Downloading reports

You can download individual charts as an Excel file by selecting the **More options** button (three dots) in the upper-right corner of a given report and then selecting **Export data** on the menu. The menu also includes options that let you sort the report in different ways. For example, to sort the report by a specific column, select **Sort by** to get more sort options.

:::image type="content" source="media/supply-and-demand-supply-coverage-open-orders-export.png" alt-text="Screenshot of the Export and sort options on the More options menu for a report.":::

## My analytics

You can use the **My analytics** feature to customize the out-of-box KPIs in the **Supply and demand insights** module. For example, you can change a line chart to a bar chart, completely remove an out-of-box chart, or make other edits to meet your company's needs. Changes that you make to the out-of-box KPIs are saved on the **My analytics** page. They don't overwrite your KPIs in the **Supply and Demand insights** module.

### Edit reports

Your reports appear as tabs at the bottom of the **My analytics** page. To switch reports, select a different tab.

To create a new report from scratch, select the plus sign (**+**) button to the right of the tabs.

> [!NOTE]
> Supply Chain Center doesn't currently support all Power BI capabilities for new reports.

:::image type="content" source="media/my-analytics-tabs.png" alt-text="Screenshot of the Report tabs and plus sign button at the bottom of the My analytics page.":::

Initially, the set of tabs corresponds to the different pages in the **Supply and demand insights** module, and each tab contains the same information. Each of these reports is a copy of what's in the **Supply and demand insights** module. Changes that you make to the reports on the **My analytics** page don't affect the reports in the **Supply and demand insights** module.

> [!IMPORTANT]
> Changes that you make on the **My analytics** page are permanent and can't be automatically reverted to their original visuals. However, the reports in the **Supply and demand insights** module will remain unchanged. Therefore, you can use them as a reference if you want to reset the reports on the **My analytics** page.

#### Add and edit charts

You can use the following expandable/collapsible panes on the right side of the **My analytics** page to edit the reports:

- **Filters** – Use this pane to change or modify filters. The filtering capability is driven by the data that's available in the data model that the out-of-box KPIs are built on.
- **Visualizations** – Use this pane to change the type of chart that's used. For example, you can change a line chart to a pie chart.
- **Fields** – This pane contains data models that visualization can be built on. These models come from the entities for the out-of-box KPIs, and from calculations that involve those entities.

To learn how fields, visualizations, and filters work together to create a chart, see [Build reports](/power-bi/fundamentals/desktop-getting-started#build-reports). For more information about filters and visualizations specifically, see [Take a tour of the report Filters pane](/power-bi/consumer/end-user-report-filter) and [Visualization types in Power BI](/power-bi/visuals/power-bi-visualization-types-for-reports-and-q-and-a).

> [!NOTE]
> The **My analytics** feature doesn't support user-specific changes. Edits that are made to the reports on the **My analytics** page are available to all users in your Supply Chain Center environment.

:::image type="content" source="media/my-analytics-filters-visualizations-fields.png" alt-text="Screenshot of the Filters, Visualizations, and Fields panes expanded on the My analytics page.":::

#### Remove charts or export the underlying data

To remove a chart from a report, select the **More options** button (three dots) in the upper-right corner of the chart, and then select **Remove** on the menu.

To download the raw data that powers a chart, select the **More options** button in the upper-right corner of the chart, and then select **Export data**.

:::image type="content" source="media/my-analytics-export-or-remove.png" alt-text="Screenshot of the Export data and Remove options on the More option menu for a chart.":::

### Personalize your report

You can personalize your report by adding text, shapes, and buttons. Just select **Text box**, **Shapes**, or **Buttons** on the toolbar at the top of the **My analytics** page, and then select an option on the menu.

Buttons can also be used to add images, as described in the following procedure.

1. Select **Buttons** on the toolbar, and then select **Blank** on the menu.

    :::image type="content" source="media/my-analytics-image-step-1.png" alt-text="Screenshot with Blank highlighted on the Buttons menu.":::

2. While the new button is selected, in the **Format** pane on the right, under **Style**, set the **Icon** option to **On**. Then change the icon type to **Custom**, and select **Browse** to upload an image.

    :::image type="content" source="media/my-analytics-image-step-2.png" alt-text="Screenshot of the icon style options in the Format pane.":::

    In the example in the following illustration, the Microsoft logo has been uploaded.

    :::image type="content" source="media/my-analytics-image-step-3.png" alt-text="Screenshot of the Microsoft logo added to a report.":::

3. Adjust the size and position of the uploaded image until you're satisfied with the result.
