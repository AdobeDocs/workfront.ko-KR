---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Salesforce 모듈
description: Adobe Workfront Fusion 시나리오에서는 Salesforce를 사용하는 워크플로를 자동화할 뿐만 아니라 이를 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '2740'
ht-degree: 0%

---

# [!DNL Salesforce] 모듈

Adobe Workfront Fusion 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다. [!DNL Salesforce]을 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

Salesforce 커넥터에 대한 비디오 소개는 다음을 참조하십시오.

* [Salesforce](https://video.tv.adobe.com/v/3427027/){target=_blank}

시나리오를 만드는 방법에 대한 지침이 필요한 경우 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* 의 일부 에디션 [!DNL Salesforce] api 액세스 권한이 있습니다. 자세한 내용은 다음에 대한 정보를 참조하십시오. [!DNL Salesforce] 의 API 액세스 권한이 있는 버전 [!DNL Salesforce] 커뮤니티 사이트.
>* 에서 반환된 특정 오류에 대한 자세한 내용은 [!DNL Salesforce] API에서 다음을 참조하십시오. [!DNL Salesforce] API 문서. 또한 의 상태를 확인할 수도 있습니다. [!DNL Salesforce] 가능한 서비스 중단에 대한 API입니다.
>

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

사용 [!DNL Salesforce] 모듈, 다음이 있어야 합니다. [!DNL Salesforce] 계정입니다.

## 검색 기본 정보 [!DNL Salesforce] 오브젝트

객체를 검색할 때 개별 검색어를 입력하거나 와일드카드 및 연산자를 사용하여 보다 복잡한 질의를 생성할 수 있습니다.

* 별표 와일드카드(\*)를 0개 이상의 문자 대용으로 사용합니다. 예를 들어 Ca\*를 검색하면 Ca로 시작하는 항목이 검색됩니다
* 물음표 와일드카드(?) 사용 단일 문자의 대용품입니다. 예를 들어 Jo?n을 검색하면 John 또는 Joan이라는 용어가 있지만 Jon은 아닌 항목이 검색됩니다
* 따옴표 연산자(&quot; &quot;)를 사용하여 정확한 구문 일치를 찾습니다. 예: &quot;Monday meeting&quot;

검색 가능성에 대한 자세한 내용은 [!DNL Salesforce] soql 및 SOSL에 대한 개발자 설명서.

## [!DNL Salesforce] 모듈 및 해당 필드

* [트리거](#triggers)
* [작업](#actions)
* [검색 결과](#searches)

### 트리거

* [[!UICONTROL 기록 감시]](#watch-for-records)
* [[!UICONTROL 아웃바운드 메시지 보기]](#watch-outbound-messages)
* [[!UICONTROL 필드 보기]](#watch-a-field)

#### [!UICONTROL 기록 감시]

이 트리거 모듈은 오브젝트 내의 레코드가 생성되거나 업데이트될 때 시나리오를 실행한다. 모듈은 연결에서 액세스하는 모든 사용자 지정 필드 및 값과 함께 레코드 또는 레코드와 연결된 모든 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Salesforce] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 유형] </td> 
   <td> <p>유형 선택 [!DNL Salesforce] 모듈에서 볼 녹화를 하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 레코드 필드]</td> 
   <td>모듈에서 조사할 필드를 선택합니다. 사용 가능한 필드는 레코드 유형에 따라 다릅니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 레코드의 최대 개수]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p>선택한 유형의 새 레코드만 시나리오에 표시할지, 선택한 유형의 새 레코드와 해당 유형의 다른 모든 레코드 변경 사항을 시나리오에 표시할지 여부를 결정합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 아웃바운드 메시지 보기]

이 트리거 모듈은 누군가가 메시지를 보낼 때 시나리오를 실행합니다. 모듈은 연결에서 액세스하는 모든 사용자 지정 필드 및 값과 함께 레코드 또는 레코드와 연결된 모든 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈에는 추가 설정이 필요합니다.

1. 로 이동 [!DNL Salesforce] 설정 페이지입니다.

   설정 페이지에 액세스하려면 버튼(&quot;)을 찾아 클릭하십시오.[!UICONTROL 설정]의 오른쪽 위 모서리에 있는 &quot; [!DNL Salesforce] 계정입니다. 다음에서 [!DNL Salesforce] 설정 페이지에서 &quot;[!UICONTROL 빠른 찾기/검색]왼쪽의 바. 검색 대상[!UICONTROL 워크플로 규칙].&quot;

1. 클릭 **[!UICONTROL 워크플로 규칙]**.
1. 다음에서 [!UICONTROL 워크플로 규칙] 페이지가 나타나면 **[!UICONTROL 새 규칙]** 규칙을 적용할 객체 유형을 선택합니다(예: &quot;[!UICONTROL 영업 기회]&quot; Opportunity 레코드에 대한 업데이트를 모니터링하는 경우 ).
1. 클릭 **[!UICONTROL 다음]**.
1. 규칙 이름, 평가 기준 및 규칙 기준을 설정한 다음 **[!UICONTROL 저장]** 및 **[!UICONTROL 다음]**.

1. 클릭 **[!UICONTROL 완료]**.
1. 새로 만든 워크플로우 규칙에서 **[!UICONTROL 편집]**..
1. 다음에서 **[!UICONTROL 워크플로우 작업 추가]** 드롭다운 목록에서 다음을 선택합니다. **[!UICONTROL 새 아웃바운드 메시지]**.

1. 새 아웃바운드 메시지에 포함할 이름, 설명, 끝점 URL 및 필드를 지정한 다음, **[!UICONTROL 저장]**.

   다음 **[!UICONTROL 끝점 URL]** 필드에는에 제공된 URL이 포함되어 있습니다. [!DNL Salesforce] [!UICONTROL 아웃바운드 메시지] 위치: [!DNL Workfront Fusion].

1. 다음으로 시작하는 시나리오 구성 [!UICONTROL 아웃바운드 메시지] 이벤트.

1. 다음을 클릭합니다. **&lt;/>** 오른쪽 하단에 있는 아이콘을 클릭하고 제공된 URL을 복사합니다.
1. (으)로 돌아가기 **[!UICONTROL 워크플로 규칙]** 페이지에서 새로 만든 규칙을 찾은 다음 **[!UICONTROL 활성화]**.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td> <p>보내는 메시지를 보는 데 사용할 웹후크를 선택합니다. 웹후크를 추가하려면 <strong>[!UICONTROL 추가]</strong> webhook의 이름과 연결을 입력합니다.</p> <p>연결에 대한 자세한 내용 [!DNL Salesforce] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Adobe Workfront Fusion]에 대한 연결 만들기 - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 레코드 유형] </td> 
   <td> <p>유형 선택 [!DNL Salesforce] 모듈에서 보내는 메시지를 감시할 녹화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 필드]</td> 
   <td> <p>모듈에서 보내는 메시지를 확인할 필드를 선택합니다. 사용 가능한 필드는 레코드 유형에 따라 다릅니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL 필드 보기]*

