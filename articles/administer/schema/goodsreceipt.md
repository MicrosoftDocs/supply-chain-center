---
title: GoodsReceipt
description: This is about GoodsReceipt entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **GoodsReceipt**

The goods receipt entity refers to a document or record that acknowledges the receipt of goods or materials into a specific location or organization. It serves as proof that the goods have been received and accepted. 

Goods receipt entity plays a crucial role in the overall procurement and inventory management cycle. It enables organizations to track and verify the arrival of goods, reconcile them with purchase orders or contracts, update inventory records, and initiate payment processes to suppliers.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountTypeCode	|	string	|	256	|	No	|	Account type code indicates the type of account. An account could be Vendor, Customer etc.	|
|	Company	|	string	|	256	|	No	|	#N/A	|
|	DateReceived	|	date	|		|	No	|	#N/A	|
|	DeliveryAddressCity	|	string	|	256	|	No	|	#N/A	|
|	DeliveryAddressCountryRegionId	|	string	|	256	|	No	|	#N/A	|
|	DeliveryAddressCountyId	|	string	|	256	|	No	|	#N/A	|
|	DeliveryAddressDescription	|	string	|	4000	|	No	|	#N/A	|
|	DeliveryAddressDistrictName	|	string	|	256	|	No	|	#N/A	|
|	DeliveryAddressDunsNumber	|	string	|	256	|	No	|	#N/A	|
|	DeliveryAddressLatitude	|	decimal	|		|	No	|	#N/A	|
|	DeliveryAddressLocationId	|	string	|	256	|	No	|	#N/A	|
|	DeliveryAddressLongitude	|	decimal	|		|	No	|	#N/A	|
|	DeliveryAddressName	|	string	|	256	|	No	|	#N/A	|
|	DeliveryAddressPostbox	|	string	|	256	|	No	|	#N/A	|
|	DeliveryAddressStateId	|	string	|	256	|	No	|	#N/A	|
|	DeliveryAddressStreet	|	string	|	256	|	No	|	#N/A	|
|	DeliveryAddressStreetNumber	|	string	|	256	|	No	|	#N/A	|
|	DeliveryAddressTimezone	|	string	|	256	|	No	|	#N/A	|
|	DeliveryAddressZipcode	|	string	|	256	|	No	|	#N/A	|
|	DeliveryBuildingCompliment	|	string	|	256	|	No	|	#N/A	|
|	DeliveryCityInKana	|	string	|	256	|	No	|	#N/A	|
|	DeliveryStreetInKana	|	string	|	256	|	No	|	#N/A	|
|	DeliveryTerm	|	string	|	256	|	No	|	#N/A	|
|	FormattedDeliveryAddress	|	string	|	256	|	No	|	#N/A	|
|	GoodsReceiptId	|	string	|	36	|	Yes	|	#N/A	|
|	GoodsReceiptNumber	|	string	|	256	|	Yes	|	#N/A	|
|	IsDeliveryAddressPrivate	|	boolean	|		|	No	|	#N/A	|
|	Name	|	string	|	256	|	No	|	#N/A	|
|	Note	|	string	|	4000	|	No	|	#N/A	|
|	OrderAccountNumber	|	string	|	256	|	No	|	#N/A	|
|	OrderVendorId	|	string	|	36	|	No	|	#N/A	|
|	ProcessId	|	string	|	256	|	No	|	#N/A	|
|	PurchaseOrderId	|	string	|	36	|	No	|	#N/A	|
|	PurchaseOrderNumber	|	string	|	256	|	No	|	#N/A	|
|	RecordId	|	string	|	256	|	No	|	#N/A	|
|	RequesterPersonnel	|	string	|	256	|	No	|	#N/A	|
|	ShippingService	|	string	|	256	|	No	|	#N/A	|
|	StageId	|	string	|	256	|	No	|	#N/A	|
