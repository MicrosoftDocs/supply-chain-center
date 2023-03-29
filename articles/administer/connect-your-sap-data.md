---
title: Connect your SAP data to Supply Chain Center
description: This article provides information about connecting your SAP data to Microsoft Supply Chain Center
author: mkannapiran 
ms.author: kamanick
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: how-to
ms.date: 03/30/2023
ms.custom: bap-template
---

# Connect your SAP data to Supply Chain Center

This article provides information about connecting your SAP data to Microsoft Supply Chain Center.

## SAP ERP connector
The SAP ERP connector, in beta, enables you to extract data from their SAP system, and allows you to invoke RFC and BAPI functions using on-premises data gateway. This SAP RFC connector is supported by Microsoft Power Platform Dataflows within Supply Chain Center. 

### Prerequisites for SAP ERP connector
Enabling SAP ERP connector requires several prerequisites to be completed. All prerequisites must be completed on the same machine where the data extraction is made, and has administrator permissions with access to the target SAP instance.   

Complete the following prerequisites:
  - Ensure the Microsoft Windows machine (64-bit OS) is updated and has access to the target SAP machine. 
  - Ensure the SAP credentials have requisite permission to run the desired RFC(s) or BAPI(s). 
  - Ensure the SAP S User credentials can download the SAP .NET Connector installer. 

## Set up the SAP ERP connector 

The following installers must exist in desktop or virtual machine before using the connector. To set up the SAP ERP connector, complete the following steps. 

  1. Go to SAP Connector for Microsoft .NET to download and install the NCo 3.0 for 64bit. 
  
     >[!Important]
     > Do not install NCo 3.1 as this version is not yet supported.
     
     - Access to the download requires a valid S-user. You may need to reach out to your SAP team for this information. 
     - You must choose the 64-bit version, the 32-bit version will not work. 
     - During installation, in the **Optional setup steps** window, make sure to select the **Install assemblies to GAC** option. 
  1. Install the SAP RFC Reader (V0.1.02232.26) which is an ADO.NET provider found here. 
     1. .NET Framework 4.7.2 or greater is required. 
     1. The SAP RFC Reader is supported by Microsoft Windows 10, Microsoft Windows 11, Microsoft Windows Server 2012 R2, Microsoft Windows Server 2016, Microsoft Windows Server 2019, Microsoft Windows Server 2022.
  1. Install the Microsoft [Power Query On prem Data gateway](https://go.microsoft.com/fwlink/?LinkId=2116849&clcid=0x409). To learn more about the gateway requirements or for support, see [Install an on-premises data gateway](/data-integration/gateway/service-gateway-install.md). 

## Connection settings for the SAP RFC connector

To instantiate your dataflow connection to SAP ERP connector you will need to create a connection string. With the following parameters: 

|          **Name**         |       **Key**       |     **Required**    |          **Type**          |            **Description**              |
|---------------------------|---------------------|---------------------|----------------------------|-----------------------------------------|
|AS Host|AppServerHost|Application Server|string|The hostname of the SAP Application Server.|
|Client | Client |Application and Message Server |Integer |The SAP client ID to connect to the SAP system.|
|AS System Number|SystemNumber|Application Server|Integer| The SAP System’s System Number. It is a number ranging from 00 to 99.|  
| Message Server | MessageServerHost |Message Server|String|Hostname of the SAP System’s Message server.| 
|Message Server Service Name/Port| MessageServerService | Message Server |String |Service Name or the Port Number under which the Message Server is listening for load balancing requests.| 
| System ID | SystemID | Message Server | String | SAP systems three-letter system ID.|
|Logon Group |LogonGroup |Message Server |String | The Logon Group for the SAP system from which the Message Server shall select and Application Server.|
|Logon Type | LogonType |Application and Message Server |String | The type of logon to the SAP system, either application server logon (type A) or Group Logon (Type B aka Message Server). Values can be “ApplicationServer” or “Group”.|

## Set up the SAP system connection string

The SAP system connector currently only supports SAP authentication. Constructing the script is dependent on connection type and is outlined below:  

  - **Application Server:**  

      - **Connection string template**: {"AppServerHost":"\<application server\>","Client":"\<client id\>","SystemNumber":"\<system number\>","LogonType":"ApplicationServer"} 

      - Replace everything between <> with your application server system settings. For example, for this server, sap.contoso.com, with the system number 00, and client ID 100, the connection string is: {"AppServerHost":"sap.contoso.com","Client":"100","SystemNumber":"00","LogonType":"ApplicationServer"}. 

  - **Message Server:** 

      - **Connection string template**: {"MessageServerHost": "\<message server\>", "MessageServerService":"\<message server service name/port\>", "LogonType": "Group",               "SystemID": "\<system id\>", "Client": "\<client id\>", "LogonGroup":"\<logon group\>"} 

      - Replace everything between <> with your message server system settings, noting that you may or may not require both MessageServerService and                 SystemID. For example, for this server, 10.0.0.1, with messge server port 3333, client ID 800, and logon group COTO, the connection strin is: {"MessageServerHost": "10.0.0.1","MessageServerService":"3333", "LogonType": "Group", "Client": "800", "LogonGroup":"COTO"}. 

> [!Note]
> Although **Data gateway** is not marked as a requirement in connection settings, identifying the Data Gateway is required for connecting to the SAP ERP connector.  
  
## Enabling Function Parsing

After connection, the RFC shows up as a function with the parameter metadata and an optional **Enable Function Parsing** option. Fill in the parameters and select **Invoke** to get the data. See your SAP produced documentation or your custom documentation for the RFC parameters.  

The function parsing mode for the connector understands contracts of two widely used RFCs: RFC_READ_TABLE and /SAPDS/RFC_READ_TABLE2. They'll take this interpretation and parse out the output in an easy to read format instead of requiring the user to do so in M script. Function parsing can be enabled not only for the above mentioned RFCs but also for RFCs with the same contract such as BBP_RFC_READ_TABLE or /BODS/RFC_READ_TABLE2 including custom RFCS deployed by the customer to the SAP system. 
  
## Authentication
  
The SAP ERP connector only supports basic SAP Authentication. Because the connector is designed to be used by multiple users of an app, the connections are not shared. Rather, each user authenticates with the SAP system.  
  
## Known Issues and Limitations

The following are some of the known issues and limitations of the SAP ERP Connector: 

  - The connector supports only RFCs and BAPIs. 
  - The connector does not support receiving messages from SAP Server. 
  - Transactional RFCs (tRFCs) are not supported. 
  - The gateway has a 2-MB payload limit for write operations and an 8-MB compressed data response limit for read operations. 
  
  
## Frequently Asked Questions (FAQ)

For answers to frequently asked questions, see [Connect your SAP data to Supply Chain Center FAQ](connect-to-sap-faq.md).

