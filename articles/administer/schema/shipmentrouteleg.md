---
title: ShipmentRouteLeg
description: This is about ShipmentRouteLeg entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **ShipmentRouteLeg**

A shipment route leg entity refers to a specific segment or part of a transportation route for a shipment or cargo. In logistics and supply chain management, a shipment route typically consists of multiple legs or stages through which the goods are transported from the point of origin to the destination. Each leg represents a distinct portion of the overall journey, often involving different modes of transportation or transit points.

The shipment route leg entity contains information about a particular leg, such as the starting point, ending point, transit points, transportation mode (e.g., road, rail, air, sea), estimated or actual departure and arrival times, distance covered, and any specific requirements or constraints for that leg. It may also include details about carriers or service providers responsible for that leg, relevant documents, tracking information, and associated costs.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	ActualArrivalTimestamp	|	timestamp	|		|	No	|	The actual arrival timestamp.	|
|	ActualDepartureTimestamp	|	timestamp	|		|	No	|	The actual departure timestamp.	|
|	ActualFlightDate	|	date	|		|	No	|	The date of the Flight.	|
|	ActualFlightLegArrivalAirportCode	|	string	|	256	|	No	|	AKA Airport Code

Three-letter codes used to identify airports.

Airport Code 
The airport code is a three letter designator for a commercial airport, or other travel point -- e.g. a large bus station. These are the codes that airlines and pilots use to identify airports and are used in timetables, baggage tags, tickets, advertisements, Airline and Global Reservation Systems. There are approximately 9,000 of them in use of a total of 17,576 available	|
|	ActualFlightLegDepartureAirportCode	|	string	|	256	|	No	|	AKA Airport Code

Three-letter codes used to identify airports.

Airport Code 
The airport code is a three letter designator for a commercial airport, or other travel point -- e.g. a large bus station. These are the codes that airlines and pilots use to identify airports and are used in timetables, baggage tags, tickets, advertisements, Airline and Global Reservation Systems. There are approximately 9,000 of them in use of a total of 17,576 available	|
|	ActualFlightNumber	|	string	|	256	|	No	|	The unique identifier of a Flight.	|
|	ActualShipmentCarrierId	|	string	|	256	|	No	|	Carrier Id of the shipment route leg	|
|	ActualShipmentCarrierNumber	|	string	|	256	|	No	|	Actual shipment carrier number of the shipment route leg	|
|	ActualTrainDepartureTimestamp	|	timestamp	|		|	No	|	The scheduled departure timestamp.	|
|	ActualTrainId	|	string	|	256	|	No	|	The unique identifier of a Train.	|
|	ActualTrainLegNumber	|	string	|	256	|	No	|	The leg number of the train schedule.	|
|	ActualVehicleId	|	string	|	256	|	No	|	The unique identifier of a Vehicle.	|
|	ActualVesselDepartureTimestamp	|	timestamp	|		|	No	|	The scheduled departure timestamp.	|
|	ActualVesselId	|	string	|	256	|	No	|	The unique identifier of a vessel/ship.	|
|	CarrierId	|	string	|	36	|	No	|	The unique identifier of a Carrier.	|
|	CarrierNumber	|	string	|	256	|	No	|	Carrier number of the shipment route leg	|
|	CarrierRouteId	|	string	|	256	|	No	|	The unique identifier of a Carrier Route.	|
|	CarrierRouteLegNumber	|	string	|	256	|	No	|	The assigned to the Carrier Route Leg.	|
|	CarrierRouteNumber	|	string	|	256	|	No	|	Carrier route number for this shipment route leg	|
|	PlannedArrivalTimestamp	|	timestamp	|		|	No	|	The planned arrival timestamp.	|
|	PlannedDepartureTimestamp	|	timestamp	|		|	No	|	The planned departure timestamp.	|
|	PlannedEarliestDeliveryTimestamp	|	timestamp	|		|	No	|	The earliest that the shipment items can be delivered.	|
|	PlannedEarliestPickUpTimestamp	|	timestamp	|		|	No	|	The earliest that the shipment items can be picked up.	|
|	PlannedFlightDate	|	date	|		|	No	|	The date of the Flight.	|
|	PlannedFlightLegArrivalAirportCode	|	string	|	256	|	No	|	AKA Airport Code

