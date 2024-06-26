---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: 연결 [!DNL Adobe Workfront Fusion] 끝 [!DNL Google Services] 사용자 정의 OAuth 클라이언트 사용
description: 다음을 사용할 수 있습니다. [!DNL Adobe Workfront Fusion] 에 연결하려면 [!DNL Google Services] 사용자 지정 OAuth 클라이언트 사용. 이 절차에는 기존 [!DNL Google] 계정입니다.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 7d2b4a9940cb21de1b8b5f2955f53b3d88040e44
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# 연결 [!DNL Adobe Workfront Fusion] 끝 [!DNL Google Services] 사용자 정의 OAuth 클라이언트 사용

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

## 전제 조건

기존 항목이 필요합니다. [!DNL Google] 연결할 계정입니다.

## 사용자 지정 OAuth 클라이언트를 사용하여 Fusion을 Google 서비스에 연결

이 연결을 만들려면 Google Cloud 플랫폼에서 프로젝트를 만들고 구성한 다음 해당 프로젝트를 기반으로 Fusion에서 연결을 구성해야 합니다.

* [프로젝트 만들기 [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform)
* [구성 [!UICONTROL OAuth 동의] 설정](#configure-oauth-consent-settings)
* [OAuth 자격 증명 만들기](#create-oauth-credentials)
* [연결 대상 [!DNL Google] 위치: [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>이 절차는 다음 용도로 사용됩니다.
>
>* 개인 사용([!DNL `@gmail.com`] 및 [!DNL `@googlemail.com`] 사용자)
>* 내부 사용([!DNL G Suite] 사용자 정의 OAuth 클라이언트 사용을 선호하는 사용자)

### 프로젝트 만들기 [!DNL Google Cloud Platform]

다음에 대한 프로젝트를 만들려면 [!DNL Google Cloud] 플랫폼:

1. 로그인 대상 [[!DNL Google Cloud] 플랫폼](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 사용 [!DNL Google] 자격 증명.
1. 왼쪽 패널에서 **[!UICONTROL 대시보드]**.
1. 클릭 **[!UICONTROL 프로젝트 만들기]** 화면의 오른쪽 상단에 있습니다.
1. 다음을 입력합니다. **[!UICONTROL 프로젝트 이름]**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL 만들기]**.

1. 다음을 클릭합니다. **[!UICONTROL API 및 서비스 활성화]** 화면 상단 근처에 있는 탭입니다.
1. 다음에서 **[!UICONTROL API 및 서비스 검색]** 화면 맨 위에 있는 필드에 사용할 서비스의 이름을 입력합니다(예: [!DNL Gmail] API 또는 [!DNL Google Drive] API).
1. 표시되면 연결할 API 또는 서비스를 클릭합니다 [!DNL Workfront Fusion].
1. 클릭 **[!UICONTROL 사용]** 을 눌러 선택한 API를 활성화합니다.
1. 활성화하려는 각 API에 대해 6~8단계를 반복합니다.

   >[!NOTE]
   >
   >다음을 활성화해야 합니다. [!DNL Google Drive] API 및 모든 API [!DNL Google] 사용할 앱(예: [!DNL Google Sheets] API).

1. 표시되는 화면에서 다음을 클릭합니다. **[!UICONTROL 자격 증명 만들기]** 오른쪽 상단 모서리입니다.
1. 섹션으로 계속 [OAuth 동의 설정 구성](#configure-oauth-consent-settings) 이 문서에서.

### 구성 [!UICONTROL OAuth 동의] 설정

1. 왼쪽 패널에서 **[!UICONTROL OAuth 동의 화면]**.
1. 선택 **[!UICONTROL 외부]**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL 만들기]**.

   >[!NOTE]
   >
   >이 옵션을 선택하면 요금이 부과되지 않습니다. 자세한 내용은 [!DNL Google]확인 요구 사항 예외에 대한 의 정보입니다.

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

1. 아래 [!UICONTROL 승인된 도메인], 클릭 **[!UICONTROL 도메인 추가]**, 및 입력 `workfrontfusion.com`.

1. 클릭 **[!UICONTROL 저장 및 계속]**.
1. 클릭 **[!UICONTROL 범위 추가 또는 제거]**.
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

1. 클릭 **[!UICONTROL 업데이트]**.
1. 클릭 **[!UICONTROL 저장 및 계속]**.
1. (선택 사항) 프로젝트에 테스트 사용자를 추가합니다.
1. 클릭 **[!UICONTROL 저장 및 계속]**.
1. 정보의 정확성을 검사한 다음 **[!UICONTROL 대시보드로 돌아가기]**.

   >[!NOTE]
   >
   >다음 방법으로 동의 화면 및 확인 신청서를 제출할 필요가 없습니다. [!DNL Google].

1. 계속 [OAuth 자격 증명 만들기](#create-oauth-credentials).

### OAuth 자격 증명 만들기

1. 왼쪽 패널에서 **[!UICONTROL 자격 증명]**.

   >[!NOTE]
   >
   >첫 번째 API 또는 서비스가 아닌 경우([!DNL Gmail] 또는 [!DNL Google Drive]) 활성화한 경우 새 자격 증명을 만들 필요가 없습니다.

1. 클릭 **[!UICONTROL 자격 증명 만들기]** 화면 상단 근처에서 을 선택합니다. **[!UICONTROL OAuth 클라이언트 ID]** 드롭다운 메뉴에서 을(를) 선택합니다.

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

1. 아래 [!UICONTROL 승인된 리디렉션 URI], 클릭 **[!UICONTROL URI 추가]** 및 입력 **1** 다음 중 하나를 선택할 수 있습니다.

   * 대상 [!DNL Gmail] 또는 [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * 기타 [!DNL Google] 앱: `https://app.workfrontfusion.com/oauth/cb/google`

1. Click **[!UICONTROL Create]**.

   다음 [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호] 표시.

1. 다음을 복사합니다. [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호] 안전한 장소로. 해당 사용자가에서 연결을 만드는 데 사용됩니다. [!DNL Workfront Fusion].
1. 계속 [연결 대상 [!DNL Google] 위치: [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

### 연결 대상 [!DNL Google] 위치: [!DNL Workfront Fusion]

에 대한 연결을 만드는 프로세스입니다 [!DNL Google] 의 모듈을 사용하는지 여부에 따라 다릅니다. [!DNL Google] 서비스(예: [!DNL Google Sheets] 또는 [!DNL Google Docs])에 연결하거나 [!DNL Google] 를 통해 [!UICONTROL HTTP] >[!UICONTROL OAuth2.0 만들기] 모듈 요청.

* [연결 대상 [!DNL Google] 다음 기간: [!DNL Google] 서비스](#connect-to-google-in-a-google-service)
* [연결 대상 [!DNL Google] 다음에서 [!UICONTROL HTTP] > [!UICONTROL OAuth2.0 요청 만들기] 모듈](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### 연결 대상 [!DNL Google] 다음 기간: [!DNL Google] 서비스

1. 위치 [!DNL Workfront Fusion], 다음 위치 찾기 [!DNL Google] 연결을 만들어야 하는 모듈입니다.
1. 클릭 **[!UICONTROL 연결 만들기]**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL 고급 설정 표시]**.

1. 다음을 입력합니다. [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호] 다음 위치에서 검색함: [[!UICONTROL OAuth 자격 증명 만들기]](#create-oauth-credentials) 각 필드에서 을(를) 클릭합니다. **[!UICONTROL 계속]**.

1. 다음으로 로그인 [!DNL Google] 계정입니다.

   다음 **[!UICONTROL 이 앱은 확인되지 않았습니다.]** 창이 표시됩니다. 창 제목에 언급된 &quot;앱&quot;은 위에서 만든 OAuth 클라이언트입니다.

1. 클릭 **[!UICONTROL 고급]**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL 다음으로 이동 [!DNL Workfront Fusion] (안전하지 않음)]** 사용자 지정 OAuth 클라이언트를 사용한 액세스를 허용합니다.

1. 클릭 **[!UICONTROL 허용]** 부여하려면 [!DNL Workfront Fusion] 권한.
1. 표시되는 창에서 을 클릭합니다. **[!UICONTROL 허용]** 다시 한 번 확인해 보십시오.

   원하는 연결에 대한 연결 [!DNL Google] 사용자 정의 OAuth 클라이언트를 사용하는 서비스가 설정됩니다.

#### 연결 대상 [!DNL Google] 다음에서 [!UICONTROL HTTP] > [!UICONTROL OAuth2.0 요청 만들기] 모듈 {#connect-to-google-in-the-http--make-an-oauth20-request-module}

에 연결하는 방법에 대한 지침: [!DNL Google] 다음에서 [!UICONTROL HTTP] > [!UICONTROL OAuth2.0 요청 만들기] 모듈, 참조 [에 대한 연결 만들기 지침 [!DNL Google] 다음에서 [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 요청] 모듈](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module) 위치: [[!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 요청] 모듈](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## 가능한 오류 메시지:[!UICONTROL [403] 액세스 구성되지 않음]

다음과 같은 경우 [!UICONTROL `403 Access Not Configured`] 오류 메시지가 표시되면 Google 클라우드 플랫폼에서 해당 API를 활성화해야 합니다. API를 활성화하려면 섹션의 단계를 따릅니다 [프로젝트 만들기 [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) 이 문서에서.
