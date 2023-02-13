---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Adobe Acrobat Sign 모듈
description: 사용 [!DNL Adobe Acrobat Sign] 모듈, 시작 [!DNL Adobe Workfront Fusion] 시나리오의 이벤트 기반 [!DNL Adobe] Acrobat Sign 계정, 계약 및 기타 레코드를 생성, 읽기 또는 업데이트하고, 설정한 기준을 사용하여 레코드를 검색하고, 문서를 업로드합니다.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 01158218-31a6-4c68-a9b7-6a678a8f40c9
source-git-commit: 8bb97b08bb5991fadbf2627f4ebfdaa25ae337ce
workflow-type: tm+mt
source-wordcount: '6579'
ht-degree: 0%

---

# [!DNL Adobe Acrobat Sign] 모듈

사용 [!DNL Adobe Acrobat Sign] 모듈, 시작 [!DNL Adobe Workfront Fusion] 시나리오의 이벤트 기반 [!DNL Adobe Acrobat Sign] 계정, 계약 및 기타 레코드를 생성, 읽기 또는 갱신하고 설정한 기준을 사용하여 레코드를 검색하고 문서를 업로드합니다.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Adobe Acrobat Sign] 커넥터 사용 권장 사항

다음 [!DNL Adobe Sign ]앱에서 eSignature 비즈니스 프로세스를 자동화합니다. [!DNL Fusion] 훨씬 더 쉽고 강력합니다.

새 사용자 대상 [!DNL Adobe Sign] 계약 갱신과 관련된 몇 가지 제약 사항에 주의를 기울여야 합니다. 계약은 일반적으로 시작된 후에는 변경되지 않습니다. 새 사용자가 [!DNL Adobe Sign] 계약 작성 모듈을 사용하여 새 계약을 만드는 데 중점을 둡니다. 그러면 다음과 같은 결과가 나옵니다 [!DNL Fusion] 자동화 작업을 보다 쉽고 [!DNL Adobe Sign].

[!DNL Adobe Sign] 계약에는 작업할 필드가 필요합니다. 이를 위한 몇 가지 옵션이 있지만, 가장 쉽고 일반적인 방법은 임시 문서를 업로드한 다음 해당 문서를 계약에 매핑하는 것입니다.

![](assets/adobe-sign-recommendations-350x168.png)

## [!DNL Adobe Acrobat Sign] 모듈 및 해당 필드

구성 시 [!DNL Adobe Acrobat Sign] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Adobe Acrobat Sign] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [액션](#actions)
* [검색 결과](#searches)

### Triggers

<!--
* [Watch for agreements](#watch-for-agreements) 
* [Watch for events](#watch-for-events)
-->

+++ **[!UICONTROL 계약 감시]**

이 트리거 모듈은 계약이 만들어지거나 업데이트될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
<td>연결 방법에 대한 지침은 [!DNL Adobe Acrobat Sign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></td>  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>새 레코드, 업데이트된 레코드 또는 둘 다를 감시할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형] </td> 
   <td>레코드를 보려는 레코드 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 텍스트 찾기]</td> 
   <td> <p>검색할 용어를 입력합니다. 이 모듈은 이러한 용어를 필드 값으로 포함하는 레코드를 반환합니다.</p> <p>의 필드 검색에 대한 자세한 내용은 [!DNL Adobe Acrobat Sign]의 "텍스트 검색 작동 방식"을 참조하십시오. <a href="https://helpx.adobe.com/sign/using/adobesign-search-users-agreements.html#HowSearchWorks">Adobe Sign 검색 - 작동 방법</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환된 최대 계약 수]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 이벤트 보기]**

이 트리거 모듈은 선택한 이벤트가 발생하면 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td>사용할 웹 후크를 선택하거나 <b>[!UICONTROL Add]</b> 다음 필드를 입력합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p>웹 후크의 이름을 입력합니다</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Adobe Acrobat Sign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 범위]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Account]</p> </li> 
     <li> <p>[!UICONTROL Group]</p> </li> 
     <li> <p>[!UICONTROL User]</p> </li> 
     <li> <p>[!UICONTROL Resource]</p> <p>[!UICONTROL 리소스]를 선택하는 경우 리소스 ID와 리소스 유형을 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 리소스 수준]</td> 
   <td> <p>보려는 리소스 유형을 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL 계약]</p> </li> 
     <li> <p>[!UICONTROL 위젯]</p> </li> 
     <li> <p>[!UICONTROL Megasings]</p> </li> 
     <li> <p>[!UICONTROL Library Documents]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook 구독 이벤트]</td> 
   <td>을(를) 선택합니다 [!DNL Adobe Sign] 모듈에서 볼 이벤트입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 응용 프로그램 표시 이름]</td> 
   <td>웹 후크를 만들 응용 프로그램의 표시 이름입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 응용 프로그램 이름]</td> 
   <td>웹 후크를 만들 응용 프로그램의 표시 이름입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 문제 알림 이메일]</td> 
   <td> <p>이 설정은 관리자 계정에만 작동합니다</p> <p>문제 알림 전자 메일을 보내려는 각 전자 메일 주소의 경우 <b>[!UICONTROL Add]</b> 전자 메일 주소를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 계약 조건부 매개 변수]</td> 
   <td>조건부 매개 변수를 추가하려면 <b>[!UICONTROL Yes]</b> 매개 변수를 추가할 레코드 유형에서 <b>[!UICONTROL Yes]</b> 활성화하려는 매개 변수에 대해 설명합니다.</td> 
  </tr> 
 </tbody> 
</table>

+++

### 액션

