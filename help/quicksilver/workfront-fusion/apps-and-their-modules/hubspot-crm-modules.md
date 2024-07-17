---
title: HubSpot CRM 모듈
description: ' [!DNL Adobe Workfront Fusion] HubSpot CRM 모듈을 사용하면 이벤트, 레코드, 연락처, 참여, 파일 및 양식 제출을 모니터링하거나  [!DNL HubSpot CRM] 계정의 레코드, 연락처, 참여, 이벤트 또는 파일을 만들고, 검색하고, 업데이트하고, 삭제할 수 있습니다.'
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: 1c56cf8aa9da7ec2644955d5533c71f60160d580
workflow-type: tm+mt
source-wordcount: '2615'
ht-degree: 0%

---

# [!DNL HubSpot CRM]개 모듈

[!DNL Adobe Workfront Fusion] [!DNL HubSpot CRM] 모듈을 사용하면 이벤트, 레코드, 연락처, 참여, 파일 및 양식 제출을 모니터링하거나 [!DNL HubSpot CRM] 계정의 레코드, 연락처, 참여, 이벤트 또는 파일을 만들고, 검색하고, 업데이트하고, 삭제할 수 있습니다.

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

[!DNL HubSpot CRM] 모듈을 사용하려면 [!DNL HubSpot CRM] 계정이 있어야 합니다.

## [!DNL Adobe Workfront Fusion]을(를) [!DNL HubSpot CRM]에 연결

[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 [연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침](../../workfront-fusion/connections/connect-to-fusion-general.md)을 참조하세요.

>[!NOTE]
>
>연결을 구성할 때 **HubSpot CRM** 연결 유형을 선택하십시오. HubSpot CRM(더 이상 사용되지 않음) 유형은 기존 연결을 지원하지만 새 연결을 만들 때는 사용하지 않는 것이 좋습니다.

## [!DNL HubSpot CRM]개 모듈 및 해당 필드

[!DNL Hubspot CRM] 모듈을 구성할 때 [!DNL Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 앱 또는 서비스의 액세스 수준과 같은 요소에 따라 이러한 필드와 함께 [!DNL Hubspot CRM] 필드가 추가로 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

![](assets/map-toggle-350x74.png)

* [CRM 오브젝트](#crm-objects)
* [기록(거래, 연락처 및 회사)](#records-deals-contacts-and-companies)
* [연락처](#contacts)
* [거래](#deals)
* [회사](#companies)
* [파일](#files)
* [티켓](#tickets)
* [API 호출 만들기](#make-an-api-call)

### CRM 오브젝트

#### [!UICONTROL CRM 개체 검색]

이 검색 모듈은 사용자 지정 속성 또는 쿼리별로 CRM 개체를 검색합니다. 제품 또는 라인 항목을 검색하려면 필수 사용자 지정 범위의 특수 연결을 사용하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td>한 실행 주기에서 모듈이 반환할 최대 항목 수를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 검색할 오브젝트 유형]</td> 
   <td>검색할 Hubspot CRM 개체의 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력 속성]</td> 
   <td>모듈의 출력에 표시할 속성을 선택합니다. 사용 가능한 필드는 선택한 개체에 따라 다릅니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 필터 기준] </td> 
   <td> <p>검색 필터링 방법 선택</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 쿼리]</strong> </p> <p>쿼리 입력 또는 매핑</p> </li> 
     <li> <p><strong>[!UICONTROL 속성]</strong> </p> <p>검색할 그룹 또는 필터를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 정렬 기준]</td> 
   <td> <p>결과를 정렬하려면 을 클릭합니다. 결과 정렬을 선택하면 다음 필드가 나타납니다. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 속성 이름]</strong> </p> <p>결과를 정렬할 속성 선택</p> </li> 
     <li> <p><strong>[!UICONTROL 방향]</strong> </p> <p>결과를 오름차순으로 정렬할지 아니면 내림차순으로 정렬할지 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Start Offset</td> 
    <td>Enter or map the ID of the first item you want to retrieve details for. This module only returns up to 5000 results at a time. Setting a start offset allows you to retrieve items other than the first 5000. If the start offset is 5000, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

### 기록(거래, 연락처 및 회사)

* [[!UICONTROL 레코드 만들기(레거시)]](#create-a-record-legacy)
* [[!UICONTROL 레코드 가져오기]](#get-a-record)
* [[!UICONTROL 레코드 업데이트]](#update-a-record)
* [[!UICONTROL 레코드 삭제]](#delete-a-record)
* [[!UICONTROL 레코드 속성 가져오기]](#get-a-record-property)
* [[!UICONTROL 레코드 보기]](#watch-records)

#### [!UICONTROL 레코드 만들기(레거시)]

이 작업 모듈은 연락처, 회사 또는 거래를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>만들려는 레코드 종류 선택</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 속성]</td> 
   <td>레코드에 설정할 속성을 입력합니다. 사용 가능한 필드는 만들려는 레코드 유형에 따라 다릅니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 가져오기]

이 작업 모듈은 연락처, 회사 또는 거래의 세부 정보를 가져옵니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>레코드 유형을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL 연락처]</li> 
     <li>[!UICONTROL Company] </li> 
     <li>[!UICONTROL Deal]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 검색 유형]</td> 
   <td>연락처를 받는 경우 ID로 식별할지 이메일 주소로 식별할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>검색할 연락처, 회사 또는 거래의 ID를 입력합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>세부 정보를 검색할 연락처의 이메일 주소를 입력합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 업데이트]

이 작업 모듈은 연락처, 회사 또는 거래를 업데이트합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td>업데이트할 레코드 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 검색 유형]</td> 
   <td> <p>연락처를 받는 경우 레코드를 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL ID]</p> </li> 
     <li> <p>[!UICONTROL Email]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>업데이트하려는 연락처, 회사 또는 거래의 ID를 입력합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>상세내역을 갱신할 담당자의 전자 메일 주소를 입력합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 속성]</td> 
   <td>레코드에 설정할 속성을 입력합니다. 사용 가능한 필드는 만들려는 레코드 유형에 따라 다릅니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 삭제]

이 작업 모듈은 연락처, 회사 또는 거래를 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td>삭제할 레코드 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>삭제할 연락처, 회사 또는 거래의 ID를 입력합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 속성 가져오기]

