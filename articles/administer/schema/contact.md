---
title: Contact
description: This article provides information about the Contact entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/15/2023
ms.custom: bap-template
---

# **Contact**

The contact entity refers to an individual or organization associated with the account.
The contact could be a primary contact person, a designated account manager, or any other relevant party representing the account.

A contact for an account entity would include information such as:

First Name and Last Name: The full name of the contact person or the organization's name.

Position/Role: The position or role the contact person holds within the organization.

Contact Details: Contact information like phone number, email address, mailing address, or any other preferred means of communication.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountId	|	string	|	36	|		|	Unique identifier of the account with which the contact is associated.	|
|	AccountIdName	|	string	|	100	|		|	AccountIdName	|
|	AccountIdYomiName	|	string	|	100	|		|	AccountIdYomiName	|
|	AccountNumber	|	string	|	256	|		|	Account number	|
|	AccountRoleCode	|	string	|	256	|		|	Select the contact's role within the company or sales process, such as decision maker, employee, or influencer.	|
|	AccountTypeCode	|	string	|	256	|		|	Account type code indicates the type of account. An account could be Vendor, Customer, Manager etc.	|
|	Address1_AddressId	|	string	|	256	|		|	Unique identifier for address 1.	|
|	Address1_AddressTypeCode	|	string	|	256	|		|	Select the primary address type.	|
|	Address1_City	|	string	|	80	|		|	Type the city for the primary address.	|
|	Address1_Composite	|	string	|	1000	|		|	Shows the complete primary address.	|
|	Address1_Country	|	string	|	80	|		|	Type the country or region for the primary address.	|
|	Address1_County	|	string	|	50	|		|	Type the county for the primary address.	|
|	Address1_Fax	|	string	|	50	|		|	Type the fax number associated with the primary address.	|
|	Address1_FreightTermsCode	|	string	|	256	|		|	Select the freight terms for the primary address to make sure shipping orders are processed correctly.	|
|	Address1_Latitude	|	decimal	|		|		|	Type the latitude value for the primary address for use in mapping and other applications.	|
|	Address1_Line1	|	string	|	250	|		|	Type the first line of the primary address.	|
|	Address1_Line2	|	string	|	250	|		|	Type the second line of the primary address.	|
|	Address1_Line3	|	string	|	250	|		|	Type the third line of the primary address.	|
|	Address1_Longitude	|	decimal	|		|		|	Type the longitude value for the primary address for use in mapping and other applications.	|
|	Address1_Name	|	string	|	200	|		|	Type a descriptive name for the primary address, such as Corporate Headquarters.	|
|	Address1_PostalCode	|	string	|	20	|		|	Type the ZIP Code or postal code for the primary address.	|
|	Address1_PostOfficeBox	|	string	|	20	|		|	Type the post office box number of the primary address.	|
|	Address1_PrimaryContactName	|	string	|	100	|		|	Type the name of the main contact at the account's primary address.	|
|	Address1_ShippingMethodCode	|	string	|	256	|		|	Select a shipping method for deliveries sent to this address.	|
|	Address1_StateOrProvince	|	string	|	50	|		|	Type the state or province of the primary address.	|
|	Address1_Telephone1	|	string	|	50	|		|	Type the main phone number associated with the primary address.	|
|	Address1_Telephone2	|	string	|	50	|		|	Type a second phone number associated with the primary address.	|
|	Address1_Telephone3	|	string	|	50	|		|	Type a third phone number associated with the primary address.	|
|	Address1_UPSZone	|	string	|	4	|		|	Type the UPS zone of the primary address to make sure shipping charges are calculated correctly and deliveries are made promptly, if shipped by UPS.	|
|	Address1_UTCOffset	|	decimal	|		|		|	Select the time zone, or UTC offset, for this address so that other people can reference it when they contact someone at this address.	|
|	Address2_AddressId	|	string	|	256	|		|	Unique identifier for address 2.	|
|	Address2_AddressTypeCode	|	string	|	256	|		|	Select the secondary address type.	|
|	Address2_City	|	string	|	80	|		|	Type the city for the secondary address.	|
|	Address2_Composite	|	string	|	1000	|		|	Shows the complete secondary address.	|
|	Address2_Country	|	string	|	80	|		|	Type the country or region for the secondary address.	|
|	Address2_County	|	string	|	50	|		|	Type the county for the secondary address.	|
|	Address2_Fax	|	string	|	50	|		|	Type the fax number associated with the secondary address.	|
|	Address2_FreightTermsCode	|	string	|	256	|		|	Select the freight terms for the secondary address to make sure shipping orders are processed correctly.	|
|	Address2_Latitude	|	decimal	|		|		|	Type the latitude value for the secondary address for use in mapping and other applications.	|
|	Address2_Line1	|	string	|	250	|		|	Type the first line of the secondary address.	|
|	Address2_Line2	|	string	|	250	|		|	Type the second line of the secondary address.	|
|	Address2_Line3	|	string	|	250	|		|	Type the third line of the secondary address.	|
|	Address2_Longitude	|	decimal	|		|		|	Type the longitude value for the secondary address for use in mapping and other applications.	|
|	Address2_Name	|	string	|	100	|		|	Type a descriptive name for the secondary address, such as Corporate Headquarters.	|
|	Address2_PostalCode	|	string	|	20	|		|	Type the ZIP Code or postal code for the secondary address.	|
|	Address2_PostOfficeBox	|	string	|	20	|		|	Type the post office box number of the secondary address.	|
|	Address2_PrimaryContactName	|	string	|	100	|		|	Type the name of the main contact at the account's secondary address.	|
|	Address2_ShippingMethodCode	|	string	|	256	|		|	Select a shipping method for deliveries sent to this address.	|
|	Address2_StateOrProvince	|	string	|	50	|		|	Type the state or province of the secondary address.	|
|	Address2_Telephone1	|	string	|	50	|		|	Type the main phone number associated with the secondary address.	|
|	Address2_Telephone2	|	string	|	50	|		|	Type a second phone number associated with the secondary address.	|
|	Address2_Telephone3	|	string	|	50	|		|	Type a third phone number associated with the secondary address.	|
|	Address2_UPSZone	|	string	|	4	|		|	Type the UPS zone of the secondary address to make sure shipping charges are calculated correctly and deliveries are made promptly, if shipped by UPS.	|
|	Address2_UTCOffset	|	decimal	|		|		|	Select the time zone, or UTC offset, for this address so that other people can reference it when they contact someone at this address.	|
|	Address3_AddressId	|	string	|	256	|		|	Unique identifier for address 3.	|
|	Address3_AddressTypeCode	|	string	|	256	|		|	Select the third address type.	|
|	Address3_City	|	string	|	80	|		|	Type the city for the 3rd address.	|
|	Address3_Composite	|	string	|	1000	|		|	Shows the complete third address.	|
|	Address3_Country	|	string	|	80	|		|	the country or region for the 3rd address.	|
|	Address3_County	|	string	|	50	|		|	Type the county for the third address.	|
|	Address3_Fax	|	string	|	50	|		|	Type the fax number associated with the third address.	|
|	Address3_FreightTermsCode	|	string	|	256	|		|	Select the freight terms for the third address to make sure shipping orders are processed correctly.	|
|	Address3_Latitude	|	decimal	|		|		|	Type the latitude value for the third address for use in mapping and other applications.	|
|	Address3_Line1	|	string	|	250	|		|	the first line of the 3rd address.	|
|	Address3_Line2	|	string	|	250	|		|	the second line of the 3rd address.	|
|	Address3_Line3	|	string	|	250	|		|	the third line of the 3rd address.	|
|	Address3_Longitude	|	decimal	|		|		|	Type the longitude value for the third address for use in mapping and other applications.	|
|	Address3_Name	|	string	|	200	|		|	Type a descriptive name for the third address, such as Corporate Headquarters.	|
|	Address3_PostalCode	|	string	|	20	|		|	the ZIP Code or postal code for the 3rd address.	|
|	Address3_PostOfficeBox	|	string	|	20	|		|	the post office box number of the 3rd address.	|
|	Address3_PrimaryContactName	|	string	|	100	|		|	Type the name of the main contact at the account's third address.	|
|	Address3_ShippingMethodCode	|	string	|	256	|		|	Select a shipping method for deliveries sent to this address.	|
|	Address3_StateOrProvince	|	string	|	50	|		|	the state or province of the third address.	|
|	Address3_Telephone1	|	string	|	50	|		|	Type the main phone number associated with the third address.	|
|	Address3_Telephone2	|	string	|	50	|		|	Type a second phone number associated with the third address.	|
|	Address3_Telephone3	|	string	|	50	|		|	Type a third phone number associated with the primary address.	|
|	Address3_UPSZone	|	string	|	4	|		|	Type the UPS zone of the third address to make sure shipping charges are calculated correctly and deliveries are made promptly, if shipped by UPS.	|
|	Address3_UTCOffset	|	decimal	|		|		|	Select the time zone, or UTC offset, for this address so that other people can reference it when they contact someone at this address.	|
|	Aging30	|	decimal	|		|		|	For system use only.	|
|	Aging30_Base	|	decimal	|		|		|	Shows the Aging 30 field converted to the system's default base currency. The calculations use the exchange rate specified in the Currencies area.	|
|	Aging60	|	decimal	|		|		|	For system use only.	|
|	Aging60_Base	|	decimal	|		|		|	Shows the Aging 60 field converted to the system's default base currency. The calculations use the exchange rate specified in the Currencies area.	|
|	Aging90	|	decimal	|		|		|	For system use only.	|
|	Aging90_Base	|	decimal	|		|		|	Shows the Aging 90 field converted to the system's default base currency. The calculations use the exchange rate specified in the Currencies area.	|
|	Anniversary	|	date	|		|		|	Enter the date of the contact's wedding or service anniversary for use in customer gift programs or other communications.	|
|	AnnualIncome	|	decimal	|		|		|	Type the contact's annual income for use in profiling and financial analysis.	|
|	AnnualIncome_Base	|	decimal	|		|		|	Shows the Annual Income field converted to the system's default base currency. The calculations use the exchange rate specified in the Currencies area.	|
|	AssistantName	|	string	|	100	|		|	Type the name of the contact's assistant.	|
|	AssistantPhone	|	string	|	50	|		|	Type the phone number for the contact's assistant.	|
|	BirthDate	|	date	|		|		|	Enter the contact's birthday for use in customer gift programs or other communications.	|
|	Business2	|	string	|	50	|		|	Type a second business phone number for this contact.	|
|	Callback	|	string	|	50	|		|	Type a callback phone number for this contact.	|
|	ChildrensNames	|	string	|	255	|		|	Type the names of the contact's children for reference in communications and client programs.	|
|	Company	|	string	|	50	|		|	Type the company phone of the contact.	|
|	ContactId	|	string	|	36	|	PK	|	Unique identifier of the contact.	|
|	ContactNumber	|	string	|	256	|	PK	|	Contact number	|
|	CreatedBy	|	string	|	256	|		|	Shows who created the record.	|
|	CreatedByExternalParty	|	string	|	256	|		|	Shows the external party who created the record.	|
|	CreatedByExternalPartyName	|	string	|	100	|		|	CreatedByExternalPartyName	|
|	CreatedByExternalPartyYomiName	|	string	|	100	|		|	CreatedByExternalPartyYomiName	|
|	CreatedByName	|	string	|	100	|		|	CreatedByName	|
|	CreatedByYomiName	|	string	|	100	|		|	CreatedByYomiName	|
|	CreatedOn	|	date	|		|		|	Shows the date and time when the record was created. The date and time are displayed in the time zone selected in Microsoft Dynamics 365 options.	|
|	CreatedOnBehalfBy	|	string	|	256	|		|	Shows who created the record on behalf of another user.	|
|	CreatedOnBehalfByName	|	string	|	100	|		|	CreatedOnBehalfByName	|
|	CreatedOnBehalfByYomiName	|	string	|	100	|		|	CreatedOnBehalfByYomiName	|
|	CreditLimit	|	decimal	|		|		|	Type the credit limit of the contact for reference when you address invoice and accounting issues with the customer.	|
|	CreditLimit_Base	|	decimal	|		|		|	Shows the Credit Limit field converted to the system's default base currency for reporting purposes. The calculations use the exchange rate specified in the Currencies area.	|
|	CreditOnHold	|	boolean	|		|		|	Select whether the contact is on a credit hold, for reference when addressing invoice and accounting issues.	|
|	CustomerSizeCode	|	string	|	256	|		|	Select the size of the contact's company for segmentation and reporting purposes.	|
|	CustomerTypeCode	|	string	|	256	|		|	Select the category that best describes the relationship between the contact and your organization.	|
|	DefaultPriceLevelId	|	string	|	256	|		|	Choose the default price list associated with the contact to make sure the correct product prices for this customer are applied in sales opportunities, quotes, and orders.	|
|	DefaultPriceLevelIdName	|	string	|	100	|		|	DefaultPriceLevelIdName	|
|	Department	|	string	|	100	|		|	Type the department or business unit where the contact works in the parent company or business.	|
|	Description	|	string	|	2000	|		|	Type additional information to describe the contact, such as an excerpt from the company's website.	|
|	DoNotBulkEMail	|	boolean	|		|		|	Select whether the contact accepts bulk email sent through marketing campaigns or quick campaigns. If Do Not Allow is selected, the contact can be added to marketing lists, but will be excluded from the email.	|
|	DoNotBulkPostalMail	|	boolean	|		|		|	Select whether the contact accepts bulk postal mail sent through marketing campaigns or quick campaigns. If Do Not Allow is selected, the contact can be added to marketing lists, but will be excluded from the letters.	|
|	DoNotEMail	|	boolean	|		|		|	Select whether the contact allows direct email sent from Microsoft Dynamics 365. If Do Not Allow is selected, Microsoft Dynamics 365 will not send the email.	|
|	DoNotFax	|	boolean	|		|		|	Select whether the contact allows faxes. If Do Not Allow is selected, the contact will be excluded from any fax activities distributed in marketing campaigns.	|
|	DoNotPhone	|	boolean	|		|		|	Select whether the contact accepts phone calls. If Do Not Allow is selected, the contact will be excluded from any phone call activities distributed in marketing campaigns.	|
|	DoNotPostalMail	|	boolean	|		|		|	Select whether the contact allows direct mail. If Do Not Allow is selected, the contact will be excluded from letter activities distributed in marketing campaigns.	|
|	DoNotSendMM	|	boolean	|		|		|	Select whether the contact accepts marketing materials, such as brochures or catalogs. Contacts that opt out can be excluded from marketing initiatives.	|
|	EducationCode	|	string	|	256	|		|	Select the contact's highest level of education for use in segmentation and analysis.	|
|	EMailAddress1	|	string	|	100	|		|	Type the primary email address for the contact.	|
|	EMailAddress2	|	string	|	100	|		|	Type the secondary email address for the contact.	|
|	EMailAddress3	|	string	|	100	|		|	Type an alternate email address for the contact.	|
|	EmployeeId	|	string	|	50	|		|	Type the employee ID or number for the contact for reference in orders, service cases, or other communications with the contact's organization.	|
|	EntityImage	|	string	|	256	|		|	Shows the default image for the record.	|
|	EntityImage_Timestamp	|	decimal	|		|		|	EntityImageTimestamp	|
|	EntityImage_URL	|	string	|	200	|		|	EntityImageURL	|
|	EntityImageId	|	string	|	256	|		|	For internal use only.	|
|	ExchangeRate	|	decimal	|		|		|	Shows the conversion rate of the record's currency. The exchange rate is used to convert all money fields in the record from the local currency to the system's default currency.	|
|	ExternalUserIdentifier	|	string	|	50	|		|	Identifier for an external user.	|
|	FamilyStatusCode	|	string	|	256	|		|	Select the marital status of the contact for reference in follow-up phone calls and other communications.	|
|	Fax	|	string	|	50	|		|	Type the fax number for the contact.	|
|	FirstName	|	string	|	50	|		|	Type the contact's first name to make sure the contact is addressed correctly in sales calls, email, and marketing campaigns.	|
|	FollowEmail	|	boolean	|		|		|	Information about whether to allow following email activity like opens, attachment views and link clicks for emails sent to the contact.	|
|	FtpSiteUrl	|	string	|	200	|		|	Type the URL for the contact's FTP site to enable users to access data and share documents.	|
|	FullName	|	string	|	160	|		|	Combines and shows the contact's first and last names so that the full name can be displayed in views and reports.	|
|	GDPROptOut	|	boolean	|		|		|	Is this contact opted out of GDPR	|
|	GenderCode	|	string	|	256	|		|	Select the contact's gender to make sure the contact is addressed correctly in sales calls, email, and marketing campaigns.	|
|	GovernmentId	|	string	|	50	|		|	Type the passport number or other government ID for the contact for use in documents or reports.	|
|	HasChildrenCode	|	string	|	256	|		|	Select whether the contact has any children for reference in follow-up phone calls and other communications.	|
|	Home2	|	string	|	50	|		|	Type a second home phone number for this contact.	|
|	ImportSequenceNumber	|	decimal	|		|		|	Unique identifier of the data import or data migration that created this record.	|
|	IsAutoCreate	|	boolean	|		|		|	Information about whether the contact was auto-created when promoting an email or an appointment.	|
|	IsBackofficeCustomer	|	boolean	|		|		|	Select whether the contact exists in a separate accounting or other system, such as Microsoft Dynamics GP or another ERP database, for use in integration processes.	|
|	IsPrivate	|	boolean	|		|		|	IsPrivate	|
|	JobTitle	|	string	|	100	|		|	Type the job title of the contact to make sure the contact is addressed correctly in sales calls, email, and marketing campaigns.	|
|	LastName	|	string	|	50	|		|	Type the contact's last name to make sure the contact is addressed correctly in sales calls, email, and marketing campaigns.	|
|	LastOnHoldTime	|	date	|		|		|	Contains the date and time stamp of the last on hold time.	|
|	LastUsedInCampaign	|	date	|		|		|	Shows the date when the contact was last included in a marketing campaign or quick campaign.	|
|	LeadSourceCode	|	string	|	256	|		|	Select the primary marketing source that directed the contact to your organization.	|
|	ManagerName	|	string	|	100	|		|	Type the name of the contact's manager for use in escalating issues or other follow-up communications with the contact.	|
|	ManagerPhone	|	string	|	50	|		|	Type the phone number for the contact's manager.	|
|	MarketingOnly	|	boolean	|		|		|	Whether is only for marketing	|
|	MasterContactIdName	|	string	|	100	|		|	MasterContactIdName	|
|	MasterContactIdYomiName	|	string	|	100	|		|	MasterContactIdYomiName	|
|	MasterId	|	string	|	256	|		|	Unique identifier of the master contact for merge.	|
|	Merged	|	boolean	|		|		|	Shows whether the account has been merged with a master contact.	|
|	MiddleName	|	string	|	50	|		|	Type the contact's middle name or initial to make sure the contact is addressed correctly.	|
|	MobilePhone	|	string	|	50	|		|	Type the mobile phone number for the contact.	|
|	ModifiedBy	|	string	|	256	|		|	Shows who last updated the record.	|
|	ModifiedByExternalParty	|	string	|	256	|		|	Shows the external party who modified the record.	|
|	ModifiedByExternalPartyName	|	string	|	100	|		|	ModifiedByExternalPartyName	|
|	ModifiedByExternalPartyYomiName	|	string	|	100	|		|	ModifiedByExternalPartyYomiName	|
|	ModifiedByName	|	string	|	100	|		|	ModifiedByName	|
|	ModifiedByYomiName	|	string	|	100	|		|	ModifiedByYomiName	|
|	ModifiedOn	|	date	|		|		|	Shows the date and time when the record was last updated. The date and time are displayed in the time zone selected in Microsoft Dynamics 365 options.	|
|	ModifiedOnBehalfBy	|	string	|	256	|		|	Shows who last updated the record on behalf of another user.	|
|	ModifiedOnBehalfByName	|	string	|	100	|		|	ModifiedOnBehalfByName	|
|	ModifiedOnBehalfByYomiName	|	string	|	100	|		|	ModifiedOnBehalfByYomiName	|
|	NickName	|	string	|	100	|		|	Type the contact's nickname.	|
|	NumberOfChildren	|	decimal	|		|		|	Type the number of children the contact has for reference in follow-up phone calls and other communications.	|
|	OnHoldTime	|	decimal	|		|		|	Shows how long, in minutes, that the record was on hold.	|
|	OriginatingLeadId	|	string	|	256	|		|	Shows the lead that the contact was created if the contact was created by converting a lead in Microsoft Dynamics 365. This is used to relate the contact to the data on the originating lead for use in reporting and analytics.	|
|	OriginatingLeadIdName	|	string	|	100	|		|	OriginatingLeadIdName	|
|	OriginatingLeadIdYomiName	|	string	|	100	|		|	OriginatingLeadIdYomiName	|
|	OverriddenCreatedOn	|	date	|		|		|	Date and time that the record was migrated.	|
|	OwnerId	|	string	|	256	|		|	Enter the user or team who is assigned to manage the record. This field is updated every time the record is assigned to a different user.	|
|	OwnerIdName	|	string	|	100	|		|	OwnerIdName	|
|	OwnerIdType	|	string	|	256	|		|	Type of Owner	|
|	OwnerIdYomiName	|	string	|	100	|		|	OwnerIdYomiName	|
|	OwningBusinessUnit	|	string	|	256	|		|	Unique identifier of the business unit that owns the contact.	|
|	OwningTeam	|	string	|	256	|		|	Unique identifier of the team who owns the contact.	|
|	OwningUser	|	string	|	256	|		|	Unique identifier of the user who owns the contact.	|
|	Pager	|	string	|	50	|		|	Type the pager number for the contact.	|
|	ParentContactId	|	string	|	256	|		|	Unique identifier of the parent contact.	|
|	ParentContactIdName	|	string	|	100	|		|	ParentContactIdName	|
|	ParentContactIdYomiName	|	string	|	100	|		|	ParentContactIdYomiName	|
|	ParentCustomerId	|	string	|	256	|		|	Select the parent account or parent contact for the contact to provide a quick link to additional details, such as financial information, activities, and opportunities.	|
|	ParentCustomerIdName	|	string	|	160	|		|	ParentCustomerIdName	|
|	ParentCustomerIdType	|	string	|	256	|		|	Parent Customer Id Type	|
|	ParentCustomerIdYomiName	|	string	|	450	|		|	ParentCustomerIdYomiName	|
|	ParticipatesInWorkflow	|	boolean	|		|		|	Shows whether the contact participates in workflow rules.	|
|	PaymentTermsCode	|	string	|	256	|		|	Select the payment terms to indicate when the customer needs to pay the total amount.	|
|	PreferredAppointmentDayCode	|	string	|	256	|		|	Select the preferred day of the week for service appointments.	|
|	PreferredAppointmentTimeCode	|	string	|	256	|		|	Select the preferred time of day for service appointments.	|
|	PreferredContactMethodCode	|	string	|	256	|		|	Select the preferred method of contact.	|
|	PreferredEquipmentId	|	string	|	256	|		|	Choose the contact's preferred service facility or equipment to make sure services are scheduled correctly for the customer.	|
|	PreferredEquipmentIdName	|	string	|	100	|		|	PreferredEquipmentIdName	|
|	PreferredServiceId	|	string	|	256	|		|	Choose the contact's preferred service to make sure services are scheduled correctly for the customer.	|
|	PreferredServiceIdName	|	string	|	100	|		|	PreferredServiceIdName	|
|	PreferredSystemUserId	|	string	|	256	|		|	Choose the regular or preferred customer service representative for reference when scheduling service activities for the contact.	|
|	PreferredSystemUserIdName	|	string	|	100	|		|	PreferredSystemUserIdName	|
|	PreferredSystemUserIdYomiName	|	string	|	100	|		|	PreferredSystemUserIdYomiName	|
|	ProcessId	|	string	|	256	|		|	Shows the ID of the process.	|
|	Salutation	|	string	|	100	|		|	Type the salutation of the contact to make sure the contact is addressed correctly in sales calls, email messages, and marketing campaigns.	|
|	ShippingMethodCode	|	string	|	256	|		|	Select a shipping method for deliveries sent to this address.	|
|	SLAId	|	string	|	256	|		|	Choose the service level agreement (SLA) that you want to apply to the Contact record.	|
|	SLAInvokedId	|	string	|	256	|		|	Last SLA that was applied to this case. This field is for internal use only.	|
|	SLAInvokedIdName	|	string	|	100	|		|	SLAInvokedIdName	|
|	SLAName	|	string	|	100	|		|	SLAName	|
|	SpousesName	|	string	|	100	|		|	Type the name of the contact's spouse or partner for reference during calls, events, or other communications with the contact.	|
|	StageId	|	string	|	256	|		|	Shows the ID of the stage.	|
|	StatusCode	|	string	|	256	|		|	Select the contact's status.	|
|	SubscriptionId	|	string	|	256	|		|	For internal use only.	|
|	Suffix	|	string	|	10	|		|	Type the suffix used in the contact's name, such as Jr. or Sr. to make sure the contact is addressed correctly in sales calls, email, and marketing campaigns.	|
|	Telephone1	|	string	|	50	|		|	Type the main phone number for this contact.	|
|	Telephone2	|	string	|	50	|		|	Type a second phone number for this contact.	|
|	Telephone3	|	string	|	50	|		|	Type a third phone number for this contact.	|
|	TerritoryCode	|	string	|	256	|		|	Select a region or territory for the contact for use in segmentation and analysis.	|
|	TimeSpentByMeOnEmailAndMeetings	|	string	|	1250	|		|	Total time spent for emails (read and write) and meetings by me in relation to the contact record.	|
|	TimeZoneRuleVersionNumber	|	decimal	|		|		|	For internal use only.	|
|	TransactionCurrencyId	|	string	|	256	|		|	Choose the local currency for the record to make sure budgets are reported in the correct currency.	|
|	TransactionCurrencyIdName	|	string	|	100	|		|	TransactionCurrencyIdName	|
|	TraversedPath	|	string	|	1250	|		|	For internal use only.	|
|	UTCConversionTimeZoneCode	|	decimal	|		|		|	Time zone code that was in use when the record was created.	|
|	VersionNumber	|	decimal	|		|		|	Version number of the contact.	|
|	WebSiteUrl	|	string	|	200	|		|	Type the contact's professional or personal website or blog URL.	|
|	YomiFirstName	|	string	|	150	|		|	Type the phonetic spelling of the contact's first name, if the name is specified in Japanese, to make sure the name is pronounced correctly in phone calls with the contact.	|
|	YomiFullName	|	string	|	450	|		|	Shows the combined Yomi first and last names of the contact so that the full phonetic name can be displayed in views and reports.	|
|	YomiLastName	|	string	|	150	|		|	Type the phonetic spelling of the contact's last name, if the name is specified in Japanese, to make sure the name is pronounced correctly in phone calls with the contact.	|
|	YomiMiddleName	|	string	|	150	|		|	Type the phonetic spelling of the contact's middle name, if the name is specified in Japanese, to make sure the name is pronounced correctly in phone calls with the contact.	|