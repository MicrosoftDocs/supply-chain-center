---
title: ShipmentRouteLegIOT
description: This article provides information about the ShipmentRouteLegIOT entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# ShipmentRouteLegIOT

The route leg that a shipment transits (already has transited) or is planned to transit and where an IOT device is associated with that route leg.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| ShipmentRouteLegIOT | EventTypeId | yes | string | 36 | Event ID of the shipment |
| ShipmentRouteLegIOT | DeviceId | yes | string | 36 | Device ID of the shipment |
| ShipmentRouteLegIOT | ShipmentId | yes | string | 36 | Shipment Id of the shipment |
| ShipmentRouteLegIOT | ShipmentRouteLegNumber | yes | integer | 9 | Shipment route leg number of the shipment |
| ShipmentRouteLegIOT | ShipmentMMSIId | no | string | 256 | Shipment MMSIID of the shipment |
| ShipmentRouteLegIOT | DeviceMaximumLatitude | no | string | 256 | Device LATITUDE of the shipment |
| ShipmentRouteLegIOT | Humidity | no | string | 256 | Humidity HUMIDITY of the shipment |
| ShipmentRouteLegIOT | LightSensorType | no | string | 256 | Light TYPE of the shipment |
| ShipmentRouteLegIOT | HumidityUnit | no | string | 256 | Humidity UNIT of the shipment |
| ShipmentRouteLegIOT | DeviceMinimumLatitude | no | string | 256 | Device LATITUDE of the shipment |
| ShipmentRouteLegIOT | DeviceTrailerPowerStatus | no | string | 256 | Device STATUS of the shipment |
| ShipmentRouteLegIOT | DeviceChargingStatus | no | string | 256 | Device STATUS of the shipment |
| ShipmentRouteLegIOT | DeviceShipmentState | no | string | 256 | Device STATE of the shipment |
| ShipmentRouteLegIOT | DeviceMaximumLongitude | no | string | 256 | Device LONGITUDE of the shipment |
| ShipmentRouteLegIOT | DeviceMinimumLongitude | no | string | 256 | Device LONGITUDE of the shipment |
| ShipmentRouteLegIOT | SensorTemp | no | string | 256 | Sensor TEMP of the shipment |
| ShipmentRouteLegIOT | SensorTempType | no | string | 256 | Sensor TYPE of the shipment |
| ShipmentRouteLegIOT | SensorTempUnit | no | string | 256 | Sensor UNIT of the shipment |
| ShipmentRouteLegIOT | SensorZoneActiveStatus | no | string | 256 | Sensor STATUS of the shipment |
| ShipmentRouteLegIOT | SensorOperatingMode | no | string | 256 | Sensor MODE of the shipment |
| ShipmentRouteLegIOT | SensorDoorStatus | no | string | 256 | Sensor STATUS of the shipment |
| ShipmentRouteLegIOT | LightSensorUnit | no | string | 256 | Light UNIT of the shipment |
| ShipmentRouteLegIOT | LightSensorValue | no | string | 256 | Light VALUE of the shipment |
| ShipmentRouteLegIOT | TiltSensorType | no | string | 256 | Tilt TYPE of the shipment |
| ShipmentRouteLegIOT | TiltSensorUnit | no | string | 256 | Tilt UNIT of the shipment |
| ShipmentRouteLegIOT | TiltSensorValue | no | string | 256 | Tilt VALUE of the shipment |
| ShipmentRouteLegIOT | DeviceInTransitStatus | no | string | 256 | Device STATUS of the shipment |
| ShipmentRouteLegIOT | DeviceMockStatus | no | string | 256 | Device STATUS of the shipment |
| ShipmentRouteLegIOT | DeviceActivity | no | string | 256 | Device ACTIVITY of the shipment |
| ShipmentRouteLegIOT | DeviceBatteryLevel | no | float | 9 | Device LEVEL of the shipment |
| ShipmentRouteLegIOT | DeviceAccuracy | no | float | 9 | Device ACCURACY of the shipment |
| ShipmentRouteLegIOT | DeviceOnlineModeStatus | no | string | 256 | Device STATUS of the shipment |
| ShipmentRouteLegIOT | DeviceVendorId | no | string | 36 | Device ID of the shipment |
| ShipmentRouteLegIOT | DeviceIMEIId | no | string | 256 | Device IMEIID of the shipment |
| ShipmentRouteLegIOT | DeviceCarrierId | no | string | 36 | Device ID of the shipment |
| ShipmentRouteLegIOT | DeviceAppVersion | no | string | 256 | Device VERSION of the shipment |
| ShipmentRouteLegIOT | DevicePlatform | no | string | 256 | Device PLATFORM of the shipment |
| ShipmentRouteLegIOT | DeviceState | no | string | 256 | Device STATE of the shipment |
| ShipmentRouteLegIOT | DeviceSpeed | no | integer | 9 | Device SPEED of the shipment |
| ShipmentRouteLegIOT | DeviceCep | no | string | 256 | Device CEP of the shipment |
| ShipmentRouteLegIOT | DeviceSignal | no | string | 256 | Device SIGNAL of the shipment |
| ShipmentRouteLegIOT | DeviceDirection | no | string | 256 | Device DIRECTION of the shipment |
| ShipmentRouteLegIOT | DeviceAlarmCode | no | string | 256 | Device CODE of the shipment |
| ShipmentRouteLegIOT | DeviceIgnitionStatus | no | string | 256 | Device STATUS of the shipment |
| ShipmentRouteLegIOT | DeviceBatteryVoltage | no | float | 9 | Device VOLTAGE of the shipment |
| ShipmentRouteLegIOT | DeviceLockFittedStatus | no | string | 256 | Device STATUS of the shipment |
| ShipmentRouteLegIOT | DevicePowerSource | no | string | 256 | Device SOURCE of the shipment |
| ShipmentRouteLegIOT | DeviceUnitModeDetail | no | string | 256 | Device DETAIL of the shipment |
