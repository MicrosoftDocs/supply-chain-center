---
title: ShipmentItem
description: This article provides information about the ShipmentItem entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# ShipmentItem

The lines on a shipment each consisting of one item.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ShipmentItem | ShipmentItemNumber | yes | integer | 10 | The shipment line number. |
| ShipmentItem | ShipmentId | yes | string | 36 | The unique identifier of a Shipment. |
| ShipmentItem | PerItemDimensionalWeight | no | decimal | 9 | The per item dimensional weight, which is the conversion of the cubic space of a shipment into pounds. Commonly referred to as dim weight. The international term is volume weight. |
| ShipmentItem | TotalQuantityDimensionalWeight | no | decimal | 9 | The dimensional weight of all items, which is the conversion of the cubic space of a shipment into pounds. Commonly referred to as dim weight. |
| ShipmentItem | ActualGrossShipmentWeight | no | decimal | 9 | The weight of the shipment, including all packing, blocking, platforms, special bracing, etc., if required. (Includes weight of unit load device, when applicable.) |
| ShipmentItem | TotalQuantityPackagedWeight | no | decimal | 9 | The total weight of all items packaged for shipment. |
| ShipmentItem | PerItemWeight | no | decimal | 9 | The individual or per item weight of an item. |
| ShipmentItem | TotalQuantityItemWeight | no | decimal | 9 | The total weight of all the items without additional packaging weights added. |
| ShipmentItem | PerItemPackagedWeight | no | decimal | 9 | The weight of each item packaged for shipment. |
| ShipmentItem | TotalItemChargeableWeight | no | decimal | 9 | The weight of the shipment used in determining airfreight charges. The chargeable weight may be the dimensional weight, or on container shipments, the gross weight of the shipment less the tare weight of the container. |
| ShipmentItem | ItemSku | no | string | 20 | The Stock Keeping Unit identifier, which is typically used for inventory-related activities. |
| ShipmentItem | CargoTypeId | no | string | 36 | The unique identifier of a Cargo Type. |
| ShipmentItem | IncotermId | no | string | 36 | The unique identifier of a Incoterm. |
| ShipmentItem | HazardousMaterialHazmatIndicator | no | boolean | 9 | Hazardous materials (Hazmat) The U.S. Government's official term for Dangerous Goods. Items of freight that are inherently harmful and classified under Title 49, Code of Federal Regulations (CFR). Hazardous Materials may only be transported under certain conditions relative to packaging, quantity carried, airplane type, location on board the airplane, etc., and in conformance with applicable rules. Also see Dangerous Goods. |
| ShipmentItem | TotalItemsDensity | no | integer | 9 | Density is weight per unit of volume. Density is computed by dividing a shipments weight by its cubic volume. Generally expressed in pounds per cubic foot in the U.S. |
| ShipmentItem | ShipmentItemNetWeight | no | decimal | 9 | Weight of the goods alone without any immediate wrappings, For example, the weight of the contents of a tin can without the weight of the can. |
| ShipmentItem | DangerousGoodsIndicator | no | boolean | 6 | Items capable of presenting a risk to the health or safety of people or property when shipped.</br></br> The term used by I.M.C.O. for hazardous materials which are capable of posing a significant risk to health, safety or property while being transported.** The United Nation's official term for Hazardous Materials. Articles or substances which are capable of posing a significant risk to the health or safety of the general public when transported by air and which are classified according to the most current editions of the ICAO Technical Instructions for the Safe Transport of Dangerous Goods by Air and the IATA Dangerous Goods Regulations. See Hazardous Materials. |
| ShipmentItem | OrderLineNumber | no | integer | 9 | The number that identifies the Order Line Item. |
| ShipmentItem | PoNumber | no | string | 36 | The unique identifier of a Purchase Order. |
| ShipmentItem | PoLineItemNumber | no | integer | 9 | The unique identifier of a PO line item. |
| ShipmentItem | OrderId | no | string | 36 | The unique number that identifies an Order. |
| ShipmentItem | PackingInstructions | no | string | 2048 | Packing instructions for the associated shipped item. |
| ShipmentItem | HandlingInstructions | no | string | 2048 | Written instructions provided by the shipper/manufacturer and designed to ensure proper handling of the cargo. This can be in the form of marks (see Cautionary Markings) on the cargo or packaging itself or in a separate document such as the bill of lading. |
| ShipmentItem | ShippedItemQuantity | no | decimal | 9 | The quantity of items shipped. |
| ShipmentItem | ItemNetWeight | no | decimal | 9 | The weight of the Item. |
| ShipmentItem | LengthWidthHeightUnitOfMeasureId | no | string | 36 | The unique identifier of a Unit Of Measure. |
| ShipmentItem | Volume | no | decimal | 9 | The volume of the shipment item. |
| ShipmentItem | VolumeUnitOfMeasureId | no | string | 36 | The unique identifier of a Unit Of Measure. |
| ShipmentItem | ItemHeight | no | decimal | 9 | The height of the Item. |
| ShipmentItem | WeightUnitOfMeasureId | no | string | 36 | The unique identifier of a Unit Of Measure. |
| ShipmentItem | ItemLength | no | decimal | 9 | The length of the Item. |
| ShipmentItem | ItemWidth | no | decimal | 9 | The width of the Item. |

EOF