<!--
* [Create a record](#create-a-record) 
* [Create an agreement](#create-an-agreement) 
* [Create related records](#create-related-records) 
* [Custom API Call](#custom-api-call) 
* [List records](#list-records) 
* [Read a record](#read-a-record) 
* [Read related records](#read-related-records) 
* [Update a record](#update-a-record) 
* [Update related record](#update-related-record) 
* [Upload document](#upload-document)
-->

+++ **[!UICONTROL 레코드 만들기]**

이 작업 모듈은 선택한 유형의 새 레코드를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 방법에 대한 지침은 [!DNL Adobe Acrobat Sign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td>요청의 헤더를 표준 JSON 개체 형태로 추가합니다. 예: <code>{"Content-type":"application/json"}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>만들 레코드 유형을 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Group]</b> </p> </li> 
     <li> <p><b>[!UICONTROL Library document]</b> </p> </li> 
     <li> <p><b>[!UICONTROL User]</b> </p> </li> 
     <li> <p><b>[!UICONTROL 웹 양식] ([!UICONTROL Widget])</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 그룹 정보]</td> 
   <td> <p>그룹의 [!UICONTROL 이름] 및 [!UICONTROL ID]를 입력하거나 매핑하고 이 그룹이 계정의 기본 그룹인지 여부를 지정합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Library document info]</td> 
   <td> <p>다음 필드를 채웁니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 보낼 파일]</b> </p> <p>추가할 각 파일에 대해 <b>[!UICONTROL 항목 추가]</b> 필드를 입력합니다.</p> 
      <ul> 
       <li><b>[!UICONTROL Transient 문서 ID]</b> <p>임시 문서의 ID를 입력합니다</p> </li> 
       <li> <p><b>[!UICONTROL URL 파일 전송]</b> </p> <p>다음 필드를 채웁니다.</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Mime-Type]</b> </p> <p>원본 파일의 MIME 유형을 입력합니다. MIME(Multipurpose Internet Mail Extension) 유형은 소프트웨어가 인터넷에서 공유되는 서로 다른 유형의 데이터를 식별할 수 있도록 하는 레이블입니다. 웹 서버와 브라우저는 MIME 유형을 사용하여 파일로 수행할 작업을 결정합니다. 예를 들어 MIME 유형을 갖는 파일입니다 <code>text/html</code> 은 MIME 유형을 사용하는 파일과 다르게 브라우저에서 처리됩니다 <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL Name]</b> </p> <p>파일 이름을 입력합니다.</p> </li> 
         <li> <p><b>[!UICONTROL URL]</b> </p> <p>전송할 파일의 URL을 입력합니다.</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL Notificate]</b> </p> <p>이 문서를 공증해야 하는지 여부를 선택합니다.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL 라이브러리 템플릿 이름]</b> </p> <p>라이브러리 템플릿의 이름을 입력하거나 매핑합니다</p> </li> 
     <li> <p><b>[!UICONTROL 공유 모드]</b> </p> <p>라이브러리 문서에 액세스할 사용자를 지정합니다.</p> </li> 
     <li> <p><b>[!UICONTROL Library document state]</b> </p> <p>문서가 작성 상태인지 아니면 활성 상태인지 선택합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 라이브러리 템플릿 유형]</b> </p> <p>사용할 각 라이브러리 템플릿 유형에 대해 <b>[!UICONTROL 항목 추가]</b> 템플릿 유형을 선택합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 마지막 이벤트 날짜]</b> </p> <p>라이브러리 문서에서 이벤트가 발생한 마지막 날짜를 입력합니다.</p> <p>지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
     <li> <p><b>[!UICONTROL 라이브러리 문서 상태]</b> </p> <p>라이브러리 문서의 상태를 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사용자 정보]</td> 
   <td> <p>다음 필드를 채웁니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Email]</b> </p> <p>사용자의 이메일 주소를 입력합니다.</p> </li> 
     <li> <p><b>[!UICONTROL은 계정 관리자입니다.]</b> </p> <p>생성된 사용자가 계정 관리자인 경우 이 옵션을 선택합니다.</p> </li> 
     <li> <p><b>[!UICONTROL User ID]</b> </p> <p>사용자의 고유 ID를 입력합니다</p> </li> 
     <li> <p><b>[!UICONTROL 계정 ID]</b> </p> <p>의 고유 ID를 입력합니다 [!DNL Adobe Acrobat Sign] 이 사용자와 연결된 계정입니다.</p> </li> 
     <li> <p><b>[!UICONTROL 이름]</b> </p> <p>사용자의 이름을 입력합니다.</p> </li> 
     <li> <p><b>[!UICONTROL Last name]</b> </p> <p>사용자의 성을 입력합니다</p> </li> 
     <li> <p><b>[!UICONTROL Company]</b> </p> <p>사용자 회사의 이름을 입력합니다.</p> </li> 
     <li> <p><b>[!UICONTROL Insertion]</b> </p> <p>사용자의 이니셜을 입력합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 로케일]</b> </p> <p>사용자의 로케일을 입력합니다. UI의 언어를 결정합니다. </p> </li> 
     <li> <p><b>[!UICONTROL Phone]</b> </p> <p>사용자의 전화 번호를 입력합니다</p> </li> 
     <li> <p><b>기본 그룹 ID</b> </p> <p>새 사용자를 추가할 그룹을 입력합니다. 아무 것도 입력하지 않으면 사용자는 계정의 기본 그룹에 추가됩니다.</p> </li> 
     <li> <p><b>[!UICONTROL Job title]</b> </p> <p>사용자의 직함을 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 웹 양식 정보]</td> 
   <td> <p>다음 필드를 채웁니다</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 파일 정보]</b> </p> <p>웹 양식에 추가할 각 파일에 대해 추가 를 클릭하고 다음 필드를 채웁니다.</p> 
      <ul> 
       <li> <p>[!UICONTROL 파일 형식]</p> <p>[!UICONTROL Document]</p> </li> 
       <li> <p>[!UICONTROL Transient 문서]</p> </li> 
       <li> <p>[!UICONTROL URL 파일 정보]</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL 웹 양식 이름]</b> </p> <p>웹 양식의 이름을 입력합니다. 이 이름은 이메일 및 웹 사이트 등의 위치에서 웹 양식을 식별하는 데 사용됩니다.</p> </li> 
     <li> <p><b>[!UICONTROL 웹 양식 상태]</b> </p> <p>새 웹 양식을 만들 상태를 선택합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 웹 양식 참가자 집합 정보]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL Member info]</b> </p> <p>참가자 세트에 추가할 각 구성원에 대해 <b>[!UICONTROL 항목 추가]</b>. </p> 
        <ul> 
         <li> <p><b>[!UICONTROL Email]</b> </p> <p>이 옵션을 비워 둡니다.</p> </li> 
         <li> <p><b>[!UICONTROL 보안 옵션]</b> </p> <p>이 사용자를 인증하기 위한 보안 옵션을 추가하려면 <b>[!UICONTROL Yes]</b>그런 다음 보안 옵션을 선택하고 필요한 필드를 채웁니다.</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL 역할]</b> </p> <p>역할을 선택합니다. 이 참가자 집합의 모든 구성원이 역할을 공유합니다.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL 웹 양식 추가 참가자 집합 정보]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL Member info]</b> </p> <p>참가자 세트에 추가할 각 구성원에 대해 <b>[!UICONTROL 항목 추가]</b>.</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Email]</b> </p> <p>이 옵션을 비워 둡니다.</p> </li> 
         <li> <p><b>[!UICONTROL 보안 옵션]</b> </p> <p>이 사용자를 인증하기 위한 보안 옵션을 추가하려면 <b>[!UICONTROL Yes]</b>그런 다음 보안 옵션을 선택하고 필요한 필드를 채웁니다.</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL 역할]</b> </p> </li> 
       <li> <p><b>[!UICONTROL 웹 양식 참가자 ID] </b> </p> <p>웹 양식 참가자의 ID를 입력합니다.</p> </li> 
       <li> <p><b>[!UICONTROL Order]</b> </p> <p>이 참가자 집합이 웹 양식과 상호 작용하는 순서를 지정합니다. 예를 들어 주문 값이 1인 참가자 그룹은 먼저, 2는 다음 순으로 진행해야 합니다. 주문 번호는 1로 시작해야 하며 시리즈에는 간격이 없습니다. </p> </li> 
       <li> <p><b>[!UICONTROL 공급자 참가자 집합 정보]</b> </p> <p>참가자를 알 수 없는 경우, 공급자가 가입자에 대한 상세내역을 제공해야 하는지 여부를 입력하고, 알 수 없는 참여자에 대해 필요한 상세내역을 포함하는 메시지를 입력합니다.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL 인증 실패 정보]</b> </p> <p>사용자에 대한 오류 또는 오류 페이지를 제공하려면 <b>[!UICONTROL Yes]</b>를 입력한 다음 다음 다음 필드를 입력합니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL URL]</b> </p> <p>오류 페이지의 URL을 입력합니다</p> </li> 
       <li> <p><b>[!UICONTROL Deframe]</b> </p> <p>오류 페이지를 웹 양식 내에 표시하려면 이 옵션을 활성화합니다</p> </li> 
       <li> <p><b>[!UICONTROL Delay]</b> </p> <p>사용자가 오류 페이지로 리디렉션되기 전에 지연을 초 단위로 입력합니다.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL CC info]</b> </p> <p>웹 양식의 최종 계약이 체결될 때 전자 메일을 받을 각 전자 메일 주소의 경우 <b>[!UICONTROL 항목 추가]</b> 전자 메일 주소를 입력합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 완료 정보]</b> </p> <p style="font-style: normal;">사용자를 위한 성공 페이지를 제공하려면 을(를) 선택합니다. <b>[!UICONTROL Yes]</b>를 입력한 다음 다음 다음 필드를 입력합니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL URL]</b> </p> <p>성공 페이지의 URL을 입력합니다</p> </li> 
       <li> <p><b>[!UICONTROL Deframe]</b> </p> <p>성공 페이지를 웹 양식 내에 표시하려면 이 옵션을 활성화합니다</p> </li> 
       <li> <p><b>[!UICONTROL Delay]</b> </p> <p>사용자가 성공 페이지로 리디렉션되기 전에 지연을 초 단위로 입력합니다.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL 그룹 ID]</b> </p> <p>웹 양식이 속한 그룹의 ID를 입력합니다. 아무 것도 입력하지 않으면 웹 양식은 계정 사용자의 기본 그룹에 속합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 마지막 이벤트 날짜]</b> </p> <p>웹 양식에서 마지막 이벤트가 발생한 날짜를 입력합니다. 형식 사용 <code>yyyy-MM-dd'T'HH:mm:ssZ</code>.</p> </li> 
     <li> <p><b>[!UICONTROL 로케일]</b> </p> <p>사용자의 로케일을 입력합니다. UI의 언어를 결정합니다. </p> </li> 
     <li> <p><b>[!UICONTROL Security Options]n</b> </p> <p>문서 보안을 설정하는 데 사용되는 암호를 입력합니다. 이 비밀번호는 관련 당사자에게 별도로 전달해야 합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 저장 정보]</b> </p> <p>계정이 문서 소산(vaulting)에 대해 설정되어 있고 계약에 따라 활성화할 수 있는 옵션이 설정되어 있는 경우 이 옵션을 사용하여 이 계약을 저장할 수 있습니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 계약 만들기]**

