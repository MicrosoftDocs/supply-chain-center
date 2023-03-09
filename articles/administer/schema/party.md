---
title: Party
description: This article provides information about the Party entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# Party

A party is an individual, organization, legal entity, social organization or business unit of interest to the business. Party is a concept that enables individuals, organizations, legal entities, social organization and business units to be related or defined with the context of roles, events and relationships. This enables us to 'anchor' disparate instances or implementations of each of the above to a common or singular instance of that individual, organization, legal entity, social organization or business unit.

For example, a large business has 20 customer masters that are used internally. PARTY enables the organization to identify and define each customer as a single party and relate (cleanse and synchronize) the multiple instances of customer to a single set of customer information. It also allows the business to look at the multiple relationships that exist among parties playing different roles over various periods of time.

For example, a business might have a vendor who is also a customer that has employees who are also customers of the business. A business might have employees who are also customers and whose spouse or family members are also customers.

In short, party enables the business to examine and record the real-world interactions of individuals, organizations, legal entities, social organizations and business units as they perform those many roles that characterize their activities and relationships to other parties. Party also provides an 'anchor' upon which to resolve multiple instances or definitions of that party so the business can develop a 'single-view' of the party.

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| Party | PartyId | yes | string | 36 | The unique identifier of a Party. |
| Party | GlobalLocationNumber | no | decimal | 15 | The Global Location Number (GLN) is a simple tool used to uniquely identify locations. It can be used to identify physical locations such as a warehouse, legal entities, or a function / department within a legal entity. The GLN is part of the GS1 system of standards. |
| Party | PartyTypeId | no | string | 36 | The unique identifier of a Party Type. |
| Party | PartyName | no | string | 128 | The name of the Party. |
