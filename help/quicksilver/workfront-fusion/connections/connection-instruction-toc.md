---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: connections-annd-webhooks
title: 에서 연결 만들기 [!DNL Adobe Workfront Fusion]
description: 연결은 연결되는 앱 또는 웹 서비스의 API에 의해 설정된 요구 사항을 준수해야 합니다. 이러한 이유로 연결 설정에 대한 지침은 앱 또는 웹 서비스에 따라 다릅니다. 이 문서는 연결에 대한 지침을 식별하고 찾는 데 도움이 됩니다 [!DNL Adobe Workfront Fusion] 선택한 앱 또는 웹 서비스에 연결합니다.
author: Becky
feature: Workfront Fusion
exl-id: fb1a2af4-da58-48ba-85b5-1903d6a3ceda
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 1%

---

# 에서 연결 만들기 [!DNL Adobe Workfront Fusion]

<!-- Audited: 3/2024-->

연결은 연결되는 앱 또는 웹 서비스의 API에 의해 설정된 요구 사항을 준수해야 합니다. 이러한 이유로 연결 설정에 대한 지침은 앱 또는 웹 서비스에 따라 다릅니다. 이 문서는 연결에 대한 지침을 식별하고 찾는 데 도움이 됩니다 [!DNL Adobe Workfront Fusion] 선택한 앱 또는 웹 서비스에 연결합니다.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td>  
   <td> <p>임의</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td>  
   <td> <p>새로운 기능: [!UICONTROL Standard]</p><p>또는</p><p>현재: [!UICONTROL Work] 이상</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td>  
   <td> 
   <p>현재: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p> 
   <p>또는</p> 
   <p>레거시: 모두 </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">제품</td>  
   <td> 
   <p>신규:</p> <ul><li>[!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Workfront] 플랜: 조직에서 구매해야 합니다. [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] 플랜: [!DNL Workfront Fusion] 포함됩니다.</li></ul> 
   <p>또는</p> 
   <p>현재: 조직에서 구매해야 합니다. [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 구성이 필요하지 않은 앱 또는 웹 서비스에 연결

대부분의 경우 모듈을 사용하여 추가 정보가 거의 없거나 전혀 없는 연결을 만들 수 있습니다. [!DNL Workfront Fusion] 은 인증을 자동으로 처리합니다.

특별한 고려 사항 없이 연결을 만드는 방법에 대한 지침은 [에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침](../../workfront-fusion/connections/connect-to-fusion-general.md).

## 에 연결 [!DNL Microsoft] 앱 또는 웹 서비스

의 대부분 [!DNL Microsoft] 의 앱 [!DNL Workfront Fusion] 추가 정보 없이 연결을 만들 수 있습니다.

다음 상황에서는 연결을 만드는 데 추가 단계가 필요합니다.

* 사용 [!DNL Microsoft Dynamics 365] 모듈.

  자세한 내용은 [[!DNL Microsoft Dynamics 365] 모듈](../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

* 에 연결 중 [!DNL Microsoft Graph API] 사용 [!UICONTROL HTTP] 모듈

  자세한 내용은 [호출 [!DNL MS Graph REST API] 를 통해 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 요청] 모듈](../../workfront-fusion/connections/call-the-ms-graph-rest-api.md).

## 에 연결 [!DNL Google] 앱 또는 웹 서비스

에 연결하는 프로세스입니다 [!DNL Google] 앱은 종류에 따라 다를 수 있습니다. [!DNL Google] 사용 중인 계정입니다. 또한, [!DNL Google] 에 연결할 때 보안 조치를 추가로 구성해야 할 수 있습니다. [!DNL Workfront Fusion].

자세한 내용은 다음을 참조하십시오.

* [연결 [!DNL Adobe Workfront Fusion] 끝 [!DNL Google Services] 사용자 정의 OAuth 클라이언트 사용](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)
* [연결 [!DNL Adobe Workfront Fusion] 끝 [!DNL Google Services] 업데이트된 보안 조치 포함](../../workfront-fusion/connections/connect-to-google-with-new-security-measures.md)

## 추가 구성이 필요한 기타 앱

다음 앱은 의 기본 구성을 따르지 않습니다. [!DNL Workfront Fusion] 연결. 해당 앱에 대한 문서에서 이러한 앱을 연결하는 방법에 대한 지침을 찾을 수 있습니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>앱/웹 서비스</th> 
   <th>연결에 대한 추가 정보</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect" class="MCXref xref">연결 [!DNL Adobe Workfront] 끝 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md" class="MCXref xref">[!DNL Adobe Workfront] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Allocadia]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md#connect" class="MCXref xref">연결 [!DNL Allocadia] 끝 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md" class="MCXref xref">[!DNL Allocadia] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Anaplan]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md#connect" class="MCXref xref">연결 [!DNL Anaplan] 끝 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md" class="MCXref xref">[!DNL Anaplan] 모듈</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL AWS S3]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md#connecti" class="MCXref xref">연결 [!DNL AWS] 끝 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md" class="MCXref xref">[!DNL AWS S3] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Azure DevOps]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md#connect" class="MCXref xref">연결 [!DNL Azure DevOps] 끝 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref">[!DNL Azure DevOps] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Bynder]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md#connect" class="MCXref xref">연결 [!DNL Bynder] 끝 [!DNL Workfront Fusion] </a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md" class="MCXref xref">[!DNL Bynder] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL CloudConvert]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md#connect" class="MCXref xref">연결 [!DNL CloudConvert] 끝 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md" class="MCXref xref">[!DNL CloudConvert] 모듈</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL Cvent]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md#connect" class="MCXref xref">연결 [!DNL Cvent] 끝 [!DNL Adobe Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md" class="MCXref xref">[!DNL Cvent] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Datadog]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md#connect" class="MCXref xref">연결 [!DNL Datadog] 끝 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md" class="MCXref xref">[!DNL Datadog] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL DocuSign]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md#connect" class="MCXref xref">연결 [!DNL DocuSign] 끝 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md" class="MCXref xref">[!DNL DocuSign] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>이메일</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md#connecti" class="MCXref xref">전자 메일을 다음으로 연결 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/email-modules.md" class="MCXref xref">[!UICONTROL Email] 모듈</a></td>

