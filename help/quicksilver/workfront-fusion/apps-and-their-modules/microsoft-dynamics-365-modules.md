---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오는 Microsoft Dynamics 365를 사용하는 워크플로우를 자동화하고 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1541'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 modules]

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Microsoft Dynamics 365]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

>[!NOTE]
>
>다음 [!DNL Microsoft Dynamics 365] 커넥터가 지원되지 않음 [!DNL Dynamics Finance and Operations].

시나리오 만들기에 대한 지침이 필요한 경우 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

를 사용하려면 [!DNL Microsoft Dynamics] 365에 [!DNL Microsoft Dynamics 365] 계정이 필요합니다.

## Workfront Fusion에 Microsoft Dynamics 365 연결

에 대한 연결을 만들 수 있습니다 [!DNL Microsoft Dynamics 365] 내에서 직접 계정 [!DNL Microsoft Dynamics 365] 모듈.

1. 어떤 경우에서도 [!DNL Microsoft Dynamics 365] 모듈 **[!UICONTROL 추가]** 다음 [!UICONTROL 연결] 필드.
1. 연결의 이름을 입력합니다.
1. 에서 **[!UICONTROL 리소스]** 필드에 주소를 입력합니다 [!DNL Dynamics 365] 계정, 제외 `https://`.
1. 클릭 **[!UICONTROL 계속]** 연결을 만들고 모듈로 돌아갑니다.