이 작업 모듈은 (내부) 이름으로 특정 레코드 속성에 대한 메타데이터를 가져옵니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td>메타데이터를 검색할 속성이 있는 레코드 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 속성 이름]</td> 
   <td>메타데이터를 검색할 속성을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 옵션 ID]</td> 
   <td> <p> 일부 속성에는 사용자가 속성 값으로 선택할 수 있는 사용 가능한 옵션 세트가 있습니다. 검색할 속성 값을 나타내는 옵션의 ID를 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 보기]

이 트리거 모듈은 지난 30일 내에 연락처, 회사 또는 거래가 수정되거나 만들어진 경우 시나리오를 시작합니다. 출력은 10,000개의 레코드로 제한됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td>보려는 속성이 있는 레코드 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>최근에 수정한 레코드 또는 최근에 만든 레코드를 볼지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력 속성]</td> 
   <td>모듈의 출력에 포함할 속성을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 연락처

* [[!UICONTROL 연락처 만들기/업데이트(레거시)]](#createupdate-a-contact-legacy)
* [[!UICONTROL 연락처 그룹 만들기/업데이트]](#createupdate-a-group-of-contacts)
* [[!UICONTROL 목록에 연락처 추가]](#add-contacts-to-a-list)
* [[!UICONTROL 목록에서 연락처 제거]](#remove-a-contact-from-a-list)
* [[!UICONTROL 연락처 병합]](#merge-contacts)
* [[!UICONTROL 연락처 검색]](#search-for-contacts)
* [[!UICONTROL 연락처 나열]](#list-contacts)
* [[!UICONTROL 회사 연락처 나열]](#list-contacts-of-a-company)

#### [!UICONTROL 연락처 만들기/업데이트(레거시)]

포털에 이미 존재하지 않는 연락처를 만들거나, 포털에 존재하는 연락처를 최신 속성 값으로 업데이트합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 속성]</td> 
   <td>연락처에 대해 설정하거나 업데이트할 속성을 입력합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 연락처 그룹 만들기/업데이트]

대화 상대 그룹을 만들거나 대화 상대가 이미 있는 경우 업데이트합니다. 일괄 처리 크기가 연락처 100개 이하로 제한된 경우 성능이 가장 좋습니다. 이 끝점을 통해 수행된 변경 사항은 비동기적으로 처리되므로 변경 사항이 연락처 레코드에 적용되는 데 몇 분이 걸릴 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">생성/업데이트할 연락처의 [!UICONTROL 배치] </td> 
   <td> <p>연락처 배치를 추가합니다.</p> <p>새 연락처를 추가하려면 <strong>[!UICONTROL 항목 추가]</strong>를 클릭하십시오. 표시되는 창에서 다음 정보를 입력하거나 매핑합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 검색 유형]</strong> </p> <p>연락처를 식별하는 방법을 선택합니다.</p> 
      <ul> 
       <li> <p>[!UICONTROL ID]</p> <p>만들거나 업데이트할 연락처의 ID를 입력하십시오. </p> </li> 
       <li> <p>[!UICONTROL Email]</p> <p>만들거나 업데이트할 연락처의 이메일 주소를 입력합니다. </p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL 속성]</strong> </p> <p>연락처에 대해 설정하거나 업데이트할 속성을 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 목록에 연락처 추가]

이 모듈은 시스템에서 이미 생성된 연락처 레코드를 연락처 목록에 추가합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 목록 ID] </td> 
   <td>연락처를 추가할 목록의 ID를 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID/Emails] </td> 
   <td> <p>목록에 추가할 연락처를 식별하는 방법을 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL IDs]</p> <p>목록에 추가하려는 연락처의 ID를 추가합니다.</p> </li> 
     <li> <p>[!UICONTROL 전자 메일]</p> <p>목록에 추가하려는 연락처의 이메일 주소를 추가합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 목록에서 연락처 제거]