이 트리거 모듈은에서 필드가 업데이트될 때 시나리오를 시작합니다. [!DNL Salesforce].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Salesforce] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 레코드 유형] </td> 
   <td> <p>모듈에서 조사할 필드가 포함된 레코드 유형을 선택합니다. [!UICONTROL 필드 기록]이 설정된 레코드 종류를 선택해야 합니다. [!DNL Salesforce] 설정. 자세한 내용은 <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">필드 내역 추적</a> 다음에서 [!DNL Salesforce] 설명서를 참조하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 필드]</td> 
   <td> <p>모듈에서 변경 사항을 감시할 필드를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 필드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 레코드 만들기]](#create-a-record)
* [[!UICONTROL 레코드 읽기]](#read-a-record)
* [[!UICONTROL 레코드 삭제]](#delete-a-record)
* [[!UICONTROL 사용자 정의 API 호출]](#custom-api-call)
* [[!UICONTROL 첨부 파일/문서 업로드]](#upload-attachmentdocument)
* [[!UICONTROL 첨부 파일/문서 다운로드]](#download-attachmentdocument)

#### [!UICONTROL 레코드 만들기]

이 작업 모듈은 개체에 새 레코드를 만듭니다.

모듈을 사용하면 모듈에서 사용할 수 있는 개체 필드를 선택할 수 있습니다. 이렇게 하면 모듈을 설정할 때 스크롤해야 하는 필드의 수가 줄어듭니다.

모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Salesforce] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 레코드 유형] </p> </td> 
   <td> <p>유형 선택 [!DNL Salesforce] 모듈에서 만들 레코드를 기록합니다. 필드는 [!UICONTROL 레코드 유형] 필드에서 선택한 레코드 유형에 따라 사용할 수 있습니다. 이러한 필드는 [!DNL Salesforce] API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 매핑할 필드 선택]</td> 
   <td> <p>새 레코드를 만들 때 모듈에서 구성할 필드를 선택합니다. 필수 필드는 목록의 맨 위에 있습니다. </p> <p>선택한 필드는 이 필드 아래에 열립니다. 이제 이러한 필드에 값을 입력할 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 읽기]

이 작업 모듈은 의 단일 개체에서 데이터를 읽습니다. [!DNL Salesforce].

레코드의 ID를 지정합니다.

모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Salesforce] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL 레코드 유형]</td>
    <td>유형 선택 [!DNL Salesforce] 모듈을 [action].read로 기록하십시오.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 레코드 필드]</td>
    <td>모듈에서 읽을 필드를 선택합니다. 필드를 하나 이상 선택해야 합니다.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL ID]</td>
    <td> <p>고유 항목 입력 또는 매핑 [!DNL Salesforce] 모듈에서 읽을 레코드의 ID입니다.</p> <p>ID를 가져오려면 [!DNL Salesforce] 를 클릭하고 마지막 슬래시(/) 뒤의 URL 끝에 있는 텍스트를 복사합니다. For example: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 삭제]

