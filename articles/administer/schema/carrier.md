---
title: Carrier
description: This article provides information about the Carrier entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **Carrier**

A company or corporation engaged in transporting passengers or goods (mail, freight, or cargo). Any entity who, in a contract of carriage, undertakes to perform or to procure the performance of carriage by rail, road, sea, air, inland waterway or by a combination of such modes.

For example, United Airlines, Air Canada, Aer Lingus, UPS, Federal Express, US Postal Service, DHL, JB Hunt, Yellow Freight, American President Lines, and Maersk-Sealand.

You can identify Carriers using their two or three character abbreviation. For example, AK for Alaska airlines. They're also identified by Standard Carrier Alpha Code (commonly known as SCAC code).


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountCode	|	string	|	256	|	No	|	The account number or contract number with the carrier.	|
|	CarrierCode	|	string	|	256	|	No	|	Carrier code.	|
|	CarrierId	|	string	|	36	|	Yes	|	The unique identifier of a Carrier.	|
|	CarrierNumber	|	string	|	256	|	Yes	|	The unique number of the carrier, used for searching.	|
|	CarrierTypeId	|	string	|	256	|	No	|	The unique identifier of a Carrier Type.	|
|	CommonCarrierIndicator	|	string	|	256	|	No	|	A transportation company that provides service to the general public at published rates.	|
|	CustomAttributes	|	string	|	256	|	No	|	Customer defined attributes for the carrier.	|
|	DirectAirCarrierIndicator	|	string	|	256	|	No	|	An air carrier that operates airplanes on a scheduled or contract (charter) basis, or both, and provides transportation for a charge. An airline as opposed to a freight forwarder.	|
|	DunBradstreetGlobalUltimate	|	string	|	256	|	No	|	There are eight types of business relationships defined in D&B WorldBase. |

## Single Location Subsidiary

A single location subsidiary has reporting responsibilities to its parent; however, it doesn't have branches or subsidiaries reporting to it. Don't confuse a single location subsidiary with a stand-alone business which is titled "single location" and isn't part of a corporate family.

## Headquarters

Headquarters are a business establishment that has branches or divisions reporting to it and is financially responsible for those branches or divisions. If the headquarters is more that 50% owned by another corporation, it's also a subsidiary. If it owns more than 50% of another corporation, then its also considered a parent.

## Branch

A branch is a secondary location for its headquarters. It has no legal responsibility for its debts, even though bills may be paid from the branch location. It has the same legal business name as its headquarters, although branches frequently operate under a different trade style than the headquarters. A branch may be located at the same address as the headquarters if it has a unique trade style. In such cases, the branch may appear to be a duplicate with a different D-U-N-S number than the headquarters record, which may confuse customers if they don't purchase the trade style field.

## Division

A division, like a branch, is a secondary location of a business. However, a division carries out specific business operations related to the headquarters under a divisional name. Divisions look like branches in D&B WorldBase and carry a branch code.

## Subsidiary

A subsidiary is a corporation that is more than 50% owned by another corporation and has a different legal business name from its parent company. A subsidiary may have branches and/or subsidiaries of its own. If it does, then its D-U-N-S Number appears in the headquarter/parent D-U-N-S Number field of its children.

## Parent

A parent is a corporation that owns more than 50 percent of another corporation. The parent company may also be a subsidiary of another corporation. If the parent also has branches, then its also considered headquarters.

## Domestic Ultimate

The Domestic Ultimate is a subsidiary within the global family tree which is the highest ranking member within a specific country.

## Global Ultimate

Global Ultimate is the top most responsible entity within the global family tree. Global Ultimate may have branches and/or subsidiaries reporting directly or indirectly to it.

|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	DunBradstreetUltimate	|	string	|	256	|	No	|	There are eight (8) types of business relationships defined in D&B WorldBase|

## Single Location Subsidiary

A single location subsidiary has reporting responsibilities to its parent; however, it doesn't have branches or subsidiaries reporting to it. Don't confuse this with a stand-alone business which is titled "single location" and isn't part of a corporate family.

## Headquarters

Headquarters is a business establishment that has branches or divisions reporting to it, and is financially responsible for those branches or divisions. If the headquarters is more that 50% owned by another corporation, it's also a subsidiary. If it owns more than 50% of another corporation, then it's also a parent.