<tr> 
   <td role="rowheader"> <p>[!DNL Gmail]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md#connect3" class="MCXref xref">연결 [!DNL Gmail] 끝 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md" class="MCXref xref">[!DNL Gmail] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Cloud]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect" class="MCXref xref">연결 [!DNL Jira Cloud] 끝 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Server]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect2" class="MCXref xref">연결 [!DNL Jira Server] 끝 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MariaDB]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md#connect" class="MCXref xref">연결 [!DNL MariaDB] 끝 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md" class="MCXref xref">[!DNL MariaDB] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Marketo]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md#connect" class="MCXref xref">연결 [!DNL Marketo] 끝 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md" class="MCXref xref">[!DNL Marketo] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MS Dynamics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md#connect" class="MCXref xref">연결 [!DNL Microsoft Dynamics 365] 끝 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref">[!DNL Microsoft Dynamics 365] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Qualtrics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md#connecti" class="MCXref xref">연결 중 [!DNL Qualtrics] 끝 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md" class="MCXref xref">[!DNL Qualtrics] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL ServiceNow]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md#connect" class="MCXref xref">연결 [!DNL ServiceNow] 끝 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md" class="MCXref xref">[!DNL ServiceNow] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SFTP</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sftp.md#connect" class="MCXref xref">SFTP를에 연결 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/sftp.md" class="MCXref xref">[!UICONTROL SFTP] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL SharePoint]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md#connect" class="MCXref xref">연결 [!DNL SharePoint] 끝 [!DNL Workfront Fusion]</a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md" class="MCXref xref">[!DNL SharePoint] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Split.io]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md#connect" class="MCXref xref">연결 [!DNL Split.io] 끝 [!DNL Workfront Fusion] </a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md" class="MCXref xref">[!DNL Split.io] 모듈</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>확장</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md#connect" class="MCXref xref">연결 [!DNL Widen] 끝 [!DNL Workfront Fusion] </a> 위치: <a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md" class="MCXref xref">[!DNL Widen] 모듈</a></td> 
  </tr> 
 </tbody> 
</table>