연락처 목록에서 연락처를 제거합니다.

>[!NOTE]
>
>동적 목록에서 연락처를 수동으로 제거할 수 없습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 목록 ID] </td> 
   <td>연락처를 제거할 목록의 ID를 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 연락처 ID] </td> 
   <td>목록에서 제거할 연락처의 ID를 입력하십시오. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 연락처 병합]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 1] </td> 
   <td>병합할 연락처 중 하나의 ID를 입력합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 2] </td> 
   <td>병합할 다른 연락처의 ID를 입력합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 연락처 검색]

검색 쿼리를 사용하여 연락처 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td>검색 쿼리를 입력합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한] </td> 
   <td>시나리오 실행 주기 동안 [!DNL Workfront Fusion]이(가) 반환해야 하는 최대 연락처 수를 입력하거나 매핑합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 연락처 나열]

포털에서 만든 모든 연락처를 반환합니다. 출력은 5000개의 연락처로 제한됩니다. 이전 또는 다음 연락처를 나열하려면 [!UICONTROL 고급] 매개 변수를 사용하여 목록을 오프셋할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td>시나리오 실행 주기 동안 최대 연락처 수 [!DNL Workfront Fusion]이(가) 반환되어야 합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력 속성]</td> 
   <td>모듈의 출력에 표시할 속성을 선택합니다. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL 회사 연락처 나열]

회사 연락처 목록을 검색합니다. 출력은 5000개의 연락처로 제한됩니다. 이전 또는 다음 연락처를 나열하려면 [!UICONTROL 고급] 매개 변수를 사용하여 목록을 오프셋할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>연락처를 나열할 회사의 ID를 입력합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td>시나리오 실행 주기 동안 최대 연락처 수 [!DNL Workfront Fusion]이(가) 반환되어야 합니다. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL 목록에 추가된 연락처 보기]

이 트리거 모듈은 새 연락처가 목록에 추가되면 시나리오를 시작합니다. 이 기능은 유료 마케팅 계정이 있는 사용자만 사용할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 목록 ID]</td> 
   <td>보려는 연락처가 포함된 목록의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력 속성]</td> 
   <td>모듈의 출력에 포함할 속성을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 거래

* [[!UICONTROL 거래/티켓 파이프라인 나열]](#list-dealticket-pipelines)
* [[!UICONTROL 거래의 CRM 파이프라인 가져오기]](#get-a-deals-crm-pipeline)

#### [!UICONTROL 거래/티켓 파이프라인 나열]

지정된 포털에 대한 모든 거래 및 티켓 파이프라인을 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 개체 유형] </td> 
   <td>거래 또는 티켓 나열 여부를 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 거래의 CRM 파이프라인 가져오기]

특정 거래 파이프라인을 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파이프라인 ID] </td> 
   <td>세부 정보를 검색할 파이프라인의 ID를 입력하거나 매핑합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 단계 ID] </td> 
   <td>세부 정보를 검색할 단계의 ID를 입력하거나 매핑합니다. </td> 
  </tr> 
 </tbody> 
</table>

### 회사

#### [!UICONTROL 도메인별로 회사 검색]

도메인 속성에 정확히 일치하는 항목을 기반으로 회사 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Domain] </td> 
   <td>검색할 회사의 도메인(예: <code>[!DNL hubspot].com</code>)을 입력하십시오. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td>시나리오 실행 주기 동안 최대 회사 수 [!DNL Workfront Fusion]이(가) 반환해야 합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력 속성]</td> 
   <td>모듈의 출력에 표시할 속성을 선택합니다. </td> 
  </tr> 
 </tbody> 
