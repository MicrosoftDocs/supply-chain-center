---
title: Item
description: This article provides information about the Item entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# Item

Something that is inventoried. A SKU, Stock keeping unit, refers to a specific item in a specific unit of measure. Supply chain center recommends to use item base unit of measure for this entity

For example, if you distributed a specific chemical in both gallon containers and barrels then you would maintain the inventory as two SKUs even though they are both the same specific chemical. However if you have only one SKU's then use ItemUnitOfMeasureConversion entity to maintain relationship between containers, barrels etc.

Items are classified as follows:

- Tool
- Product
- Raw Material
- Kit
- Replacement Part
- Unit
- Miscellaneous Item

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| Item | ItemSku | yes | string | 20 | The Stock Keeping Unit identifier, which is typically used for inventory-related activities. |
| Item | TargetReturnPrice | no | decimal | 9 | A price established as part of a strategy to yield a specific return on investment.</br></br> Target-Return Price = (unit cost) + ((desired return)\*(invested capital))/unit sales</br></br> The Target-Return Price ignores competitor's pricing and price elasticity. |
| Item | StandardWholesalePrice | no | decimal | 9 | The standard, or default, price charged wholesalers for the Product. |
| Item | LotSizeQuantity | no | decimal | 9 | The quantity of Item to be purchased or manufactured.</br></br> The objective is to spread setup and ordering costs over a large number of pieces (Items) to reduce unit costs. |
| Item | MinimumStockQuantity | no | decimal | 9 | A control limit within a stock control system which could indicate the point at which an order should be placed, or indicate if stocks are too low, for a specific item. |
| Item | MinimumOrderQuantity | no | decimal | 9 | The smallest order quantity which, in principle, is allowed. |
| Item | ListPrice | no | decimal | 9 | The standard retail price of the Product before the application of any discount.</br></br>This is the price that normally appears in catalogs, on purchase orders and invoices. |
| Item | MaximumStorageHumidity | no | decimal | 9 | The maximum storage humidity that the item may be stored at. |
| Item | MinimumStorageHumidityUomId | no | string | 36 | The unique identifier of a Unit Of Measure. |
| Item | MaximumStorageHumidityUomId | no | string | 36 | The unique identifier of a Unit Of Measure. |
| Item | StandardCost | no | decimal | 9 | The estimated or calculated cost to manufacture or produce the Product. Often used for calculating the value of the Item for inventory purposes. |
| Item | StandardQuantityUnitOfMeasureId | no | string | 36 | The unique identifier of a Unit Of Measure. |
| Item | ActiveItemInventoryPeriodNumberOfDays | no | integer | 6 | The number of days that the organization defines as the 'active item period'. |
| Item | ManufacturerId | no | string | 36 | The unique identifier of a Manufacturer. |
| Item | RepairableItemIndicator | no | boolean | 1 | An inventory item that is not normally consumed in use but one which will be repaired and re-used as part of the normal stock policy for that item. Such items have a repair lead-time as well as a procurement lead-time. |
| Item | CommodityTypeId | no | string | 36 | The unique identifier of a Commodity Type. |
| Item | ItemTypeId | no | string | 36 | The unique identifier of an Item Type. |
| Item | FamilyGroupId | no | string | 36 | The unique identifier of a Family Group. |
| Item | TrackSerialNumberIndicator | no | boolean | 6 | Indicates that the Item must be tracked by Serial Number. |
| Item | ActiveInventoryItemIndicator | no | boolean | 1 | Any item or element of inventory which has been used or sold within a given period. |
| Item | HazardousMaterialIndicator | no | boolean | 1 | Any substance that has been determined by the Occupational Safety and Health Administration (OSHA) as having the potential to cause a physical or health hazard. This is based on its potential for burning, exploding, or otherwise causing an injury to workers or the likelihood that exposure will result in acute or chronic health effects among employees |
| Item | EligibleForExportIndicator | no | boolean | 1 | Indicates that the Product is eligible for export to foreign countries without restriction. |
| Item | SerializedItemIndicator | no | boolean | 1 | Indicates that the Item is serialized. |
| Item | ConsignmentItemIndicator | no | boolean | 1 | Consignments can be used to keep track of inventory that you don't own, but at the time you sell it, you must pay for it. |
| Item | MinimumStorageHumidity | no | decimal | 6 | The minimum storage humidity that the item may be stored at. |
| Item | ItemElectronicProductCode | no | decimal | 9 | EPC is the RFID version of the UPC barcode.</br></br> EPC is intended to be used for specific product identification. However, EPC goes beyond UPC by not only identifying the product as an SKU, but also providing access to additional data about the origin and history of the specific units.</br></br> The EPC tag itself identifies the manufacturer, product, version, and serial number. It's the serial number that takes EPC to the next level.</br></br> This is the key to data related to specific lots/batches as well as potentially tracking the specific unit's history as it moves through the supply chain. |
| Item | GlobalTradeItemNumber | no | decimal | 9 | The Global Trade Item Number (GTIN) is an identifier for trade items that was developed by GS1. |
| Item | ComponentPartIdentifier | no | string | 30 | The Component / Part Identifier (CPID) is used to identify components or parts that are used in the assembly of a larger item. The CPID is part of the GS1 system of standards. |
| Item | ItemLength | no | decimal | 9 | The standard item length. |
| Item | ProductId | no | string | 36 | The unique identifier of a Product. |
| Item | EuropeanArticleNumber | no | decimal | 9 | A 13 digit barcoding standard which is a superset of the original 12-digit Universal Product Code (UPC).</br></br>aka International Article Number (abbreviation of EAN retained) |
| Item | ItemDescription | no | string | 512 | The description of the Item. |
| Item | ItemName | no | string | 128 | The name of the Item. |
| Item | PluCode | no | decimal | 9 | PLU Codes are typically assigned to fresh produce but can also be assigned to other items as well. |
| Item | UniversalProductCode | no | decimal | 14 | A system that identifies products by type and by manufacturer.</br></br> A UPC consists of twelve (12) digits. Six (6) indicate the Manufacturer and six (6) digits describe the product.</br></br> UPCs appear on product packages as bar codes, which are graphic symbols that are read by optical scanner devices.</br></br> UPCs are assigned by the Uniform Code Council of Dayton, Ohio. |
| Item | EngineeringReferenceNumber | no | integer | 12 | The number used by manufacturing or engineering when referencing the Product. |
| Item | ItemWidth | no | decimal | 9 | The standard item width. |
| Item | MinimumStorageTemperature | no | decimal | 9 | The minimum temperature at which the item may be stored. |
| Item | ShelfLifeDays | no | integer | 6 | The amount of time that a product can be stored before it can no longer be safely consumed or sold. |
| Item | MinimumStorageTemperatureUomId | no | string | 36 | The unique identifier of a Unit Of Measure. |
| Item | MaximumStorageTemperatureUomId | no | string | 36 | The unique identifier of a Unit Of Measure. |
| Item | MaximumStorageTemperature | no | decimal | 6 | The maximum temperature at which the item may be stored. |
| Item | WeightUomId | no | string | 36 | The unique identifier of a Unit Of Measure. |
| Item | LwhUomId | no | string | 36 | The unique identifier of a Unit Of Measure. |
| Item | ItemHeight | no | decimal | 6 | The standard item height. |
| Item | ItemVolume | no | decimal | 6 | The standard item volume. |
| Item | ItemWeight | no | decimal | 6 | The standard item weight. |
| Item | ItemVolumeUomId | no | string | 36 | The unique identifier of a Unit Of Measure. |

EOF