이 작업 모듈은 오브젝트의 기존 레코드를 삭제합니다.

레코드의 ID를 지정합니다.

모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Salesforce] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 레코드 유형] </td> 
   <td> <p>유형 선택 [!DNL Salesforce] 모듈에서 삭제할 레코드를 기록합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>고유 항목 입력 또는 매핑 [!DNL Salesforce] 모듈에서 삭제할 레코드의 ID입니다.</p> <p>ID를 가져오려면 [!DNL Salesforce] 를 클릭하고 마지막 슬래시(/) 뒤의 URL 끝에 있는 텍스트를 복사합니다. For example: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 사용자 정의 API 호출]

이 작업 모듈에서는 다음을 위한 사용자 지정 인증 호출을 만들 수 있습니다. [!DNL Salesforce] API. 이렇게 하면 다른 사용자가 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다 [!DNL Salesforce] 모듈.

모듈은 다음을 반환합니다.

* **[!UICONTROL 상태 코드]** (숫자): HTTP 요청의 성공 또는 실패를 나타냅니다. 이것은 인터넷에서 찾아볼 수 있는 표준 코드입니다.
* **[!UICONTROL 헤더]** (개체): 출력 본문과 관련이 없는 응답/상태 코드에 대한 보다 자세한 컨텍스트입니다. 응답 헤더에 표시되는 일부 헤더가 응답 헤더는 아니므로 유용하지 않을 수 있습니다.

  응답 헤더는 모듈을 구성할 때 선택한 HTTP 요청에 따라 다릅니다.

* **[!UICONTROL 본문]** (개체): 모듈을 구성할 때 선택한 HTTP 요청에 따라 일부 데이터를 다시 받을 수 있습니다. 해당 데이터(예: 의 데이터) [!UICONTROL GET] request가 이 개체에 포함되어 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Salesforce] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>상대 경로 입력<code> &lt;Instance URL&gt;/services/data/v46.0/</code>.</p> <p>사용 가능한 엔드포인트 목록은 <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Salesforce REST API 개발자 안내서</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 메서드]</p> </td> 
   td&gt; <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>표준 JSON 개체 형식으로 요청의 헤더를 추가합니다.예: <code>{"Content-type":"application/json"}</code>. Workfront Fusion은 사용자에게 권한 부여 헤더를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p>표준 JSON 개체의 형식으로 API 호출에 대한 쿼리를 추가합니다.예: <code>{"name":"something-urgent"}</code></p> </td> 
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

