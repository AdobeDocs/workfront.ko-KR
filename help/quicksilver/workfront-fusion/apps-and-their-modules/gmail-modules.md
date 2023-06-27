---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Gmail 모듈
description: 다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 Gmail을 사용하는 워크플로를 자동화할 수 있을 뿐만 아니라 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1833'
ht-degree: 0%

---

# [!DNL Gmail] 모듈

다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다 [!DNL Gmail]을 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

시나리오를 만드는 방법에 대한 지침이 필요한 경우 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). 모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
   <td>
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime]이 있는 경우 [!DNL Adobe Workfront] 플랜, 조직은 다음을 구매해야 합니다. [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오. [!DNL Workfront Fusion] [!UICONTROL Ultimate]에 포함되어 있습니다. [!DNL Workfront] 계획.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 조직에서 구매해야 함 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 전제 조건

사용 [!DNL Gmail] 모듈, 다음이 있어야 합니다. [!DNL Gmail] 계정입니다.

## 연결 [!DNL Gmail] 끝 [!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [연결 [!DNL Gmail] 끝 [!DNL Workfront Fusion] [!DNL G Suite] 사용](#connect-gmail-to-workfront-fusion-usingg-suite)
* [연결 [!DNL Gmail] 끝 [!DNL Workfront Fusion] 사용 [!DNL gmail.com] 또는 [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### 연결 [!DNL Gmail] 끝 [!DNL Workfront Fusion] 사용[!DNL  G Suite] {#connect-gmail-to-workfront-fusion-using-g-suite}

연결에 대한 자세한 내용 [!DNL G Suite] 계정 위치: [!UICONTROL Workfront Fusion], 참조 [모듈의 앱 또는 웹 서비스 연결 [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) 이 문서에서 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### 연결 [!DNL Gmail] 끝 [!DNL Workfront Fusion] 사용 [!DNL gmail.com] 또는 [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

다음과 같은 경우 [!DNL @gmail.com] 또는 [!DNL @googlemail.com] 사용자에서 OAuth 클라이언트를 만들어야 합니다. [다음 [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 를 얻기 위해서 [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호].

OAuth 클라이언트를 만들고 [!UICONTROL 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호], 참조 [사용자 지정 OAuth 클라이언트를 사용하여 Adobe Workfront Fusion을 Google 서비스에 연결](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## [!DNL Gmail] 모듈 및 해당 필드

를 구성할 때 [!DNL Gmail] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Gmail] 앱이나 서비스의 액세스 수준 등에 따라 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [트리거](#triggers)
* [액션](#actions)
* [반복기](#iterators)

### 트리거

#### [!UICONTROL 이메일 보기]

이 트리거 모듈은 처리할 새 이메일이 수신되면 시나리오를 실행합니다.

모듈은 연결에서 액세스하는 모든 사용자 지정 필드 및 값과 함께 레코드 또는 레코드와 연결된 모든 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Gmail] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">연결 [!DNL Gmail] [!UICONTROL Workfront Fusion]으로</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
   <td> <p>보려는 전자 메일 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 필터 유형] </td> 
   <td> <p>전자 메일 시청에 사용할 필터 유형 선택</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Simple filter]</strong> </p> <p>[!UICONTROL Criteria], [!UICONTROL 발신자 이메일 주소], [!UICONTROL 제목] 및 [!UICONTROL 검색 구문] 필드를 채웁니다.</p> </li> 
     <li> <p> <strong>[!UICONTROL Gmail 필터]</strong> </p> <p>[!UICONTROL 쿼리] 필드에 이메일을 필터링하는 데 사용할 쿼리를 입력합니다.</p> <p>에 대한 자세한 내용 [!DNL Gmail] 필터, 참조 <a href="https://support.google.com/mail/answer/7190">연산자 검색</a> 다음에서 [!DNL Gmail] 설명서를 참조하십시오.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 기준]</td> 
   <td>[!UICONTROL all email], [!UICONTROL only read emails] 또는 [!UICONTROL only unread] 이메일을 시청할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 발신자 이메일 주소]</td> 
   <td> <p> 해당 주소에서 전송된 이메일만 시청하려면 이메일 주소를 입력하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject]</td> 
   <td>제목에서 해당 텍스트 문자열이 있는 이메일만 보려면 텍스트 문자열을 입력합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search phrase]</td> 
   <td>이메일의 어디에나 해당 텍스트 문자열이 있는 이메일만 보려면 텍스트 문자열을 입력합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이메일 메시지를 가져올 때 읽음으로 표시]</td> 
   <td> <p> 검색된 이메일을 읽은 것으로 표시하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 최대 결과 수]</td> 
   <td> <p> 다음에 대한 최대 결과 수 설정 [!DNL Workfront Fusion] 는 한 주기 동안 와 함께 작동합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 이메일 보내기]](#send-an-email)
* [[!UICONTROL 초안 만들기]](#create-a-draft)
* [[!UICONTROL 이메일을 읽은 상태로 표시]](#mark-an-email-as-read)
* [[!UICONTROL 이메일을 읽지 않음으로 표시]](#mark-an-email-as-unread)
* [[!UICONTROL 이메일 이동]](#move-an-email)
* [[!UICONTROL 이메일 복사]](#copy-an-email)
* [[!UICONTROL 이메일 삭제]](#delete-an-email)
* [[!UICONTROL 이메일 레이블 수정]](#modify-email-labels)

#### [!UICONTROL 이메일 보내기]

이 작업 모듈은 새 이메일을 전송합니다.

전자 메일 수신자를 지정합니다.

모듈은 전자 메일의 ID 및 연결된 필드와 연결이 액세스하는 모든 사용자 지정 필드 및 값을 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Gmail] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">연결 [!DNL Gmail] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL From]</td> 
   <td> <p>발신자 이메일 주소를 입력하거나 매핑합니다.</p> <p>참고: 잘못된 이메일 주소를 입력하면 계정에 내 주소가 아닌 다른 주소에서 이메일을 보낼 수 있는 권한이 없을 수 있으므로 메시지를 보낼 때 오류가 발생할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To] </td> 
   <td> <p>클릭 <strong>[!UICONTROL 추가]</strong>를 클릭한 다음 각 수신자의 이메일 주소를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject] </td> 
   <td> <p>이메일 제목을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>이메일 콘텐츠(메시지 본문)를 입력하거나 매핑합니다. HTML 태그가 허용됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 첨부 파일] </td> 
   <td> <p>클릭 <strong>[!UICONTROL 추가]</strong> 첨부 파일을 추가합니다. 이전 모듈에서 파일을 매핑할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copy recipients]</td> 
   <td> <p> 클릭 <strong>[!UICONTROL 추가]</strong>그런 다음 각 사본 수신자의 이메일 주소를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Blind copy recipients]</td> 
   <td> <p> 클릭 <strong>[!UICONTROL 추가]</strong>를 클릭한 다음 각 블라인드 카피 수신자의 이메일 주소를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 초안 만들기]

이 작업 모듈은 새 이메일 초안을 만들어 지정한 폴더에 추가합니다.

초안을 생성할 폴더를 지정합니다.

모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 이메일 초안의 ID와 관련 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Gmail] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">연결 [!DNL Gmail] [!UICONTROL Workfront Fusion]으로</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
   <td> <p>다음 항목 선택 [!DNL Gmail] 초안을 만들 폴더입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To] </td> 
   <td> <p>클릭 <strong>[!UICONTROL 추가]</strong>를 클릭한 다음 각 수신자의 이메일 주소를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject] </td> 
   <td> <p>이메일 제목을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>이메일 콘텐츠(메시지 본문)를 입력하거나 매핑합니다. HTML 태그가 허용됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 첨부 파일] </td> 
   <td> <p>클릭 <strong>[!UICONTROL 추가]</strong> 첨부 파일을 추가합니다. 이전 모듈에서 파일을 매핑할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copy recipients]</td> 
   <td> <p> 클릭 <strong>[!UICONTROL 추가]</strong>그런 다음 각 사본 수신자의 이메일 주소를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Blind copy recipients]</td> 
   <td> <p> 클릭 <strong>[!UICONTROL 추가]</strong>를 클릭한 다음 각 블라인드 카피 수신자의 이메일 주소를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이메일을 읽은 상태로 표시]

