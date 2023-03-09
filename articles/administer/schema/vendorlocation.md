---
title: VendorLocation
description: This article provides information about the VendorLocation entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 11/3/2022
ms.custom: bap-template
---

# VendorLocation

The Vendor location(s) of the associated Location Type for the indicated period.

For example:

- Headquarters
- Boston Office
- Support
- Marketing
- Legal
- Mail-To
- Ship-To
- Legal Documentation-To

| **Entity Name** | **Attribute Name** | **IsPrimaryKey** | **Data Type** | **Data Length** | **Description** |
| --- | --- | --- | --- | --- | --- |
| VendorLocation | LocationTypeId | yes | string | 36 | The unique identifier of a Location Type. |
| VendorLocation | PeriodStartTimestamp | yes | timestamp | 14 | The period start timestamp associated with the information. |
| VendorLocation | VendorId | yes | string | 36 | The unique identifier of a Vendor. |
| VendorLocation | VendorLocationId | yes | string | 36 | The unique identifier of a Location. |
| VendorLocation | HoldDate | no | timestamp | 14 | Vendor location hold date |
| VendorLocation | PurchasingSiteFlag | no | boolean | 6 | Purchasing site flag |
| VendorLocation | ManufacturingIndicator | no | boolean | 9 | Is the location a manufacturing location (yes/no) |
| VendorLocation | HoldFlag | no | boolean | 6 | Hold flag for the vendor |
| VendorLocation | FreightTerms | no | string | 4000 | Freight terms with the vendor |
| VendorLocation | InvoiceCurrencyCode | no | string | 3 | Invoice currency code for business transacton with vendor |
| VendorLocation | PaymentCurrencyCode | no | string | 3 | Payment currency code for business transaction with vendor |
| VendorLocation | EmailAddress | no | string | 256 | Email address of the vendor |
| VendorLocation | VendorLocationName | no | string | 256 | Name of the location |
| VendorLocation | PeriodEndTimestamp | no | timestamp | 14 | The period end timestamp associated with the information. |
| VendorLocation | PhoneNumber | no | string | 256 | Phone number of the vendor |
| VendorLocation | CustomerId | no | string | 36 | Customer Id the vendor maintains |
| VendorLocation | CustomerWarehouseId | no | string | 36 | Warehouse Id the vendor services or supports |
| VendorLocation | Fax | no | string | 256 | Fax number of the vendor |

EOF