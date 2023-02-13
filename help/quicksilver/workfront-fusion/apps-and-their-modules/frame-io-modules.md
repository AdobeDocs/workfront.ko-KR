---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Frame.io 모듈
description: 다음 [!DNL Adobe Workfront Fusion Frame].io modules enable you to monitor, create, update, retrieve, or delete assets and comments in your [!DNL Frame.io] 계정이 필요합니다.
author: Becky
feature: Workfront Fusion
exl-id: 373a86f6-fbba-4914-b08d-a3a035ac0ae4
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2263'
ht-degree: 0%

---

# [!DNL Frame.io] 모듈

다음 [!DNL Adobe Workfront Fusion] [!DNL Frame.io] 모듈을 사용하면 사용자의 자산과 주석을 모니터링, 생성, 업데이트, 검색 또는 삭제할 수 있습니다 [!DNL Frame.io] 계정이 필요합니다.

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

를 사용하려면 [!DNL Frame.io] 모듈이면 반드시 [!DNL Frame.io] account

## Connect [!DNL Frame.io] to [!UICONTROL Adobe Workfront Fusion]

에 연결할 수 있습니다. [!DNL Frame.io] api 토큰 사용 또는 OAuth 2.0 사용.

[연결 대상 [!DNL Frame.io] api 토큰 사용](#connect-to-frameio-using-an-api-token)

[연결 대상 [!DNL Frame.io] OAuth 2.0 PKCE 사용](#connect-to-frameio-using-oauth-20-pkce)

### 연결 대상 [!DNL Frame.io] api 토큰 사용

연결 [!DNL Frame.io] 계정 대상 [!DNL Workfront Fusion] api 토큰을 사용하면 [!DNL Frame.io] 계정을 삽입하고 [!DNL Workfront Fusion] [!DNL Frame.io] [!UICONTROL 연결 만들기] 대화 상자.

1. 에 로그인합니다. [!DNL Frame.io] 계정이 필요합니다.
1. 로 이동합니다. **[!UICONTROL 토큰]** 페이지의 [!DNL Frame.io] 개발자.
1. 클릭 **[!UICONTROL 새로 만들기]**.
1. 토큰 이름을 입력하고 사용할 범위를 선택한 다음 **[!UICONTROL 만들기]**.
1. 제공된 토큰을 복사합니다.
1. 이동 [!DNL Workfront Fusion] 그리고 [!DNL Frame.io] 모듈 **[!UICONTROL 연결 만들기]** 대화 상자.
1. 에서 **[!UICONTROL 연결 유형]** 필드, 선택 **[!DNL Frame.io]**.
1. 5단계에서 복사한 토큰을 **[!UICONTROL 사용자 [!DNL Frame.io] API 키]** 필드를 입력하고 **[!UICONTROL 계속]** 연결을 설정하려면 다음을 수행하십시오.

연결이 설정되었습니다. 모듈 설정을 계속 진행할 수 있습니다.

### 연결 대상 [!DNL Frame.io] OAuth 2.0 PKCE 사용

연결을 만들 수 있습니다 [!DNL Frame.io] 선택적 클라이언트 ID와 함께 OAuth 2.0 PKCE 사용. 연결에 클라이언트 ID를 포함하려는 경우, [!DNL Frame.io] 계정이 필요합니다.

* [연결 대상 [!DNL Frame.io] oaUth 2.0 PKCE 사용(클라이언트 ID 없음)](#connect-to-frameio-using-using-oauth-20-pkce-without-client-id)
* [연결 대상 [!DNL Frame.io] oaUth 2.0 PKCE 사용(클라이언트 ID와 함께)](#connect-to-frameio-using-using-oauth-20-pkce-with-client-id)

#### 연결 대상 [!DNL Frame.io] oaUth 2.0 PKCE 사용(클라이언트 ID 없음)

1. 이동 [!DNL Workfront Fusion] 그리고 [!DNL Frame.io] 모듈 **[!UICONTROL 연결 만들기]** 대화 상자.
1. 에서 **[!UICONTROL 연결 유형]** 필드, 선택 **[!UICONTROL [!DNL Frame.io]OAuth 2.0 PKCE]**.
1. 새 연결의 이름을 **[!UICONTROL 연결 이름]** 필드.
1. 클릭 **[!UICONTROL 계속]** 연결을 설정하려면 다음을 수행하십시오.

연결이 설정되었습니다. 모듈 설정을 계속 진행할 수 있습니다.

#### 연결 대상 [!DNL Frame.io] oaUth 2.0 PKCE 사용(클라이언트 ID와 함께)

1. 에서 OAuth 2.0 앱 만들기 [!DNL Frame.io]. 자세한 내용은 [!DNL Frame.io] 설명서 [!UICONTROL OAuth 2.0 코드 인증 흐름].

   >[!IMPORTANT]
   >
   >에서 OAuth 2.0 앱을 만들 때 [!DNL Frame.io]:
   >
   >* 리디렉션 URI로 다음을 입력합니다.
   >   
   >  미국/APAC `https://app.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >  EMEA `https://app-eu.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >* PCKE 옵션을 활성화합니다.



1. 제공된 을 복사합니다. `client_id`.
1. 이동 [!DNL Workfront Fusion] 그리고 [!DNL Frame.io] 모듈 **[!UICONTROL 연결 만들기]** 대화 상자.
1. 에서 **[!UICONTROL 연결 유형]** 필드, 선택 **[!UICONTROL [!DNL Frame.io]OAuth 2.0 PKCE]**.
1. 새 연결의 이름을 **[!UICONTROL 연결 이름]** 필드.
1. 클릭 **[!UICONTROL 고급 설정 표시]**.
1. 을(를) 입력합니다. `client_id` 2단계에서 **[!UICONTROL 클라이언트 ID]** 필드.
1. 클릭 **[!UICONTROL 계속]** 연결을 설정하려면 다음을 수행하십시오.

연결이 설정되었습니다. 모듈 설정을 계속 진행할 수 있습니다.

## [!DNL Frame.io] 모듈 및 해당 필드

구성 시 [!DNL Frame.io] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Frame.io] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [자산](#assets)
* [댓글](#comments)
* [프로젝트](#projects)
* [기타](#other)

### 자산

* [[!UICONTROL 자산 만들기]](#create-an-asset)
* [[!UICONTROL 자산 삭제]](#delete-an-asset)
* [[!UICONTROL 자산 가져오기]](#get-an-asset)
* [[!UICONTROL 자산 나열]](#list-assets)
* [[!UICONTROL 자산 업데이트]](#update-an-asset)
* [[!UICONTROL 삭제된 자산 보기]](#watch-asset-deleted)
* [[!UICONTROL 업데이트된 자산 레이블 감시]](#watch-asset-label-updated)
* [[!UICONTROL 새 자산 보기]](#watch-new-asset)

#### [!UICONTROL 자산 만들기]

이 작업 모듈은 새 자산을 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>연결 생성에 대한 지침은 [!DNL Frame.io]를 참조하십시오. <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>자산을 만들 프로젝트를 소유하는 팀을 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프로젝트 ID] </td> 
   <td> <p>프로젝트를 선택하거나 자산을 만들 프로젝트의 ID를 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 ID] </td> 
   <td> <p>폴더를 선택하거나 자산을 만들 폴더의 ID를 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type] </td> 
   <td> <p>폴더를 만들지 아니면 파일을 만들지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>새 파일 또는 폴더의 이름을 입력합니다.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Type </td> 
    <td> <p>Select the type of file you want to upload.</p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Size </td> 
    <td> <p>The file size in bytes.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 URL] </td> 
   <td> <p>업로드할 파일의 URL을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description] </td> 
   <td> <p>자산에 대한 간단한 설명을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 자산 삭제]

이 작업 모듈은 지정된 자산을 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>연결 생성에 대한 지침은 [!DNL Frame.io]를 참조하십시오. <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>삭제할 자산이 포함된 프로젝트를 소유하는 팀을 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프로젝트 ID]</td> 
   <td> <p> 삭제할 자산이 들어 있는 프로젝트 또는 프로젝트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 ID] </td> 
   <td> <p>삭제할 자산이 들어 있는 폴더를 선택합니다</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>삭제할 자산을 선택하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 자산 가져오기]

이 작업 모듈은 자산 세부 사항을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>연결 생성에 대한 지침은 [!DNL Frame.io]를 참조하십시오. <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>세부 사항을 검색할 자산이 포함된 프로젝트를 소유하는 팀을 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프로젝트 ID]</td> 
   <td> <p> 세부 사항을 검색할 자산이 포함된 프로젝트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 ID] </td> 
   <td> <p>세부 사항을 검색할 자산이 들어 있는 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>자산을 선택하거나 세부 사항을 검색할 자산의 ID를 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 자산 나열]

이 검색 모듈은 지정된 프로젝트 폴더의 모든 자산을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>연결 생성에 대한 지침은 [!DNL Frame.io]를 참조하십시오. <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>자산을 검색할 폴더가 포함된 프로젝트를 소유하는 팀을 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프로젝트 ID]</td> 
   <td> <p> 자산을 검색할 폴더가 포함된 프로젝트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 ID] </td> 
   <td> <p>자산을 나열할 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한] </td> 
   <td> <p>최대 자산 수 설정 [!DNL Workfront Fusion] 은 한 실행 주기 동안 반환됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### `[!UICONTROL Update an Asset]`

