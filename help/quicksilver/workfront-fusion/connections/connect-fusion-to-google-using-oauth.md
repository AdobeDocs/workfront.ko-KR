---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: 사용자 지정 OAuth 클라이언트를 사용하여  [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 연결
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 0%

---

# 사용자 지정 OAuth 클라이언트를 사용하여 [!DNL Adobe Workfront Fusion]을(를) [!DNL Google Services]에 연결

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [사용자 지정 OAuth 클라이언트를 사용하여 Adobe Workfront Fusion을 Google 서비스에 연결](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-fusion-to-google-using-oauth.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

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
   <p>현재: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시: 모두 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>신규:</p> <ul><li>[!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Workfront] 플랜: 조직에서 [!DNL Adobe Workfront Fusion]을(를) 구매해야 합니다.</li><li>[!UICONTROL Ultimate] [!DNL Workfront] 계획: [!DNL Workfront Fusion]이(가) 포함되어 있습니다.</li></ul>
   <p>또는</p>
   <p>현재: 조직에서 [!DNL Adobe Workfront Fusion]을(를) 구매해야 합니다.</p>
   </td> 
  </tr>
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## 전제 조건

이 연결을 만들려면 기존 [!DNL Google] 계정이 필요합니다.

## 사용자 지정 OAuth 클라이언트를 사용하여 Fusion을 Google 서비스에 연결

이 연결을 만들려면 Google Cloud 플랫폼에서 프로젝트를 만들고 구성한 다음 해당 프로젝트를 기반으로 Fusion에서 연결을 구성해야 합니다.

* [ [!DNL Google Cloud Platform]에 프로젝트 만들기](#create-a-project-on-google-cloud-platform)
* [[!UICONTROL OAuth 동의 구성] 설정](#configure-oauth-consent-settings)
* [OAuth 자격 증명 만들기](#create-oauth-credentials)
* [ [!DNL Google] in [!DNL Workfront Fusion]에 연결](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>이 절차는 다음 용도로 사용됩니다.
>
>* 개인 사용([!DNL `@gmail.com`] 및 [!DNL `@googlemail.com`]명의 사용자)
>* 내부 사용( 사용자 지정 OAuth 클라이언트를 사용하는 사용자 [!DNL Google Workspace]명)

### [!DNL Google Cloud Platform]에 프로젝트 만들기

[!DNL Google Cloud] 플랫폼에서 프로젝트를 만들려면:

1. [!DNL Google] 자격 증명을 사용하여 [[!DNL Google Cloud] 플랫폼](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project)에 로그인합니다.
1. 왼쪽 패널에서 **[!UICONTROL 대시보드]**&#x200B;를 클릭합니다.
1. 화면 오른쪽 상단의 **[!UICONTROL 프로젝트 만들기]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 프로젝트 이름]**&#x200B;을(를) 입력한 다음 **[!UICONTROL 만들기]**&#x200B;를 클릭합니다.

1. 화면 상단 근처에 있는 **[!UICONTROL API 및 서비스 사용]** 탭을 클릭합니다.
1. 화면 상단의 **[!UICONTROL API 및 서비스 검색]** 필드에 사용할 서비스 이름(예: [!DNL Gmail] API 또는 [!DNL Google Drive] API)을 입력합니다.
1. 표시되면 [!DNL Workfront Fusion]에 연결할 API 또는 서비스를 클릭합니다.
1. 선택한 API를 사용하려면 **[!UICONTROL 사용]**&#x200B;을 클릭하세요.
1. 활성화하려는 각 API에 대해 6~8단계를 반복합니다.

   >[!NOTE]
   >
   >[!DNL Google Drive] API와 사용하려는 모든 [!DNL Google] 앱의 API(예: [!DNL Google Sheets] API)를 활성화해야 합니다.

1. 표시되는 화면에서 오른쪽 상단의 **[!UICONTROL 자격 증명 만들기]**&#x200B;를 클릭합니다.
1. 이 문서의 [OAuth 동의 설정 구성](#configure-oauth-consent-settings) 섹션을 계속합니다.

### [!UICONTROL OAuth 동의] 설정 구성

1. 왼쪽 패널에서 **[!UICONTROL OAuth 동의 화면]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 외부]**&#x200B;를 선택한 다음 **[!UICONTROL 만들기]**&#x200B;를 클릭합니다.

   >[!NOTE]
   >
   >이 옵션을 선택하면 요금이 부과되지 않습니다. 자세한 내용은 확인 요구 사항에 대한 예외 항목에 대한 [!DNL Google]의 정보를 참조하십시오.

1. 다음과 같이 필수 필드를 채웁니다.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 앱 이름]</p> </td> 
      <td> <p>동의를 요청하는 앱의 이름을 입력합니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 사용자 지원 이메일]</td> 
      <td>사용자가 이 앱에 연결할 때 동의에 대한 질문이 있는 경우 연락할 수 있는 이메일 주소를 입력하십시오.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 전자 메일 주소]</td> 
      <td>Google에서 프로젝트 변경 사항에 대해 알리는 데 사용할 수 있는 이메일 주소를 하나 이상 입력합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. [!UICONTROL 승인된 도메인]에서 **[!UICONTROL 도메인 추가]**&#x200B;를 클릭하고 `workfrontfusion.com`을(를) 입력하십시오.

1. **[!UICONTROL 저장 후 계속]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 범위 추가 또는 제거]**&#x200B;를 클릭합니다.
1. 오른쪽 패널에서 다음 범위를 활성화합니다.

<table style="table-layout:auto">
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>서비스/API</th> 
      <th>필수 범위</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p>[!DNL Gmail]</p> </td> 
      <td> <p>https://mail.google.com/</p> <p>https://www.googleapis.com/auth/gmail.labels</p> <p>https://www.googleapis.com/auth/gmail.send</p> <p>https://www.googleapis.com/auth/gmail.readonly</p> <p>https://www.googleapis.com/auth/gmail.compose</p> <p>https://www.googleapis.com/auth/gmail.insert</p> <p>https://www.googleapis.com/auth/gmail.modify</p> <p>https://www.googleapis.com/auth/gmail.metadata</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!DNL Google Drive]</p> </td> 
      <td> <p>https://www.googleapis.com/auth/drive</p> <p>https://www.googleapis.com/auth/drive.readonly</p> </td> 
     </tr> 
    </tbody> 
   </table>

목록을 확장하거나 목록의 다음 페이지로 이동하여 모두 표시해야 할 수 있습니다.

1. **[!UICONTROL 업데이트]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 저장 후 계속]**&#x200B;을 클릭합니다.
1. (선택 사항) 프로젝트에 테스트 사용자를 추가합니다.
1. **[!UICONTROL 저장 후 계속]**&#x200B;을 클릭합니다.
1. 정보가 정확한지 검사한 다음 **[!UICONTROL 대시보드로 돌아가기]**&#x200B;를 클릭합니다.

   >[!NOTE]
   >
   >[!DNL Google]까지 동의 화면과 확인 신청서를 제출할 필요가 없습니다.