이 작업 모듈은 계약을 작성하여 서명을 위해 전송한 다음 계약 ID를 반환합니다.

>[!NOTE]
>
>임시 문서로 서명하도록 문서를 업로드한 다음 이 문서를 [!UICONTROL 보낼 파일] 의 필드 [!UICONTROL 계약 만들기] 모듈. 예를 보려면 이 문서에서 &quot;문서 업로드&quot;를 참조하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
<td>연결 방법에 대한 지침은 [!DNL Adobe Acrobat Sign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></td>  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td>요청의 헤더를 표준 JSON 개체 형태로 추가합니다. 예: <code>{"Content-type":"application/json"}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 보낼 파일]</td> 
   <td> <p>계약에 포함할 각 항목에 대해 <b>[!UICONTROL 항목 추가]</b> 다음 필드를 채웁니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 파일 형식]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL Document]</b> </p> <p>다음 필드를 채웁니다.</p> 
        <ul> 
         <li> <p><b>[!UICONTROL 작성일]</b> </p> <p>문서를 만든 날짜를 형식으로 입력하거나 매핑합니다 <code>yyyy-MM-dd'T'HH:mm:ssZ</code>. 예, <code>2016-02-25T18:46:19Z</code> UTC 시간을 나타냅니다.</p> </li> 
         <li> <p><b>[!UICONTROL ID]</b> </p> <p>문서의 ID를 입력하거나 매핑합니다.</p> </li> 
         <li> <p><b>[!UICONTROL Label]</b> </p> <p>파일의 고유 레이블을 입력하거나 매핑합니다. 사용자 지정 워크플로우의 경우 워크플로우 정의의 해당 파일 요소에 파일을 매핑합니다. 사용자 지정 워크플로 계약 작성 요청의 경우 지정해야 합니다.</p> </li> 
         <li> <p><b>[!UICONTROL 페이지 수]</b> </p> <p>문서의 페이지 수를 입력하거나 매핑합니다.</p> </li> 
         <li> <p><b>[!UICONTROL Mime-Type]</b> </p> <p>원본 파일의 MIME 유형을 입력하거나 매핑합니다. MIME(Multipurpose Internet Mail Extension) 유형은 소프트웨어가 인터넷에서 공유되는 서로 다른 유형의 데이터를 식별할 수 있도록 하는 레이블입니다. 웹 서버와 브라우저는 MIME 유형을 사용하여 파일로 수행할 작업을 결정합니다. 예를 들어 MIME 유형을 갖는 파일입니다 <code>text/html</code> 은 MIME 유형을 사용하는 파일과 다르게 브라우저에서 처리됩니다 <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL Name]</b> </p> <p>문서의 이름을 입력하거나 매핑합니다.<br></p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL Library document ID]</b> </p> <p>라이브러리 문서의 ID를 입력합니다</p> </li> 
       <li> <p><b>[!UICONTROL Transient 문서 ID]</b> </p> <p>임시 문서의 ID를 입력합니다</p> </li> 
       <li> <p><b>[!UICONTROL URL 파일 전송]</b> </p> <p>다음 필드를 채웁니다.</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Mime-Type]</b> </p> <p>원본 파일의 MIME 유형을 입력합니다. MIME(Multipurpose Internet Mail Extension) 유형은 소프트웨어가 인터넷에서 공유되는 서로 다른 유형의 데이터를 식별할 수 있도록 하는 레이블입니다. 웹 서버와 브라우저는 MIME 유형을 사용하여 파일로 수행할 작업을 결정합니다. 예를 들어 MIME 유형을 갖는 파일입니다 <code>text/html</code> 은 MIME 유형을 사용하는 파일과 다르게 브라우저에서 처리됩니다 <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL Name]</b> </p> <p>파일 이름을 입력합니다.</p> </li> 
         <li> <p><b>[!UICONTROL URL]</b> </p> <p>전송할 파일의 URL을 입력합니다.</p> </li> 
        </ul> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Label]</b> </p> <p>파일의 레이블을 입력합니다.</p> </li> 
     <li> <p><b>[!UICONTROL Notificate]</b> </p> <p>이 옵션을 활성화하여 파일을 공증해야 함을 나타냅니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 계약 이름]</td> 
   <td>새 계약의 이름을 입력합니다. 이 이름은 이메일 및 웹 사이트 등의 위치에서 계약을 식별하는 데 사용됩니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 참가자 집합 정보]</td> 
   <td> <p>추가할 각 참가자 세트에 대해 <b>[!UICONTROL 항목 추가]</b> 다음 필드를 입력합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Members]</b> </p> <p>참가자 세트에 추가할 각 사용자에 대해 <b>[!UICONTROL 항목 추가]</b> 사용자의 이메일 주소를 입력합니다.</p> </li> 
     <li> <p><b>[!UICONTROL Order]</b> </p> <p>이 참가자 세트가 계약에 서명해야 하는 시점을 지정합니다. 예를 들어, 순서 값이 1인 참가자 그룹은 먼저 서명해야 하며, 2는 다음에 서명해야 합니다. 주문 번호는 1로 시작해야 하며 시리즈에는 간격이 없습니다. </p> </li> 
     <li> <p><b>[!UICONTROL 역할]</b> </p> <p>이 참가자 집합에 대한 역할을 선택합니다. 집합에 있는 모든 참여자가 이 역할을 받습니다.</p> </li> 
     <li> <p><b>[!UICONTROL ID]</b> </p> <p>이 참가자 세트의 ID를 입력하거나 매핑합니다.</p> </li> 
     <li> <p><b>[!UICONTROL Label]</b> </p> <p>참가자 세트에 대한 고유한 레이블을 입력하거나 매핑합니다. 사용자 지정 워크플로우의 경우, 기여도 세트에 지정된 레이블은 사용자 지정 워크플로우의 기여도 단계에 매핑해야 합니다.</p> </li> 
     <li> <p><b>[!UICONTROL Name]</b> </p> <p>참가자 세트의 이름을 입력합니다. 이 이름은 계약 내에서 고유해야 합니다.</p> </li> 
     <li> <p><b>[!UICONTROL Private 메시지]</b> </p> <p>이 참가자 집합에 대한 메시지를 입력하거나 매핑합니다. 집합에 있는 모든 참가자가 이 메시지를 받습니다.</p> </li> 
     <li> <p><b>[!UICONTROL Visible pages]</b> </p> <p>이 계약에 대해 제한된 문서 가시성을 사용할 수 있는 경우 이 참가자 세트에 표시되는 파일을 지정합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 서명 유형]</td> 
   <td> <p>계약에 필요한 서명 유형을 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL E-sign]</b> </p> <p>그 계약서는 전자적으로 서명되어야 한다.</p> </li> 
     <li> <p><b>[!UICONTROL Written]</b> </p> <p>동의서는 수동으로 서명해야 하며, 서명된 동의서는 스캔 및 업로드해야 합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td> <p>이 계약의 상태를 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Authoring]</b> </p> <p>이 계약에 필드를 편집하거나 추가할 수 있습니다.</p> </li> 
     <li> <p><b>[!UICONTROL Draft]</b> </p> <p>이 계약서를 발송하기 전에 점진적으로 작성할 수 있습니다.</p> </li> 
     <li> <p><b>[!UICONTROL In Process]</b> </p> <p>이 계약은 즉시 전송됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CCs]</td> 
   <td> <p>이해 관계자와 같이 서명하지 않아도 되는 이해관계자에게 이 계약서를 보낼 수 있습니다. 이들은 서명 프로세스가 시작될 때 전자 메일을 받고 최종 서명을 받을 때 다른 전자 메일을 받습니다. 계약서의 PDF 사본도 받습니다. </p> <p>이 계약에 대해 참조하려는 각 사용자에 대해 <b>[!UICONTROL 항목 추가]</b> 다음 필드를 채웁니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Email]</b> </p> <p>계약에 참조할 이메일 주소를 입력하거나 매핑합니다.</p> </li> 
     <li> <p><b>[!UICONTROL Label]</b> </p> <p>워크플로우 설명과 같이 이 이메일 주소의 레이블을 입력하거나 매핑합니다</p> </li> 
     <li> <p><b>[!UICONTROL Visible pages]</b> </p> </li> 
     <li> <p>이 계약에 대해 제한된 문서 가시성을 사용할 수 있는 경우 이 참가자 세트에 표시되는 파일을 지정합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email 옵션]</td> 
   <td> <p>각 유형의 전자 메일에 대해 해당 유형의 전자 메일을 모든 참여자에게 전송할지 여부를 선택합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 완료 이메일]</b> </p> <p>이 계약이 완료, 취소, 만료 또는 거부되면 전자 메일을 보냅니다.</p> </li> 
     <li> <p><b>[!UICONTROL In-Flight 이메일]</b> </p> <p>이 계약이 위임되거나 교체되면 전자 메일을 보냅니다.</p> </li> 
     <li> <p><b>[!UICONTROL 계약 시작 전자 메일]</b> </p> <p>이 계약이 만들어지거나 작업에 대한 작업이 요청될 때 이메일을 보냅니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 외부 ID]</td> 
   <td> <p>이 계약의 ID를 입력하거나 매핑합니다. 계약을 만들 때 이를 지정하고 이후 모듈이나 쿼리에서 계약을 찾는 데 사용할 수 있습니다.</p> <p>참고: 외부 ID 값은 API를 통해 모든 참여자에게 표시되므로 중요한 토큰을 포함하는 데 사용해서는 안 됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 병합 필드 정보]</td> 
   <td> <p>기본값을 지정할 계약의 각 필드에 대해 <b>[!UICONTROL 항목 추가]</b> 기본값을 입력하고 필드 이름을 입력합니다.</p> <p>편집 가능한 필드에 대해 서명자에게 값이 표시됩니다. 읽기 전용 필드의 경우 서명 프로세스 중에 제공된 값을 편집할 수 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 공증인 정보]</td> 
   <td> <p>다음 필드를 채웁니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Impression]</b> </p> <p>이 계약을 공증할 약속의 제안된 시간과 일자를 입력하거나 매핑합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 참고]</b> </p> <p>공증인 세션에 포함할 메모를 입력하거나 매핑합니다.</p> </li> 
     <li> <p><b>[!UICONTROL Payment]</b> </p> <p>서명자 또는 계약 발신자에 의해 공증인이 지급되는지 여부를 선택합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 공증인 유형]</b> </p> <p>공증인 유형을 선택합니다</p> 
      <ul> 
       <li> <p>[!UICONTROL 공급자 공증인]</p> <p>공증인은 공증인이 제공한다.</p> </li> 
       <li> <p>[!UICONTROL B변 공증인]</p> <p>공증인은 고객이 제공한다.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Post 서명 옵션]</td> 
   <td> <p>계약 서명 후 서명자에게 성공 페이지로 이동할지 여부를 선택합니다. 선택하는 경우 <b>[!UICONTROL Yes]</b>을 눌러 다음 필드를 입력합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 리디렉션 지연]</b> </p> <p>서명자가 성공 페이지로 리디렉션되기 전 시간(초)을 나타내는 숫자를 입력하거나 매핑합니다. 이 값이 0보다 큰 경우 사용자가 먼저 표준을 확인합니다 [!DNL Adobe Sign] 성공 메시지와 함께 지연이 성공 페이지로 리디렉션됩니다.</p> </li> 
     <li> <p><b>[!UICONTROL 리디렉션 URL]</b> </p> <p>서명 프로세스를 성공적으로 완료한 후 사용자가 전송될 공개 액세스 가능한 URL을 입력하거나 매핑합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 보안 옵션]</td> 
   <td> <p>PDF 문서 보안을 위해 사용할 보조 암호를 입력하거나 매핑합니다. </p> <p>중요 사항: [!DNL Adobe Sign] 이 비밀번호는 공유되지 않으므로 관련자에게 별도로 전달해야 합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 저장 정보]</td> 
   <td>계정이 문서 소산(vaulting)에 대해 설정되어 있고 계약에 따라 활성화할 수 있는 옵션이 설정되어 있는 경우 이 옵션을 사용하여 이 계약을 저장할 수 있습니다.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 관련 레코드 만들기]**

