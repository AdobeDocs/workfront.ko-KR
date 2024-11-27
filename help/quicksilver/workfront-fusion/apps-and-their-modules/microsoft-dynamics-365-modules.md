---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365 모듈
description: ' [!DNL Adobe Workfront Fusion] 시나리오에서는 Microsoft Dynamics 365를 사용하는 워크플로를 자동화할 수 있을 뿐만 아니라 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.'
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: f6b00b98d3375e5660d684f1fad682fa721517aa
workflow-type: tm+mt
source-wordcount: '1733'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 modules]

[!DNL Adobe Workfront Fusion] 시나리오에서는 [!DNL Microsoft Dynamics 365]을(를) 사용하는 워크플로를 자동화하고 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

>[!NOTE]
>
>[!DNL Microsoft Dynamics 365] 커넥터가 [!DNL Dynamics Finance and Operations]을(를) 지원하지 않습니다.
>
>Microsoft Dynamics 365 재무 및 작업 모듈의 경우 [[!DNL Microsoft Dynamics 365 Finance and Operations modules]](/help/quicksilver/workfront-fusion/apps-and-their-modules/dynamics-finance-operations-modules.md)을(를) 참조하십시오.

시나리오를 만드는 방법에 대한 지침이 필요하면 [시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)를 참조하십시오.

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)을 참조하세요.

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
   <p>현재 라이선스 요구 사항: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합을 위한 [!UICONTROL [!DNL Workfront Fusion]] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Adobe Workfront] 플랜이 있는 경우 조직에서 이 문서에 설명된 기능을 사용하려면 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다. [!DNL Workfront Fusion]이(가) [!UICONTROL Ultimate] [!DNL Workfront] 계획에 포함되어 있습니다.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 이 문서에 설명된 기능을 사용하려면 조직에서 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다.</p>
   </td> 
  </tr>
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## 전제 조건

[!DNL Microsoft Dynamics] 365를 사용하려면 [!DNL Microsoft Dynamics 365] 계정이 있어야 합니다.

## Microsoft Dynamics 365를 Workfront Fusion에 연결

[!DNL Microsoft Dynamics 365] 모듈 내에서 직접 [!DNL Microsoft Dynamics 365] 계정에 연결할 수 있습니다.

>[!NOTE]
>
>일부 Microsoft 앱은 개별 사용자 권한에 연결된 동일한 연결을 사용합니다. 따라서 연결을 만들 때 권한 동의 화면에는 현재 애플리케이션에 필요한 새 권한 외에도 이 사용자의 연결에 대해 이전에 부여된 모든 권한이 표시됩니다.
>
>예를 들어 사용자가 Excel 커넥터를 통해 부여된 &quot;테이블 읽기&quot; 권한을 가지고 있는 다음 Outlook 커넥터에서 연결을 만들어 이메일을 읽은 경우 권한 동의 화면에 이미 부여된 &quot;테이블 읽기&quot; 권한과 새로 필요한 &quot;이메일 쓰기&quot; 권한이 모두 표시됩니다.

1. [!DNL Microsoft Dynamics 365] 모듈에서 [!UICONTROL 연결] 필드 옆에 있는 **[!UICONTROL 추가]**&#x200B;를 클릭합니다.
1. 연결의 이름을 입력합니다.
1. **[!UICONTROL 리소스]** 필드에 `https://` 없이 [!DNL Dynamics 365] 계정의 주소를 입력합니다.
1. 연결을 만들고 모듈로 돌아가려면 **[!UICONTROL 계속]**&#x200B;을 클릭하세요.

