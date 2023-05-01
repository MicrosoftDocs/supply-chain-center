---
title: FreightTerms
description: This is about FreightTerms entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **FreightTerms**

Freight terms entity refers to shipping terms or delivery terms. It refers to the conditions and responsibilities associated with the transportation of goods from one location to another. These terms define who is responsible for various aspects of the shipment, such as transportation costs, insurance, and risk of loss or damage.

Some commonly used freight terms include:

Ex Works (EXW): The seller makes the goods available at their premises, and the buyer is responsible for all transportation costs and risks.

Free Carrier (FCA): The seller delivers the goods to a carrier or a named location specified by the buyer. The buyer assumes responsibility once the goods are handed over to the carrier.

Free Alongside Ship (FAS): The seller delivers the goods to a port or a dock, and the buyer takes responsibility from that point onward, including loading costs and risks.

Free on Board (FOB): The seller is responsible for delivering the goods to a named port of shipment, and the buyer assumes responsibility once the goods are on board the vessel.

Cost and Freight (CFR): The seller pays for the transportation of the goods to the destination port, while the buyer is responsible for insurance and other costs from the port onward.

Cost, Insurance, and Freight (CIF): Similar to CFR, but the seller also provides insurance coverage for the goods during transportation.

Delivered at Place (DAP): The seller is responsible for delivering the goods to a specified location, excluding import clearance and any applicable taxes or duties.

Delivered Duty Paid (DDP): The seller is responsible for delivering the goods to the buyer's location, including import clearance and all taxes or duties.

|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	Company	|	string	|	256	|	No	|	#N/A	|
|	DoRetailSogetTransportationChargesAdded	|	string	|	256	|	No	|	#N/A	|
|	FreightChargeTerms	|	string	|	4000	|	No	|	#N/A	|
|	FreightTermsId	|	string	|	36	|	Yes	|	#N/A	|
|	FreightTermsNumber	|	string	|	256	|	Yes	|	#N/A	|
|	IntraStatCode	|	string	|	256	|	No	|	#N/A	|
|	IsCashOnDelivery	|	boolean	|		|	No	|	#N/A	|
|	SalesTaxLocationRole	|	string	|	256	|	No	|	#N/A	|
|	TermsCode	|	string	|	256	|	No	|	#N/A	|
|	TermsDescription	|	string	|	4000	|	No	|	#N/A	|
|	WillShipmentConfirmationTransferCharges	|	boolean	|		|	No	|	#N/A	|