이 작업 모듈은 선택한 모듈에 연결된 레코드를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Adobe Acrobat Sign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 인증 헤더를 자동으로 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td>생성된 레코드를 연결할 원본 레코드의 레코드 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agreement]/[!UICONTROL Library Document]/[!UICONTROL User]/[!UICONTROL Widget ID]</td> 
   <td>생성된 레코드를 연결할 객체의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 계약 관련 필드]</td> 
   <td> <p>만들려는 관련 필드 유형을 선택합니다</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 양식 필드]</b> </p> <p>만들려는 필드가 포함된 템플릿의 템플릿 ID를 입력합니다</p> </li> 
     <li> <p><b>[!UICONTROL 미리 알림]</b> </p> <p>다음 필드를 채웁니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Recipient 참가자 ID]</b> </p> <p>미리 알림을 받을 각 참가자에 대해 [!UICONTROL 항목 추가]를 클릭하고 참여자의 ID를 입력합니다.</p> </li> 
       <li> <p><b>[!UICONTROL 상태]</b> </p> <p>새 레코드의 경우 상태는 [!UICONTROL Active]여야 합니다.</p> </li> 
       <li> <p><b>[!UICONTROL 첫 번째 미리 알림 지연]</b> </p> <p>첫 번째 미리 알림을 보내기 전에 지연 시간(시간)을 입력합니다. 허용되는 최소값은 1시간이고 최대값은 계약 생성 및 만료 시간(시간)의 차이보다 클 수 없습니다. 이 지연을 설정하지 않으면 첫 번째 미리 알림은 빈도를 기반으로 합니다.</p> </li> 
       <li> <p><b>[!UICONTROL 미리 알림 빈도]</b> </p> <p>미리 알림을 보낼 빈도를 설정합니다. 빈도를 제공하지 않으면 미리 알림을 한 번 보냅니다.</p> </li> 
       <li> <p><b>[!UICONTROL 마지막으로 보낸 날짜]</b> </p> <p>이 필드는 시스템에 의해 설정됩니다.</p> </li> 
       <li> <p><b>[!UICONTROL 다음 전송 날짜]</b> </p> <p>이 필드는 비워 두거나 [!UICONTROL ONCE]로 설정해야 합니다.</p> </li> 
       <li> <p><b>[!UICONTROL 참고]</b> </p> <p>미리 알림에 포함할 메모를 입력합니다. 이 기능은 참여자에게 참여가 필요한 이유를 알리는 데 유용합니다.</p> </li> 
       <li> <p><b>[!UICONTROL 시작 미리 알림 카운터]부터</b> </p> <p>사용 가능한 시점에 계약을 생성할 시점을 기준으로 미리 알림을 전송할지 여부를 선택합니다.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL 서명자 ID 보고서]</b> </p> <p>PDF 문서의 보안을 유지하는 데 사용되는 암호를 입력합니다.</p> </li> 
     <li> <p><b>[!UICONTROL Views]</b> </p> <p>다음 필드를 입력합니다</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Name]</b> </p> <p>만들 보기의 이름을 선택합니다.</p> </li> 
       <li> <p><b>[!UICONTROL 자동 로그인 사용자]</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 를 입력하여 반환된 URL에 사용자를 자동으로 로그인합니다.</p> </li> 
       <li> <p><b>[!UICONTROL 프레임 상위]</b> </p> <p>반환된 URL의 프레임을 지정할 수 있는 상위 도메인 URL의 쉼표로 구분된 목록을 입력하거나 매핑합니다. 비워 두면 [!DNL Adobe Acrobat Sign] 페이지가 iframe에서 볼 수 없습니다.</p> </li> 
       <li> <p><b>[!UICONTROL 로케일]</b> </p> <p>보기를 만들 언어를 입력합니다. </p> </li> 
       <li> <p><b>[!UICONTROL No chrome 플래그]</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 탐색 머리글이나 바닥글 없이 포함된 페이지를 표시하려면 을(를) 클릭합니다.</p> </li> 
       <li> <p><b>[!UICONTROL 파일 편집 가능]</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 파일을 추가하거나 제거하여 파일 업로드 섹션을 편집하려는 경우. 이것은 접근 제어 기계주의가 아닙니다. 기본값은 [!UICONTROL Yes]입니다.</p> </li> 
       <li> <p><b>[!UICONTROL Library document]</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 라이브러리 문서 링크를 표시하려면 다음 단계를 따르세요. 기본값은 [!UICONTROL Yes]입니다.</p> </li> 
       <li> <p><b>[!UICONTROL 로컬 파일]</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 로컬 파일 업로드 단추가 나타나도록 하려면 기본값은 [!UICONTROL Yes]입니다.</p> </li> 
       <li> <p><b>[!UICONTROL Web Connectors]</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 웹 소스의 문서를 연결하는 링크가 표시되도록 하려면 기본값은 예입니다.</p> </li> 
       <li> <p><b>[!UICONTROL이 미리 보기를 선택함]</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 작성 페이지를 작성 모드로 설정하려면 다음을 수행하십시오.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Member share]</b> </p> <p>계약을 공유할 각 구성원에 대해 <b>[!UICONTROL 항목 추가]</b> 구성원의 전자 메일 주소와 해당 구성원에게 메시지를 입력합니다.</p> </li> 
     <li> <p>[!UICONTROL 위임 참가자 집합]</p> 
      <ul> 
       <li> <p><b>[!UICONTROL 참가자 집합 ID]</b> </p> <p>참가자 세트의 ID를 입력합니다</p> </li> 
       <li> <p><b>[!UICONTROL Member info]</b> </p> <p>추가할 각 구성원에 대해 [!UICONTROL 항목 추가]를 클릭하고 구성원에 대한 전자 메일 주소와 전화 정보를 입력합니다.</p> </li> 
       <li> <p><b>[!UICONTROL Private 메시지]</b> </p> <p>메시지를 입력합니다. 참가자 집합의 모든 구성원이 이 메시지를 받습니다.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 라이브러리 보기 정보]</td> 
   <td> <p>다음 필드를 채웁니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Name]</b> </p> <p>라이브러리 템플릿의 이름을 입력합니다. 이 이름은 이메일 및 웹 사이트에 사용됩니다.</p> </li> 
     <li> <p><b>[!UICONTROL 자동 로그인 사용자]</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 를 입력하여 반환된 URL에 사용자를 자동으로 로그인합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 프레임 상위]</b> </p> <p>반환된 URL의 프레임을 지정할 수 있는 상위 도메인 URL의 쉼표로 구분된 목록을 입력하거나 매핑합니다. 비워 두면 [!DNL Adobe Acrobat Sign] 페이지가 iframe에서 볼 수 없습니다.</p> </li> 
     <li> <p><b>[!UICONTROL 로케일]</b> </p> <p>보기를 만들 언어를 입력합니다. </p> </li> 
     <li> <p><b>[!UICONTROL No chrome 플래그]</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 탐색 머리글이나 바닥글 없이 포함된 페이지를 표시하려면 을(를) 클릭합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 보기 구성 보내기]</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> [!UICONTROL Send] 보기를 구성하려면 다음 필드를 입력합니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL 계약 이름]</b> </p> <p>작성 페이지에서 라이브러리 문서의 계약 이름을 입력하거나 매핑합니다.</p> </li> 
       <li> <p><b>[!UICONTROL 파일 편집 가능]</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 파일을 추가하거나 제거하여 파일 업로드 섹션을 편집하려는 경우. 이것은 접근 제어 기계주의가 아닙니다. 기본값은 [!UICONTROL Yes]입니다.</p> </li> 
       <li> <p><b>[!UICONTROL 로컬 파일]</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 라이브러리 문서 링크를 표시하려면 다음 단계를 따르세요. 기본값은 [!UICONTROL Yes]입니다.</p> </li> 
       <li> <p><b>[!UICONTROL Web Connectors]</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 웹 소스의 문서를 연결하는 링크가 표시되도록 하려면 기본값은 [!UICONTROL Yes]입니다.</p> </li> 
       <li> <p><b>미리 보기를 선택함</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 작성 페이지를 작성 모드로 설정하려면 다음을 수행하십시오.</p> </li> 
      </ul> <p> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사용자 보기 정보]</td> 
   <td> <p>다음 필드를 채웁니다</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Name]</b> </p> <p>요청된 사용자 보기의 이름을 선택합니다.</p> </li> 
     <li> <p><b>[!UICONTROL 자동 로그인 사용자]</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 을 입력하여 사용자를 자동으로 로그인합니다. 선택 <b>[!UICONTROL No]</b> 자격 증명이 필요합니다. 기본값은 [!UICONTROL No]입니다.</p> </li> 
     <li> <p><b>[!UICONTROL 프레임 상위]</b> </p> <p>반환된 URL의 프레임을 지정할 수 있는 상위 도메인 URL의 쉼표로 구분된 목록을 입력하거나 매핑합니다. 비워 두면 [!DNL Adobe Acrobat Sign] 페이지가 iframe에서 볼 수 없습니다.</p> </li> 
     <li> <p><b>Chrome 플래그가 없음</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 탐색 머리글이나 바닥글 없이 포함된 페이지를 표시하려면 을(를) 클릭합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Widget 관련 필드]</td> 
   <td> <p>생성할 관련 레코드를 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL Views]</p> <p>다음 필드를 입력합니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Name]</b> </p> <p>요청된 웹 양식 보기의 이름을 선택합니다</p> </li> 
       <li> <p><b>[!UICONTROL 자동 로그인 사용자]</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 을 입력하여 사용자를 자동으로 로그인합니다. 선택 <b>[!UICONTROL No]</b> 자격 증명이 필요합니다. 기본값은 [!UICONTROL No]입니다.</p> </li> 
       <li> <p><b>[!UICONTROL 프레임 상위]</b> </p> <p>반환된 URL의 프레임을 지정할 수 있는 상위 도메인 URL의 쉼표로 구분된 목록을 입력하거나 매핑합니다. 비워 두면 [!DNL Adobe Acrobat Sign] 페이지가 iframe에서 볼 수 없습니다.</p> </li> 
       <li> <p><b>[!UICONTROL 로케일]</b> </p> <p>보기를 만들 언어를 입력합니다. </p> </li> 
       <li> <p><b>[!UICONTROL No chrome 플래그]</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 탐색 머리글이나 바닥글 없이 포함된 페이지를 표시하려면 을(를) 클릭합니다.</p> </li> 
       <li> <p>[!UICONTROL 개인화된 서명 보기 구성]</p> <p>개인화된 서명 보기를 구성하려면 을 선택합니다 <b>[!UICONTROL Yes]</b> 다음 필드를 채웁니다.</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Email]</b> </p> <p>새로 만든 웹 양식을 받은 사람의 이메일 주소를 입력합니다</p> </li> 
         <li> <p><b>[!UICONTROL Comment]</b> </p> <p>API 호출자가 서명자의 ID를 설정하는 방법을 설명하는 설명을 입력합니다. 이 정보는 [!DNL Adobe Acrobat Sign] 감사 추적.</p> </li> 
         <li> <p><b>[!UICONTROL 만료]</b> </p> <p>이 웹 양식의 개인화에 대한 만료 날짜를 입력합니다. </p> <p>지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
         <li> <p><b>[!UICONTROL Reusable]</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 의도한 서명자가 양식에 두 번 이상 서명할 수 있도록 하려면</p> </li> 
        </ul> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Member share]</b> </p> <p>계약을 공유할 각 구성원에 대해 <b>[!UICONTROL 항목 추가]</b> 구성원의 전자 메일 주소와 해당 구성원에게 메시지를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 사용자 지정 API 호출]**
