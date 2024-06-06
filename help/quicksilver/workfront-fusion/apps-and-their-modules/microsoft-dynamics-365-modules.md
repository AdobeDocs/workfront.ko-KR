---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365 모듈
description: 다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 Microsoft Dynamics 365를 사용하는 워크플로를 자동화할 수 있을 뿐만 아니라 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '1724'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 modules]

다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다 [!DNL Microsoft Dynamics 365]을 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

>[!NOTE]
>
>다음 [!DNL Microsoft Dynamics 365] 커넥터가 지원되지 않음 [!DNL Dynamics Finance and Operations].

시나리오를 만드는 방법에 대한 지침이 필요한 경우 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

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

사용 [!DNL Microsoft Dynamics] 365, 다음 항목이 있어야 합니다. [!DNL Microsoft Dynamics 365] 계정입니다.

## Microsoft Dynamics 365를 Workfront Fusion에 연결

에 대한 연결을 만들 수 있습니다. [!DNL Microsoft Dynamics 365] 내에서 직접 계정 [!DNL Microsoft Dynamics 365] 모듈.

>[!NOTE]
>
>일부 Microsoft 앱은 개별 사용자 권한에 연결된 동일한 연결을 사용합니다. 따라서 연결을 만들 때 권한 동의 화면에는 현재 애플리케이션에 필요한 새 권한 외에도 이 사용자의 연결에 대해 이전에 부여된 모든 권한이 표시됩니다.
>
>예를 들어 사용자가 Excel 커넥터를 통해 부여된 &quot;테이블 읽기&quot; 권한을 가지고 있는 다음 Outlook 커넥터에서 연결을 만들어 이메일을 읽은 경우 권한 동의 화면에 이미 부여된 &quot;테이블 읽기&quot; 권한과 새로 필요한 &quot;이메일 쓰기&quot; 권한이 모두 표시됩니다.

1. 다음 중 하나 [!DNL Microsoft Dynamics 365] 모듈, 클릭 **[!UICONTROL 추가]** 다음 옆에 [!UICONTROL 연결] 필드.
1. 연결의 이름을 입력합니다.
1. 다음에서 **[!UICONTROL 리소스]** 필드에 주소를 입력합니다. [!DNL Dynamics 365] 계정, 없음 `https://`.
1. 클릭 **[!UICONTROL 계속]** 를 클릭하여 연결을 만들고 모듈로 돌아갑니다.

