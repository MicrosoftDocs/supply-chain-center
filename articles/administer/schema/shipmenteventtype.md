---
title: ShipmentEventType
description: This article provides information about the ShipmentEventType entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# ShipmentEventType

A type of event that may be associated with a Shipment for a period of time or a point in time. For example: Abandonment, Area check, Break Bulk, Customs Entry, Customs Exit, Detention, Devanning, Embargo, In Bond, In Customs, In-Transit Entry, Lay Order, Shipment Aboard, and Shipment Alongside.

ABANDONMENT: A proceeding wherein a shipper/consignee seeks authority to abandon all or parts of their cargo.

AREACHECK: A request to physically look for cargo in the cargo terminal warehouse. This term is used when tracing cargo. It may also be referred to as a floorcheck.

BREAK BULK: Disassembling or unpacking a consolidated shipment for delivery or for reconsignment. To 'breakbulk' is to unload packaged cargo from a 'breakbulk ship' or from a container and to distribute it.

CUSTOMS ENTRY: The shipment has enter customs processing.

CUSTOMS EXIT: The shipment has exited or completed customs.

DETENTION: A penalty charge against shippers or consignees for delaying carrier's equipment beyond allowed time. Demurrage applies to cargo; detention applies to equipment. See Per Diem.

DEVANNING: The removal of cargo from a container. Also known as unstuffing, unloading or stripping.

EMBARGO

Temporary refusal to accept cargo for transportation at certain points or in certain routes due to the type or class of cargo, limitations of facilities, emergencies, or other abnormal circumstances.

IN BOND

As applied to air freight coming into the United States, the term ""in Bond"" refers to a procedure under U.S. Customs rules where the clearance of cargo is postponed until the cargo reaches an inland Customs point rather than subjecting the cargo to clearance procedures at the first arriving U.S. gateway airport where process might be more time consuming. The procedure is so named because the cargo moves under the carrier's bond (financial liability assured by the carrier) from the gateway airport and remains In Bond until Customs releases the cargo at the inland Customs point (airport).

IN CUSTOMS

The shipment is in customs, which is the government service which is responsible for the administration of Customs law and the collection of duties and taxes relating thereto, and which has responsibility for the application of other laws and regulations relative to the importation, transit, and exportation of goods.

INBOND

A term applied to air cargo coming into the USA. This designates a procedure under which U.S. Customs' clearance of cargo is postponed until the cargo reaches an inland customs point rather than at congested gateway cities. Cargo moves under the carrier's bond (posted with U.S. Customs) from the gateway to the inland customs port.

IN-QUARANTINE

A restraint placed on an operation to protect the public against a health hazard. A ship may be quarantined so that it cannot leave a protected point. During the quarantine period, the Q flag is hoisted.

IN-TRANSIT CLEANING

The stopping of articles, such as peanuts, etc., for cleaning at a point between the point of origin and destination.

IN-TRANSIT ENTRY

Allows foreign merchandise arriving at one port to be transported in bond to another port, where a superseding entry is filed.

LAY ORDER

The period during which imported merchandise may remain at the place of unloading without some action being taken for its disposition.

NO SHOW

Shipper who fails to show up to ship an already booked shipment. Also, a shipment which fails to show up at destination off a flight.

OFFLOAD

Removing the cargo from the aircraft.

ON-HAND

Cargo is confirmed at a particular airport and available for the customer to pick up.

SHIPMENT ABOARD

Referring to cargo being put, or laden, onto a means of conveyance.

SHIPMENT ALONGSIDE

A phrase referring to the side of a ship. Goods delivered alongside are to be placed on the dock or barge within reach of the transport ship's tackle so that they can be loaded.

SHIPMENT CONSOLIDATION

The combining of smaller shipments into a single shipment that is sent to a destination point.

The reorganization of corporations to combine two or more into a successor corporation.

In order to handle small lot of consignment efficiently and competitively, freight forwarders usually put many consignments into one lot then tender to carrier for forwarding. In this case, each consignment will be shipped with one HAWB respectively and In order to handle small lot of consignment efficiently and competitively, freight forwarder usually put many consignments into one lot then tender to carrier for forwarding. In this case, each consignment will be shipped with one HAWB respectively.

TERMINATED/PICKUP

The consignee has retrieved cargo from the airport.

VANNING

A term sometimes used for stowing cargo in a container."

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ShipmentEventType | ShipmentEventTypeId | yes | string | 36 | The unique identifier of a Shipment Event Type. |
| ShipmentEventType | ShipmentEventTypeDescription | no | string | 512 | The description of a Shipment Event Type. |
| ShipmentEventType | ShipmentEventTypeName | no | string | 128 | The name of a Shipment Event Type.. |