이 모듈에서 사용자 지정 API 호출을 수행할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Adobe Acrobat Sign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>상대 경로 입력 <code>https://api.[region].adobesign.com/api/rest/v6/</code></p> <p>참고: 사용 가능한 끝점 목록에 대해서는 [!DNL Adobe Sign] API 참조.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 메서드]</p> </td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 인증 헤더를 자동으로 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열] </td> 
   <td> <p>요청 쿼리 문자열을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>표준 JSON 개체 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>다음과 같은 조건문을 사용하는 경우 <code>if</code> json에서 따옴표를 조건문 외부에 지정합니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 임시 문서 업로드]</td> 
   <td> <p>임시 문서를 업로드하려면 업로드할 문서의 소스 파일을 입력합니다.</p> <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 레코드 나열]**

이 작업 모듈은 계정이 액세스할 수 있는 선택한 유형의 모든 레코드를 나열합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Adobe Acrobat Sign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 인증 헤더를 자동으로 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td>관련 레코드를 검색할 레코드 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 로케일]</td> 
   <td> <p>사용자의 로케일을 입력합니다. UI의 언어를 결정합니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 외부 ID]</td> 
   <td>외부 ID(외부 ID)를 입력하거나 매핑합니다. [!DNL Adobe Acrobat Sign])을 클릭하여 되돌릴 계약에 대해 지정합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 그룹 ID]</td> 
   <td>나열할 레코드와 연관된 그룹의 ID를 입력합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 숨겨진(레코드) 표시]</td> 
   <td>결과에 숨겨진 레코드를 포함하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cursor] / [!UICONTROL Start Index]</td> 
   <td> <p>모듈이 반환해야 하는 첫 번째 레코드 수를 입력합니다. </p> <p>참고: 이 필드는 페이지 매기기를 위한 [!UICONTROL 최대 반환 레코드 수] 필드와 결합됩니다. 예를 들어 [!UICONTROL Maximum number of returned events]가 100이고 [!UICONTROL Start Index]가 101이면 모듈은 레코드 101-200 또는 두 번째 결과 페이지를 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환된 최대 레코드 수]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈을 [action]에 넣을 최대 레코드 수를 입력하거나 매핑합니다.</p> <p>참고: 이 필드는 페이지 매김을 위한 [!UICONTROL Cursor] 또는 [!UICONTROL Start Index] 필드와 결합됩니다. 예를 들어 [!UICONTROL Maximum number of returned events]가 100이고 [!UICONTROL Start Index]가 101이면 모듈은 레코드 101-200 또는 두 번째 결과 페이지를 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 상위 도메인 URL]</td> 
   <td> <p>반환된 URL의 프레임을 지정할 수 있는 상위 도메인 URL의 쉼표로 구분된 목록을 입력하거나 매핑합니다. 비워 두면 [!DNL Adobe Acrobat Sign] 페이지가 iframe에서 볼 수 없습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 레코드 읽기]**

