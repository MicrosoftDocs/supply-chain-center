---
title: AccountPaymentTerm
description: This is about AccountPaymentTerm entity.
author: mkannapiran
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply - chain - center
ms.topic: conceptual
ms.date: 04 / 21 / 2023
ms.custom: bap - template
---

# **AccountPaymentTerm**

Account Payment terms refer to the agreed-upon conditions and requirements that govern the payment process between a buyer and a seller in a business transaction. These terms outline when and how payments should be made, including details such as the payment method, due date etc. Payment terms are usually negotiated between the buyer and seller before the transaction takes place. They help establish clear expectations and ensure that both parties are aware of their payment obligations, reducing the risk of payment disputes and providing a framework for efficient financial management.


|	Attribute	|	Datatype	|	Length	|	Primary Key	|	Description	|
|---------------|--------|------|----------|-----------|
|	AccountPaymentTermId	|	string	|	36	|	Yes	|	Id of the payment term for the account	|
|	AccountPaymentTermNumber	|	string	|	256	|	Yes	|	Number or code of the payment term for the account	|
|	Company	|	string	|	256	|	No	|	Company of the account	|
|	CreditCardCreditCheckType	|	string	|	256	|	No	|	Credit card credit check type	|
|	CreditCardPaymentType	|	string	|	256	|	No	|	Credit card payment type	|
|	CustomerDueDateUpdatePolicy	|	string	|	256	|	No	|	Customer due date update policy	|
|	CutOffDayOfMonth	|	string	|	256	|	No	|	Cut off day of month for payment term	|
|	Days	|	integer	|		|	No	|	Payment term days	|
|	Description	|	string	|	4000	|	No	|	Description of the payment term	|
|	IsCashPayment	|	boolean	|		|	No	|	Is the account enabled for cash payment	|
|	IsCertifiedCompanyCheck	|	boolean	|		|	No	|	Is certified company check	|
|	IsDefaultPaymentTerm	|	boolean	|		|	No	|	Is this a default payment term	|
|	Name	|	string	|	256	|	No	|	Name of the payment term for account	|
|	NumberOfMonth	|	string	|	256	|	No	|	Number of month for payment terms	|
|	NumberOfMonths	|	string	|	256	|	No	|	Number of months for payment terms	|
|	PaymentDayName	|	string	|	256	|	No	|	Name of the payment day	|
|	PaymentMethodType	|	string	|	256	|	No	|	Method of payment for this account or to this account. Example if it s a customer then it would be payment terms for accounts receivables and if it s a vendor or service provider then it would be payment terms for accounts payables	|
|	PaymentScheduleName	|	string	|	256	|	No	|	Name of the payment schedule	|