Three-letter codes used to identify airports.

Airport Code 
The airport code is a three letter designator for a commercial airport, or other travel point -- e.g. a large bus station. These are the codes that airlines and pilots use to identify airports and are used in timetables, baggage tags, tickets, advertisements, Airline and Global Reservation Systems. There are approximately 9,000 of them in use of a total of 17,576 available	|
|	PlannedFlightLegDepartureAirportCode	|	string	|	256	|	No	|	AKA Airport Code

Three-letter codes used to identify airports.

Airport Code 
The airport code is a three letter designator for a commercial airport, or other travel point -- e.g. a large bus station. These are the codes that airlines and pilots use to identify airports and are used in timetables, baggage tags, tickets, advertisements, Airline and Global Reservation Systems. There are approximately 9,000 of them in use of a total of 17,576 available	|
|	PlannedFlightNumber	|	string	|	256	|	No	|	The unique identifier of a Flight.	|
|	PlannedLatestDeliveryTimestamp	|	timestamp	|		|	No	|	The latest that the shipment items can be delivered.	|
|	PlannedLatestPickUpTimestamp	|	timestamp	|		|	No	|	The latest that the shipment items can be picked-up.	|
|	PlannedSailingSegmentNumber	|	string	|	256	|	No	|	The ordered segment number associated with this segment (leg) of the sailing schedule.	|
|	PlannedShippingCarrierId	|	string	|	256	|	No	|	Planned shipping carrier Id of the shipment route leg	|
|	PlannedShippingCarrierNumber	|	string	|	256	|	No	|	Planned shipping carrier number of the shipment route leg	|
|	PlannedTowNumber	|	string	|	256	|	No	|	Planned tow number of the shipment route leg	|
|	PlannedTrainDepartureTimestamp	|	timestamp	|		|	No	|	The scheduled departure timestamp.	|
|	PlannedTrainId	|	string	|	256	|	No	|	The unique identifier of a Train.	|
|	PlannedTrainLegNumber	|	string	|	256	|	No	|	The leg number of the train schedule.	|
|	PlannedTrainNumber	|	string	|	256	|	No	|	Train number of the shipment route leg	|
|	PlannedVehicleId	|	string	|	256	|	No	|	The unique identifier of a Vehicle.	|
|	PlannedVehicleNumber	|	string	|	256	|	No	|	Planned vessel number of the shipment route leg	|
|	PlannedVesselDepartureTimestamp	|	timestamp	|		|	No	|	The scheduled departure timestamp.	|
|	PlannedVesselId	|	string	|	256	|	No	|	The unique identifier of a vessel/ship.	|
|	PlannedVesselNumber	|	string	|	256	|	No	|	Vessel number of the shipment route leg	|
|	RouteLegTypeId	|	string	|	256	|	No	|	The unique identifier of a Route Leg Type.	|
|	RouteLegTypeNumber	|	string	|	256	|	No	|	The unique number of shipment route leg type	|
|	ShipmentId	|	string	|	36	|	No	|	The unique identifier of a Shipment.	|
|	ShipmentLegFromGeoLocationId	|	string	|	36	|	No	|	The unique identifier of a Location. This is autogenerated by Supply chain center or D365 applications	|
|	ShipmentLegFromGeoLocationNumber	|	string	|	256	|	No	|	The unique number of a location. This is a referenced in an external system to identify the unique location	|
|	ShipmentLegToGeoLocationId	|	string	|	36	|	No	|	The unique identifier of a Location. This is autogenerated by Supply chain center or D365 applications	|
|	ShipmentLegToGeoLocationNumber	|	string	|	256	|	No	|	The unique number of a location. This is a referenced in an external system to identify the unique location	|
|	ShipmentMethodName	|	string	|	256	|	No	|	The unique identifier of a Shipment Method.	|
|	ShipmentNumber	|	string	|	256	|	No	|	The shipment number for the shipment route leg	|
|	ShipmentRouteLegId	|	string	|	36	|	Yes	|	The unique Id of the shipment route leg	|
|	ShipmentRouteLegNumber	|	string	|	256	|	Yes	|	The unique number of the shipment route leg	|
