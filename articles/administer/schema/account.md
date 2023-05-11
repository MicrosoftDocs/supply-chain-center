---
title: Account
description: This article provides information about the Account entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **Account**

Accounts refer to a business or organization that is being tracked and managed within an ERP system as a customer or vendor. An account record within an ERP typically contains detailed information about the business or organization, such as its name, address, industry, size, type of account and contact information. 

An account may be linked to related records such as contacts, opportunities, and activities. Users can see a complete picture of their interactions with the account. They can also track the status of sales opportunities, customer service issues, Purchases, Shipments, and other business activities. 

Accounts are a fundamental element of any ERP system, as they provide a way to organize and manage customer, vendor, third party service providers, and track all interactions, activities, and transactions over time.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountCategoryCode	|	string	|	256	|	No	|	Indicates if the customer account is standard or preferred.	|
|	AccountCategoryCodeName	|	string	|	256	|	No	|	Account category code name.	|
|	AccountClassificationCode	|	string	|	256	|	No	|	A classification code to indicate the potential value of the customer account based on the projected return on investment, cooperation level, sales cycle length, or other criteria.	|
|	AccountClassificationCodeName	|	string	|	256	|	No	|	Account type code indicates the type of account. An account could be Vendor, Customer etc.	|
|	AccountGroupNumber	|	string	|	256	|	No	|	Account group number.	|
|	AccountId	|	string	|	36	|	Yes	|	A unique identifier of an account. The account could be a customer or vendor etc. AccountId is an auto generated ID by Microsoft Dynamics 365 or Microsoft Supply Chain Center. |
|	AccountNumber	|	string	|	256	|	Yes	|	A number or code that is used for the account to quickly search for and identify it in system views.	|
|	AccountPaymentTerm	|	string	|	256	|	No	|	The payment terms for the account.	|
|	AccountRatingCode	|	string	|	256	|	No	|	A rating to indicate the value of the customer account.	|
|	AccountTypeCode	|	string	|	256	|	Yes	|	Account type code indicates the type of account. An account could be Vendor, Customer etc.	|
|	Address1_AddressId	|	string	|	256	|	No	|	The unique identifier for address 1.	|
|	Address1_AddressTypeCode	|	string	|	256	|	No	|	The primary address type.	|
|	address1_addresstypecodename	|	string	|	256	|	No	|	The address type code name.	|
|	Address1_City	|	string	|	256	|	No	|	The city for the primary address.	|
|	Address1_Composite	|	string	|	256	|	No	|	The complete primary address.	|
|	Address1_Country	|	string	|	256	|	No	|	The country or region for the primary address.	|
|	Address1_County	|	string	|	256	|	No	|	The county for the primary address.	|
|	Address1_Fax	|	string	|	256	|	No	|	The fax number for the primary address.	|
|	Address1_FreightTermsCode	|	string	|	256	|	No	|	The freight terms for the primary address to make sure shipping orders are processed correctly.	|
|	address1_freighttermscodename	|	string	|	256	|	No	|	Freight terms code name.	|
|	Address1_Latitude	|	decimal	|		|	No	|	The latitude value for the primary address. Used for mapping and other applications.	|
|	Address1_Line1	|	string	|	256	|	No	|	The first line of the primary address.	|
|	Address1_Line2	|	string	|	256	|	No	|	The second line of the primary address.	|
|	Address1_Line3	|	string	|	256	|	No	|	The third line of the primary address.	|
|	Address1_Longitude	|	decimal	|		|	No	|	The longitude value for the primary address. Used for mapping and other applications.	|
|	Address1_Name	|	string	|	256	|	No	|	A descriptive name for the primary address. For example, Corporate Headquarters.	|
|	Address1_PostalCode	|	string	|	256	|	No	|	The ZIP Code or postal code for the primary address.	|
|	Address1_PostOfficeBox	|	string	|	256	|	No	|	The post office box number for the primary address.	|
|	Address1_PrimaryContactName	|	string	|	256	|	No	|	The name of the main contact at the account's primary address.	|
|	Address1_ShippingMethodCode	|	string	|	256	|	No	|	The shipping method for deliveries sent to this address.	|
|	address1_shippingmethodcodename	|	string	|	256	|	No	|	The shipping method code name.	|
|	Address1_StateOrProvince	|	string	|	256	|	No	|	The state or province of the primary address.	|
|	Address1_Telephone1	|	string	|	256	|	No	|	The main phone number for the primary address.	|
|	Address1_Telephone2	|	string	|	256	|	No	|	A second phone number for the primary address.	|
|	Address1_Telephone3	|	string	|	256	|	No	|	A third phone number for the primary address.	|
|	Address1_UPSZone	|	string	|	256	|	No	|	The UPS zone of the primary address. Used for UPS shipments to make sure the shipping charges are calculated correctly and deliveries are made promptly. |
|	Address1_UTCOffset	|	string	|	256	|	No	|	The time zone, or UTC offset, for this address. Used as a reference when you contact someone at this address.	|
|	Address2_AddressId	|	string	|	256	|	No	|	Unique identifier for address 2.	|
|	Address2_AddressTypeCode	|	string	|	256	|	No	|	The secondary address type.	|
|	Address2_City	|	string	|	256	|	No	|	Type the city for the secondary address.	|
|	Address2_Composite	|	string	|	256	|	No	|	Shows the complete secondary address.	|
|	Address2_Country	|	string	|	256	|	No	|	Type the country or region for the secondary address.	|
|	Address2_County	|	string	|	256	|	No	|	Type the county for the secondary address.	|
|	Address2_Fax	|	string	|	256	|	No	|	Type the fax number for the secondary address.	|
|	Address2_FreightTermsCode	|	string	|	256	|	No	|	The freight terms for the secondary address to make sure shipping orders are processed correctly.	|
|	Address2_Latitude	|	decimal	|		|	No	|	Type the latitude value for the secondary address. Used for mapping and other applications.	|
|	Address2_Line1	|	string	|	256	|	No	|	Type the first line of the secondary address.	|
|	Address2_Line2	|	string	|	256	|	No	|	Type the second line of the secondary address.	|
|	Address2_Line3	|	string	|	256	|	No	|	Type the third line of the secondary address.	|
|	Address2_Longitude	|	decimal	|		|	No	|	Type the longitude value for the secondary address. Used for mapping and other applications.	|
|	Address2_Name	|	string	|	256	|	No	|	A descriptive name for the secondary address. For example, Corporate Headquarters.	|
|	Address2_PostalCode	|	string	|	256	|	No	|	The ZIP Code or postal code for the secondary address.	|
|	Address2_PostOfficeBox	|	string	|	256	|	No	|	The post office box number of the secondary address.	|
|	Address2_PrimaryContactName	|	string	|	256	|	No	|	The name of the main contact at the account's secondary address.	|
|	Address2_ShippingMethodCode	|	string	|	256	|	No	|	The shipping method for deliveries sent to this address.	|
|	Address2_StateOrProvince	|	string	|	256	|	No	|	The state or province for the secondary address.	|
|	Address2_Telephone1	|	string	|	256	|	No	|	The main phone number for the secondary address.	|
|	Address2_Telephone2	|	string	|	256	|	No	|	A second phone number for the secondary address.	|
|	Address2_Telephone3	|	string	|	256	|	No	|	A third phone number for the secondary address.	|
|	Address2_UPSZone	|	string	|	256	|	No	|	The UPS zone of the secondary address. Used for UPS shipments to make sure the shipping charges are calculated correctly and deliveries are made promptly.	|
|	Address2_UTCOffset	|	string	|	256	|	No	|	The time zone, or UTC offset, for this address so that other people can reference it when they contact someone at this address.	|
|	ADX_CreatedByIPAddress	|	string	|	256	|	No	|	Created by IP address.	|
|	ADX_CreatedByUsername	|	string	|	256	|	No	|	Created by user name.	|
|	ADX_ModifiedByIPAddress	|	string	|	256	|	No	|	Modified by IP address.	|
|	ADX_ModifiedByUsername	|	string	|	256	|	No	|	Modified by user name.	|
|	Aging30	|	string	|	256	|	No	|	For system use only.	|
|	Aging30_Base	|	string	|	256	|	No	|	The base currency equivalent of the aging 30 field.	|
|	Aging60	|	string	|	256	|	No	|	For system use only.	|
|	Aging60_Base	|	string	|	256	|	No	|	The base currency equivalent of the aging 60 field.	|
|	Aging90	|	string	|	256	|	No	|	For system use only.	|
|	Aging90_Base	|	string	|	256	|	No	|	The base currency equivalent of the aging 90 field.	|
|	BillingAccount	|	string	|	256	|	No	|	Billing account	|
|	BusinessTypeCode	|	string	|	256	|	No	|	The legal designation or other business type of the account for contracts or reporting purposes.	|
|	Company	|	string	|	256	|	No	|	Company name for the account.	|
|	CreatedByExternalParty	|	string	|	256	|	No	|	The external party who created the record.	|
|	CreditLimit	|	string	|	256	|	No	|	The credit limit of the account. CreditLimitBase is a useful reference when you address invoice and accounting issues with the customer.	|
|	CreditLimitBase	|	string	|	256	|	No	|	Credit limit base.	|
|	CreditLimitIsMandatory	|	string	|	256	|	No	|	Indicates that a credit limit is mandatory for the account.	|
|	CreditOnHold	|	string	|	256	|	No	|	Indicates if the credit for the account is on hold. CreditOnHold a useful reference while addressing the invoice and accounting issues with the customer.	|
|	CreditRating	|	string	|	256	|	No	|	Credit rating of the account.	|
|	CustomerGroupId	|	string	|	36	|	No	|	Default customer group ID.	|
|	CustomerPaymentMethod	|	string	|	256	|	No	|	Default customer payment method.	|
|	CustomerSizeCode	|	string	|	256	|	No	|	The size category or range of the account for segmentation and reporting purposes.	|
|	CustomerTypeCodeName	|	string	|	256	|	No	|	Customer type code. 	|
|	DefaultPriceLevelId	|	string	|	256	|	No	|	Default price level ID.	|
|	DefaultVendorPaymentMethodName	|	string	|	256	|	No	|	Default vendor payment method name.	|
|	Description	|	string	|	4000	|	No	|	Type additional information to describe the account. For example, an excerpt from the company's website.	|
|	DoNotBulkEmail	|	string	|	256	|	No	|	Don't bulk email to the account.	|
|	DoNotBulkPostalMail	|	string	|	256	|	No	|	Indicates if the account allows bulk postal mail sent through marketing campaigns or quick campaigns. If Do Not Allow is selected, the account can be added to marketing lists, but is excluded from the postal mail.	|
|	DoNotEmail	|	string	|	256	|	No	|	Don't email address of the account.	|
|	DoNotFax	|	string	|	256	|	No	|	Indicates if the account allows faxes. If Do Not Allow is selected, the account is excluded from fax activities distributed in marketing campaigns.	|
|	DoNotPhone	|	string	|	256	|	No	|	Indicates if the account allows phone calls. If Do Not Allow is selected, the account is excluded from phone call activities distributed in marketing campaigns.	|
|	DoNotPostalMail	|	string	|	256	|	No	|	Indicates if the account allows direct mail. If Do Not Allow is selected, the account is excluded from letter activities distributed in marketing campaigns.	|
|	DoNotSendMM	|	string	|	256	|	No	|	Indicated if the account accepts marketing materials, such as brochures or catalogs.	|
|	EmailAddress1	|	string	|	256	|	No	|	The email address of the account.	|
|	EmailAddress1Description	|	string	|	4000	|	No	|	Description of email 1.	|
|	EmailAddress2	|	string	|	256	|	No	|	Alternate email address of the account.	|
|	EmailAddress3	|	string	|	256	|	No	|	Alternate email address of the account.	|
|	EntityImage	|	string	|	256	|	No	|	Shows the default image for the record.	|
|	EntityImageId	|	string	|	256	|	No	|	For internal use only.	|
|	ExchangeRate	|	string	|	256	|	No	|	The conversion rate of the record's currency. The exchange rate is used to convert all money fields in the record from the local currency to the system's default currency.	|
|	Fax	|	string	|	256	|	No	|	The fax number for the account.	|
|	FaxDescription	|	string	|	4000	|	No	|	Description of the fax number.	|
|	FaxExtension	|	string	|	256	|	No	|	Fax extension.	|
|	FollowEmail	|	string	|	256	|	No	|	Email of the account to follow.	|
|	FTPSiteURL	|	string	|	256	|	No	|	The URL for the account's FTP site to enable users to access data and share documents.	|
|	GDPROptOut	|	string	|	256	|	No	|	GDPR opt-out.	|
|	GeoLocationId	|	string	|	36	|	No	|	The unique identifier of a Location. Supply Chain Center or Dynamics 365 applications generate the GeoLocationId. |
|	GeoLocationNumber	|	string	|	256	|	No	|	The unique number of a location. GeoLocationNumber is a referenced in an external system to identify the unique location.	|
|	IdentificationNumber	|	string	|	256	|	No	|	Identification number for the account.	|
|	IndustryCode	|	string	|	256	|	No	|	The account's primary industry for use in marketing segmentation and demographic analysis.	|
|	IndustryCodeName	|	string	|	256	|	No	|	Industry code name.	|
|	InternalAccountNumber	|	string	|	256	|	Yes	|	A unique number for an account. The account number is the user preferred number or an internal number to identify the account.	|
|	InvoiceAddress	|	string	|	256	|	No	|	Invoice address for the account.	|
|	InvoiceVendorAccount	|	string	|	256	|	No	|	Invoice to vendor account.	|
|	Language	|	string	|	256	|	No	|	The language of the account.	|
|	LastOnHoldTime	|	string	|	256	|	No	|	Contains the date and time stamp of the last on hold time.	|
|	LastUsedInCampaign	|	string	|	256	|	No	|	The date when the account was last included in a marketing campaign or quick campaign.	|
|	ManagingPartnerId	|	string	|	256	|	No	|	The ID of the managing partner.	|
|	MappedVendorAccount	|	string	|	256	|	No	|	Mapped vendor account.	|
|	MarketCap	|	string	|	256	|	No	|	The market capitalization of the account to identify the company's equity. Used as an indicator in financial performance analysis.	|
|	MarketCapBase	|	string	|	256	|	No	|	The market cap base of the account.	|
|	MarketingOnly	|	string	|	256	|	No	|	Whether is only for marketing.	|
|	MasterId	|	string	|	256	|	No	|	The master account that the account was merged with.	|
|	Merged	|	string	|	256	|	No	|	Indicates if the account has been merged with another account.	|
|	Name	|	string	|	256	|	No	|	The company or business name.	|
|	NumberOfEmployees	|	integer	|		|	No	|	The number of employees that work at the account for use in marketing segmentation and demographic analysis.	|
|	OneTimeCustomer	|	string	|	256	|	No	|	One time customer.	|
|	OnHoldStatus	|	string	|	256	|	No	|	On hold status	|
|	OnHoldTime	|	string	|	256	|	No	|	Indicates how long, in minutes, that the record was on hold.	|
|	OpenDeals	|	string	|	256	|	No	|	Open deals.	|
|	OpenDealsDate	|	date	|		|	No	|	The date of open deals.	|
|	OpenDealsState	|	string	|	256	|	No	|	The state of open deals.	|
|	OpenRevenue	|	string	|	256	|	No	|	Open revenue.	|
|	OpenRevenueBase	|	string	|	256	|	No	|	The open revenue base.	|
|	OpenRevenueDate	|	date	|		|	No	|	The open revenue date.	|
|	OpenRevenueState	|	string	|	256	|	No	|	The open revenue state.	|
|	OriginatingLeadId	|	string	|	256	|	No	|	Originating lead ID.	|
|	OwnershipCode	|	string	|	256	|	No	|	The account's ownership structure. For example, public or private.	|
|	OwningBusinessUnit	|	string	|	256	|	No	|	The business unit that the record owner belongs to.	|
|	ParentAccountId	|	string	|	256	|	No	|	A unique parent ID of the account.	|
|	ParentAccountIdName	|	string	|	256	|	No	|	A unique name of the parent ID of the account.	|
|	ParticipatesInWorkflow	|	string	|	256	|	No	|	For system use only. Legacy Microsoft Dynamics CRM 3.0 workflow data.	|
|	PartyCountry	|	string	|	256	|	No	|	Country of the party.	|
|	PartyNumber	|	string	|	256	|	No	|	Party number of the account.	|
|	PartyStateProvince	|	string	|	256	|	No	|	State or province of the party or account.	|
|	PaymentDay	|	string	|	256	|	No	|	Payment day.	|
|	PaymentSchedule	|	string	|	256	|	No	|	Payment schedule.	|
|	PaymentTermsBaseDays	|	string	|	256	|	No	|	Base days for payment terms.	|
|	PreferredAppointmentDayCode	|	string	|	256	|	No	|	The preferred day of the week for service appointments.	|
|	PreferredAppointmentTimeCode	|	string	|	256	|	No	|	The preferred time of day for service appointments.	|
|	PreferredContactMethodCode	|	string	|	256	|	No	|	The preferred method of contact.	|
|	PreferredEquipmentId	|	string	|	256	|	No	|	The preferred equipment ID of the account.	|
|	PreferredServiceId	|	string	|	256	|	No	|	The preferred service ID of the account.	|
|	PreferredSystemUserId	|	string	|	256	|	No	|	The preferred service representative for reference when you schedule service activities for the account.	|
|	PreferredTermsCode	|	string	|	256	|	No	|	The preferred terms code.	|
|	PrimaryContactId	|	string	|	256	|	No	|	The primary contact for the account to provide quick access to contact details.	|
|	PrimaryContactIdDescription	|	string	|	256	|	No	|	Description of primary contact.	|
|	PrimaryFacebookId	|	string	|	256	|	No	|	Primary Facebook ID.	|
|	PrimaryLinkedinDescription	|	string	|	256	|	No	|	Description of the primary LinkedIn account.	|
|	PrimaryLinkedinId	|	string	|	256	|	No	|	Primary LinkedIn ID.	|
|	PrimarySatoriId	|	string	|	256	|	No	|	Primary Satori ID for Account. |
|	PrimaryTwitterId	|	string	|	256	|	No	|	Primary Twitter ID for Account.	|
|	PrimaryTwitterIddescription	|	string	|	4000	|	No	|	Description of primary Twitter ID for Account.	|
|	ProcessId	|	string	|	256	|	No	|	Shows the ID of the process.	|
|	Revenue	|	string	|	256	|	No	|	The annual revenue for the account. Used as an indicator in financial performance analysis.	|
|	RevenueBase	|	string	|	256	|	No	|	The revenue base of the account.	|
|	SalesAccelerationInsightId	|	string	|	256	|	No	|	The sales acceleration insight ID.	|
|	SalesTaxGroup	|	string	|	256	|	No	|	The sales tax group.	|
|	SegmentId	|	string	|	256	|	No	|	The segment ID.	|
|	SharesOutstanding	|	string	|	256	|	No	|	The number of shares available to the public for the account. This number is used as an indicator in financial performance analysis.	|
|	ShippingMethodCode	|	string	|	256	|	No	|	The shipping method for deliveries sent to the account's address to designate the preferred carrier or other delivery option.	|
|	SIC	|	string	|	256	|	No	|	The Standard Industrial Classification (SIC) code that indicates the account's primary industry of business, for use in marketing segmentation and demographic analysis.	|
|	SLAId	|	string	|	256	|	No	|	The SLA ID of the. 	|
|	SLAInvokedId	|	string	|	256	|	No	|	The SLA Invoke ID.	|
|	StageId	|	string	|	256	|	No	|	The Stage ID of the account.	|
|	StockExchange	|	string	|	256	|	No	|	The Stock exchange of the account.	|
|	TaxExempt	|	string	|	256	|	No	|	Tax exempt.	|
|	TaxExemptNumber	|	string	|	256	|	No	|	Tax exempt number.	|
|	Telephone1	|	string	|	256	|	No	|	The telephone number of the account.	|
|	Telephone1Description	|	string	|	4000	|	No	|	A description for telephone1.	|
|	Telephone1Extension	|	string	|	256	|	No	|	The extension number for telephone1.	|
|	Telephone2	|	string	|	256	|	No	|	An alternate telephone number for the account.	|
|	Telephone3	|	string	|	256	|	No	|	An alternate telephone number for the account.	|
|	TerritoryCode	|	string	|	256	|	No	|	The territory code for the account.	|
|	TerritoryId	|	string	|	256	|	No	|	The territory ID for the account.	|
|	TickerSymbol	|	string	|	256	|	No	|	Ticker symbol for the account.	|
|	TimeSpentByMeOnEmailAndMeetings	|	string	|	256	|	No	|	Time spent on the account to send emails and meetings.	|
|	TransactionCurrencyId	|	string	|	256	|	No	|	Transaction currency of the account.	|
|	TransactionCurrencyIdDescription	|	string	|	256	|	No	|	Description of the transaction currency of the account.	|
|	TraversedPath	|	string	|	256	|	No	|	Traversed path of the account.	|
|	VendorCreatedByWorkflow	|	string	|	256	|	No	|	Vendor created by	.|
|	VendorGroup	|	string	|	256	|	No	|	Vendor group.	|
|	VendorId	|	string	|	36	|	No	|	A Unique ID for the vendor.	|
|	VendorKnownAsName	|	string	|	256	|	No	|	Vendor known as name.	|
|	VendorNumber	|	string	|	256	|	No	|	A unique number of the vendor.	|
|	VendorOrganizationName	|	string	|	256	|	No	|	Vendor organization name.	|
|	WebsiteURL	|	string	|	256	|	No	|	URL of the account.	|
|	WebsiteURLDescription	|	string	|	4000	|	No	|	URL of the website.	|
|	YomiName	|	string	|	256	|	No	|	Type the phonetic spelling of the company name, if specified in Japanese, to make sure the name is pronounced correctly in phone calls and other communications.	|
