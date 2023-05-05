---
title: Account
description: This is about Account entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap - template
---

# **Account**

Accounts refer to a business or organization that is being tracked and managed within the ERP system as a customer or vendor. An account record within an ERP typically contains detailed information about the business or organization, such as its name, address, industry, size, type of account and contact information. An account may be linked to related records such as contacts, opportunities, and activities. This allows users to see a complete picture of their interactions with the account and to track the status of sales opportunities, customer service issues, Purchases, Shipments, and other business activities. Accounts are a fundamental element of any ERP system, as they provide a way to organize and manage customer, vendor, 3rd party service providers track all interactions, activities and transactions over time.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountCategoryCode	|	string	|	256	|	No	|	Select a category to indicate whether the customer account is standard or preferred.	|
|	AccountCategoryCodeName	|	string	|	256	|	No	|	Account category code name	|
|	AccountClassificationCode	|	string	|	256	|	No	|	Select a classification code to indicate the potential value of the customer account based on the projected return on investment, cooperation level, sales cycle length or other criteria.	|
|	AccountClassificationCodeName	|	string	|	256	|	No	|	Account type code indicates the type of account. An account could be Vendor, Customer etc.	|
|	AccountGroupNumber	|	string	|	256	|	No	|	Account group number	|
|	AccountId	|	string	|	36	|	Yes	|	A unique identifier of an account. The account could be a customer or vendor etc. AccountId is an auto generated Id by Microsoft D365 or Supply chain center. 	|
|	AccountNumber	|	string	|	256	|	Yes	|	Number or code for the account to quickly search and identify the account in system views.	|
|	AccountPaymentTerm	|	string	|	256	|	No	|	Payment terms for the account	|
|	AccountRatingCode	|	string	|	256	|	No	|	Select a rating to indicate the value of the customer account.	|
|	AccountTypeCode	|	string	|	256	|	Yes	|	Account type code indicates the type of account. An account could be Vendor, Customer etc.	|
|	Address1_AddressId	|	string	|	256	|	No	|	Unique identifier for address 1.	|
|	Address1_AddressTypeCode	|	string	|	256	|	No	|	Select the primary address type.	|
|	address1_addresstypecodename	|	string	|	256	|	No	|	Address type code name	|
|	Address1_City	|	string	|	256	|	No	|	Type the city for the primary address.	|
|	Address1_Composite	|	string	|	256	|	No	|	Shows the complete primary address.	|
|	Address1_Country	|	string	|	256	|	No	|	Type the country or region for the primary address.	|
|	Address1_County	|	string	|	256	|	No	|	Type the county for the primary address.	|
|	Address1_Fax	|	string	|	256	|	No	|	Type the fax number associated with the primary address.	|
|	Address1_FreightTermsCode	|	string	|	256	|	No	|	Select the freight terms for the primary address to make sure shipping orders are processed correctly.	|
|	address1_freighttermscodename	|	string	|	256	|	No	|	Freight terms code name	|
|	Address1_Latitude	|	decimal	|		|	No	|	Type the latitude value for the primary address for use in mapping and other applications.	|
|	Address1_Line1	|	string	|	256	|	No	|	Type the first line of the primary address.	|
|	Address1_Line2	|	string	|	256	|	No	|	Type the second line of the primary address.	|
|	Address1_Line3	|	string	|	256	|	No	|	Type the third line of the primary address.	|
|	Address1_Longitude	|	decimal	|		|	No	|	Type the longitude value for the primary address for use in mapping and other applications.	|
|	Address1_Name	|	string	|	256	|	No	|	Type a descriptive name for the primary address, such as Corporate Headquarters.	|
|	Address1_PostalCode	|	string	|	256	|	No	|	Type the ZIP Code or postal code for the primary address.	|
|	Address1_PostOfficeBox	|	string	|	256	|	No	|	Type the post office box number of the primary address.	|
|	Address1_PrimaryContactName	|	string	|	256	|	No	|	Type the name of the main contact at the account's primary address.	|
|	Address1_ShippingMethodCode	|	string	|	256	|	No	|	Select a shipping method for deliveries sent to this address.	|
|	address1_shippingmethodcodename	|	string	|	256	|	No	|	Shipping method code name	|
|	Address1_StateOrProvince	|	string	|	256	|	No	|	Type the state or province of the primary address.	|
|	Address1_Telephone1	|	string	|	256	|	No	|	Type the main phone number associated with the primary address.	|
|	Address1_Telephone2	|	string	|	256	|	No	|	Type a second phone number associated with the primary address.	|
|	Address1_Telephone3	|	string	|	256	|	No	|	Type a third phone number associated with the primary address.	|
|	Address1_UPSZone	|	string	|	256	|	No	|	Type the UPS zone of the primary address to make sure shipping charges are calculated correctly and deliveries are made promptly, if shipped by UPS.	|
|	Address1_UTCOffset	|	string	|	256	|	No	|	Select the time zone, or UTC offset, for this address so that other people can reference it when they contact someone at this address.	|
|	Address2_AddressId	|	string	|	256	|	No	|	Unique identifier for address 2.	|
|	Address2_AddressTypeCode	|	string	|	256	|	No	|	Select the secondary address type.	|
|	Address2_City	|	string	|	256	|	No	|	Type the city for the secondary address.	|
|	Address2_Composite	|	string	|	256	|	No	|	Shows the complete secondary address.	|
|	Address2_Country	|	string	|	256	|	No	|	Type the country or region for the secondary address.	|
|	Address2_County	|	string	|	256	|	No	|	Type the county for the secondary address.	|
|	Address2_Fax	|	string	|	256	|	No	|	Type the fax number associated with the secondary address.	|
|	Address2_FreightTermsCode	|	string	|	256	|	No	|	Select the freight terms for the secondary address to make sure shipping orders are processed correctly.	|
|	Address2_Latitude	|	decimal	|		|	No	|	Type the latitude value for the secondary address for use in mapping and other applications.	|
|	Address2_Line1	|	string	|	256	|	No	|	Type the first line of the secondary address.	|
|	Address2_Line2	|	string	|	256	|	No	|	Type the second line of the secondary address.	|
|	Address2_Line3	|	string	|	256	|	No	|	Type the third line of the secondary address.	|
|	Address2_Longitude	|	decimal	|		|	No	|	Type the longitude value for the secondary address for use in mapping and other applications.	|
|	Address2_Name	|	string	|	256	|	No	|	Type a descriptive name for the secondary address, such as Corporate Headquarters.	|
|	Address2_PostalCode	|	string	|	256	|	No	|	Type the ZIP Code or postal code for the secondary address.	|
|	Address2_PostOfficeBox	|	string	|	256	|	No	|	Type the post office box number of the secondary address.	|
|	Address2_PrimaryContactName	|	string	|	256	|	No	|	Type the name of the main contact at the account's secondary address.	|
|	Address2_ShippingMethodCode	|	string	|	256	|	No	|	Select a shipping method for deliveries sent to this address.	|
|	Address2_StateOrProvince	|	string	|	256	|	No	|	Type the state or province of the secondary address.	|
|	Address2_Telephone1	|	string	|	256	|	No	|	Type the main phone number associated with the secondary address.	|
|	Address2_Telephone2	|	string	|	256	|	No	|	Type a second phone number associated with the secondary address.	|
|	Address2_Telephone3	|	string	|	256	|	No	|	Type a third phone number associated with the secondary address.	|
|	Address2_UPSZone	|	string	|	256	|	No	|	Type the UPS zone of the secondary address to make sure shipping charges are calculated correctly and deliveries are made promptly, if shipped by UPS.	|
|	Address2_UTCOffset	|	string	|	256	|	No	|	Select the time zone, or UTC offset, for this address so that other people can reference it when they contact someone at this address.	|
|	ADX_CreatedByIPAddress	|	string	|	256	|	No	|	Created by IP address	|
|	ADX_CreatedByUsername	|	string	|	256	|	No	|	Created by user name	|
|	ADX_ModifiedByIPAddress	|	string	|	256	|	No	|	Modified by IP address	|
|	ADX_ModifiedByUsername	|	string	|	256	|	No	|	Modified by user name	|
|	Aging30	|	string	|	256	|	No	|	For system use only.	|
|	Aging30_Base	|	string	|	256	|	No	|	The base currency equivalent of the aging 30 field.	|
|	Aging60	|	string	|	256	|	No	|	For system use only.	|
|	Aging60_Base	|	string	|	256	|	No	|	The base currency equivalent of the aging 60 field.	|
|	Aging90	|	string	|	256	|	No	|	For system use only.	|
|	Aging90_Base	|	string	|	256	|	No	|	The base currency equivalent of the aging 90 field.	|
|	BillingAccount	|	string	|	256	|	No	|	Billing account	|
|	BusinessTypeCode	|	string	|	256	|	No	|	Select the legal designation or other business type of the account for contracts or reporting purposes.	|
|	Company	|	string	|	256	|	No	|	Company of the account	|
|	CreatedByExternalParty	|	string	|	256	|	No	|	Shows the external party who created the record.	|
|	CreditLimit	|	string	|	256	|	No	|	Type the credit limit of the account. This is a useful reference when you address invoice and accounting issues with the customer.	|
|	CreditLimitBase	|	string	|	256	|	No	|	Credit limit base	|
|	CreditLimitIsMandatory	|	string	|	256	|	No	|	Credit limit is mandatory for the account	|
|	CreditOnHold	|	string	|	256	|	No	|	Select whether the credit for the account is on hold. This is a useful reference while addressing the invoice and accounting issues with the customer.	|
|	CreditRating	|	string	|	256	|	No	|	Credit rating of the account	|
|	CustomerGroupId	|	string	|	36	|	No	|	Default customer group Id	|
|	CustomerPaymentMethod	|	string	|	256	|	No	|	Default customer payment method	|
|	CustomerSizeCode	|	string	|	256	|	No	|	Select the size category or range of the account for segmentation and reporting purposes.	|
|	CustomerTypeCodeName	|	string	|	256	|	No	|	Customer type code 	|
|	DefaultPriceLevelId	|	string	|	256	|	No	|	Default price level Id	|
|	DefaultVendorPaymentMethodName	|	string	|	256	|	No	|	Default vendor payment method name	|
|	Description	|	string	|	4000	|	No	|	Type additional information to describe the account, such as an excerpt from the company's website.	|
|	DoNotBulkEmail	|	string	|	256	|	No	|	Do not bulk email to the account	|
|	DoNotBulkPostalMail	|	string	|	256	|	No	|	Select whether the account allows bulk postal mail sent through marketing campaigns or quick campaigns. If Do Not Allow is selected, the account can be added to marketing lists, but will be excluded from the postal mail.	|
|	DoNotEmail	|	string	|	256	|	No	|	Do not email address of the account	|
|	DoNotFax	|	string	|	256	|	No	|	Select whether the account allows faxes. If Do Not Allow is selected, the account will be excluded from fax activities distributed in marketing campaigns.	|
|	DoNotPhone	|	string	|	256	|	No	|	Select whether the account allows phone calls. If Do Not Allow is selected, the account will be excluded from phone call activities distributed in marketing campaigns.	|
|	DoNotPostalMail	|	string	|	256	|	No	|	Select whether the account allows direct mail. If Do Not Allow is selected, the account will be excluded from letter activities distributed in marketing campaigns.	|
|	DoNotSendMM	|	string	|	256	|	No	|	Select whether the account accepts marketing materials, such as brochures or catalogs.	|
|	EmailAddress1	|	string	|	256	|	No	|	Email of the account	|
|	EmailAddress1Description	|	string	|	4000	|	No	|	Description of email 1	|
|	EmailAddress2	|	string	|	256	|	No	|	Alternate email of the account	|
|	EmailAddress3	|	string	|	256	|	No	|	Alternate email of the account	|
|	EntityImage	|	string	|	256	|	No	|	Shows the default image for the record.	|
|	EntityImageId	|	string	|	256	|	No	|	For internal use only.	|
|	ExchangeRate	|	string	|	256	|	No	|	Shows the conversion rate of the record's currency. The exchange rate is used to convert all money fields in the record from the local currency to the system's default currency.	|
|	Fax	|	string	|	256	|	No	|	Type the fax number for the account.	|
|	FaxDescription	|	string	|	4000	|	No	|	Description of the fax	|
|	FaxExtension	|	string	|	256	|	No	|	Fax extension	|
|	FollowEmail	|	string	|	256	|	No	|	Email of the account to follow	|
|	FTPSiteURL	|	string	|	256	|	No	|	Type the URL for the account's FTP site to enable users to access data and share documents.	|
|	GDPROptOut	|	string	|	256	|	No	|	GDPR optout	|
|	GeoLocationId	|	string	|	36	|	No	|	The unique identifier of a Location. This is autogenerated by Supply chain center or D365 applications	|
|	GeoLocationNumber	|	string	|	256	|	No	|	The unique number of a location. This is a referenced in an external system to identify the unique location	|
|	IdentificationNumber	|	string	|	256	|	No	|	Identification number of the account	|
|	IndustryCode	|	string	|	256	|	No	|	Select the account's primary industry for use in marketing segmentation and demographic analysis.	|
|	IndustryCodeName	|	string	|	256	|	No	|	Industry code name	|
|	InternalAccountNumber	|	string	|	256	|	Yes	|	A unique number of an account. The account number is the user preferred number or an internal number to identify the account	|
|	InvoiceAddress	|	string	|	256	|	No	|	Invoice address of the account	|
|	InvoiceVendorAccount	|	string	|	256	|	No	|	Invoice to vendor account	|
|	Language	|	string	|	256	|	No	|	Language of the account	|
|	LastOnHoldTime	|	string	|	256	|	No	|	Contains the date and time stamp of the last on hold time.	|
|	LastUsedInCampaign	|	string	|	256	|	No	|	Shows the date when the account was last included in a marketing campaign or quick campaign.	|
|	ManagingPartnerId	|	string	|	256	|	No	|	Id of the managing partner	|
|	MappedVendorAccount	|	string	|	256	|	No	|	Mapped vendor account	|
|	MarketCap	|	string	|	256	|	No	|	Type the market capitalization of the account to identify the company's equity, used as an indicator in financial performance analysis.	|
|	MarketCapBase	|	string	|	256	|	No	|	Market cap base of the account	|
|	MarketingOnly	|	string	|	256	|	No	|	Whether is only for marketing	|
|	MasterId	|	string	|	256	|	No	|	Shows the master account that the account was merged with.	|
|	Merged	|	string	|	256	|	No	|	Shows whether the account has been merged with another account.	|
|	Name	|	string	|	256	|	No	|	Type the company or business name.	|
|	NumberOfEmployees	|	integer	|		|	No	|	Type the number of employees that work at the account for use in marketing segmentation and demographic analysis.	|
|	OneTimeCustomer	|	string	|	256	|	No	|	One time customer	|
|	OnHoldStatus	|	string	|	256	|	No	|	On hold status	|
|	OnHoldTime	|	string	|	256	|	No	|	Shows how long, in minutes, that the record was on hold.	|
|	OpenDeals	|	string	|	256	|	No	|	Open deals	|
|	OpenDealsDate	|	date	|		|	No	|	Date of open deals	|
|	OpenDealsState	|	string	|	256	|	No	|	State of open deals 	|
|	OpenRevenue	|	string	|	256	|	No	|	Open revenue	|
|	OpenRevenueBase	|	string	|	256	|	No	|	Open revenue base	|
|	OpenRevenueDate	|	date	|		|	No	|	Open revenue date	|
|	OpenRevenueState	|	string	|	256	|	No	|	Open revenue state	|
|	OriginatingLeadId	|	string	|	256	|	No	|	Originating lead Id	|
|	OwnershipCode	|	string	|	256	|	No	|	Select the account's ownership structure, such as public or private.	|
|	OwningBusinessUnit	|	string	|	256	|	No	|	Shows the business unit that the record owner belongs to.	|
|	ParentAccountId	|	string	|	256	|	No	|	A unique parent Id of the account	|
|	ParentAccountIdName	|	string	|	256	|	No	|	A unique name of the parent Id of the account	|
|	ParticipatesInWorkflow	|	string	|	256	|	No	|	For system use only. Legacy Microsoft Dynamics CRM 3.0 workflow data.	|
|	PartyCountry	|	string	|	256	|	No	|	Country of the party	|
|	PartyNumber	|	string	|	256	|	No	|	Party number of the account	|
|	PartyStateProvince	|	string	|	256	|	No	|	State or province of the party or account	|
|	PaymentDay	|	string	|	256	|	No	|	Payment day	|
|	PaymentSchedule	|	string	|	256	|	No	|	Payment schedule	|
|	PaymentTermsBaseDays	|	string	|	256	|	No	|	Base days for payment terms	|
|	PreferredAppointmentDayCode	|	string	|	256	|	No	|	Select the preferred day of the week for service appointments.	|
|	PreferredAppointmentTimeCode	|	string	|	256	|	No	|	Select the preferred time of day for service appointments.	|
|	PreferredContactMethodCode	|	string	|	256	|	No	|	Select the preferred method of contact.	|
|	PreferredEquipmentId	|	string	|	256	|	No	|	Preferred equipment Id of the account	|
|	PreferredServiceId	|	string	|	256	|	No	|	Preferred service Id of the account	|
|	PreferredSystemUserId	|	string	|	256	|	No	|	Choose the preferred service representative for reference when you schedule service activities for the account.	|
|	PreferredTermsCode	|	string	|	256	|	No	|	Preferred terms code	|
|	PrimaryContactId	|	string	|	256	|	No	|	Choose the primary contact for the account to provide quick access to contact details.	|
|	PrimaryContactIdDescription	|	string	|	256	|	No	|	Description of primary contact	|
|	PrimaryFacebookId	|	string	|	256	|	No	|	Primary Facebook Id	|
|	PrimaryLinkedinDescription	|	string	|	256	|	No	|	Description of the primary LinkedIn account	|
|	PrimaryLinkedinId	|	string	|	256	|	No	|	Primary LinkedIn Id	|
|	PrimarySatoriId	|	string	|	256	|	No	|	Primary Satori ID for Account	|
|	PrimaryTwitterId	|	string	|	256	|	No	|	Primary Twitter ID for Account	|
|	PrimaryTwitterIddescription	|	string	|	4000	|	No	|	Description of primary Twitter ID for Account	|
|	ProcessId	|	string	|	256	|	No	|	Shows the ID of the process.	|
|	Revenue	|	string	|	256	|	No	|	Type the annual revenue for the account, used as an indicator in financial performance analysis.	|
|	RevenueBase	|	string	|	256	|	No	|	Revenue base of the account	|
|	SalesAccelerationInsightId	|	string	|	256	|	No	|	Sales acceleration insight Id	|
|	SalesTaxGroup	|	string	|	256	|	No	|	Sales tax group	|
|	SegmentId	|	string	|	256	|	No	|	Segment Id	|
|	SharesOutstanding	|	string	|	256	|	No	|	Type the number of shares available to the public for the account. This number is used as an indicator in financial performance analysis.	|
|	ShippingMethodCode	|	string	|	256	|	No	|	Select a shipping method for deliveries sent to the account's address to designate the preferred carrier or other delivery option.	|
|	SIC	|	string	|	256	|	No	|	Type the Standard Industrial Classification (SIC) code that indicates the account's primary industry of business, for use in marketing segmentation and demographic analysis.	|
|	SLAId	|	string	|	256	|	No	|	SLA Id of the 	|
|	SLAInvokedId	|	string	|	256	|	No	|	SLA Invoke Id	|
|	StageId	|	string	|	256	|	No	|	Stage Id of the account	|
|	StockExchange	|	string	|	256	|	No	|	Stock exchange of the account	|
|	TaxExempt	|	string	|	256	|	No	|	Tax exempt	|
|	TaxExemptNumber	|	string	|	256	|	No	|	Tax exempt number	|
|	Telephone1	|	string	|	256	|	No	|	Telephone number of the account	|
|	Telephone1Description	|	string	|	4000	|	No	|	Description of the telephone1	|
|	Telephone1Extension	|	string	|	256	|	No	|	Extension number of the telephone1	|
|	Telephone2	|	string	|	256	|	No	|	Alternate telephone number of the account	|
|	Telephone3	|	string	|	256	|	No	|	Alternate telephone number of the account	|
|	TerritoryCode	|	string	|	256	|	No	|	Territory code of the account	|
|	TerritoryId	|	string	|	256	|	No	|	Territory Id of the account	|
|	TickerSymbol	|	string	|	256	|	No	|	Ticker symbol of the account	|
|	TimeSpentByMeOnEmailAndMeetings	|	string	|	256	|	No	|	Time spent on the account to send emails and meetings	|
|	TransactionCurrencyId	|	string	|	256	|	No	|	Transaction currency of the account	|
|	TransactionCurrencyIdDescription	|	string	|	256	|	No	|	Description of the transaction currency of the account	|
|	TraversedPath	|	string	|	256	|	No	|	Traversed path of the account	|
|	VendorCreatedByWorkflow	|	string	|	256	|	No	|	Vendor created by	|
|	VendorGroup	|	string	|	256	|	No	|	Vendor group	|
|	VendorId	|	string	|	36	|	No	|	Unique Id of the vendor	|
|	VendorKnownAsName	|	string	|	256	|	No	|	Vendor known as name	|
|	VendorNumber	|	string	|	256	|	No	|	Unique number of the vendor	|
|	VendorOrganizationName	|	string	|	256	|	No	|	Vendor organization name	|
|	WebsiteURL	|	string	|	256	|	No	|	URL of the account	|
|	WebsiteURLDescription	|	string	|	4000	|	No	|	URL of the website	|
|	YomiName	|	string	|	256	|	No	|	Type the phonetic spelling of the company name, if specified in Japanese, to make sure the name is pronounced correctly in phone calls and other communications.	|
