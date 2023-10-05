---
title: AccountPaymentTerm
description: This article provides information about the AccountPaymentTerm entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 05/05/2023
ms.custom: bap-template
---

# **AccountPaymentTerm**

[!INCLUDE[banner](../../includes/banner.md)]

Account Payment terms refer to the agreed-upon conditions and requirements that govern the payment process between a buyer and a seller in a business transaction. These terms outline when and how payments should be made and include details such as the payment method and due date. 

Payment terms are negotiated between the buyer and seller before the transaction takes place. They help establish clear expectations and ensure that both parties are aware of their payment obligations, reducing the risk of payment disputes and providing a framework for efficient financial management.



|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountPaymentTermId	|	string	|	36	|	Yes	|	The ID of the payment term for the account.	|
|	AccountPaymentTermNumber	|	string	|	256	|	Yes	|	The number or code for the payment term for the account.	|
|	Company	|	string	|	256	|	No	|	The name of the company for the account.	|
|	CreditCardCreditCheckType	|	string	|	256	|	No	|	The credit card credit check type.	|
|	CreditCardPaymentType	|	string	|	256	|	No	|	The credit card payment type.	|
|	CustomerDueDateUpdatePolicy	|	string	|	256	|	No	|	The customer due date update policy.	|
|	CutOffDayOfMonth	|	string	|	256	|	No	|	The cutoff day of month for the payment term.	|
|	Days	|	integer	|		|	No	|	The number of days in the payment term.	|
|	Description	|	string	|	4000	|	No	|	A description of the payment term.	|
|	IsCashPayment	|	boolean	|		|	No	|	Indicates if the account is enabled for cash payment.	|
|	IsCertifiedCompanyCheck	|	boolean	|		|	No	|	Is this account a certified account, yes or no boolean value.	|
|	IsDefaultPaymentTerm	|	boolean	|		|	No	|	The default payment term.	|
|	Name	|	string	|	256	|	No	|	The name of the payment term for the account.	|
|	NumberOfMonth	|	string	|	256	|	No	|	The length of payment terms expressed in months. |
|	NumberOfMonths	|	string	|	256	|	No	|	The length of payment terms expressed in months.	|
|	PaymentDayName	|	string	|	256	|	No	|	The name of the payment day.	For example, first day of the month, fifth day of the month, etc. |
|	PaymentMethodType	|	string	|	256	|	No	|	The method of payment for this account or to this account. For example, if it's for a customer, then its payment terms are for accounts receivables. If it's for a vendor or service provider, then its payment terms are for accounts payables.	|
|	PaymentScheduleName	|	string	|	256	|	No	|	The name of the payment schedule.	|
