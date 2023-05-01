---
title: BillOfMaterials
description: This is about BillOfMaterials entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **BillOfMaterials**

A bill of materials (BOM) is a comprehensive list of all the components, parts, materials, and assemblies required to manufacture a product. It serves as a structured document that provides detailed information about each item needed to build or assemble a product.

The BOM includes the following details for each item:
Part number or identifier: A unique identifier for each component.
Quantity: The number of units required for each component.
Unit of measure: The unit in which the quantity is measured (e.g., pieces, meters, kilograms).
Manufacturer and supplier information: The account number or manufacturer number of the component.



|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountId	|	string	|	36	|	No	|	A unique identifier of an account. The account could be a customer or vendor etc. AccountId is an auto generated Id by Microsoft D365 or Supply chain center. 	|
|	AccountNumber	|	string	|	256	|	No	|	Number or code for the account to quickly search and identify the account in system views.	|
|	AccountTypeCode	|	string	|	256	|	No	|	Account type code indicates the type of account. An account could be Vendor, Customer etc.	|
|	BillOfMaterialsId	|	string	|	36	|	Yes	|	Unique id of the bill of materials. This is auto generated Id.	|
|	BillOfMaterialsNumber	|	string	|	256	|	Yes	|	Unique number of the bill of materials. 	|
|	ComponentProductId	|	string	|	36	|	No	|	Unique Id of the component in the bill of material	|
|	ComponentProductNumber	|	string	|	256	|	No	|	Unique number of the component in the bill of material. 	|
|	ComponentQuantity	|	decimal	|		|	No	|	component quantity required to build the product	|
|	ItemInstallationSequence	|	integer	|		|	No	|	Product installation sequence number	|
|	ItemSku	|	string	|	256	|	No	|	Unique number of the product	|
|	LineBillOfMaterialId	|	string	|	256	|	Yes	|	Is the item number of Bill of Materials. 	|
|	ProductId	|	string	|	36	|	No	|	Unique Id of the product	|
|	SubBillOfMaterialId	|	string	|	256	|	No	|	The unique bill of material Id for this component if this component is another bill of material	|
|	UoMId	|	string	|	36	|	No	|	Unit of measure Id	|
|	UoMNumber	|	string	|	256	|	No	|	Unit of measure ISO code	|
|	ValidFromDate	|	date	|		|	No	|	The date by which this record becomes effective. Validity start date of this record	|
|	ValidToDate	|	date	|		|	No	|	The date by which this record expires. Validity end of this record	|
|	WarehouseId	|	string	|	36	|	No	|	Unique id of the warehouse	|
|	WarehouseNumber	|	string	|	256	|	Yes	|	Unique number of the warehouse	|
