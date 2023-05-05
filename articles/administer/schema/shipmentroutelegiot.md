---
title: ShipmentRouteLegIOT
description: This is about ShipmentRouteLegIOT entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **ShipmentRouteLegIOT**

The route leg that a shipment transits (already has transited) or is planned to transit and where an IOT device is associated with that route leg.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	DeviceAccuracy	|	string	|	256	|	No	|	Device ACCURACY of the shipment	|
|	DeviceActivity	|	string	|	256	|	No	|	Device ACTIVITY of the shipment	|
|	DeviceAlarmCode	|	string	|	256	|	No	|	Device CODE of the shipment	|
|	DeviceAppVersion	|	string	|	256	|	No	|	Device VERSION of the shipment	|
|	DeviceBatteryLevel	|	string	|	256	|	No	|	Device LEVEL of the shipment	|
|	DeviceBatteryVoltage	|	string	|	256	|	No	|	Device VOLTAGE of the shipment	|
|	DeviceCarrierId	|	string	|	256	|	No	|	Device ID of the shipment	|
|	DeviceCep	|	string	|	256	|	No	|	Device CEP of the shipment	|
|	DeviceChargingStatus	|	string	|	4000	|	No	|	Device STATUS of the shipment	|
|	DeviceDirection	|	string	|	256	|	No	|	Device DIRECTION of the shipment	|
|	DeviceIgnitionStatus	|	string	|	4000	|	No	|	Device STATUS of the shipment	|
|	DeviceIMEIId	|	string	|	256	|	No	|	Device IMEIID of the shipment	|
|	DeviceInTransitStatus	|	string	|	4000	|	No	|	Device STATUS of the shipment	|
|	DeviceLockFittedStatus	|	string	|	4000	|	No	|	Device STATUS of the shipment	|
|	DeviceMaximumLatitude	|	decimal	|		|	No	|	Device LATITUDE of the shipment	|
|	DeviceMaximumLongitude	|	decimal	|		|	No	|	Device LONGITUDE of the shipment	|
|	DeviceMinimumLatitude	|	decimal	|		|	No	|	Device LATITUDE of the shipment	|
|	DeviceMinimumLongitude	|	decimal	|		|	No	|	Device LONGITUDE of the shipment	|
|	DeviceMockStatus	|	string	|	256	|	No	|	Device STATUS of the shipment	|
|	DeviceOnlineModeStatus	|	string	|	4000	|	No	|	Device STATUS of the shipment	|
|	DevicePlatform	|	string	|	256	|	No	|	Device PLATFORM of the shipment	|
|	DevicePowerSource	|	string	|	256	|	No	|	Device SOURCE of the shipment	|
|	DeviceShipmentState	|	string	|	256	|	No	|	Device STATE of the shipment	|
|	DeviceSignal	|	string	|	256	|	No	|	Device SIGNAL of the shipment	|
|	DeviceSpeed	|	string	|	256	|	No	|	Device SPEED of the shipment	|
|	DeviceState	|	string	|	256	|	No	|	Device STATE of the shipment	|
|	DeviceTrailerPowerStatus	|	string	|	4000	|	No	|	Device STATUS of the shipment	|
|	DeviceUnitModeDetail	|	string	|	256	|	No	|	Device DETAIL of the shipment	|
|	DeviceUoMId	|	string	|	256	|	No	|	Unit of measure Id	|
|	DeviceUoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
|	DeviceVendorId	|	string	|	256	|	No	|	Device ID of the shipment	|
|	EventTypeId	|	string	|	256	|	No	|	Event ID of the shipment	|
|	Humidity	|	string	|	256	|	No	|	Humidity HUMIDITY of the shipment	|
|	HumidityUoMId	|	string	|	256	|	No	|	Unit of measure Id	|
|	HumidityUoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
|	LightSensorType	|	string	|	256	|	No	|	Light TYPE of the shipment	|
|	LightSensorUnit	|	string	|	256	|	No	|	Light UNIT of the shipment	|
|	LightSensorValue	|	string	|	256	|	No	|	Light VALUE of the shipment	|
|	SensorDoorStatus	|	string	|	4000	|	No	|	Sensor STATUS of the shipment	|
|	SensorOperatingMode	|	string	|	256	|	No	|	Sensor MODE of the shipment	|
|	SensorTemp	|	string	|	256	|	No	|	Sensor TEMP of the shipment	|
|	SensorTempType	|	string	|	256	|	No	|	Sensor TYPE of the shipment	|
|	SensorTempUoMId	|	string	|	256	|	No	|	Unit of measure Id	|
|	SensorTempUoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
|	SensorZoneActiveStatus	|	string	|	4000	|	No	|	Sensor STATUS of the shipment	|
|	ShipmentId	|	string	|	36	|	No	|	Shipment Id of the shipment	|
|	ShipmentMMSIId	|	string	|	256	|	No	|	Shipment MMSIID of the shipment	|
|	ShipmentNumber	|	string	|	256	|	No	|	Shipment number associated with shipment route leg IOT	|
|	ShipmentRouteLegIOTId	|	string	|	36	|	Yes	|	The unqiue Id of the shipment route leg IOT	|
|	ShipmentRouteLegIOTNumber	|	string	|	256	|	Yes	|	The unique number of the shipment route leg IOT	|
|	ShipmentRouteLegNumber	|	string	|	256	|	No	|	Shipment route leg number of the shipment	|
|	TiltSensorType	|	string	|	256	|	No	|	Tilt TYPE of the shipment	|
|	TiltSensorUoMId	|	string	|	256	|	No	|	Unit of measure Id	|
|	TiltSensorUoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
|	TiltSensorValue	|	string	|	256	|	No	|	Tilt VALUE of the shipment	|