</table>

### 파일

* [[!UICONTROL 폴더 만들기]](#create-a-folder)
* [[!UICONTROL 폴더 삭제]](#delete-a-folder)
* [[!UICONTROL 파일 이동]](#move-a-file)

#### [!UICONTROL 폴더 만들기]

이 모듈은 폴더를 생성합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 이름] </td> 
   <td>새 폴더의 이름을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 상위 폴더 ID] </td> 
   <td>생성 중인 폴더의 상위 폴더 ID를 선택합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더 삭제]

폴더를 삭제된 것으로 표시합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>삭제할 폴더의 ID를 입력합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 이동]

파일을 다른 폴더로 이동합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 ID] </td> 
   <td>이동할 파일의 ID를 입력하거나 매핑합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 ID] </td> 
   <td>파일을 이동할 폴더의 ID를 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이름]</td> 
   <td>이동된 파일의 이름을 입력합니다.</td> 
  </tr> 
 </tbody> 
</table>

### 티켓

#### [!UICONTROL 티켓 삭제]

ID로 기존 티켓을 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>삭제할 티켓의 ID를 입력합니다. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL API 호출 만들기]

사용자 지정 API 호출을 수행할 수 있습니다.

>[!NOTE]
>
>다음 엔드포인트는 2023년 8월 31일에 HubSpot API에서 더 이상 사용되지 않으며 Fusion 모듈에서 더 이상 사용할 수 없습니다.
>
>* 콘텐츠 이벤트 나열
>* 소셜 이벤트 나열
>* 달력 작업 이벤트 나열
>* 모든 캘린더 이벤트 나열
>* 캘린더 작업 만들기
>* ID별 캘린더 작업 가져오기
>* 캘린더 작업 업데이트
>* 캘린더 작업 삭제

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>https://api.hubapi.com/에 상대적인 경로를 입력합니다. 예: /contacts/v1/lists/all/contacts/all</p> <p>사용 가능한 끝점 목록은 <a href="https://legacydocs.hubspot.com/docs/overview">[!DNL HubSpot] API 설명서</a>를 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 메서드]</p> </td> 
   <td> <p>사용할 HTTP 메서드를 선택합니다.</p> <p>[!UICONTROL GET]</p> <p>를 클릭하여 항목에 대한 정보를 검색합니다.</p> <p>[!UICONTROL POST]</p> <p>새 항목을 만듭니다.</p> <p>[!UICONTROL PUT]</p> <p>기존 항목을 업데이트/바꿉니다.</p> <p>[!UICONTROL PATCH]</p> <p>부분 항목 업데이트를 수행합니다.</p> <p>[!UICONTROL DELETE]</p> <p>항목을 삭제합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p> 원하는 요청 헤더를 입력합니다. 인증 헤더를 추가할 필요가 없습니다. 이미 추가했습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p> 요청 쿼리 문자열을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>표준 JSON 개체 형식으로 API 호출에 대한 본문 콘텐츠를 추가합니다. JSON에서 <code>if</code>과(와) 같은 조건문을 사용할 때는 따옴표를 조건문 외부에 넣으십시오.<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**예:** 다음 API 호출은 [!DNL HubSpot] 계정의 모든 연락처를 반환합니다.
>
>**URL**: `/contacts/v1/lists/all/contacts/all`
>
>**메서드**: `GET`
>
>![](assets/hubspot-api-config.png)
>
>검색 일치 항목은 [!UICONTROL 번들] > [!UICONTROL 본문] > [!UICONTROL 연락처]의 모듈 출력에서 찾을 수 있습니다.
>
>이 예에서는 3개의 연락처가 반환되었습니다.
>
>![](assets/hubspot-api-output.png)

## 새 애플리케이션 만들기

1. [!DNL HubSpot] 개발자 계정에 로그인합니다.
1. **[!UICONTROL 앱 만들기]** 옵션을 선택합니다.
1. 앱 이름을 입력하고 대화 상자를 [!UICONTROL 저장]합니다.
1. Webhook에 필요한 범위를 선택합니다.

   예를 들어 새 연락처를 만들거나 삭제할 때 모듈을 트리거하기 위한 연락처 범위를 추가합니다.

   [!UICONTROL 연락처 범위]만 있으면 연락처, 거래 및 회사 이벤트 웹후크를 받을 수 있습니다.

   >[!IMPORTANT]
   >
   >[!UICONTROL 리디렉션 URL] 필드를 입력하지 마십시오.