이 작업 모듈은 단일 레코드에서 정보를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Adobe Acrobat Sign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 인증 헤더를 자동으로 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td>관련 레코드를 검색할 레코드 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 ID]</td> 
   <td>검색할 레코드의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 관련 레코드 읽기]**

단일 레코드와 관련된 추가 정보를 읽어 보십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Adobe Acrobat Sign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 인증 헤더를 자동으로 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td>관련 레코드를 검색할 레코드 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 ID](예: [!UICONTROL 계정 ID])</td> 
   <td>관련 레코드를 검색할 레코드의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 기타 필드]</td> 
   <td>레코드 유형 및 관련 필드를 기준으로 특정 필드에 정보를 입력합니다.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 레코드 업데이트]**

이 작업 모듈은 [!DNL Adobe Acrobat Sign].

>[!IMPORTANT]
>
>* 가장 좋은 방법은 계약에 대한 상당한 변경 사항이 예상되는 경우 기존 계약을 업데이트하는 대신 새 계약을 만드는 것입니다.
>* 일부 업데이트 기능 필수 필드입니다. 업데이트를 구성할 때 모든 필수 필드를 입력해야 합니다. 필수 필드는 굵게 표시되어 있습니다. [!DNL Workfront Fusion] 모듈.
>




<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Adobe Acrobat Sign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 인증 헤더를 자동으로 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 ID] </td> 
   <td>업데이트할 레코드의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td>업데이트할 레코드 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 기타 필드]</td> 
   <td> <p>레코드 유형 및 관련 필드를 기준으로 특정 필드에 정보를 입력합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Agreement]</b> </p> <p>가장 좋은 방법은 계약에 대한 상당한 변경 사항이 예상되는 경우 기존 계약을 업데이트하는 대신 새 계약을 만드는 것입니다.</p> </li> 
     <li> <p><b>[!UICONTROL Library document]</b> </p> <p>업데이트할 필드를 선택한 다음 선택한 필드를 채웁니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL 상태]</b> </p> <p>라이브러리 문서의 새 상태를 선택합니다.</p> </li> 
       <li> <p><b>[!UICONTROL Name]</b> </p> <p>라이브러리 템플릿의 이름을 입력하거나 매핑합니다</p> </li> 
       <li> <p><b>[!UICONTROL 공유 모드]</b> </p> <p>라이브러리 문서에 액세스할 사용자를 지정합니다.</p> </li> 
       <li> <p><b>[!UICONTROL 라이브러리 템플릿 유형]</b> </p> <p>사용할 각 라이브러리 템플릿 유형에 대해 <b>[!UICONTROL 항목 추가]</b> 템플릿 유형을 선택합니다.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL User]</b> </p> <p>업데이트할 필드를 선택한 다음 선택한 필드를 채웁니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL 이름]</b> </p> <p>사용자의 이름을 입력합니다.</p> </li> 
       <li> <p><b>[!UICONTROL Last name]</b> </p> <p>사용자의 성을 입력합니다</p> </li> 
       <li> <p><b>[!UICONTROL Company]</b> </p> <p>사용자 회사의 이름을 입력합니다.</p> </li> 
       <li> <p><b>[!UICONTROL Phone]</b> </p> <p>사용자의 전화 번호를 입력합니다</p> </li> 
       <li> <p><b>[!UICONTROL 기본 그룹 ID]</b> </p> <p>새 사용자를 추가할 그룹을 입력합니다. 아무 것도 입력하지 않으면 사용자는 계정의 기본 그룹에 추가됩니다.</p> </li> 
       <li> <p><b>[!UICONTROL Job title]</b> </p> <p>사용자의 직함을 입력합니다.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL 웹 양식] ([!UICONTROL 위젯])</b> </p> <p>레코드 유형 및 관련 필드를 기준으로 특정 필드에 정보를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 관련 레코드 업데이트]**