1. [OAuth 자격 증명 만들기](#create-oauth-credentials)를 계속합니다.

### OAuth 자격 증명 만들기

1. 왼쪽 패널에서 **[!UICONTROL 자격 증명]**&#x200B;을 클릭합니다.

   >[!NOTE]
   >
   >활성화한 첫 번째 API 또는 서비스([!DNL Gmail] 또는 [!DNL Google Drive])가 아닌 경우 새 자격 증명을 만들 필요가 없습니다.

1. 화면 상단 근처에 있는 **[!UICONTROL 자격 증명 만들기]**&#x200B;를 클릭한 다음 드롭다운 메뉴에서 **[!UICONTROL OAuth 클라이언트 ID]**&#x200B;을(를) 선택합니다.

1. 다음과 같이 필수 필드를 채웁니다.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Application type]</td> 
      <td> <p> [!UICONTROL 웹 애플리케이션]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 이름]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. [!UICONTROL 승인된 리디렉션 URI]에서 **[!UICONTROL URI 추가]**&#x200B;를 클릭하고 다음 중 **one**&#x200B;을(를) 입력하십시오.

   * [!DNL Gmail] 또는 [!DNL Google Drive]의 경우: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * 다른 [!DNL Google]개 앱의 경우: `https://app.workfrontfusion.com/oauth/cb/google`

