---
title: Connect your SAP data to Supply Chain Center
description: This article provides information about how to connect your SAP data to Microsoft Supply Chain Center.
author: mkannapiran 
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: how-to
ms.date: 03/30/2023
ms.custom: bap-template
---

# Connect your SAP data to Supply Chain Center

[!INCLUDE[banner](../includes/banner.md)]

This article provides information about how to connect your SAP data to Microsoft Supply Chain Center.

## SAP ERP connector

The SAP ERP connector, which is currently in beta, lets you extract data from your SAP system, and invoke Remote Function Call (RFC) and Business Application Programming Interface (BAPI) functions by using an on-premises data gateway. The SAP ERP connector is supported by Microsoft Power Platform dataflows in Supply Chain Center.

### Prerequisites for the SAP ERP connector

Before you can enable the SAP ERP connector, the following prerequisites must be completed. All these prerequisites must be completed on the same machine where the data extraction is done. The user must have administrator permissions on the machine which has access to the target SAP instance.

- Ensure that the Microsoft Windows machine (64-bit operating system) is updated and has access to the target SAP machine.
- Ensure that the SAP credentials have the necessary permission to run the desired RFCs or BAPIs.
- Ensure that the SAP S-user credentials can download the installer for SAP ERP Connector for Microsoft .NET (NCo).

## Set up the SAP ERP connector

Some installers must exist on the desktop or virtual machine before you can use the connector. Follow these steps to set up the SAP ERP connector.

1. Go to the [SAP Connector for Microsoft .NET](https://support.sap.com/en/product/connectors/msnet.html) page to download and install NCo 3.0 for 64 bit.

    > [!IMPORTANT]
    > Do **not** install NCo 3.1, because that version isn't yet supported.

    - Access to the download requires a valid S-user. You might have to contact your SAP team for this information.
    - You must select the 64-bit version. The 32-bit version won't work.
    - During installation, on the **Optional setup steps** page, be sure to select the **Install assemblies to GAC** option.

1. Install the [SAP RFC Reader](https://download.microsoft.com/download/6/3/c/63c54361-0fbb-4078-844f-45a3d9c1ce5a/SapRfcReaderInstall.msi) (V0.1.02232.26).

    - The SAP RFC Reader is an ADO.NET provider. The .NET Framework version 4.7.2 or later is required.
    - The SAP RFC Reader is supported by Windows 10, Windows 11, Windows Server 2012 R2, Windows Server 2016, Windows Server 2019, and Windows Server 2022.

1. Install the [Power Query On-premises Data gateway](https://go.microsoft.com/fwlink/?LinkId=2116849&clcid=0x409). For more information about the gateway requirements, or for support, see [Install an on-premises data gateway](/data-integration/gateway/service-gateway-install).

## Connection settings for the SAP RFC connector

To instantiate your dataflow connection to the SAP ERP connector, you must create a connection string that includes the following parameters.

| Name | Key | Required by | Type | Description |
|---|---|---|---|---|
| AS Host | AppServerHost | Application Server | String | The host name of the SAP Application Server. |
| Client | Client | Application and Message Server | Integer | The SAP client ID that's used to connect to the SAP system. |
| AS System Number | SystemNumber | Application Server | Integer | The SAP system's system number, which is a number from 00 through 99. |
| Message Server | MessageServerHost | Message Server | String | The host name of the SAP system's Message Server. | 
| Message Server Service Name/Port | MessageServerService | Message Server | String | The service name or port number that the Message Server is listening under for load balancing requests. | 
| System ID | SystemID | Message Server | String | The SAP system's three-letter system ID. |
| Logon Group | LogonGroup | Message Server | String | The SAP system's logon group, which the Message Server and Application Server selects from. |
| Logon Type | LogonType | Application and Message Server | String | The type of logon to the SAP system: either Application Server logon (type A) or group logon (type B, also known as Message Server logon). The value can be **ApplicationServer** or **Group**. |

## Set up the SAP system connection string

The SAP ERP connector currently supports only SAP authentication. Construction of the script depends on the connection type, as outlined here:

- **Application Server:** Use the following template for the connection string:

    \{"AppServerHost":"\<application server\>","Client":"\<client id\>","SystemNumber":"\<system number\>","LogonType":"ApplicationServer"\}

    Replace each placeholder in angle brackets (\<&hellip;\>) with your Application Server's system settings. For example, here's the connection string for server sap.contoso.com that uses system number 00 and client ID 100:

    \{"AppServerHost":"sap.contoso.com","Client":"100","SystemNumber":"00","LogonType":"ApplicationServer"\}

- **Message Server:** Use the following template for the connection string:

    \{"MessageServerHost": "\<message server\>", "MessageServerService":"\<message server service name/port\>", "LogonType": "Group", "SystemID": "\<system id\>", "Client": "\<client id\>", "LogonGroup":"\<logon group\>"\}

    Replace each placeholder in angle brackets (\<&hellip;\>) with your Message Server's system settings. However, note that you might not need both the **MessageServerService** parameter and the **SystemID** parameter. For example, here's the connection string for server 10.0.0.1 that uses Message Server port 3333, client ID 800, and logon group COTO:

    \{"MessageServerHost": "10.0.0.1","MessageServerService":"3333", "LogonType": "Group", "Client": "800", "LogonGroup":"COTO"\}

> [!IMPORTANT]
> Although **Data gateway** isn't marked as a requirement in the connection settings, identification of the data gateway is required for connection to the SAP ERP connector.

## Enable function parsing

After connection, the RFC appears as a function that has the parameter metadata and an optional **Enable Function Parsing** option. Fill in the parameters, and then select **Invoke** to get the data. For information about the RFC parameters, see your SAP-produced documentation or your custom documentation.

The function parsing mode for the connector can interpret contracts of two widely used RFCs: RFC\_READ\_TABLE and /SAPDS/RFC\_READ_TABLE2. Based on its interpretation, it parses the output in an easy-to-read format. Therefore, the user doesn't have to perform this action in M script.

Function parsing can be enabled not only for the previously mentioned RFCs but also for RFCs that use the same contract, such as BBP\_RFC\_READ\_TABLE or /BODS/RFC\_READ\_TABLE2. These RFC include custom RFCS that the customer deployed to the SAP system.

## Authentication

The SAP ERP connector supports only basic SAP authentication. Because the connector is designed to be used by multiple users of an app, the connections aren't shared. Instead, each user authenticates with the SAP system.

## Known issues and limitations

Here are some of the known issues and limitations of the SAP ERP connector:

- The connector supports only RFCs and BAPIs.
- The connector doesn't support receiving messages from SAP Server.
- Transactional RFCs (tRFCs) aren't supported.
- The gateway has a 2-megabyte (MB) payload limit for write operations and an 8-MB compressed data response limit for read operations.

## Frequently asked questions

For answers to frequently asked questions, see [Connect your SAP data to Supply Chain Center FAQ](../troubleshoot-faqs/connect-to-sap-faq.md).
