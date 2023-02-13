---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 전자 메일
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오 Microsoft Office 365 Email을 사용하는 워크플로우를 자동화하고 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 29b69e8c-a889-441e-a052-287f1db2052d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1838'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Email]

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!UICONTROL Microsoft Office 365 전자 메일]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

를 사용하려면 [!UICONTROL Office 365 전자 메일] with [!DNL Adobe Workfront Fusion]를 채울 때는 [!UICONTROL Office 365 계정]. www.office.com에서 만들 수 있습니다.

연결 방법에 대한 지침은 [!UICONTROL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. [연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침](../../workfront-fusion/connections/connect-to-fusion-general.md)

동의를 부여하면 다음 위치로 다시 리디렉션됩니다. [!UICONTROL Workfront Fusion] 시나리오를 계속 작성할 수 있는 관리 페이지입니다.

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

를 사용하려면 [!DNL Microsoft Office 365 Email] 모듈이면 반드시 [!DNL Microsoft Office 365 Email] 계정이 필요합니다.

## [!DNL Microsoft Office 365 Email] 모듈 및 해당 필드

구성 시 [!DNL Microsoft Office 365 Email] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Microsoft Office 365 Email] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [메시지](#message)
* [초안 메시지](#draft-message)
* [첨부 파일](#attachment)
* [기타](#other)

### 메시지

* [[!UICONTROL 메시지 보기]](#watch-messages)
* [[!UICONTROL 메시지 검색]](#search-messages)
* [[!UICONTROL 메시지 가져오기]](#get-a-message)
* [[!UICONTROL 메시지 만들기 및 보내기]](#create-and-send-a-message)
* [[!UICONTROL 메시지 이동]](#move-a-message)
* [[!UICONTROL 메시지 삭제]](#delete-a-message)

#### [!UICONTROL 메시지 보기]

새 이메일 메시지를 보내거나 받을 때 트리거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Watch Messages]</p> </td> 
   <td> <p>보려는 메시지를 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL만 읽지 않음]</li> 
     <li>[!UICONTROL 전용 읽기]</li> 
     <li>[!UICONTROL All]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메일 폴더]</td> 
   <td> <p>보려는 메시지가 포함된 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>검색 쿼리를 입력합니다. 검색 쿼리를 작성하는 방법에 대한 자세한 내용은 [!DNL Microsoft] 지원 문서 <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">메일 및 사람 검색 [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한] </td> 
   <td> <p>최대 메시지 수를 입력합니다 [!DNL Workfront Fusion] 한 시나리오 실행 주기 동안 를 반환해야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 메시지 검색]

특정 기준에 따라 메시지를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메일 폴더]</td> 
   <td> <p>검색할 메시지가 포함된 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>검색 쿼리를 입력합니다. 검색 쿼리를 작성하는 방법에 대한 자세한 내용은 [!DNL Microsoft] 지원 문서 <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">메일 및 사람 검색 [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td> <p>결과를 정렬할 방법을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL 제목(오름차순 또는 내림차순)]</li> 
     <li>[!UICONTROL 만든 날짜 시간(오름차순 또는 내림차순)]</li> 
     <li>[!UICONTROL 마지막으로 수정한 날짜 시간(오름차순 또는 내림차순)]</li> 
     <li>[!UICONTROL 받은 날짜 시간(오름차순 또는 내림차순)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>최대 메시지 수를 입력합니다 [!DNL Workfront Fusion] 한 시나리오 실행 주기 동안 를 반환해야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 메시지 가져오기]

특정 메시지의 메타데이터를 가져옵니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메시지 ID]</td> 
   <td> <p> 메타데이터를 검색할 메시지의 ID를 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get MIME 콘텐츠]</td> 
   <td>메시지의 MIME 콘텐츠에 대한 데이터를 검색하려면 이 옵션을 활성화하십시오. [!UICONTROL MIME] 콘텐츠에는 이미지, 오디오, 비디오 또는 기타 파일 유형이 포함될 수 있습니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 메시지 만들기 및 보내기]

이메일 메시지를 만들고 전송합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>메시지의 제목란을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Body Content Type]</td> 
   <td>메시지의 본문 내용이 HTML인지 아니면 텍스트인지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td> <p>전자 메일의 메시지 본문 텍스트를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>이메일의 중요도를 선택합니다</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>메시지를 보낼 이메일 주소를 추가합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>연락처의 이름을 입력합니다</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>연락처의 이메일 주소를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>메시지 사본을 받을 수신자를 추가합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>연락처의 이름을 입력합니다</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>연락처의 이메일 주소를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bcc Recipients]</p> </td> 
   <td> <p>다른 수신자가 자신의 이름이나 이메일 주소를 볼 수 없도록 메시지에 복사할 수신자를 추가합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>연락처의 이름을 입력합니다</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>연락처의 이메일 주소를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 첨부 파일]</p> </td> 
   <td> <p>전자 메일에 첨부 파일 추가:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 파일 이름]</strong> </p> <p>파일 이름을 입력합니다. 예: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>필드에 파일 데이터를 입력하거나 파일의 소스를 매핑합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Internet Message Headers]</td> 
   <td> <p>이메일에 대한 메시지 헤더를 추가합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>헤더의 이름을 입력합니다</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>헤더에 사용할 값을 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 메시지 이동]

