---
title: ShipmentItemConsolidation
description: This article provides information about the ShipmentItemConsolidation entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# ShipmentItemConsolidation

The consolidation of shipment items for transfer. Shipments Items are not breakable (SHIPMENT CONSOLIDATION). Shipment Item Consolidation deals with Shipments that can be broken at the item level.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ShipmentItemConsolidation | ConsolidatedShipmentId | yes | string | 36 | The unique identifier of a Shipment. |
| ShipmentItemConsolidation | ConsolidatedShipmentItemNumber | yes | integer | 10 | The shipment line number. |
| ShipmentItemConsolidation | ShipmentId | yes | string | 36 | The unique identifier of a Shipment. |
| ShipmentItemConsolidation | ShipmentItemNumber | yes | integer | 9 | The shipment line number. |
| ShipmentItemConsolidation | PackedVolume | no | decimal | 9 | The volume of the Packing Type in which the associated Lot of shipped items are packed.</br></br>For example: Lot 3 consisting of 35 cans are packed in a box of external length, external width and external height measurements.</br></br> This enables shipped to plan for containerizing shipped items. |
| ShipmentItemConsolidation | WeightUnitOfMeasureId | no | string | 36 | The unique identifier of a Unit Of Measure. |
| ShipmentItemConsolidation | VolumeUnitOfMeasureId | no | string | 36 | The unique identifier of a Unit Of Measure. |
| ShipmentItemConsolidation | ContainerId | no | string | 36 | The unique identifier of the container.</br></br> This would be the 'serial number' of the container if it is serialized. |
| ShipmentItemConsolidation | PackingTypeId | no | string | 36 | The unique identifier of a Packing Type. |
| ShipmentItemConsolidation | PackedWeight | no | decimal | 9 | The weight of the Packing Type in which the associated Lot of shipped items are packed.</br></br>For example: Lot 3 consisting of 35 cans are packed in a box of external length, external width and external height measurements.</br></br>This enables shipped to plan for containerizing shipped items. |
| ShipmentItemConsolidation | PackedLength | no | decimal | 9 | The length of the Packing Type in which the associated Lot of shipped items are packed.</br></br>For example: Lot 3 consisting of 35 cans are packed in a box of external length, external width and external height measurements.</br></br> This enables shipped to plan for containerizing shipped items. |
| ShipmentItemConsolidation | Quantity | no | decimal | 9 | The quantity of shipped items in the associated lot. |
| ShipmentItemConsolidation | PackedWidth | no | decimal | 9 | The width of the Packing Type in which the associated Lot of shipped items are packed.</br></br>For example: Lot 3 consisting of 35 cans are packed in a box of external length, external width and external height measurements.</br></br>This enables shipped to plan for containerizing shipped items. |
| ShipmentItemConsolidation | LwhUnitOfMeasureId | no | string | 36 | The unique identifier of a Unit Of Measure. |
| ShipmentItemConsolidation | PackedHeight | no | decimal | 9 | The height of the Packing Type in which the associated Lot of shipped items are packed.</br></br>For example: Lot 3 consisting of 35 cans are packed in a box of external length, external width and external height measurements.</br></br>This enables shipped to plan for containerizing shipped items. |

EOF