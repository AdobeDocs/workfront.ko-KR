---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion에서 큰 파일 작업
description: 현재 Workfront 및 HTTP 커넥터에서 대용량 파일을 지원할 수 있습니다.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: d380f495c098e45897ca58627571dfc7dfdcb0f7
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 0%

---

# Adobe Workfront Fusion에서 큰 파일 작업

현재 Workfront 및 HTTP 커넥터에서 대용량 파일을 지원할 수 있습니다.

## 큰 파일 크기가 시나리오 실행 시간에 미치는 영향

큰 파일은 Fusion 시나리오에서 업로드, 다운로드 또는 처리하는 데 시간이 걸릴 수 있습니다. 파일 크기에는 제한이 없지만 시나리오 실행 시간에는 40분 제한이 있습니다. 따라서 큰 파일이 실행되어 40분 이상 걸리는 경우 시나리오가 실패합니다.

시나리오 실행 시간은 시나리오 크기, 모듈 복잡성 및 네트워크 속도의 영향을 받을 수도 있습니다. 따라서 큰 파일을 사용할 때는 시나리오의 이러한 측면을 고려하는 것이 좋습니다.


<!--
## Connectors that do not support large files

Some Fusion connectors do not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.

The following connectors do **not** support large files. 

* Archive
* Box
* Convert
* CSV
* Datastores
* Flow control
* FTP
* JSON
* JWT
* Markdown
* Math
* Microsoft Word templates
* MIME
* Microsoft SQL
* SFTP
* Adobe Acrobat Sign
* SOAP
* Tools
* XML

If a connector is not on this list, it does not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.-->






<!--## Connectors that support large files

The following connectors support large files.

Workfront
HTTP
Webhooks
Salesforce
Microsoft Email
Workfront Proof
AEM Assets
Email
Slack
Jira
Microsoft Excel
SharePoint
Frame.io
Adobe PDF Services
Marketo
Azure Devops 
Google Email
Jira Server
Google Sheets
Microsoft OneDrive
ServiceNow 
AWS S3
Bynder
OneDrive Business
Adobe Authenticator
Google Drive
Microsoft Dynamics
Google Docs
NetSuite
Airtable
Azure AD
QuickBase 
Adobe Target
Adobe Campaign Classic
Microsoft Calendar
Workfront Planning
HubSpot CRM  
DropBox
Cloud Convert
Egnyte
Adobe Firefly
OpenAI / Chat GPT
Allocadia
Cvent
GitLab 
Google Team Drive
Google Calendar
Workfront SDL Managed Translation
Widen
Workfront Boards
Google Slides
Qualtrics
Microsoft Power BI
Adobe Photoshop
Anaplan
DocuSign 
MariaDB
Adobe Creative Cloud Libraries
Figma
AEM Forms
Datadog
GitHub 
Google Forms
Adobe I/O Events
Trello
Workday
Adobe Journey Optimizer
Adobe Lightroom









If a file is not on this list, it does not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.

-->