전자 메일 메시지를 사서함의 선택한 폴더로 이동합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메시지 ID]</td> 
   <td> <p> 다른 폴더로 이동할 메시지의 ID를 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메일 폴더] </td> 
   <td> <p>메시지를 이동할 폴더의 ID를 선택하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 메시지 삭제]

기존 이메일 메시지를 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메시지 ID]</td> 
   <td> <p> 삭제할 메시지의 ID를 선택하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 초안 메시지

* [초안 메시지 만들기](#create-a-draft-message)
* [초안 메시지 보내기](#send-a-draft-message)
* [메시지 업데이트](#update-a-message)

#### [!UICONTROL 초안 메시지 만들기]

새 이메일 메시지를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>메시지의 제목란을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body Content Type]</td> 
   <td>메시지의 본문 내용이 HTML인지 아니면 텍스트인지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td> <p>전자 메일의 메시지 본문 텍스트를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>이메일의 중요도를 선택합니다</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>메시지를 보낼 수신자를 추가합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>연락처의 이름을 입력합니다</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>연락처의 이메일 주소를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>수신자 추가 메시지 사본을 받을 사람:</p> 
    <ul> 
     <li> <p><strong>이름</strong> </p> <p>연락처의 이름을 입력합니다</p> </li> 
     <li> <p><strong>이메일 주소</strong> </p> <p>연락처의 이메일 주소를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>숨은 참조 수신자</p> </td> 
   <td> <p>다른 수신자가 자신의 이름이나 이메일 주소를 볼 수 없도록 메시지에 복사할 수신자를 추가합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>연락처의 이름을 입력합니다</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>연락처의 이메일 주소를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 첨부 파일]</p> </td> 
   <td> <p>전자 메일에 첨부 파일 추가:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 파일 이름]</strong> </p> <p>파일 이름을 입력합니다. 예: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>필드에 파일 데이터를 입력하거나 파일의 소스를 매핑합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 초안 메시지 보내기]

현재 초안으로 설정된 이메일 메시지를 보냅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 초안 메시지 ID]</td> 
   <td> <p> 보낼 초안의 메시지 ID를 선택하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 메시지 업데이트]

기존 메시지를 업데이트합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메시지 ID 입력]</td> 
   <td> <p>업데이트할 메시지를 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 입력]</strong> </p> <p>메시지 ID를 입력하거나 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 목록에서 선택]</strong> </p> <p>업데이트할 메시지가 포함된 폴더를 선택하고 메시지를 선택합니다</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>메시지의 제목란을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td> <p>전자 메일의 메시지 본문 텍스트를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>이메일의 중요도를 선택합니다</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>메시지를 보낼 이메일 주소를 추가합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>연락처의 이름을 입력합니다</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>연락처의 이메일 주소를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>수신자 추가 메시지 사본을 받을 사람:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>연락처의 이름을 입력합니다</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>연락처의 이메일 주소를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bcc Recipients]</p> </td> 
   <td> <p>다른 수신자가 자신의 이름이나 이메일 주소를 볼 수 없도록 메시지에 복사할 수신자를 추가합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>연락처의 이름을 입력합니다</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>연락처의 이메일 주소를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 첨부 파일]</p> </td> 
   <td> <p>전자 메일에 첨부 파일 추가:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 파일 이름]</strong> </p> <p>파일 이름을 입력합니다. 예: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>필드에 파일 데이터를 입력하거나 파일의 소스를 매핑합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 읽은 상태로 표시]</td> 
   <td>업데이트된 메시지를 읽은 상태로 표시하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
 </tbody> 
</table>

### 첨부 파일

* [[!UICONTROL 첨부 파일 나열]](#list-attachments)
* [[!UICONTROL 첨부 파일 다운로드]](#download-an-attachment)

#### [!UICONTROL 첨부 파일 나열]

이 모듈은 지정된 메시지에 속하는 첨부 파일 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메시지 ID]</td> 
   <td> <p> 첨부 파일을 검색할 메시지의 ID를 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 첨부 파일 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 첨부 파일 다운로드]

이 모듈은 지정된 첨부 파일을 다운로드합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메시지 ID]</td> 
   <td> <p> 다운로드할 첨부 파일이 포함된 메시지의 ID를 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 첨부 파일 ID]</td> 
   <td> <p>다운로드할 첨부 파일의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 기타

* [[!UICONTROL API 호출 만들기]](#make-an-api-call)
* [[!UICONTROL 첨부 파일 추가]](#add-an-attachment)

#### [!UICONTROL API 호출 만들기]

이 모듈에서 사용자 지정 API 호출을 수행할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>상대 경로 입력 <code>https://graph.microsoft.com</code>. 예:<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 메서드]</p> </td> 
   td&gt; <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다. 예: <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] 사용자를 위해 인증 헤더를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p> 표준 JSON 개체 형태로 API 호출에 대한 쿼리를 추가합니다.</p> </td> 
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

#### [!UICONTROL 첨부 파일 추가]

이 모듈은 메시지에 큰 첨부 파일을 추가합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메시지 ID]</td> 
   <td> <p> 첨부 파일을 추가할 메시지의 ID를 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 파일]</td> 
   <td> <p>이전 모듈에서 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