이 작업 모듈은 특정 객체와 관련된 레코드를 업데이트합니다.

>[!IMPORTANT]
>
>* 가장 좋은 방법은 계약에 대한 상당한 변경 사항이 예상되는 경우 기존 계약을 업데이트하는 대신 새 계약을 만드는 것입니다.
>* 일부 업데이트 기능 필수 필드입니다. 업데이트를 구성할 때 모든 필수 필드를 입력해야 합니다. 필수 필드는 굵게 표시되어 있습니다. [!DNL Workfront Fusion] 모듈.
>




<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Adobe Acrobat Sign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 인증 헤더를 자동으로 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td>관련 필드가 연관된 레코드의 레코드 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agreement]/[!UICONTROL Library Document]/[!UICONTROL User]/[!UICONTROL Widget ID]</td> 
   <td>생성된 레코드를 연결할 객체의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 기타 필드]</td> 
   <td> <p>레코드 유형 및 관련 필드를 기준으로 특정 필드에 정보를 입력합니다.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Agreement]</b> </p> <p>가장 좋은 방법은 계약에 대한 상당한 변경 사항이 예상되는 경우 기존 계약을 업데이트하는 대신 새 계약을 만드는 것입니다.</p> </li> 
     <li> <p><b>[!UICONTROL Library document]</b> </p> <p>업데이트할 필드를 선택한 다음 선택한 필드를 채웁니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL State]</b> </p> <p>라이브러리 문서의 새 상태를 선택합니다.</p> </li> 
       <li> <p><b>[!UICONTROL 참고]</b> </p> <p>메모의 텍스트를 입력하거나 매핑합니다.</p> </li> 
       <li> <p><b>[!UICONTROL Visibility]</b> </p> <p>라이브러리 문서를 표시할지 여부를 선택합니다.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL User]</b> </p> <p>업데이트할 필드를 선택한 다음 선택한 필드를 채웁니다.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL 그룹 정보 목록]</b> </p> <p>다음 필드를 채웁니다</p> 
        <ul> 
         <li> <p><b>[!UICONTROL 상태]</b> </p> <p>사용자의 새 상태를 선택합니다.</p> </li> 
         <li> <p><b>[!UICONTROL ID]</b> </p> <p>그룹의 고유 ID를 입력합니다</p> </li> 
         <li> <p><b>[!UICONTROL은 그룹 관리자입니다.]</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 이 사용자를 그룹 관리자로 만들려면</p> </li> 
         <li> <p><b>기본 그룹입니다.</b> </p> <p>선택 <b>[!UICONTROL Yes]</b> 이 그룹을 사용자의 기본 그룹으로 업데이트하려면</p> </li> 
         <li> <p><b>[!UICONTROL 작성일]</b> </p> <p>그룹을 만든 날짜를 입력합니다.</p> <p>지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Adobe Workfront Fusion]에 강제 입력</a>.</p> </li> 
         <li> <p><b>[!UICONTROL Name]</b> </p> <p>그룹 이름을 입력하거나 매핑합니다.</p> </li> 
         <li> <p><b>[!UICONTROL 라이브러리 문서 작성 표시]</b> </p> <p>이러한 설정은 사용자가 라이브러리 문서를 만들 수 있는지 여부를 결정합니다</p> 
          <ul> 
           <li> <p>[!UICONTROL Value]</p> <p>허용</p> </li> 
           <li> <p>[!UICONTROL 상속]</p> <p>그룹 또는 계정에서 그룹 설정 상속</p> </li> 
          </ul> </li> 
         <li> <p><b>[!UICONTROL 워크플로우로 제한된 보내기]</b> </p> <p>이러한 설정은 사용자가 워크플로우를 사용해서만 계약을 만들 수 있는지 여부를 결정합니다.</p> 
          <ul> 
           <li> <p>[!UICONTROL Value]</p> <p>허용</p> </li> 
           <li> <p>[!UICONTROL 상속]</p> <p>그룹 또는 계정에서 그룹 설정 상속</p> </li> 
          </ul> </li> 
         <li> <p><b>[!UICONTROL 사용자가 전송할 수 있음]</b> </p> 
          <ul> 
           <li> <p>[!UICONTROL Value]</p> <p>허용</p> </li> 
           <li> <p>[!UICONTROL 상속]</p> <p>그룹 또는 계정에서 그룹 설정 상속</p> </li> 
          </ul> </li> 
        </ul> </li> 
      </ul> 
      <ul> 
       <li> <p><b>[!UICONTROL State]</b> </p> <p>사용자의 새 상태를 선택하고 사용자를 활성화하거나 비활성화하려는 이유에 대한 설명을 입력합니다.</p> </li> 
       <li> <p><b>[!UICONTROL 로케일]</b> </p> <p>사용자의 로케일을 입력합니다. UI의 언어를 결정합니다. </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL 웹 양식] ([!UICONTROL 위젯])</b> </p> <p>레코드 유형 및 관련 필드를 기준으로 특정 필드에 정보를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 문서 업로드]**

