# ShipmentRouteLeg

The route leg that a shipment transits (already has transited) or is planned to transit. Note that a shipment route can be changed or modified and then the leg may have a status of:

- Leg Planned
- Leg Scheduled
- Leg Modified From Original Planned Leg
- Leg Completed

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ShipmentRouteLeg | ShipmentLegNumber | yes | integer | 9 | The unique identifier of the Shipment Leg Number, which equals the shipment leg 'sequence number'. |
| ShipmentRouteLeg | ShipmentId | yes | string | 36 | The unique identifier of a Shipment. |
| ShipmentRouteLeg | PlannedVesselDepartureTimestamp | no | timestamp | 14 | The scheduled departure timestamp. |
| ShipmentRouteLeg | PlannedVesselId | no | string | 36 | The unique identifier of a vessel/ship. |
| ShipmentRouteLeg | ActualVesselId | no | string | 36 | The unique identifier of a vessel/ship. |
| ShipmentRouteLeg | PlannedSailingSegmentNumber | no | integer | 9 | The ordered segment number associated with this segment (leg) of the sailing schedule. |
| ShipmentRouteLeg | ActualFlightLegArrivalAirportCode | no | string | 3 | AKA Airport Code</br></br>Three-letter codes used to identify airports.</br></br>Airport Code</br></br>The airport code is a three letter designator for a commercial airport, or other travel point -- For example a large bus station. These are the codes that airlines and pilots use to identify airports and are used in timetables, baggage tags, tickets, advertisements, Airline and Global Reservation Systems. There are approximately 9,000 of them in use of a total of 17,576 available |
| ShipmentRouteLeg | ActualFlightNumber | no | string | 36 | The unique identifier of a Flight. |
| ShipmentRouteLeg | ActualCarrierId | no | string | 36 | The unique identifier of a Carrier. |
| ShipmentRouteLeg | ActualFlightLegDepartureAirportCode | no | string | 3 | AKA Airport Code</br></br>Three-letter codes used to identify airports.</br></br>Airport Code</br></br>The airport code is a three-letter designator for a commercial airport, or other travel point, for example a large bus station. These are the codes that airlines and pilots use to identify airports and are used in timetables, baggage tags, tickets, advertisements, Airline and Global Reservation Systems. There are approximately 9,000 of them in use of a total of 17,576 available |
| ShipmentRouteLeg | ActualFlightDate | no | date | 14 | The date of the Flight. |
| ShipmentRouteLeg | ActualVesselDepartureTimestamp | no | timestamp | 14 | The scheduled departure timestamp. |
| ShipmentRouteLeg | ActualTrainId | no | string | 36 | The unique identifier of a Train. |
| ShipmentRouteLeg | PlannedTrainLegNumber | no | integer | 9 | The leg number of the train schedule. |
| ShipmentRouteLeg | ActualTrainLegNumber | no | integer | 9 | The leg number of the train schedule. |
| ShipmentRouteLeg | ActualTrainDepartureTimestamp | no | timestamp | 14 | The scheduled departure timestamp. |
| ShipmentRouteLeg | PlannedTrainDepartureTimestamp | no | timestamp | 14 | The scheduled departure timestamp. |
| ShipmentRouteLeg | PlannedVehicleId | no | string | 36 | The unique identifier of a Vehicle. |
| ShipmentRouteLeg | PlannedTowId | no | string | 36 | The unique identifier of a Train. |
| ShipmentRouteLeg | PlannedTrainId | no | string | 36 | The unique identifier of a Train. |
| ShipmentRouteLeg | ActualVehicleId | no | string | 36 | The unique identifier of a Vehicle. |
| ShipmentRouteLeg | PlannedFlightLegArrivalAirportCode | no | string | 3 | AKA Airport Code</br></br>Three-letter codes used to identify airports.</br></br>Airport Code</br></br>The airport code is a three letter designator for a commercial airport, or other travel point for example a large bus station. These are the codes that airlines and pilots use to identify airports and are used in timetables, baggage tags, tickets, advertisements, Airline and Global Reservation Systems. There are approximately 9,000 of them in use of a total of 17,576 available |
| ShipmentRouteLeg | ShipmentLegToLocationId | no | string | 36 | The unique identifier of the To-Location. |
| ShipmentRouteLeg | ShipmentLegFromLocationId | no | string | 36 | The unique identifier of the From-Location. |
| ShipmentRouteLeg | PlannedLatestPickUpTimestamp | no | timestamp | 14 | The latest that the shipment items can be picked-up. |
| ShipmentRouteLeg | PlannedEarliestPickUpTimestamp | no | timestamp | 14 | The earliest that the shipment items can be picked up. |
| ShipmentRouteLeg | RouteLegTypeId | no | string | 36 | The unique identifier of a Route Leg Type. |
| ShipmentRouteLeg | CarrierId | no | string | 36 | The unique identifier of a Carrier. |
| ShipmentRouteLeg | ShipmentMethodName | no | string | 256 | The unique identifier of a Shipment Method. |
| ShipmentRouteLeg | CarrierRouteLegNumber | no | integer | 9 | The assigned to the Carrier Route Leg. |
| ShipmentRouteLeg | CarrierRouteId | no | string | 36 | The unique identifier of a Carrier Route. |
| ShipmentRouteLeg | PlannedEarliestDeliveryTimestamp | no | timestamp | 9 | The earliest that the shipment items can be delivered. |
| ShipmentRouteLeg | PlannedFlightNumber | no | string | 36 | The unique identifier of a Flight. |
| ShipmentRouteLeg | PlannedCarrierId | no | string | 36 | The unique identifier of a Carrier. |
| ShipmentRouteLeg | PlannedFlightLegDepartureAirportCode | no | string | 3 | AKA Airport Code</br></br> Three-letter codes used to identify airports.</br></br>Airport Code</br></br>The airport code is a three letter designator for a commercial airport, or other travel point for example a large bus station. These are the codes that airlines and pilots use to identify airports and are used in timetables, baggage tags, tickets, advertisements, Airline and Global Reservation Systems. There are approximately 9,000 of them in use of a total of 17,576 available |
| ShipmentRouteLeg | PlannedFlightDate | no | date | 14 | The date of the Flight. |
| ShipmentRouteLeg | ActualArrivalTimestamp | no | timestamp | 14 | The actual arrival timestamp. |
| ShipmentRouteLeg | PlannedDepartureTimestamp | no | timestamp | 14 | The planned departure timestamp. |
| ShipmentRouteLeg | PlannedLatestDeliveryTimestamp | no | timestamp | 14 | The latest that the shipment items can be delivered. |
| ShipmentRouteLeg | ActualDepartureTimestamp | no | timestamp | 14 | The actual departure timestamp. |
| ShipmentRouteLeg | PlannedArrivalTimestamp | no | timestamp | 14 | The planned arrival timestamp. |