이 작업 모듈을 사용하면 기존 자산의 이름, 설명 또는 사용자 지정 필드를 업데이트할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>연결 생성에 대한 지침은 [!DNL Frame.io]를 참조하십시오. <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>자산을 업데이트할 프로젝트를 소유하는 팀을 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프로젝트 ID] </td> 
   <td> <p>프로젝트를 선택하거나 자산을 업데이트할 프로젝트의 ID를 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 ID] </td> 
   <td> <p>폴더를 선택하거나 자산을 업데이트할 폴더의 ID를 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>업데이트된 파일의 이름을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description] </td> 
   <td> <p>업데이트된 자산에 대한 간단한 설명을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 삭제된 자산 보기]

이 트리거 모듈은 자산이 삭제되면 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> 웹 후크의 이름(예: 삭제된 자산)을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>연결 생성에 대한 지침은 [!DNL Frame.io]를 참조하십시오. <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>이 웹 후크가 만들어지는 팀을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 업데이트된 자산 레이블 감시]

이 트리거 모듈은 자산의 상태가 설정, 변경 또는 제거될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> 웹 후크의 이름을 입력합니다(예: 자산 상태가 업데이트됨).</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>연결 생성에 대한 지침은 [!DNL Frame.io]를 참조하십시오. <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>이 웹 후크가 만들어지는 팀을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 새 자산 보기]

