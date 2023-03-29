---
title: Connect your SAP data to Supply Chain Center
description: This article provides information about connecting your SAP data to Microsoft Supply Chain Center
author: johnmichalak
ms.author: johnmichalak
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: how-to
ms.date: 03/30/2023
ms.custom: bap-template
---

# Connect your SAP data to Supply Chain Center

## SAP ERP connector
The SAP ERP connector, in beta, enables users to extract data from their SAP system and allows you to invoke RFC and BAPI functions using on-premises data gateway. This SAP RFC connector is supported by Power Platform Dataflows within Supply Chain Center. 

### Pre-requisites for SAP ERP connector
Enabling SAP ERP connector requires several pre-requisites to be completed. All pre-requisites must be completed on the same machine where extraction will be made and has admin permissions with access to the target SAP instance.   

  - Ensure the windows machine (64-bit OS) is updated and has access to the target SAP machine 
  - Ensure SAP credentials have requisite permission to run the desired RFC(s) or BAPI(s) 
  - Ensure SAP S User credentials can download the SAP .NET Connector installer 

**Setup instructions** 

The following installers must exist in desktop or virtual machine before using the connector: 

  - Go to SAP Connector for Microsoft .NET to download and install the NCo 3.0 for 64bit 
    - Do not install NCo 3.1 as this version is not yet supported  
    - Access to the download requires a valid S-user. You may need to reach out to your SAP team 
    - You must choose the 64-bit version, the 32-bit version will not work 
    - During installation, in the Optional setup steps window, make sure to select the Install assemblies to GAC option 
  - Install the SAP RFC Reader (V0.1.02232.26) which is an ADO.NET provider found here. 
    - .NET Framework 4.7.2 or greater is required 
    - Supported by Windows 10, Windows 11, Windows Server 2012 R2, Windows Server 2016, Windows Server 2019, Windows Server 2022 
  - Install the Power Query On prem Data gateway (https://go.microsoft.com/fwlink/?LinkId=2116849&clcid=0x409). To learn more about the gateway requirements or for support, follow this link (https://learn.microsoft.com/en-us/data-integration/gateway/service-gateway-install). 

**Connection Settings: Connecting to SAP RFC** 

To instantiate your dataflow connection to SAP ERP connector you will need to create a connection string. With the following parameters: 

|          **Name**         |       **Key**       |     **Required**    |          **Type**          |            **Description**              |
|---------------------------|---------------------|---------------------|----------------------------|-----------------------------------------|
|AS Host|AppServerHost|Application Server|string|The hostname of the SAP Application Server|
|Client | Client |Application and Message Server |Integer |The SAP client ID to connect to the SAP system|
|AS System Number|SystemNumber|Application Server|Integer| The SAP System’s System Number. It is a number ranging from 00 to 99 |  
| Message Server | MessageServerHost |Message Server|String|Hostname of the SAP System’s Message server| 
|Message Server Service Name/Port| MessageServerService | Message Server |String |Service Name or the Port Number under which the Message Server is listening for load balancing requests| 
| System ID | SystemID | Message Server | String | SAP systems three-letter system ID |
|Logon Group |LogonGroup |Message Server |String | The Logon Group for the SAP system from which the Message Server shall select and Application Server |
|Logon Type | LogonType |Application and Message Server |String | The type of logon to the SAP system, either application server logon (type A) or Group Logon (Type B aka Message Server). Values can be “ApplicationServer” or “Group” |

Setup SAP system connection string - This connector supports SAP authentication only currently. Constructing the script is dependent on connection type and is outlined below:  

  - **Application Server:**  

      - Connection string template: {"AppServerHost":"<application server>","Client":"<client id>","SystemNumber":"<system number","LogonType":"ApplicationServer"} 

      - You will want to replace everything in <> with your application server system settings eg for a server sap.contoso.com with system number 00 and client id 100         it would be {"AppServerHost":"sap.contoso.com","Client":"100","SystemNumber":"00","LogonType":"ApplicationServer"} 

  - **Message Server:** 

      - Connection string template: {"MessageServerHost": "<message server>", "MessageServerService":"<message server service name/port>", "LogonType": "Group",               "SystemID": "<system id>", "Client": "<client id>", "LogonGroup":"<logon group>"} 

      - You will want to replace everything in <> with your message server system settings noting that you may or may not require both MessageServerService and                 SystemID eg for a server 10.0.0.1 with messge server port 3333 and client id 800 and logon group COTO it would be {"MessageServerHost": "10.0.0.1",                     "MessageServerService":"3333", "LogonType": "Group", "Client": "800", "LogonGroup":"COTO"} 

  Although **Data gateway** is not marked as a requirement in connection settings, identifying the Data Gateway will be required for connecting to the SAP ERP connector.  
  
**Enabling Function Parsing**

 After connections the RFC will show up as a function with the parameter metadata and an optional “Enable Function Parsing” option. Fill in the parameters and click Invoke to get the data. Users should rely on their SAP produced documentation or custom documentation for RFC parameters.  

The function parsing mode for the connector understands contracts of two widely used RFCs: RFC_READ_TABLE and /SAPDS/RFC_READ_TABLE2. They will take this interpretation and parse out the output in an easy to read format instead of requiring the user to do so in M script. Function parsing can be enabled not only for the above mentioned RFCs but also for RFCs with the same contract such as BBP_RFC_READ_TABLE or /BODS/RFC_READ_TABLE2 including custom RFCS deployed by the customer to the SAP system. 
  
**Authentication**
  
The SAP ERP connector only supports basic SAP Authentication. Because the connector is designed to be used by multiple users of an app, the connections are not shared. Rather, each user will authenticate with the SAP system.  
  
**Known Issues and Limitations**

The following are some of the known issues and limitations of the SAP ERP Connector: 

  - The connector supports only RFCs and BAPIs 
  - The connector does not support receiving messages from SAP Server 
  - Transactional RFCs (tRFCs) are not supported. 
  - The gateway has a 2-MB payload limit for write operations and an 8-MB compressed data response limit for read operations 
  
  
**Frequently Asked Questions (FAQ)**

**Q**: The SAP ERP Beta connector is labeled as 3rd Party, is this connector not created or managed by Microsoft?
  
**A**: The connector was created by Microsoft and is managed by Microsoft. As a beta connector it will hold a “3rd party” label until it becomes generally available.  

**Q**: I am getting the following error when attempting to connect “The given data source kind is not supported Data source kind SAPERP”, how do I address?  
**A**: As a custom connector we default save the connection in your [System Drive]\Windows\ServiceProfiles\PBIEqwService\Documents\Power BI Desktop\Custom Connectors folder, if this folder does not exist or if gateway is configured to use a different custom connector folder you will see the above error. To remediate the user will need to copy the SAPERP.mez connector file from [System Drive]\Windows\ServiceProfiles\PBIEqwService\Documents\Power BI Desktop\Custom Connectors and copy in to the folder that you configured in your gateway.  

**Q**: Do I always need to identify a Data gateway in connection settings?
**A**: As part of connection setting you must identify a Data gateway in order to successfully connect through the SAP ERP connector 

**Q**: My connection continues to fail, what can I do to remediate? 
**A**: Make sure to check that installers described above are up to date and current. Reinstalling drivers may solve your connection issues.  