## Branch

A branch is a secondary location for its headquarters. It has no legal responsibility for its debts, even though bills may be paid from the branch location. It has the same legal business name as its headquarters, although branches frequently operate under a different trade style than the headquarters. A branch may be located at the same address as the headquarters if it has a unique trade style. In such cases, the branch may appear to be a duplicate with a different D-U-N-S number than the headquarters record, which may confuse customers if they don't purchase the trade style field.

## Division

A division, like a branch, is a secondary location of a business. However, a division carries out specific business operations related to the headquarters under a divisional name. Divisions look like branches in D&B WorldBase and carry a branch code.

## Subsidiary

A subsidiary is a corporation that is more than 50% owned by another corporation and has a different legal business name from its parent company. A subsidiary may have branches and/or subsidiaries of its own. If it does, then its D-U-N-S Number appears in the headquarters/parent D-U-N-S Number field of its children.

## Parent

A parent is a corporation that owns more than 50 percent of another corporation. The parent company may also be a subsidiary of another corporation. If the parent also has branches, then it's also considered headquarters.

## Domestic Ultimate

The Domestic Ultimate is a subsidiary within the global family tree that is the highest ranking member within a specific country.

## Global Ultimate

Global Ultimate is the top most responsible entity within the global family tree. Global Ultimate may have branches and/or subsidiaries reporting directly or indirectly to it.	

|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	FaaIdentificationNumber	|	string	|	256	|	No	|	A unique identifier given to an air carrier by the FAA once they have successfully completed a security training program.	|
|	FirstOperationDate	|	date	|		|	No	|	The date that the Carrier was first in operation.	|
|	IataAirlineDesignator	|	string	|	256	|	No	|	The IATA three-number airline accounting code and airline prefix code. As per the provisions of IATA Resolution 767, a company may qualify for:</br>
   * A three-numeric airline accounting code for use on passenger traffic documents if engaged in providing passenger transportation services only.</br>
   * A three-numeric airline prefix code for use on cargo traffic documents if providing cargo transportation services only.</br>
   * An identical three-numeric airline accounting code and a three-numeric airline prefix code if providing both passenger and cargo transportation services.	</br>|
|	IataCarrierIndicator |	string	|	256	|	No	|	An airline that is a member of IATA and may accept, carry, and bill for air shipments. Intra-US counterpart is ATA.	|
|	IcaoAirlineDesignator	|	string	|	256	|	No	|	The ICAO airline designator is a code that is assigned by the International Civil Aviation Organization (ICAO) to an aircraft operating agencies, aeronautical authorities, and services related to international aviation, each are allocated both a three-letter designator and a telephony designator. These codes are unique by airline, unlike the IATA airline designator codes (see section above). The designators are listed in ICAO Document 8585: Designators for Aircraft Operating Agencies, Aeronautical Authorities and Services. </br>
An example is:</br>
Operator: American Airlines Three-letter designator: AAL (the original ICAO-two-letter-designator AA was used until 1987 and is also the IATA code of the airline)</br>
Telephony designator: AMERICAN |
|	IntegratedCarrierIndicator	|	string	|	256	|	No	|	A carrier that provides door-to-door air cargo transportation using its own or contracted airplanes and motor trucks, and performs this service under the authority of a singe air waybill. For example, United Parcel Service and Federal Express.	|
|	IsBroker	|	boolean	|		|	No	|	Is the carrier a broker	|
|	ModeCode	|	string	|	256	|	No	|	Preferred carrier mode code	|
|	Name	|	string	|	256	|	No	|	The name of the carrier	|
|	PronumberCode	|	string	|	256	|	No	|	Unique pronumber code	|
|	ScacCommonCarrierCode	|	string	|	256	|	No	|	Standard Carrier Abbreviation Code identifying an individual common carrier. A three letter carrier code followed by a suffix identifies the carrier's equipment. A suffix of "U" is a container and "C" is a chassis.	|
|	TrackingBaseURL	|	string	|	256	|	No	|	URL for shipment tracking	|
|	UnapprovedIndirectAirCarrierIndicator	|	string	|	256	|	No	|	An indirect air carrier who hasn't completed the FAA security training program and doesn't have an FAA identification number.	|
|	Website	|	string	|	256	|	No	|	URL of the carrier	|