>[!NOTE]
>
>등록 시 [!DNL Workfront Fusion] 다음 위치에서 [!DNL Microsoft Azure] 포털에서 다음 리디렉션 URI를 사용하십시오.
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`



## [!DNL Microsoft Dynamics 365] 모듈 및 해당 필드

구성 시 [!DNL Microsoft Dynamics 365] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Microsoft Dynamics 365] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL 감시 레코드(예약됨)]](#watch-records-scheduled)
* [[!UICONTROL 감시 레코드(실시간)]](#watch-records-real-time)
* [[!UICONTROL 레코드 만들기]](#create-record)
* [[!UICONTROL API 호출 만들기]](#make-an-api-call)
* [[!UICONTROL 레코드 삭제]](#delete-record)
* [[!UICONTROL 레코드 읽기]](#read-records)
* [[!UICONTROL 레코드 업데이트]](#update-record)
* [[!UICONTROL 레코드 검색]](#search-records)

### [!UICONTROL 감시 레코드(예약됨)]

이 예약된 트리거 모듈은 지정한 개체의 레코드가 다음에 마지막으로 예약된 실행 후 생성되거나 업데이트되면 시나리오를 실행합니다 [!DNL Dynamics 365].

모듈의 출력은 검색된 레코드가 새 레코드인지 아니면 업데이트되었는지를 나타냅니다(해당 기간에 추가되고 업데이트되었으면 새 레코드로 표시됨). 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 문제는 사용자가 지정하는 정기적으로 예약된 간격에 따라 발생합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결 방법에 대한 지침은 [!DNL Microsoft Dynamics 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> 참조하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include]</td> 
   <td>모듈의 시청 여부를 선택합니다 <strong>[!UICONTROL 새 레코드만]</strong>, <strong>[!UICONTROL 업데이트된 레코드만]</strong>, 또는 <strong>[!UICONTROL 새 레코드 및 모든 변경 내용]</strong>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>시나리오에서 보려는 [!UICONTROL Microsoft Dynamics 365] 레코드 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td> <p>이 모듈의 출력 번들에 포함할 정보를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 최대 레코드]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 감시 레코드(실시간)]

이 인스턴트 트리거 모듈은 지정하는 레코드(개체)가 [!DNL Dynamics 365].

이 모듈에는 웹 후크가 필요합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>이 모듈에 사용할 웹 후크를 선택합니다. </p> <p>새 웹 후크를 추가하려면 다음을 수행합니다.</p> 
    <ol> 
     <li value="1"> <p>클릭 <strong>[!UICONTROL Add]</strong> 웹 후크 필드의 오른쪽에 있습니다.</p> </li> 
     <li value="2"> <p>에서 <strong>[!UICONTROL Webhook]</strong> 이름 필드에 웹 후크를 설명하는 이름을 입력합니다.</p> </li> 
     <li value="3"> <p>에서 <strong>[!UICONTROL Connection]</strong> 필드에서 선택한 연결을 사용할 연결을 선택합니다</p> <p>연결 방법에 대한 지침은 [!DNL Microsoft Dynamics 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> 참조하십시오. </p> </li> 
     <li value="4"> <p>클릭 <strong>[!UICONTROL Save]</strong> 웹 후크를 저장하고 모듈로 돌아가려면 를 클릭합니다.</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 만들기]

이 작업 모듈은 약속 또는 작업과 같은 엔터티를 만듭니다.

만들려는 엔티티에 대한 정보를 지정합니다.

이 모듈은 연결에 액세스하는 사용자 지정 필드 및 값과 함께 새 엔티티 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Microsoft Dynamics 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> 참조하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>모듈에서 생성할 엔티티 유형을 선택합니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 속성 필드]</td> 
   <td>이러한 필드에 지정된 속성에 대해 작업 항목이 가질 값을 입력합니다. 사용 가능한 필드는 엔티티 유형에 따라 다릅니다.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL API 호출 만들기]

이 작업 모듈을 사용하면 [!DNL Microsoft Dynamics 365] API. 이렇게 하면 다른 방식으로 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다 [!DNL Microsoft Dynamics 365] 모듈.

이 모듈은 상태 코드, 헤더 및 본문에 대한 정보를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

자세한 내용은 [!DNL Microsoft] 사용에 대한 설명서 [!DNL Dynamics 365 Customer Engagement Web API].

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결 방법에 대한 지침은 [!DNL Microsoft Dynamics 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> 참조하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>상대 경로 입력 <code>&lt;Instance URL>/api/data/v9.1/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> <p>자세한 내용</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 사용자를 위해 인증 헤더를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p>표준 JSON 개체 형태로 API 호출에 대한 쿼리를 추가합니다.</p> <p>For example: <code>{"name":"something-urgent"}</code></p> </td> 
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

### [!UICONTROL 레코드 삭제]

이 작업 모듈은 엔터티를 삭제합니다.

엔티티의 ID를 지정합니다.

이 모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 엔티티 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결 방법에 대한 지침은 [!DNL Microsoft Dynamics 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> 참조하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td> <p>모듈을 삭제할 엔터티 유형을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>고유 번호를 입력하거나 매핑합니다 [!DNL Microsoft Dynamics 365] 모듈을 삭제할 레코드의 ID입니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 읽기]

이 작업 모듈은 의 단일 엔티티에서 데이터를 읽습니다. [!DNL Microsoft Dynamics 365].

엔티티의 ID를 지정합니다.

이 모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 엔티티 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결 방법에 대한 지침은 [!DNL Microsoft Dynamics 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> 참조하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>모듈을 읽을 엔터티 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td> <p>이 모듈의 출력 번들에 포함할 정보를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>고유 번호를 입력하거나 매핑합니다 [!DNL Microsoft Dynamics 365] 모듈을 읽을 레코드의 ID입니다.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 업데이트]

이 작업 모듈은 엔터티를 업데이트합니다.

엔티티의 ID를 지정합니다.

이 모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 업데이트된 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결 방법에 대한 지침은 [!DNL Microsoft Dynamics 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> 참조하십시오. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>모듈을 업데이트할 엔티티 유형을 선택합니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 속성 필드]</td> 
   <td>이러한 필드에 지정된 속성에 대해 작업 항목이 가질 값을 입력합니다. 사용 가능한 필드는 엔티티 유형에 따라 다릅니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>고유 번호를 입력하거나 매핑합니다 [!DNL Microsoft Dynamics] 모듈을 업데이트할 레코드의 365 ID입니다.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 검색]

이 검색 모듈은 [!DNL Microsoft Dynamics 365] 지정한 검색 쿼리와 일치합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결 방법에 대한 지침은 [!DNL Microsoft Dynamics 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> 참조하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>모듈을 업데이트할 엔티티 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filters]</td> 
   <td> <p>이 검색에 사용할 필터를 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Standard Filters]</strong> </p> <p>필드와 연산자를 선택하고 검색할 값을 입력하거나 매핑하여 필터를 설정합니다. AND 또는 OR 규칙을 사용하여 필터를 만들 수 있습니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 쿼리 함수]</strong> </p> <p>을(를) 입력합니다. [!DNL Dynamics 365] 검색하는 데 사용할 웹 API 쿼리 함수입니다. </p> <p>쿼리 함수에 대한 자세한 내용은 <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">웹 API 쿼리 함수 참조</a> 에서 [!DNL Microsoft] 설명서.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 정렬]</td> 
   <td> <p>항목이 반환되는 순서를 지정합니다. 여러 정렬을 추가할 수 있습니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Field]</strong> </p> <p>결과를 정렬할 필드를 지정합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Direction]</strong> </p> <p>정렬 방향을 지정합니다(오름차순 또는 내림차순).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 최대 레코드]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td> <p>이 모듈의 출력 번들에 포함할 정보를 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