1. Click **[!UICONTROL Create]**.

   [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호]가 표시됩니다.

1. [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호]를 안전한 위치에 복사합니다. [!DNL Workfront Fusion]에서 연결하는 데 사용합니다.
1. [연결 [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)을 계속합니다.

### [!DNL Workfront Fusion]의 [!DNL Google]에 연결

[!DNL Google]에 대한 연결 만들기 프로세스는 [!DNL Google] 서비스의 모듈(예: [!DNL Google Sheets] 또는 [!DNL Google Docs])을 사용하는지 또는 [!UICONTROL HTTP] >[!UICONTROL OAuth2.0] 요청 모듈을 통해 [!DNL Google]에 연결하는 경우에 따라 다릅니다.

* [ [!DNL Google] 서비스의  [!DNL Google] 에 연결](#connect-to-google-in-a-google-service)
* [[!UICONTROL HTTP] > [!UICONTROL OAuth2.0 요청 만들기] 모듈에서  [!DNL Google] 에 연결](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### [!DNL Google] 서비스의 [!DNL Google]에 연결

1. [!DNL Workfront Fusion]에서 연결을 만들어야 하는 [!DNL Google] 모듈을 찾습니다.
1. **[!UICONTROL 연결 만들기]**&#x200B;를 클릭한 다음 **[!UICONTROL 고급 설정 표시]**&#x200B;를 클릭합니다.

1. 각 필드에 [[!UICONTROL OAuth 자격 증명 만들기]](#create-oauth-credentials)에서 검색한 [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호]을(를) 입력한 다음 **[!UICONTROL 계속]**&#x200B;을(를) 클릭합니다.

1. [!DNL Google] 계정으로 로그인합니다.

   **[!UICONTROL 이 앱이 확인되지 않음]** 창이 표시됩니다. 창 제목에 언급된 &quot;앱&quot;은 위에서 만든 OAuth 클라이언트입니다.

1. 사용자 지정 OAuth 클라이언트를 사용한 액세스를 허용하려면 **[!UICONTROL 고급]**&#x200B;을 클릭한 다음 **[!UICONTROL 안전하지 않은 [!DNL Workfront Fusion](으)로 이동]**&#x200B;을 클릭합니다.

1. [!DNL Workfront Fusion] 권한을 부여하려면 **[!UICONTROL 허용]**&#x200B;을 클릭하세요.
1. 표시되는 창에서 **[!UICONTROL 허용]**&#x200B;을 다시 클릭하여 선택 항목을 확인합니다.

   사용자 지정 OAuth 클라이언트를 사용하여 원하는 [!DNL Google] 서비스에 연결합니다.

#### [!UICONTROL HTTP] > [!UICONTROL OAuth2.0 요청 만들기] 모듈에서 [!DNL Google]에 연결 {#connect-to-google-in-the-http--make-an-oauth20-request-module}

[!UICONTROL HTTP] > [!UICONTROL OAuth2.0 요청 만들기] 모듈에서 [!DNL Google]에 연결하는 방법에 대한 지침은 [HTTP] > [!UICONTROL OAuth 2.0 요청 만들기] 모듈 만들기](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)([[!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 요청 만들기] 모듈](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md))에 연결하는 방법에 대한 지침을 참조하십시오. [!DNL Google] [!UICONTROL 

## 가능한 오류 메시지:[!UICONTROL [403] 액세스가 구성되지 않음]

[!UICONTROL `403 Access Not Configured`] 오류 메시지가 표시되면 Google Cloud Platform에서 해당 API를 활성화해야 합니다. API를 사용하려면 이 문서의 [프로젝트 만들기 [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) 섹션에 있는 단계를 따릅니다.