>[!NOTE]
>
>등록 시 [!DNL Workfront Fusion] (으)로 [!DNL Microsoft Azure] 포털에서 다음 리디렉션 URI를 사용하십시오.
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`


## [!DNL Microsoft Dynamics 365] 모듈 및 해당 필드

를 구성할 때 [!DNL Microsoft Dynamics 365] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Microsoft Dynamics 365] 앱이나 서비스의 액세스 수준 등에 따라 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL 레코드 보기(예약됨)]](#watch-records-scheduled)
* [[!UICONTROL 레코드 보기(실시간)]](#watch-records-real-time)
* [[!UICONTROL 레코드 만들기]](#create-record)
* [[!UICONTROL API 호출 만들기]](#make-an-api-call)
* [[!UICONTROL 레코드 삭제]](#delete-record)
* [[!UICONTROL 레코드 읽기]](#read-records)
* [[!UICONTROL 레코드 업데이트]](#update-record)
* [[!UICONTROL 레코드 검색]](#search-records)

### [!UICONTROL 레코드 보기(예약됨)]

이 예약된 트리거 모듈은 지정한 개체의 레코드가 마지막 예약된 실행 이후에 만들어지거나 업데이트될 때 시나리오를 실행합니다 [!DNL Dynamics 365].

모듈의 출력은 발견한 레코드가 새로 추가되었는지 또는 업데이트되었는지 여부를 나타냅니다(기간에 추가되고 업데이트된 경우 새로 추가됨으로 표시됨). 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 작업은 사용자가 지정한 정기적으로 예약된 간격으로 발생합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결에 대한 자세한 내용 [!DNL Microsoft Dynamics 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">연결 [!DNL Microsoft Dynamics 365] 끝 [!DNL Workfront Fusion]</a> 이 문서에서. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include]</td> 
   <td>모듈을 감시할지 여부를 선택합니다. <strong>[!UICONTROL 새 레코드만]</strong>, <strong>[!UICONTROL 업데이트된 레코드만]</strong>, 또는 <strong>[!UICONTROL 새 레코드 및 모든 변경 사항]</strong>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 엔티티 유형]</td> 
   <td>시나리오에서 보려는 [!UICONTROL Microsoft Dynamics 365] 레코드 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td> <p>이 모듈에 대한 출력 번들에 포함할 정보를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 최대 레코드]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 보기(실시간)]

이 인스턴스 트리거 모듈은에서 지정한 레코드(개체)가 만들어지거나 업데이트될 때 시나리오를 실행합니다 [!DNL Dynamics 365].

이 모듈에는 웹후크가 필요합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>이 모듈에 사용할 웹후크를 선택합니다. </p> <p>새 Webhook를 추가하려면</p> 
    <ol> 
     <li value="1"> <p>클릭 <strong>[!UICONTROL 추가]</strong> Webhook 필드의 오른쪽</p> </li> 
     <li value="2"> <p>다음에서 <strong>[!UICONTROL Webhook]</strong> 이름 필드에 webhook의 수사적 이름을 입력합니다.</p> </li> 
     <li value="3"> <p>다음에서 <strong>[!UICONTROL Connection]</strong> 필드에서 선택한 연결에 사용할 연결을 선택합니다</p> <p>연결에 대한 자세한 내용 [!DNL Microsoft Dynamics 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">연결 [!DNL Microsoft Dynamics 365] 끝 [!DNL Workfront Fusion]</a> 이 문서에서. </p> </li> 
     <li value="4"> <p>클릭 <strong>[!UICONTROL 저장]</strong> 을 클릭하여 webhook을 저장하고 모듈로 돌아갑니다.</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 만들기]

이 작업 모듈은 약속 또는 작업과 같은 엔터티를 만듭니다.

생성할 엔티티에 대한 정보를 지정합니다.

모듈은 새 엔티티의 ID 및 연결된 필드와 연결이 액세스하는 모든 사용자 지정 필드 및 값을 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Microsoft Dynamics 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">연결 [!DNL Microsoft Dynamics 365] 끝 [!DNL Workfront Fusion]</a> 이 문서에서. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 엔티티 유형]</td> 
   <td>모듈에서 만들 엔티티 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 매핑할 필드 선택]</td> 
   <td>레코드를 만들 때 값을 포함할 필드를 선택합니다. 사용 가능한 필드는 엔티티 유형에 따라 다릅니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 속성 필드]</td> 
   <td> 선택한 필드입니다. 주어진 속성에 대해 레코드에 보유할 값을 입력합니다. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL API 호출 만들기]

이 작업 모듈에서는 다음을 위한 사용자 지정 인증 호출을 만들 수 있습니다. [!DNL Microsoft Dynamics 365] API. 이렇게 하면 다른 사용자가 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다 [!DNL Microsoft Dynamics 365] 모듈.

모듈은 상태 코드, 헤더 및 본문에 대한 정보를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

자세한 내용은 [!DNL Microsoft] 사용 방법에 대한 설명서 [!DNL Dynamics 365 Customer Engagement Web API].

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결에 대한 자세한 내용 [!DNL Microsoft Dynamics 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">연결 [!DNL Microsoft Dynamics 365] 끝 [!DNL Workfront Fusion]</a> 이 문서에서. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>상대 경로 입력 <code>&lt;Instance URL>/api/data/v9.1/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> <p>의 추가 정보</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>표준 JSON 개체 형태로 요청의 헤더를 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 인증 헤더를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p>표준 JSON 개체 형식으로 API 호출에 대한 쿼리를 추가합니다.</p> <p>For example: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>다음과 같은 조건문을 사용할 때 <code>if</code> json에서 따옴표를 조건문 외부에 넣습니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 삭제]

이 작업 모듈은 엔티티를 삭제합니다.

엔티티의 ID를 지정합니다.

모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 엔티티 ID 및 연결된 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결에 대한 자세한 내용 [!DNL Microsoft Dynamics 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">연결 [!DNL Microsoft Dynamics 365] 끝 [!DNL Workfront Fusion]</a> 이 문서에서. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 엔티티 유형]</td> 
   <td> <p>모듈에서 삭제할 엔티티 유형을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>고유 항목 입력 또는 매핑 [!DNL Microsoft Dynamics 365] 모듈에서 삭제할 레코드의 ID입니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 읽기]

이 작업 모듈은 의 단일 엔티티에서 데이터를 읽습니다. [!DNL Microsoft Dynamics 365].

엔티티의 ID를 지정합니다.

모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 엔티티 ID 및 연결된 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결에 대한 자세한 내용 [!DNL Microsoft Dynamics 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">연결 [!DNL Microsoft Dynamics 365] 끝 [!DNL Workfront Fusion]</a> 이 문서에서. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 엔티티 유형]</td> 
   <td>모듈에서 읽을 엔티티 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td> <p>이 모듈에 대한 출력 번들에 포함할 정보를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>고유 항목 입력 또는 매핑 [!DNL Microsoft Dynamics 365] 모듈에서 읽을 레코드의 ID입니다.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 업데이트]

이 작업 모듈은 엔티티를 업데이트합니다.

엔티티의 ID를 지정합니다.

모듈은 업데이트된 레코드의 ID 및 연결된 필드와 연결이 액세스하는 모든 사용자 지정 필드 및 값을 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결에 대한 자세한 내용 [!DNL Microsoft Dynamics 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">연결 [!DNL Microsoft Dynamics 365] 끝 [!DNL Workfront Fusion]</a> 이 문서에서. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 엔티티 유형]</td> 
   <td>모듈을 업데이트할 엔티티 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 매핑할 필드 선택]</td> 
   <td>레코드를 만들 때 값을 포함할 필드를 선택합니다. 사용 가능한 필드는 엔티티 유형에 따라 다릅니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 속성 필드]</td> 
   <td>선택된 필드입니다. 주어진 속성에 대해 레코드에 보유할 값을 입력합니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>고유 항목 입력 또는 매핑 [!DNL Microsoft Dynamics] 모듈이 업데이트하려는 레코드의 365 ID.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 검색]

이 검색 모듈은 의 개체에서 레코드를 찾습니다. [!DNL Microsoft Dynamics 365] 지정한 검색 쿼리와 일치하는 쿼리입니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>연결에 대한 자세한 내용 [!DNL Microsoft Dynamics 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">연결 [!DNL Microsoft Dynamics 365] 끝 [!DNL Workfront Fusion]</a> 이 문서에서. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 엔티티 유형]</td> 
   <td>모듈을 업데이트할 엔티티 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filters]</td> 
   <td> <p>이 검색에 사용할 필터를 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 표준 필터]</strong> </p> <p>필드 및 연산자를 선택하고 검색할 값을 입력하거나 매핑하여 필터를 설정합니다. 필터에 AND 또는 OR 규칙을 사용할 수 있습니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 쿼리 함수]</strong> </p> <p>다음을 입력합니다. [!DNL Dynamics 365] 검색하는 데 사용할 웹 API 쿼리 함수입니다. </p> <p>쿼리 함수에 대한 자세한 내용은 <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">웹 API 쿼리 함수 참조</a> 다음에서 [!DNL Microsoft] 설명서를 참조하십시오.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort]</td> 
   <td> <p>항목이 반환되는 순서를 지정합니다. 여러 정렬을 추가할 수 있습니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 필드]</strong> </p> <p>결과를 정렬할 필드를 지정합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Direction]</strong> </p> <p>정렬 방향(오름차순 또는 내림차순)을 지정합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 최대 레코드]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td> <p>이 모듈에 대한 출력 번들에 포함할 정보를 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