>[!NOTE]
>
>[!DNL Microsoft Azure] 포털에서 [!DNL Workfront Fusion]을(를) 등록할 때 다음 리디렉션 URI를 사용하십시오.
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`


## [!DNL Microsoft Dynamics 365]개 모듈 및 해당 필드

[!DNL Microsoft Dynamics 365] 모듈을 구성할 때 [!DNL Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 앱 또는 서비스의 액세스 수준과 같은 요소에 따라 이러한 필드와 함께 [!DNL Microsoft Dynamics 365] 필드가 추가로 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

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

이 예약된 트리거 모듈은 지정한 개체의 레코드가 [!DNL Dynamics 365]에서 마지막으로 예약된 실행 이후에 만들어지거나 업데이트될 때 시나리오를 실행합니다.

모듈의 출력은 발견한 레코드가 새로 추가되었는지 또는 업데이트되었는지 여부를 나타냅니다(기간에 추가되고 업데이트된 경우 새로 추가됨으로 표시됨). 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 작업은 사용자가 지정한 정기적으로 예약된 간격으로 발생합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Microsoft Dynamics 365] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">[!DNL Microsoft Dynamics 365]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include]</td> 
   <td>모듈이 <strong>[!UICONTROL 새 레코드만]</strong>, <strong>[!UICONTROL 업데이트된 레코드만]</strong> 또는 <strong>[!UICONTROL 새 레코드와 모든 변경 사항]</strong>을(를) 시청할지 여부를 선택합니다.</td> 
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

이 인스턴트 트리거 모듈은 지정한 레코드(개체)가 [!DNL Dynamics 365]에서 만들어지거나 업데이트될 때 시나리오를 실행합니다.

이 모듈에는 웹후크가 필요합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>이 모듈에 사용할 웹후크를 선택합니다. </p> <p>새 Webhook를 추가하려면</p> 
    <ol> 
     <li value="1"> <p>Webhook 필드 오른쪽에 있는 <strong>[!UICONTROL Add]</strong>을(를) 클릭합니다.</p> </li> 
     <li value="2"> <p><strong>[!UICONTROL Webhook]</strong> 이름 필드에 Webhook를 설명하는 이름을 입력합니다.</p> </li> 
     <li value="3"> <p><strong>[!UICONTROL 연결]</strong> 필드에서 선택한 항목을 사용할 연결을 선택합니다</p> <p>[!DNL Microsoft Dynamics 365] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">[!DNL Microsoft Dynamics 365]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오. </p> </li> 
     <li value="4"> <p>웹후크를 저장하고 모듈로 돌아가려면 <strong>[!UICONTROL 저장]</strong>을(를) 클릭합니다.</p> </li> 
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
   <td> <p>[!DNL Microsoft Dynamics 365] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">[!DNL Microsoft Dynamics 365]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오. </p> </td> 
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

이 작업 모듈을 사용하면 [!DNL Microsoft Dynamics 365] API에 대해 사용자 지정 인증된 호출을 수행할 수 있습니다. 이렇게 하면 다른 [!DNL Microsoft Dynamics 365] 모듈에서 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다.

모듈은 상태 코드, 헤더 및 본문에 대한 정보를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

자세한 내용은 [!DNL Dynamics 365 Customer Engagement Web API] 사용에 대한 [!DNL Microsoft] 설명서를 참조하세요.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Microsoft Dynamics 365] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">[!DNL Microsoft Dynamics 365]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p><code>&lt;Instance URL>/api/data/v9.1/</code>과(와) 관련된 경로를 입력하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 [!DNL Adobe Workfront Fusion]</a>에서 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP 요청 메서드를 참조하십시오.</p> <p>의 추가 정보</p> </td> 
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
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>JSON에서 <code>if</code>과(와) 같은 조건문을 사용할 때 따옴표를 조건문 외부에 넣으십시오.</p> 
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
  <td> <p>[!DNL Microsoft Dynamics 365] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">[!DNL Microsoft Dynamics 365]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 엔티티 유형]</td> 
   <td> <p>모듈에서 삭제할 엔티티 유형을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>모듈에서 삭제할 레코드의 고유 [!DNL Microsoft Dynamics 365] ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 읽기]

이 작업 모듈은 [!DNL Microsoft Dynamics 365]의 단일 엔터티에서 데이터를 읽습니다.

엔티티의 ID를 지정합니다.

모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 엔티티 ID 및 연결된 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Microsoft Dynamics 365] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">[!DNL Microsoft Dynamics 365]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오. </p> </td> 
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
   <td>모듈에서 읽을 레코드의 고유 [!DNL Microsoft Dynamics 365] ID를 입력하거나 매핑합니다.</td> 
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
  <td> <p>[!DNL Microsoft Dynamics 365] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">[!DNL Microsoft Dynamics 365]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오. </p> </td> 
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
   <td>모듈을 업데이트할 레코드의 고유 [!DNL Microsoft Dynamics] 365 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 검색]

이 검색 모듈은 지정한 검색 쿼리와 일치하는 [!DNL Microsoft Dynamics 365]의 개체에서 레코드를 찾습니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Microsoft Dynamics 365] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">[!DNL Microsoft Dynamics 365]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오. </p> </td> 
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
     <li> <p><strong>[!UICONTROL 쿼리 함수]</strong> </p> <p>검색할 [!DNL Dynamics 365] 웹 API 쿼리 함수를 입력하십시오. </p> <p>쿼리 함수에 대한 자세한 내용은 [!DNL Microsoft] 설명서의 <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">웹 API 쿼리 함수 참조</a>를 참조하십시오.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort]</td> 
   <td> <p>항목이 반환되는 순서를 지정합니다. 여러 정렬을 추가할 수 있습니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 필드]</strong> </p> <p>결과를 정렬할 필드를 지정합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 방향]</strong> </p> <p>정렬 방향(오름차순 또는 내림차순)을 지정합니다.</p> </li> 
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