이 작업 모듈은 이메일을 읽은 것으로 표시합니다.

이메일과 해당 폴더의 ID를 지정합니다.

모듈은 전자 메일의 ID 및 연결된 필드와 연결이 액세스하는 모든 사용자 지정 필드 및 값을 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Gmail] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">연결 [!DNL Gmail] [!UICONTROL Workfront Fusion]으로</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
   <td> <p>다음 항목 선택 [!DNL Gmail] 전자 메일이 포함된 폴더입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이메일 ID(UID)]</td> 
   <td> <p> 이메일 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이메일을 읽지 않음으로 표시]

이 작업 모듈은 이메일 또는 이메일 초안을 읽지 않음으로 표시합니다.

이메일과 해당 폴더의 ID를 지정합니다.

모듈은 전자 메일의 ID 및 연결된 필드와 연결이 액세스하는 모든 사용자 지정 필드 및 값을 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Gmail] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">연결 [!DNL Gmail] [!UICONTROL Workfront Fusion]으로</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
   <td> <p>다음 항목 선택 [!DNL Gmail] 전자 메일이 포함된 폴더입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이메일 ID(UID)] </td> 
   <td> <p>읽지 않음으로 표시할 전자 메일의 전자 메일 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이메일 이동]

이 작업 모듈은 이메일 또는 이메일 초안을 사용자가 지정하는 폴더로 이동합니다.