임시 문서를 업로드합니다. 임시 문서는 업로드한 후 7일 동안 사용할 수 있습니다.

>[!NOTE]
>
>임시 문서로 서명하도록 문서를 업로드한 다음 파일을 파일에 매핑하여 계약 작성 모듈의 필드를 보내는 것이 좋습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Adobe Acrobat Sign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 인증 헤더를 자동으로 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 ID]</td> 
   <td>업데이트할 레코드의 ID를 입력하거나 매핑합니다</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL MIME 유형]</td> 
   <td>원본 파일의 MIME 유형을 입력합니다. MIME(Multipurpose Internet Mail Extension) 유형은 소프트웨어가 인터넷에서 공유되는 서로 다른 유형의 데이터를 식별할 수 있도록 하는 레이블입니다. 웹 서버와 브라우저는 MIME 유형을 사용하여 파일로 수행할 작업을 결정합니다. 예를 들어 MIME 유형을 갖는 파일입니다 <code>text/html</code> 은 MIME 유형을 사용하는 파일과 다르게 브라우저에서 처리됩니다 <code>image/jpeg</code>.</td> 
  </tr> 
 </tbody> 
</table>

**예:** 이 워크플로우에서 서명할 문서(이전에 Workfront에서 다운로드됨)가 임시 문서로 업로드됩니다.

![](assets/sign-example-1-350x308.png)

다음 [!UICONTROL 문서 업로드] 이 모듈은 문서에 [!DNL Adobe Acrobat Sign] 이후 모듈에서 참조할 수 있는 ID입니다. 계약이 만들어지면 업로드된 문서의 ID가 [!UICONTROL 보낼 파일] 필드.

![](assets/sign-example-2-350x356.png)

+++

### 검색 결과

+++ **[!UICONTROL 계약 검색]**

이 검색 모듈은 제공하는 기준에 따라 계약을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Adobe Acrobat Sign] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 텍스트 필터]</td> 
   <td> <p>계약 메타데이터에서 텍스트를 검색합니다. </p> 
    <ul> 
     <li> <p><b>[!UICONTROL 텍스트 찾기]</b> </p> <p>계약 메타데이터에 찾을 텍스트를 입력합니다. 각 단어는 별도의 텍스트 항목으로 처리됩니다. </p> </li> 
     <li> <p><b>[!UICONTROL에서 텍스트 찾기]</b> </p> <p>텍스트를 찾을 메타데이터 필드를 선택합니다. 아무 것도 선택하지 않으면 모듈은 모든 메타데이터를 검색합니다.</p> </li> 
    </ul> <p>이 모듈은 선택한 필드에 입력된 텍스트 중 어느 하나를 포함하는 계약을 반환합니다. 예: "봄 캠페인"을 입력하고 제목 및 참고 옵션을 선택하면 제목 또는 참고에 "봄" 또는 "캠페인"이라는 단어가 포함된 계약이 반환됩니다.</p> <p>의 필드 검색에 대한 자세한 내용은 [!DNL Adobe Acrobat Sign]의 "텍스트 검색 작동 방식"을 참조하십시오. <a href="https://helpx.adobe.com/sign/using/adobesign-search-users-agreements.html#HowSearchWorks">[!DNL Adobe Sign] 검색 - 작동 방법</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작성일]</td> 
   <td>날짜를 선택합니다. 모듈은 생성된 날짜가 이 기준과 일치하는 레코드만 반환합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 만료 날짜]</td> 
   <td>날짜를 선택합니다. 모듈은 만료 날짜가 이 기준과 일치하는 레코드만 반환합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL 수정 날짜]</p> </td> 
   <td>날짜를 선택합니다. 모듈은 수정된 날짜가 이 기준과 일치하는 레코드만 반환합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 외부 ID]</td> 
   <td> <p> 외부 ID는 어떤 형태로든 사용할 수 있지만 일반적으로 " 형태로 계약에 발신자가 할당한 ID입니다&lt;groupid&gt;:&lt;id&gt;".</p> <p>추가할 각 외부 ID에 대해 <b>[!UICONTROL Add]</b> 외부 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 그룹 ID]</td> 
   <td> <p>그룹 ID는 그룹을 만들 때 할당된 식별자입니다.</p> <p>추가할 각 외부 ID에 대해 <b>[!UICONTROL Add]</b> 외부 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>특정 계약에 지정된 ID입니다. </p> <p>추가할 각 외부 ID에 대해 <b>[!UICONTROL Add]</b> 외부 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 상위 ID]</td> 
   <td> <p>계약의 상위 개체에 할당된 ID입니다. </p> <p>추가할 각 외부 ID에 대해 <b>[!UICONTROL Add]</b> 외부 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 참가자 전자 메일]</td> 
   <td> <p>참가자의 이메일 주소입니다. </p> <p>추가할 각 외부 ID에 대해 <b>[!UICONTROL Add]</b> 외부 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 역할]</td> 
   <td>반환된 결과를 포함할 역할을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 정렬 기준]</td> 
   <td>모듈에서 결과를 정렬하려면 결과를 정렬할 필드를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 정렬 순서]r</td> 
   <td>모듈에서 결과를 정렬하려면 오름차순 또는 내림차순으로 정렬할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 상태]</td> 
   <td>반환된 결과를 포함할 상태를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>반환된 결과를 포함할 계약 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subtypes]</td> 
   <td>반환된 결과를 포함할 계약 하위 유형을 선택합니다. 라이브러리 템플릿 계약만 기능 하위 유형을 사용합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User ID]</td> 
   <td> <p>계약이 공유되는 사용자의 사용자 ID입니다.</p> <p>추가할 각 사용자 ID에 대해 <b>[!UICONTROL Add]</b> 사용자 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td>반환된 결과를 포함할 가시성 수준을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시작 인덱스]</td> 
   <td> <p>반환할 첫 번째 결과의 위치를 입력합니다. 이를 [!UICONTROL 최대 반환된 결과]와 결합하여 페이지 매김 결과를 생성합니다</p> <p>예: 한 번에 100개의 결과를 반환하는 경우 100을 입력하여 결과 100-200을 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환된 최대 결과 수]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈을 [action]에 넣을 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++