>[!INFO]
>
>**예:** 다음 API 호출은 의 모든 사용자 목록을 [!DNL Salesforce] 계정:
>
>* **URL**: `query`
>
>* **방법**: [!UICONTROL GET]
>
>* **쿼리 문자열**:
>
>* **키**: `q`
>
>* **값**: `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>검색 일치 항목은 아래의 모듈 출력에서 찾을 수 있습니다. **[!UICONTROL 번들] > [!UICONTROL 본문] > [!UICONTROL 레코드]**.
>
>이 예에서는 6명의 사용자가 반환되었습니다.
>
>![](assets/matches-of-the-search-350x573.png)


#### [!UICONTROL 첨부 파일/문서 업로드]

이 작업 모듈은 파일을 업로드하여 지정한 레코드에 첨부하거나 문서를 업로드합니다.

모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 첨부 파일 또는 문서의 ID와 관련 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Salesforce] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 업로드 유형]</td> 
   <td>모듈에서 첨부 파일을 업로드할지 문서를 업로드할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>첨부 파일을 업로드할 오브젝트의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더]</td> 
   <td>모듈을 업로드할 파일이 포함된 폴더를 선택합니다. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 소스 파일]</td> 
   <td>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 첨부 파일/문서 다운로드]

이 작업 모듈은 레코드에서 문서 또는 첨부 파일을 다운로드합니다.

레코드의 ID와 원하는 다운로드 유형을 지정합니다.

모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 첨부 파일 또는 문서의 ID와 관련 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Salesforce] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL 다운로드 유형]</td>
    <td> <p>Salesforce에서 다운로드할 파일 유형을 지정합니다.</p> 
     <ul> 
      <li>[!UICONTROL 첨부 파일]</li> 
      <li>[!UICONTROL 문서]</li> 
      <li>[!UICONTROL ContentDocument](의 라이브러리에 업로드된 문서임) [!DNL Saleforce CRM Content] 또는 [!DNL Salesforce Files].)</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[!UICONTROL ID] / </p> <p>[!UICONTROL 첨부 파일 ID] / </p> <p>[!UICONTROL ContentDocument ID]</p> </td>
    <td> <p>고유 항목 입력 또는 매핑 [!DNL Salesforce] 모듈을 다운로드할 레코드의 ID입니다.</p> <p>ID를 가져오려면 [!DNL Salesforce] 를 클릭하고 마지막 슬래시(/) 뒤의 URL 끝에 있는 텍스트를 복사합니다. For example: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 레코드 업데이트]

이 작업 모듈은 오브젝트의 레코드를 편집합니다.

모듈을 사용하면 모듈에서 사용할 수 있는 개체 필드를 선택할 수 있습니다. 이렇게 하면 모듈을 설정할 때 스크롤해야 하는 필드의 수가 줄어듭니다.

모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Salesforce] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>업데이트할 레코드의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 레코드 유형] </p> </td> 
   <td> <p>유형 선택 [!DNL Salesforce] 모듈을 업데이트할 레코드입니다. 필드는 레코드 유형 필드에서 선택한 레코드 유형에 따라 사용할 수 있습니다. 이러한 필드는 [!DNL Salesforce] API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 매핑할 필드 선택]</td> 
   <td> <p>새 레코드를 만들 때 모듈에서 구성할 필드를 선택합니다. 필수 필드는 목록의 맨 위에 있습니다. </p> <p>선택한 필드는 이 필드 아래에 열립니다. 이제 이러한 필드에 값을 입력할 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 검색 결과

#### [!UICONTROL 쿼리를 사용하여 검색]

이 검색 모듈은 의 개체에서 레코드를 찾습니다. [!DNL Salesforce] 지정한 검색 쿼리와 일치하는 쿼리입니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Salesforce] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 검색 유형]</td> 
   <td> <p>모듈에서 수행할 검색 유형을 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL Simple]</p> </li> 
     <li> <p>[!UICONTROL Using SOSL (Salesforce Object Search Language)]</p> </li> 
     <li> <p>[!UICONTROL Using SOQL(Salesforce 개체 쿼리 언어)]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 유형] </p> </td> 
   <td> <p>단순 검색 유형을 선택한 경우 다음 유형을 선택합니다. [!DNL Salesforce] 모듈에서 검색할 레코드를 기록합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query] / [!UICONTROL SOSL Query] / [!UICONTROL SOQL Query]</td> 
   <td> <p>검색할 쿼리를 입력합니다.</p> <p>SOSL에 대한 자세한 내용은 <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Salesforce 개체 검색 언어(SOSL)</a> 다음에서 [!DNL Salesforce] 설명서를 참조하십시오.</p> <p>SOQL에 대한 자세한 내용은 <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Salesforce 개체 쿼리 언어(SOQL)</a> 다음에서 [!DNL Salesforce] 설명서를 참조하십시오.</p> <p>참고: 매개 변수의 값을 참고하십시오 <code>RETURNING </code>는 모듈의 출력에 영향을 줍니다. 를 사용하는 경우 <code>LIMIT</code>, [!DNL Fusion] 은(는) [!UICONTROL 최대 레코드 수] 필드의 설정을 무시합니다. 제한을 설정하지 않으면 [!UICONTROL LIMIT = 최대 레코드 수] 값이 삽입됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 레코드의 최대 개수]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 검색]

이 작업 모듈은 지정된 조건을 충족하는 모든 레코드를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결에 대한 자세한 내용 [!DNL Salesforce] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기[!DNL  Adobe Workfront Fusion] - 기본 지침</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 유형]</td> 
   <td> <p>검색할 객체 유형을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 검색 기준]</td> 
   <td>검색할 필드, 쿼리에 사용할 연산자 및 필드에서 검색할 값을 선택합니다. AND 또는 OR를 사용하여 쿼리를 연결할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>모듈의 출력에 포함할 필드를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 결과 집합]</td> 
   <td>모듈이 모든 일치 레코드를 반환할지, 첫 번째 일치 레코드만 반환할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximal]</td> 
   <td>각 시나리오 실행 주기 동안 모듈이 검색할 최대 레코드 수를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>