이 트리거 모듈은 새 자산을 만들 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> 웹 후크의 이름(예: 생성된 자산)을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>연결 생성에 대한 지침은 [!DNL Frame.io]를 참조하십시오. <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>이 웹 후크가 만들어지는 팀을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 댓글

* [[!UICONTROL 댓글 만들기]](#create-a-comment)
* [[!UICONTROL 댓글 삭제]](#delete-a-comment)
* [[!UICONTROL 댓글 받기]](#get-a-comment)
* [[!UICONTROL 주석 나열]](#list-comments)
* [[!UICONTROL 댓글 업데이트]](#update-a-comment)
* [[!UICONTROL 업데이트된 댓글 보기]](#watch-comment-updated)
* [[!UICONTROL 새 댓글 보기]](#watch-new-comment)

#### [!UICONTROL 댓글 만들기]

이 작업 모듈은 자산에 새 주석을 추가하거나 응답합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>연결 생성에 대한 지침은 [!DNL Frame.io]를 참조하십시오. <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type] </td> 
   <td> <p>댓글을 작성할지 또는 댓글에 답글을 달을지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>설명을 추가할 자산이 포함된 프로젝트를 소유하는 팀을 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프로젝트 ID] </td> 
   <td> <p>프로젝트를 선택하거나 주석을 추가할 자산이 포함된 프로젝트의 ID를 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 ID] </td> 
   <td> <p>폴더를 선택하거나 주석을 추가할 자산이 포함된 폴더의 ID를 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>주석을 추가할 자산을 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment ID] </td> 
   <td> <p>답장을 추가할 댓글을 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p> 댓글 또는 답장의 텍스트 내용을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timestamp] </td> 
   <td> <p>주석을 연결할 비디오에 프레임 번호를 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 댓글 삭제]

이 작업 모듈은 기존 주석을 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>연결 생성에 대한 지침은 [!DNL Frame.io]를 참조하십시오. <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID]</td> 
   <td> <p> 주석을 삭제할 자산이 포함된 프로젝트를 소유하는 팀을 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프로젝트 ID]</td> 
   <td> <p> 프로젝트를 선택하거나 주석을 삭제할 자산이 포함된 프로젝트의 ID를 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 ID]</td> 
   <td> <p> 댓글을 삭제할 자산이 들어 있는 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>삭제할 주석이 포함된 자산을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment ID] </td> 
   <td> <p>삭제할 주석을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 댓글 받기]

