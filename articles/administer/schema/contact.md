---
title: Contact
description: This article provides information about the Contact entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/30/2023
ms.custom: bap-template
---

# Contact

The contact entity refers to an individual or organization associated with the account.
The contact could be a primary contact person, a designated account manager, or any other relevant party representing the account.

A contact for an account entity would include information such as:

First Name and Last Name: The full name of the contact person or the organization's name.

Position/Role: The position or role the contact person holds within the organization.

Contact Details: Contact information like phone number, email address, mailing address, or any other preferred means of communication.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountId	|	string	|	36	|		|	Unique identifier of the account with which the contact is associated.	|
|	AccountIdName	|	string	|	100	|		|	Unique identifier of the account name.	|
|	AccountIdYomiName	|	string	|	100	|		|	Unique identifier of the account Yomi name.	|
|	AccountNumber	|	string	|	256	|		|	The account number.	|
|	AccountRoleCode	|	string	|	256	|		|	A contact's role within the company or sales process (for example, "decision maker", "employee", or "influencer".	|
|	AccountTypeCode	|	string	|	256	|		|	The type of account (for example, "Vendor", "Customer", or "Manager".	|
|	Address1_AddressId	|	string	|	256	|		|	Unique identifier for the primary address.	|
|	Address1_AddressTypeCode	|	string	|	256	|		|	Code for the primary address type.	|
|	Address1_City	|	string	|	80	|		|	The city for the primary address.	|
|	Address1_Composite	|	string	|	1000	|		|	The complete primary address.	|
|	Address1_Country	|	string	|	80	|		|	The country or region for the primary address.	|
|	Address1_County	|	string	|	50	|		|	The county for the primary address.	|
|	Address1_Fax	|	string	|	50	|		|	The fax number associated with the primary address.	|
|	Address1_FreightTermsCode	|	string	|	256	|		|	Code for the freight terms of the primary address to ensure shipping orders are processed correctly.	|
|	Address1_Latitude	|	decimal	|		|		|	The latitude value for the primary address for use in mapping and other applications.	|
|	Address1_Line1	|	string	|	250	|		|	The first line of the primary address.	|
|	Address1_Line2	|	string	|	250	|		|	The second line of the primary address.	|
|	Address1_Line3	|	string	|	250	|		|	The third line of the primary address.	|
|	Address1_Longitude	|	decimal	|		|		|	The longitude value for the primary address for use in mapping and other applications.	|
|	Address1_Name	|	string	|	200	|		|	Descriptive name for the primary address (for example, "Corporate Headquarters").	|
|	Address1_PostalCode	|	string	|	20	|		|	The ZIP Code or postal code for the primary address.	|
|	Address1_PostOfficeBox	|	string	|	20	|		|	The post office box number of the primary address.	|
|	Address1_PrimaryContactName	|	string	|	100	|		|	The name of the main contact at the account's primary address.	|
|	Address1_ShippingMethodCode	|	string	|	256	|		|	Shipping method code for deliveries sent to this address.	|
|	Address1_StateOrProvince	|	string	|	50	|		|	The state or province of the primary address.	|
|	Address1_Telephone1	|	string	|	50	|		|	The main phone number associated with the primary address.	|
|	Address1_Telephone2	|	string	|	50	|		|	Second phone number associated with the primary address.	|
|	Address1_Telephone3	|	string	|	50	|		|	Third phone number associated with the primary address.	|
|	Address1_UPSZone	|	string	|	4	|		|	The UPS zone of the primary address. Ensures that shipping charges are calculated correctly and deliveries are made promptly, if shipped by UPS.	|
|	Address1_UTCOffset	|	decimal	|		|		|	The time zone (UTC offset) for the primary address. Allows users to reference the time zone when contacting someone at this address.	|
|	Address2_AddressId	|	string	|	256	|		|	Unique identifier for the secondary address.	|
|	Address2_AddressTypeCode	|	string	|	256	|		|	The secondary address type.	|
|	Address2_City	|	string	|	80	|		|	The city for the secondary address.	|
|	Address2_Composite	|	string	|	1000	|		|	The complete secondary address.	|
|	Address2_Country	|	string	|	80	|		|	The country or region for the secondary address.	|
|	Address2_County	|	string	|	50	|		|	The county for the secondary address.	|
|	Address2_Fax	|	string	|	50	|		|	The fax number associated with the secondary address.	|
|	Address2_FreightTermsCode	|	string	|	256	|		|	The freight terms for the secondary address. Ensures that shipping orders are processed correctly.	|
|	Address2_Latitude	|	decimal	|		|		|	The latitude value of the secondary address for use in mapping and other applications.	|
|	Address2_Line1	|	string	|	250	|		|	The first line of the secondary address.	|
|	Address2_Line2	|	string	|	250	|		|	The second line of the secondary address.	|
|	Address2_Line3	|	string	|	250	|		|	The third line of the secondary address.	|
|	Address2_Longitude	|	decimal	|		|		|	The longitude value of the secondary address for use in mapping and other applications.	|
|	Address2_Name	|	string	|	100	|		|	Descriptive name for the secondary address (for example, "Corporate Headquarters").	|
|	Address2_PostalCode	|	string	|	20	|		|	The ZIP Code or postal code for the secondary address.	|
|	Address2_PostOfficeBox	|	string	|	20	|		|	The post office box number of the secondary address.	|
|	Address2_PrimaryContactName	|	string	|	100	|		|	The name of the main contact at the account's secondary address.	|
|	Address2_ShippingMethodCode	|	string	|	256	|		|	Shipping method code for deliveries sent to this address.	|
|	Address2_StateOrProvince	|	string	|	50	|		|	The state or province of the secondary address.	|
|	Address2_Telephone1	|	string	|	50	|		|	The main phone number associated with the secondary address.	|
|	Address2_Telephone2	|	string	|	50	|		|	The second phone number associated with the secondary address.	|
|	Address2_Telephone3	|	string	|	50	|		|	The third phone number associated with the secondary address.	|
|	Address2_UPSZone	|	string	|	4	|		|	The UPS zone of the secondary address. Ensures that shipping charges are calculated correctly and deliveries are made promptly, if shipped by UPS.	|
|	Address2_UTCOffset	|	decimal	|		|		|	Time zone (UTC offset) for this address. Allows users to reference the time zone when they contact someone at this address.	|
|	Address3_AddressId	|	string	|	256	|		|	Unique identifier for the third address.	|
|	Address3_AddressTypeCode	|	string	|	256	|		|	The third address type.	|
|	Address3_City	|	string	|	80	|		|	The city for the third address.	|
|	Address3_Composite	|	string	|	1000	|		|	The complete third address.	|
|	Address3_Country	|	string	|	80	|		|	The country or region for the third address.	|
|	Address3_County	|	string	|	50	|		|	The county for the third address.	|
|	Address3_Fax	|	string	|	50	|		|	The fax number associated with the third address.	|
|	Address3_FreightTermsCode	|	string	|	256	|		|	The freight terms for the third address. Ensures that shipping orders are processed correctly.	|
|	Address3_Latitude	|	decimal	|		|		|	The latitude value for the third address for use in mapping and other applications.	|
|	Address3_Line1	|	string	|	250	|		|	The first line of the third address.	|
|	Address3_Line2	|	string	|	250	|		|	The second line of the third address.	|
|	Address3_Line3	|	string	|	250	|		|	The third line of the third address.	|
|	Address3_Longitude	|	decimal	|		|		|	The longitude value for the third address for use in mapping and other applications.	|
|	Address3_Name	|	string	|	200	|		|	Descriptive name for the third address (for example, "Corporate Headquarters").	|
|	Address3_PostalCode	|	string	|	20	|		|	The ZIP Code or postal code for the third address.	|
|	Address3_PostOfficeBox	|	string	|	20	|		|	The post office box number of the third address.	|
|	Address3_PrimaryContactName	|	string	|	100	|		|	The name of the main contact at the account's third address.	|
|	Address3_ShippingMethodCode	|	string	|	256	|		|	Shipping method code for deliveries sent to this address.	|
|	Address3_StateOrProvince	|	string	|	50	|		|	The state or province of the third address.	|
|	Address3_Telephone1	|	string	|	50	|		|	The main phone number associated with the third address.	|
|	Address3_Telephone2	|	string	|	50	|		|	Second phone number associated with the third address.	|
|	Address3_Telephone3	|	string	|	50	|		|	Third phone number associated with the primary address.	|
|	Address3_UPSZone	|	string	|	4	|		|	The UPS zone of the third address. Ensures that shipping charges are calculated correctly and deliveries are made promptly, if shipped by UPS.	|
|	Address3_UTCOffset	|	decimal	|		|		|	The time zone (UTC offset) for the third address. Allows users to reference the time zone when they contact someone at this address.	|
|	Aging30	|	decimal	|		|		|	For system use only.	|
|	Aging30_Base	|	decimal	|		|		|	The Aging 30 field value converted to the system's default base currency. The calculations use the exchange rate specified in the Currencies area.	|
|	Aging60	|	decimal	|		|		|	For system use only.	|
|	Aging60_Base	|	decimal	|		|		|	The Aging 60 field value converted to the system's default base currency. The calculations use the exchange rate specified in the Currencies area.	|
|	Aging90	|	decimal	|		|		|	For system use only.	|
|	Aging90_Base	|	decimal	|		|		|	The Aging 90 field value converted to the system's default base currency. The calculations use the exchange rate specified in the Currencies area.	|
|	Anniversary	|	date	|		|		|	The date of the contact's wedding or service anniversary. For use in customer gift programs or other communications.	|
|	AnnualIncome	|	decimal	|		|		|	The contact's annual income. For use in profiling and financial analysis.	|
|	AnnualIncome_Base	|	decimal	|		|		|	The Annual Income field value converted to the system's default base currency. The calculations use the exchange rate specified in the Currencies area.	|
|	AssistantName	|	string	|	100	|		|	The name of the contact's assistant.	|
|	AssistantPhone	|	string	|	50	|		|	The phone number for the contact's assistant.	|
|	BirthDate	|	date	|		|		|	The contact's birthday. For use in customer gift programs or other communications.	|
|	Business2	|	string	|	50	|		|	Second business phone number for the contact.	|
|	Callback	|	string	|	50	|		|	Callback phone number for the contact.	|
|	ChildrensNames	|	string	|	255	|		|	The names of the contact's children. For reference in communications and client programs.	|
|	Company	|	string	|	50	|		|	The company phone number of the contact.	|
|	ContactId	|	string	|	36	|	PK	|	Unique identifier of the contact.	|
|	ContactNumber	|	string	|	256	|	PK	|	The contact number.	|
|	CreatedBy	|	string	|	256	|		|	The user who created the record.	|
|	CreatedByExternalParty	|	string	|	256	|		|	The external party who created the record.	|
|	CreatedByExternalPartyName	|	string	|	100	|		|	The external party name who created the record.	|
|	CreatedByExternalPartyYomiName	|	string	|	100	|		|	The external party Yomi name of who created the record	|
|	CreatedByName	|	string	|	100	|		|	The name of the user who created the record.	|
|	CreatedByYomiName	|	string	|	100	|		|	The Yomi name of the user who created the record.	|
|	CreatedOn	|	date	|		|		|	The date and time when the record was created. Displayed in the time zone selected in Dynamics 365.	|
|	CreatedOnBehalfBy	|	string	|	256	|		|	The user who created the record on behalf of another user.	|
|	CreatedOnBehalfByName	|	string	|	100	|		|	The name of the user who created the record on behalf of another user.	|
|	CreatedOnBehalfByYomiName	|	string	|	100	|		|	The Yomi name of the user who created the record on behalf of another user.	|
|	CreditLimit	|	decimal	|		|		|	The credit limit of the contact. For reference when addressing invoice and accounting issues with the customer.	|
|	CreditLimit_Base	|	decimal	|		|		|	Shows the Credit Limit field value converted to the system's default base currency for reporting purposes. The calculations use the exchange rate specified in the Currencies area.	|
|	CreditOnHold	|	boolean	|		|		|	Specifies whether the contact is on a credit hold. Referenced when addressing invoice and accounting issues.	|
|	CustomerSizeCode	|	string	|	256	|		|	The size of the contact's company. Used for segmentation and reporting purposes.	|
|	CustomerTypeCode	|	string	|	256	|		|	The category that best describes the relationship between the contact and your organization.	|
|	DefaultPriceLevelId	|	string	|	256	|		|	The default price list associated with the contact. Ensures that the correct product prices for this customer are applied in sales opportunities, quotes, and orders.	|
|	DefaultPriceLevelIdName	|	string	|	100	|		|	The name of the default price list associated with the contact.	|
|	Department	|	string	|	100	|		|	The department or business unit where the contact works in the parent company or business.	|
|	Description	|	string	|	2000	|		|	Additional information that describes the contact (for example, an excerpt from the company's website.	|
|	DoNotBulkEMail	|	boolean	|		|		|	Specifies whether the contact accepts bulk email sent through marketing campaigns or quick campaigns. If **Do Not Allow** is selected, the contact can be added to marketing lists, but will be excluded from the email.	|
|	DoNotBulkPostalMail	|	boolean	|		|		|	Specifies whether the contact accepts bulk postal mail sent through marketing campaigns or quick campaigns. If **Do Not Allow** is selected, the contact can be added to marketing lists, but will be excluded from the letters.	|
|	DoNotEMail	|	boolean	|		|		|	Specifies whether the contact allows direct email sent from Microsoft Dynamics 365. If **Do Not Allow** is selected, Microsoft Dynamics 365 will not send the email.	|
|	DoNotFax	|	boolean	|		|		|	Specifies whether the contact allows faxes. If **Do Not Allow** is selected, the contact is excluded from any fax activities distributed in marketing campaigns.	|
|	DoNotPhone	|	boolean	|		|		|	Specifies whether the contact accepts phone calls. If **Do Not Allow** is selected, the contact is excluded from any phone call activities distributed in marketing campaigns.	|
|	DoNotPostalMail	|	boolean	|		|		|	Specifies whether the contact allows direct mail. If **Do Not Allow** is selected, the contact is excluded from letter activities distributed in marketing campaigns.	|
|	DoNotSendMM	|	boolean	|		|		|	Specifies whether the contact accepts marketing materials, such as brochures or catalogs. Contacts that opt out can be excluded from marketing initiatives.	|
|	EducationCode	|	string	|	256	|		|	Code representing the contact's highest level of education. For use in segmentation and analysis.	|
|	EMailAddress1	|	string	|	100	|		|	The primary email address for the contact.	|
|	EMailAddress2	|	string	|	100	|		|	The secondary email address for the contact.	|
|	EMailAddress3	|	string	|	100	|		|	Alternate email address for the contact.	|
|	EmployeeId	|	string	|	50	|		|	Employee ID or number for the contact. Referenced in orders, service cases, or other communications with the contact's organization.	|
|	EntityImage	|	string	|	256	|		|	Default enity image for the record.	|
|	EntityImage_Timestamp	|	decimal	|		|		|	Timestamp of the default enity image for the record.	|
|	EntityImage_URL	|	string	|	200	|		|	Image URL of the default enity image for the record.	|
|	EntityImageId	|	string	|	256	|		|	For internal use only.	|
|	ExchangeRate	|	decimal	|		|		|	The conversion rate of the record's currency. The exchange rate is used to convert all money fields in the record from the local currency to the system's default currency.	|
|	ExternalUserIdentifier	|	string	|	50	|		|	Identifier for an external user.	|
|	FamilyStatusCode	|	string	|	256	|		|	Marital status of the contact. Referenced in follow-up phone calls and other communications.	|
|	Fax	|	string	|	50	|		|	Fax number for the contact.	|
|	FirstName	|	string	|	50	|		|	Contact's first name. Ensures that the contact is addressed correctly in sales calls, email, and marketing campaigns.	|
|	FollowEmail	|	boolean	|		|		|	Specifies whether to allow following email activity like opens, attachment views, and link clicks for emails sent to the contact.	|
|	FtpSiteUrl	|	string	|	200	|		|	The URL for the contact's FTP site to enable users to access data and share documents.	|
|	FullName	|	string	|	160	|		|	Combined first and last names for the contact. Used to display the contact's full name in views and reports.	|
|	GDPROptOut	|	boolean	|		|		|	Specifies whether the contact has opted out of General Data Protection Regulation (GDPR).	|
|	GenderCode	|	string	|	256	|		|	The contact's gender. Ensures that the contact is addressed correctly in sales calls, email, and marketing campaigns.	|
|	GovernmentId	|	string	|	50	|		|	The passport number or other government ID of the contact for use in documents or reports.	|
|	HasChildrenCode	|	string	|	256	|		|	Code for whether the contact has any children. Referenced in follow-up phone calls and other communications.	|
|	Home2	|	string	|	50	|		|	Second home phone number for the contact.	|
|	ImportSequenceNumber	|	decimal	|		|		|	Unique identifier of the data import or data migration process that created this record.	|
|	IsAutoCreate	|	boolean	|		|		|	Specifies whether the contact was autogenerated when promoting an email or an appointment.	|
|	IsBackofficeCustomer	|	boolean	|		|		|	Specifies whether the contact exists in a separate accounting or other system (for example, Microsoft Dynamics GP or another ERP database) for use in integration processes.	|
|	IsPrivate	|	boolean	|		|		|	Specifies whether the contact is private.	|
|	JobTitle	|	string	|	100	|		|	The job title of the contact. Ensures that the contact is addressed correctly in sales calls, email, and marketing campaigns.	|
|	LastName	|	string	|	50	|		|	The contact's last name. Ensures that the contact is addressed correctly in sales calls, email, and marketing campaigns.	|
|	LastOnHoldTime	|	date	|		|		|	Contains the date and timestamp of the last on hold time.	|
|	LastUsedInCampaign	|	date	|		|		|	The date when the contact was last included in a marketing campaign or quick campaign.	|
|	LeadSourceCode	|	string	|	256	|		|	The primary marketing source that directed the contact to your organization.	|
|	ManagerName	|	string	|	100	|		|	The name of the contact's manager. For use in escalating issues or other follow-up communications with the contact.	|
|	ManagerPhone	|	string	|	50	|		|	The phone number for the contact's manager.	|
|	MarketingOnly	|	boolean	|		|		|	Specifies whether the contact is to be used only for marketing.	|
|	MasterContactIdName	|	string	|	100	|		|	Unique identifier of the master contact name.	|
|	MasterContactIdYomiName	|	string	|	100	|		|	Unique identifier of the master contact Yomi name.	|
|	MasterId	|	string	|	256	|		|	Unique identifier of the master contact for merge.	|
|	Merged	|	boolean	|		|		|	Specifies whether the account has been merged with a master contact.	|
|	MiddleName	|	string	|	50	|		|	The contact's middle name or initial. Ensures that the contact is addressed correctly.	|
|	MobilePhone	|	string	|	50	|		|	The mobile phone number for the contact.	|
|	ModifiedBy	|	string	|	256	|		|	User who last updated the record.	|
|	ModifiedByExternalParty	|	string	|	256	|		|	External party who modified the record.	|
|	ModifiedByExternalPartyName	|	string	|	100	|		|	Name of the external party who modified the record.	|
|	ModifiedByExternalPartyYomiName	|	string	|	100	|		|	Yomi name of the external party who modified the record.	|
|	ModifiedByName	|	string	|	100	|		|	Name of the user who modified the record.	|
|	ModifiedByYomiName	|	string	|	100	|		|	Yomi name of the user who modified the record.	|
|	ModifiedOn	|	date	|		|		|	Date and time when the record was last updated. The date and time are displayed in the time zone selected in Microsoft Dynamics 365.	|
|	ModifiedOnBehalfBy	|	string	|	256	|		|	User who last updated the record on behalf of another user.	|
|	ModifiedOnBehalfByName	|	string	|	100	|		|	Name of the user who last updated the record on behalf of another user.	|
|	ModifiedOnBehalfByYomiName	|	string	|	100	|		|	Yomi name of the user who last updated the record on behalf of another user.	|
|	NickName	|	string	|	100	|		|	The contact's nickname.	|
|	NumberOfChildren	|	decimal	|		|		|	The number of children the contact has. Referenced in follow-up phone calls and other communications.	|
|	OnHoldTime	|	decimal	|		|		|	How long (in minutes) that the record was on hold.	|
|	OriginatingLeadId	|	string	|	256	|		|	Unique indentifier of the originating lead for the contact, if the contact was created by converting a lead in Dynamics 365. Used to relate the contact to the data on the originating lead for use in reporting and analytics.	|
|	OriginatingLeadIdName	|	string	|	100	|		|	Name of the originating lead for the contact, if the contact was created by converting a lead in Dynamics 365.	|
|	OriginatingLeadIdYomiName	|	string	|	100	|		|	Yomi name of the originating lead for the contact, if the contact was created by converting a lead in Dynamics 365.	|
|	OverriddenCreatedOn	|	date	|		|		|	Date and time that the record was migrated.	|
|	OwnerId	|	string	|	256	|		|	Unique indentifier of the user or team (owner) assigned to manage the record. This field is updated every time the record is assigned to a different user.	|
|	OwnerIdName	|	string	|	100	|		|	Name of the user or team (owner) assigned to manage the record. |
|	OwnerIdType	|	string	|	256	|		|	Type of the user or team (owner) assigned to manage the record.	|
|	OwnerIdYomiName	|	string	|	100	|		|	Yomi name of the user or team (owner) assigned to manage the record.	|
|	OwningBusinessUnit	|	string	|	256	|		|	Business unit that owns the contact.	|
|	OwningTeam	|	string	|	256	|		|	Team who owns the contact.	|
|	OwningUser	|	string	|	256	|		|	User who owns the contact.	|
|	Pager	|	string	|	50	|		|	Pager number for the contact.	|
|	ParentContactId	|	string	|	256	|		|	Unique identifier of the parent contact.	|
|	ParentContactIdName	|	string	|	100	|		|	Name of the parent contact.	|
|	ParentContactIdYomiName	|	string	|	100	|		|	Yomi name	of the parent contact.|
|	ParentCustomerId	|	string	|	256	|		|	Unique identifier of the parent account or parent customer. Referenced to provide a quick link to additional details, such as financial information, activities, and opportunities.	|
|	ParentCustomerIdName	|	string	|	160	|		|	Name of the parent account or parent customer.	|
|	ParentCustomerIdType	|	string	|	256	|		|	Type	of the parent account or parent customer.|
|	ParentCustomerIdYomiName	|	string	|	450	|		|	Yomi name of the parent account or parent customer.	|
|	ParticipatesInWorkflow	|	boolean	|		|		|	Specifies whether the contact participates in workflow rules.	|
|	PaymentTermsCode	|	string	|	256	|		|	Code for the payment terms to indicate when the customer needs to pay the total amount.	|
|	PreferredAppointmentDayCode	|	string	|	256	|		|	Preferred day of the week for service appointments.	|
|	PreferredAppointmentTimeCode	|	string	|	256	|		|	Preferred time of day for service appointments.	|
|	PreferredContactMethodCode	|	string	|	256	|		|	Preferred method of contact.	|
|	PreferredEquipmentId	|	string	|	256	|		|	Unique identifier of the contact's preferred service facility or equipment. Ensures that services are scheduled correctly for the customer.	|
|	PreferredEquipmentIdName	|	string	|	100	|		|	Name of the contact's preferred service facility or equipment.	|
|	PreferredServiceId	|	string	|	256	|		|	Unique identifier of the contact's preferred service. Ensures that services are scheduled correctly for the customer.	|
|	PreferredServiceIdName	|	string	|	100	|		|	Name of the contact's preferred service.	|
|	PreferredSystemUserId	|	string	|	256	|		|	Unique identifier of the regular or preferred customer service representative. Referenced when scheduling service activities for the contact.	|
|	PreferredSystemUserIdName	|	string	|	100	|		|	Name of the regular or preferred customer service representative.	|
|	PreferredSystemUserIdYomiName	|	string	|	100	|		|	Yomi name of the regular or preferred customer service representative.	|
|	ProcessId	|	string	|	256	|		|	Unique identifier of the process.	|
|	Salutation	|	string	|	100	|		|	Salutation of the contact. Ensures that the contact is addressed correctly in sales calls, email messages, and marketing campaigns.	|
|	ShippingMethodCode	|	string	|	256	|		|	Shipping method code for deliveries sent to this address.	|
|	SLAId	|	string	|	256	|		|	Unique identifier of the service level agreement (SLA) to apply to the contact record.	|
|	SLAInvokedId	|	string	|	256	|		|	Last SLA that was applied to this case. This field is for internal use only.	|
|	SLAInvokedIdName	|	string	|	100	|		|	Name of the last SLA that was applied to this case.	|
|	SLAName	|	string	|	100	|		|	Name of the SLA.	|
|	SpousesName	|	string	|	100	|		|	Name of the contact's spouse or partner. Referenced during calls, events, or other communications with the contact.	|
|	StageId	|	string	|	256	|		|	Unique identifier of the stage.	|
|	StatusCode	|	string	|	256	|		|	Code for the contact's status.	|
|	SubscriptionId	|	string	|	256	|		|	For internal use only.	|
|	Suffix	|	string	|	10	|		|	Suffix used in the contact's name (for example, Jr. or Sr.). Ensures that the contact is addressed correctly in sales calls, email, and marketing campaigns.	|
|	Telephone1	|	string	|	50	|		|	Main phone number for the contact.	|
|	Telephone2	|	string	|	50	|		|	Second phone number for the contact.	|
|	Telephone3	|	string	|	50	|		|	Third phone number for the contact.	|
|	TerritoryCode	|	string	|	256	|		|	Region or territory for the contact for use in segmentation and analysis.	|
|	TimeSpentByMeOnEmailAndMeetings	|	string	|	1250	|		|	Total time spent for emails (read and write) and meetings in relation to the contact record.	|
|	TimeZoneRuleVersionNumber	|	decimal	|		|		|	For internal use only.	|
|	TransactionCurrencyId	|	string	|	256	|		|	Unique identifier of the local currency for the record. Ensures that budgets are reported in the correct currency.	|
|	TransactionCurrencyIdName	|	string	|	100	|		|	Name of the local currency for the record.	|
|	TraversedPath	|	string	|	1250	|		|	For internal use only.	|
|	UTCConversionTimeZoneCode	|	decimal	|		|		|	Time zone code used when the record was created.	|
|	VersionNumber	|	decimal	|		|		|	Version number of the contact.	|
|	WebSiteUrl	|	string	|	200	|		|	Contact's professional or personal website or blog URL.	|
|	YomiFirstName	|	string	|	150	|		|	Phonetic spelling of the contact's first name, if the name is specified in Japanese. Ensures that the name is pronounced correctly in phone calls with the contact.	|
|	YomiFullName	|	string	|	450	|		|	Combined phonetic spelling of the contact's first and last names of the contact, if the name is specified in Japanese. Ensures that the full phonetic name can be displayed in views and reports.	|
|	YomiLastName	|	string	|	150	|		|	Phonetic spelling of the contact's last name, if the name is specified in Japanese. Ensures that the name is pronounced correctly in phone calls with the contact.	|
|	YomiMiddleName	|	string	|	150	|		|	Phonetic spelling of the contact's middle name, if the name is specified in Japanese. Ensures that the name is pronounced correctly in phone calls with the contact.	|
