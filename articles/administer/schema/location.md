---
title: Location
description: This article provides information about the Location entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# Location

A location is a physical point that can be defined as a single latitude / longitude. A location can be used to describe:

- The address of a physical structure.
- The location of a business or service.
- The location of a component.
- The delivery location for a shipment or mai.l

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| Location | LocationId | yes | string | 36 | The unique identifier of a Location. |
| Location | LocationPostalCode | no | string | 1024 | The unique identifier of a Postal Code. |
| Location | LocationLongitude | no | decimal | 15 | The location east or west in reference to the Prime Meridian, which is designated as zero (0) degrees longitude. The distance between lines of longitude are greater at the equator and smaller at the higher latitudes, intersecting at the earth's North and South Poles. Time zones are correlated to longitude.</br></br>Longitude is often measured in degrees, minutes, seconds (ddd mm ss), but other formats are also commonly used: gps coordinate (ddd mm.mmmm), decimal degrees (ddd.dddd). |
| Location | LocationLatitude | no | decimal | 15 | The location north or south in reference to the equator, which is designated at zero (0) degrees. Parallel lines that circle the globe both north and south of the equator.</br></br>Latitude is often measured in degrees, minutes, seconds (ddd mm ss), but other formats are also commonly used: gps coordinate (ddd mm.mmmm), decimal degrees (ddd.dddd). |
| Location | LocationAddressLine2 | no | string | 512 | The 'street' component of a location. Includes street name, apartment, suite number or PO Box. |
| Location | LocationCity | no | string | 128 | The 'city' component of a location. |
| Location | LocationStateId | no | string | 256 | The unique identifier of the State = State Code.</br></br>A two-digit FIPS code assigned by the NIST to identify each State and statistically equivalent entity. The NIST assigns the codes based on the alphabetic sequence of State names (Puerto Rico and the Outlying Areas appear at the end); it documents these codes in a FIPS publication (FIPS PUB 5). Also, a two-digit code assigned by the Census Bureau to identify each State within its census geographic division (Puerto Rico and the Outlying Areas appear at the end). |
| Location | TimezoneId | no | string | 36 | The unique identifier of a time zone. |
| Location | DaylightSavingsTimeObservedIndicator | no | boolean | 10 | Indicates whether daylight savings time (DST) is observed at this location. |
| Location | CountryId | no | string | 256 | The unique identifier of the Country. |
| Location | GlobalLocationNumber | no | decimal | 15 | The Global Location Number (GLN) is a simple tool used to uniquely identify locations. It can be used to identify physical locations such as a warehouse, legal entities, or a function / department within a legal entity. The GLN is part of the GS1 system of standards. |
| Location | LocationDatum | no | string | 5 | Latitude and longitude are based on a datum. A datum is a reference point, surface or axis against which measurements are made.</br></br>Different datums can be used for determining the latitude and longitude. If different datums are used the latitude and longitude for a single point (location) may be different.</br></br>WGS 84 is a datum that is used on most GPS equipment. |
| Location | LocationElevation | no | integer | 10 | The distance above sea level of this location at ground level. |
| Location | LocationElevationUnitOfMeasureId | no | string | 36 | The elevation unit of measurement. |
| Location | LocationAddressLine1 | no | string | 512 | The 'street' component of a location. Includes street name, apartment, suite number or PO Box. |
| Location | LocationName | no | string | 128 | The name of a location. |
| Location | LocationDescription | no | string | 512 | The description of a location. |

EOF