이 작업 모듈은 지정된 댓글에 대한 세부 정보를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>연결 생성에 대한 지침은 [!DNL Frame.io]를 참조하십시오. <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>자산을 검색할 폴더가 포함된 프로젝트를 소유하는 팀을 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프로젝트 ID] </td> 
   <td> <p>자산을 검색할 폴더가 포함된 프로젝트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 ID] </td> 
   <td> <p>자산을 나열할 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>검색할 주석이 포함된 자산을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment ID] </td> 
   <td> <p>세부 정보를 검색할 설명을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 주석 나열]

이 검색 모듈은 지정된 자산의 모든 주석을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>연결 생성에 대한 지침은 [!DNL Frame.io]를 참조하십시오. <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>주석을 검색할 폴더가 포함된 프로젝트를 소유하는 팀을 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프로젝트 ID] </td> 
   <td> <p>주석을 검색할 폴더가 포함된 프로젝트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 ID] </td> 
   <td> <p>설명을 나열할 자산이 포함된 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>설명을 나열할 자산을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한] </td> 
   <td> <p>최대 댓글 수 설정 [!DNL Workfront Fusion] 은 한 실행 주기 동안 반환됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 댓글 업데이트]

이 작업 모듈은 기존 주석을 편집합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>연결 생성에 대한 지침은 [!DNL Frame.io]를 참조하십시오. <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>주석을 업데이트할 자산이 포함된 프로젝트를 소유하는 팀을 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프로젝트 ID] </td> 
   <td> <p>설명을 업데이트할 자산이 포함된 프로젝트 \ 를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 ID] </td> 
   <td> <p>댓글을 업데이트할 자산이 들어 있는 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>주석을 업데이트할 자산을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment ID] </td> 
   <td> <p>업데이트할 설명을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p> 주석의 텍스트 컨텐츠를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timestamp] </td> 
   <td> <p>주석이 연결된 비디오에 프레임 번호를 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 업데이트된 댓글 보기]

이 트리거 모듈은 주석을 편집할 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name] </td> 
   <td> <p>웹 후크의 이름을 입력합니다(예: 댓글 편집됨).</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>연결 생성에 대한 지침은 [!DNL Frame.io]를 참조하십시오. <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>이 웹 후크가 만들어지는 팀을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 새 댓글 보기]

이 트리거 모듈은 새 댓글 또는 응답이 생성될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name] </td> 
   <td> <p>웹 후크의 이름(예: 새 주석)을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>연결 생성에 대한 지침은 [!DNL Frame.io]를 참조하십시오. <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>이 웹 후크가 만들어지는 팀을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 프로젝트

#### [!UICONTROL 프로젝트 나열]

이 검색 모듈은 지정된 팀의 모든 프로젝트를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>연결 생성에 대한 지침은 [!DNL Frame.io]를 참조하십시오. <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>프로젝트를 검색할 팀을 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한] </td> 
   <td> <p>최대 프로젝트 수 설정 [!DNL Workfront Fusion] 은 한 실행 주기 동안 반환됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 기타

#### [!UICONTROL API 호출 만들기]

이 모듈에서 사용자 지정 API 호출을 수행할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>연결 생성에 대한 지침은 [!DNL Frame.io]를 참조하십시오. <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>상대 경로 입력 <code>https://api.frame.io</code>. 예: <code> /v2/teams</code></p> <p>참고: 사용 가능한 끝점 목록에 대해서는 [!DNL Frame.io] API 참조.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 메서드]</p> </td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 인증 헤더를 자동으로 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열] </td> 
   <td> <p>요청 쿼리 문자열을 입력합니다. 쿼리 문자열에 포함할 각 매개 변수에 대해 <b>[!UICONTROL 항목 추가]</b> 필드의 이름과 원하는 값을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>표준 JSON 개체 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>다음과 같은 조건문을 사용하는 경우 <code>if</code> json에서 따옴표를 조건문 외부에 지정합니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**예:** 다음 API 호출은 [!DNL Frame.io] 계정:

URL: `/v2/teams`

메서드: `GET`

![](assets/api-call-example.png)

결과는 모듈의 Output(번들 > Body)에서 찾을 수 있습니다.

이 예제에서는 1개 팀의 세부 사항이 반환되었습니다.

![](assets/api-call-output.png)