폴더, 대상 폴더 및 전자 메일의 ID를 지정합니다.

모듈은 전자 메일의 ID 및 연결된 필드와 연결이 액세스하는 모든 사용자 지정 필드 및 값을 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Gmail] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">연결 [!DNL Gmail] [!UICONTROL Workfront Fusion]으로</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
   <td> <p>다음 항목 선택 [!DNL Gmail] 이동할 전자 메일이 포함된 소스 폴더입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 대상 폴더]</td> 
   <td> <p> 다음 항목 선택 [!DNL Gmail] 이메일을 이동할 대상 폴더입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이메일 ID(UID)]</td> 
   <td> <p> 이동할 전자 메일의 전자 메일 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이메일 복사]

이 작업 모듈은 이메일 또는 이메일 초안을 사용자가 지정하는 폴더로 복사합니다.

폴더, 대상 폴더 및 전자 메일의 ID를 지정합니다.

모듈은 전자 메일의 ID 및 연결된 필드와 연결이 액세스하는 모든 사용자 지정 필드 및 값을 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Gmail] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">연결 [!DNL Gmail] [!UICONTROL Workfront Fusion]으로</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
   <td> <p>다음 항목 선택 [!DNL Gmail] 복사할 전자 메일이 포함된 소스 폴더.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 대상 폴더]</td> 
   <td> <p>다음 항목 선택 [!DNL Gmail] 이메일을 복사할 대상 폴더입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이메일 ID(UID)]</td> 
   <td> <p>복사할 이메일의 이메일 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이메일 삭제]

이 작업 모듈은 지정한 폴더에서 이메일 또는 이메일 초안을 제거합니다.

모듈은 전자 메일의 ID 및 연결된 필드와 연결이 액세스하는 모든 사용자 지정 필드 및 값을 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Gmail] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">연결 [!DNL Gmail] [!UICONTROL Workfront Fusion]으로</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL [!DNL Gmail] 메시지 ID]</p> </td> 
   <td> <p>삭제하려는 이메일의 이메일 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permanently] </td> 
   <td> <p>모듈이 이메일을 휴지통 폴더로 이동하는 대신 영구적으로 삭제할 수 있도록 하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이메일 레이블 수정]

이 작업 모듈은 지정한 이메일 메시지의 레이블을 수정합니다.

모듈은 전자 메일의 ID 및 연결된 필드와 연결이 액세스하는 모든 사용자 지정 필드 및 값을 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Gmail] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">연결 [!DNL Gmail] [!UICONTROL Workfront Fusion]으로</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Gmail] 메시지 ID]</td> 
   <td> <p> 삭제하려는 이메일의 이메일 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>추가할 [!UICONTROL 레이블]</p> </td> 
   <td> <p>추가할 레이블을 선택한 이메일 메시지에 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>제거할 [!UICONTROL 레이블]</td> 
   <td> <p> 선택한 이메일 메시지에서 제거할 레이블을 선택하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>[!UICONTROL 추가할 레이블] 및 [!UICONTROL 제거할 레이블] 필드는 사용자가 만든 레이블만 로드합니다.

### 반복기

#### [!UICONTROL 첨부 파일 반복]

이메일 첨부 파일을 반복할 수 있습니다. 각 첨부 파일은 모듈의 출력에 있는 별도의 번들입니다. 자세한 내용은 [Adobe Workfront Fusion의 반복자 모듈](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 소스 모듈] </td> 
   <td> <p>첨부 파일을 반복할 모듈을 선택합니다. </p> </td> 
  </tr> 
 </tbody> 
</table>
