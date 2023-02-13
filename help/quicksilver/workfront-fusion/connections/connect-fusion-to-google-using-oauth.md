---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 사용자 지정 OAuth 클라이언트 사용
description: 다음을 사용할 수 있습니다 [!DNL Adobe Workfront Fusion] 에 연결 [!DNL Google Services] 사용자 지정 OAuth 클라이언트 사용. 이 절차에는 [!DNL Google] 계정이 필요합니다.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 사용자 지정 OAuth 클라이언트 사용

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!UICONTROL Pro] 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 전제 조건

기존 [!DNL Google] 이 연결을 만들 계정입니다.

## 프로젝트 만들기 [!DNL Google Cloud Platform]

다음 절차는 다음과 같습니다.

* 개인 사용([!DNL @gmail.com] 및 [!DNL @googlemail.com] user)
* 내부 사용([!DNL G Suite] 사용자 지정 OAuth 클라이언트를 사용하는 사용자)

에서 프로젝트를 생성하려면 [!DNL Google Cloud] 플랫폼:

1. 에 로그인 [[!DNL Google Cloud] 플랫폼](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 사용 [!DNL Google] 자격 증명.
1. 왼쪽 패널에서 **[!UICONTROL 대시보드]**.
1. 클릭 **[!UICONTROL 프로젝트 만들기]** 화면 오른쪽 상단 모서리에서
1. 을(를) 입력합니다. **[!UICONTROL 프로젝트 이름]**&#x200B;를 클릭한 다음 **[!UICONTROL 만들기]**.

1. 을(를) 클릭합니다. **[!UICONTROL API 및 서비스 활성화]** 화면 상단 근처에 있는 탭입니다.
1. 에서 **[!UICONTROL API 및 서비스 검색]** 화면 상단의 필드에서 사용할 서비스 이름(예: [!DNL Gmail] API 또는 [!DNL Google Drive] API).
1. 표시되는 경우 연결할 API 또는 서비스를 클릭합니다 [!DNL Workfront Fusion].
1. 클릭 **[!UICONTROL 활성화]** 를 클릭하여 선택한 API를 활성화합니다.
1. 활성화할 각 API에 대해 6~8단계를 반복합니다.

   >[!NOTE]
   >
   >활성화 [!DNL Google Drive] API 및 모든 API [!DNL Google] 사용할 앱(예: [!DNL Google Sheets] API).

1. 표시되는 화면에서 를 클릭합니다. **[!UICONTROL 자격 증명 만들기]** 오른쪽 상단 모서리에서
1. 섹션을 계속합니다 [OAuth 동의 설정 구성](#configure-oauth-consent-settings) 참조하십시오.

## 구성 [!UICONTROL OAuth 동의] 설정

1. 왼쪽 패널에서 **[!UICONTROL OAuth 동의 화면]**.
1. 선택 **[!UICONTROL 외부]**&#x200B;를 클릭한 다음 **[!UICONTROL 만들기]**.

   >[!NOTE]
   >
   >이 옵션을 선택하면 요금이 부과되지 않습니다. 자세한 내용은 [!DNL Google]검증 요구 사항에 대한 예외에 대한 정보입니다.

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
      <td role="rowheader">[!UICONTROL User Support Email]</td> 
      <td>이 앱에 연결할 때 사용자 동의에 대한 질문이 있는 사용자에게 연락할 수 있는 이메일 주소를 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 이메일 주소]</td> 
      <td>Google에서 프로젝트 변경 사항에 대해 알리는 데 사용할 수 있는 이메일 주소를 한 개 이상 입력합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 아래 [!UICONTROL 인증된 도메인]를 클릭합니다. **[!UICONTROL 도메인 추가]**, , 을 입력합니다. `workfrontfusion.com`.

1. 클릭 **[!UICONTROL 저장 후 계속]**.
1. 클릭 **[!UICONTROL 범위 추가 또는 제거]**.
1. 오른쪽 패널에서 다음 범위를 활성화합니다.

<table style="table-layout:auto">
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>서비스/API</th> 
      <th>필요한 범위</th> 
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

목록을 확장하거나 목록의 다음 페이지로 이동하여 모두 확인해야 할 수 있습니다.

1. 클릭 **[!UICONTROL 업데이트]**.
1. 클릭 **[!UICONTROL 저장 후 계속]**.
1. (선택 사항) 테스트 사용자를 프로젝트에 추가합니다.
1. 클릭 **[!UICONTROL 저장 후 계속]**.
1. 정보를 정확히 검사한 다음 **[!UICONTROL 대시보드로 돌아가기]**.

   >[!NOTE]
   >
   >을 통해 동의 화면과 확인 신청서를 제출할 필요가 없습니다 [!DNL Google].

1. 계속 [OAuth 자격 증명 만들기](#create-oauth-credentials).

## OAuth 자격 증명 만들기

1. 왼쪽 패널에서 **[!UICONTROL 자격 증명]**.

   >[!NOTE]
   >
   >첫 번째 API 또는 서비스가 아닌 경우([!DNL Gmail] 또는 [!DNL Google Drive]) 새 자격 증명을 만들 필요가 없습니다.

1. 클릭 **[!UICONTROL 자격 증명 만들기]** 화면 상단 근처에 있는 를 선택한 다음 **[!UICONTROL OAuth 클라이언트 ID]** 를 클릭합니다.

1. 다음과 같이 필수 필드를 채웁니다.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 응용 프로그램 유형]</td> 
      <td> <p> [!UICONTROL 웹 응용 프로그램]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. 아래 [!UICONTROL 허가된 리디렉션 URI]를 클릭합니다. **[!UICONTROL URI 추가]** 을 입력합니다. **하나** 다음 중 하나를 수행합니다.

   * 대상 [!DNL Gmail] 또는 [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * 기타 [!DNL Google] 앱: `https://app.workfrontfusion.com/oauth/cb/google`

1. Click **[!UICONTROL Create]**.

   다음 [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호] 표시합니다.

1. 를 복사합니다. [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호] 보안 위치에 배치합니다. 이 매개 변수를 사용하여 을 연결합니다. [!DNL Workfront Fusion].
1. 계속 [연결 대상 [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

## 연결 대상 [!DNL Google] in [!DNL Workfront Fusion]

연결을 만드는 프로세스입니다 [!DNL Google] 모듈은 [!DNL Google] 서비스(예: [!DNL Google Sheets] 또는 [!DNL Google Docs])에 대해 또는 [!DNL Google] 사용 [!UICONTROL HTTP] >[!UICONTROL OAuth2.0 만들기] 요청 모듈입니다.

* [연결 대상 [!DNL Google] 에서 [!DNL Google] 서비스](#connect-to-google-in-a-google-service)
* [연결 대상 [!DNL Google] 에서 [!UICONTROL HTTP] > [!UICONTROL OAuth2.0 요청 만들기] 모듈](#connect-to-google-in-the-http--make-an-oauth20-request-module)

### 연결 대상 [!DNL Google] 에서 [!DNL Google] 서비스

1. in [!DNL Workfront Fusion]에서 를 찾습니다. [!DNL Google] 연결을 만들어야 하는 모듈입니다.
1. 클릭 **[!UICONTROL 연결 만들기]**&#x200B;를 클릭한 다음 **[!UICONTROL 고급 설정 표시]**.

1. 을(를) 입력합니다. [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호] 에서 검색됨 [[!UICONTROL OAuth 자격 증명 만들기]](#create-oauth-credentials) 각 필드에서 **[!UICONTROL 계속]**.

1. 다음 주소로 로그인 [!DNL Google] 계정이 필요합니다.

   다음 **[!UICONTROL 이 앱이 확인되지 않았습니다.]** 창이 표시됩니다. 창 제목에 언급된 &quot;앱&quot;은 위에서 만든 OAuth 클라이언트입니다.

1. 클릭 **[!UICONTROL 고급]**&#x200B;를 클릭한 다음 **[!UICONTROL 이동 [!DNL Workfront Fusion] (안전하지 않음)]** 사용자 지정 OAuth 클라이언트를 사용하여 액세스를 허용합니다.

1. 클릭 **[!UICONTROL 허용]** 부여 [!DNL Workfront Fusion] 권한.
1. 표시되는 창에서 **[!UICONTROL 허용]** 선택 사항을 다시 확인합니다.

   원하는 연결 [!DNL Google] 사용자 지정 OAuth 클라이언트를 사용하는 서비스가 설정되었습니다.

### 연결 대상 [!DNL Google] 에서 [!UICONTROL HTTP] > [!UICONTROL OAuth2.0 요청 만들기] 모듈 {#connect-to-google-in-the-http--make-an-oauth20-request-module}

연결 방법에 대한 지침은 [!DNL Google] 에서 [!UICONTROL HTTP] > [!UICONTROL OAuth2.0 요청 만들기] 모듈 [연결 만들기 지침 [!DNL Google] 에서 [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 요청 만들기] 모듈](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instruct) in [[!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 요청 만들기] 모듈](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## 가능한 오류 메시지:[!UICONTROL [403년] 액세스가 구성되지 않음]

만약 [!UICONTROL [403년] 액세스가 구성되지 않음] 오류 메시지가 표시되면 Google Cloud Platform에서 해당 API를 활성화해야 합니다. API를 활성화하려면 섹션의 단계를 수행하십시오 [프로젝트 만들기 [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) 참조하십시오.
