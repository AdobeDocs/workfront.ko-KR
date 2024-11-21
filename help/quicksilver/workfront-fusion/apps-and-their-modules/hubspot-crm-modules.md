---
title: HubSpot CRM 모듈
description: ' [!DNL Adobe Workfront Fusion] HubSpot CRM 모듈을 사용하면 이벤트, 레코드, 연락처, 참여, 파일 및 양식 제출을 모니터링하거나  [!DNL HubSpot CRM] 계정의 레코드, 연락처, 참여, 이벤트 또는 파일을 만들고, 검색하고, 업데이트하고, 삭제할 수 있습니다.'
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '6411'
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

## HubSpot CRM API 정보

HubSpot CRM 커넥터는 다음을 사용합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">기본 URL</td> 
   <td>https://api.hubapi.com</td> 
  </tr>
  <tr> 
   <td role="rowheader">API 태그</td> 
   <td>v2.0.14</td> 
  </tr>
 </tbody> 
 </table>

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
* [참여 횟수](#engagements)
* [이벤트 및 알림](#events-and-notifications)
* [파일](#files)
* [작업](#tasks)
* [사용자](#users)
* [티켓](#tickets)
* [양식](#forms)
* [소셜 미디어(브로드캐스트)](#social-media-broadcast)
* [블로그 게시물](#blog-posts)
  <!--* [Workflows]-->
* [구독](#subscriptions)
  <!--* [Associations](#associations)-->
* [기타](#other)

+++**CRM 개체**

### CRM 오브젝트

* [CRM 오브젝트 검색](#search-for-crm-objects)
* [CRM 오브젝트 보기](#watch-crm-objects)

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
  </tr> 
   <tr> 
    <td role="rowheader">시작 오프셋</td> 
    <td>세부 정보를 검색할 첫 번째 항목의 ID를 입력하거나 매핑합니다. 이 모듈은 한 번에 최대 5000개의 결과만 반환합니다. 시작 오프셋을 설정하면 처음 5000 이외의 항목을 검색할 수 있습니다. 시작 오프셋이 5000이면 모듈은 항목 5000-9999를 반환합니다.</td> 
   </tr>
 </tbody> 
</table>

#### CRM 오브젝트 보기

이 트리거 모듈은 CRM 개체가 생성되거나 업데이트될 때 시나리오를 시작합니다.

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
   <td> <p>검색할 객체 유형을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력 속성]</td> 
   <td>이 모듈에 대한 출력에 포함할 속성을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 생성됨/업데이트됨]</td> 
   <td>생성된(신규) 또는 업데이트된(수정된) 객체를 감시할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 필터 기준]</td> 
   <td>필터를 추가하여 특정 조건이 충족될 때만 시나리오가 시작되도록 할 수 있습니다.<ul><li><b>쿼리</b><p>필터링 기준으로 사용할 쿼리를 입력합니다.</li><li><b>속성</b><p>결과를 필터링하는 데 사용할 각 속성에 대해 <b>항목 추가</b>를 클릭하고 속성 이름, 연산자 및 속성 값을 입력하십시오.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**거래, 연락처 및 회사 기록**

### 기록(거래, 연락처 및 회사)

* [레코드 만들기](#create-a-record)
* [[!UICONTROL 레코드 만들기(레거시)]](#create-a-record-legacy)
* [[!UICONTROL 레코드 삭제]](#delete-a-record)
* [[!UICONTROL 레코드 가져오기]](#get-a-record)
* [[!UICONTROL 레코드 속성 가져오기]](#get-a-record-property)
* [목록 레코드](#list-records)
* [[!UICONTROL 레코드 업데이트]](#update-a-record)
* [[!UICONTROL 레코드 보기]](#watch-records)

#### 레코드 만들기

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
   <td> <p>만들려는 레코드 유형을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 속성 그룹]</td> 
   <td>레코드를 만들 때 추가할 각 속성에 대해 속성을 찾을 그룹을 선택합니다. 속성 그룹이 열리고 속성 값을 입력할 수 있습니다. 사용 가능한 속성 그룹 및 속성은 만들려는 레코드 유형에 따라 다릅니다.</td> 
  </tr> 
 </tbody> 
</table>

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
   <td> <p>만들려는 레코드 유형을 선택합니다.</p> </td> 
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

#### 목록 레코드

이 검색 모듈은 연락처, 회사 또는 거래 목록을 반환합니다. 출력은 5000개의 연락처, 12,500개의 회사 또는 12,500개의 거래로 제한됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 유형]</td> 
   <td> <p>반환할 레코드 유형을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력 속성]</td> 
   <td>이 모듈에 대한 출력에 포함할 속성을 선택합니다.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
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

+++

+++**연락처**

### 연락처

* [[!UICONTROL 목록에 연락처 추가]](#add-contacts-to-a-list)
* [연락처 만들기/업데이트](#createupdate-a-contact)
* [[!UICONTROL 연락처 만들기/업데이트(레거시)]](#createupdate-a-contact-legacy)
* [[!UICONTROL 연락처 그룹 만들기/업데이트]](#createupdate-a-group-of-contacts)
* [[!UICONTROL 연락처 나열]](#list-contacts)
* [[!UICONTROL 회사 연락처 나열]](#list-contacts-of-a-company)
* [[!UICONTROL 연락처 병합]](#merge-contacts)
* [[!UICONTROL 목록에서 연락처 제거]](#remove-a-contact-from-a-list)
* [[!UICONTROL 연락처 검색]](#search-for-contacts)
* [목록에 추가된 연락처 보기](#watch-contacts-added-to-a-list)

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

#### 연락처 만들기/업데이트

이 작업 모듈은 포털에 존재하지 않는 연락처를 만듭니다. 포털에 연락처가 있으면 이 모듈은 제공된 값으로 연락처를 업데이트합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 속성 그룹]</td> 
   <td>연락처를 만들 때 추가하려는 각 속성에 대해 속성이 있는 그룹을 선택합니다. 속성 그룹이 열리고 속성 값을 입력할 수 있습니다.</td> 
  </tr> 
 </tbody> 
</table>

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
  </tr> 
   <tr> 
    <td role="rowheader">연락처 ID [시작 오프셋] </td> 
    <td>목록을 시작할 사용자의 ID를 입력하거나 매핑합니다. 예를 들어, 연락처 ID를 101번째 연락처의 ID로 설정하면 모듈은 연락처 1-5000이 아닌 연락처 101-5100을 나열할 수 있습니다. </td> 
   </tr>
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
  </tr> 
   <tr> 
    <td role="rowheader">연락처 ID [시작 오프셋] </td> 
    <td>목록을 시작할 사용자의 ID를 입력하거나 매핑합니다. 예를 들어, 연락처 ID를 101번째 연락처의 ID로 설정하면 모듈은 연락처 1-5000이 아닌 연락처 101-5100을 나열할 수 있습니다. </td> 
   </tr>
 </tbody> 
</table>

#### [!UICONTROL 연락처 병합]

이 작업 모듈은 연락처를 병합합니다.

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

+++

+++**거래**

### 거래

* [[!UICONTROL 거래의 CRM 파이프라인 가져오기]](#get-a-deals-crm-pipeline)
* [[!UICONTROL 거래/티켓 파이프라인 나열]](#list-dealticket-pipelines)

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

+++

+++**회사**

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

+++

+++**참여**

### 참여 횟수

* [CRM 개체와 참여 연결](#associate-an-engagement-with-a-crm-object)
* [참여 만들기](#create-an-engagement)
* [참여 삭제](#delete-an-engagement)
* [참여 보기](#watch-engagements)

#### CRM 개체와 참여 연결

이 작업 모듈은 계약을 연락처, 회사 또는 거래와 연결합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 유형]</td> 
   <td>참여를 연결할 CRM 레코드 유형을 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 참여 ID]</td> 
  <td>개체와 연결할 계약의 ID를 입력하거나 매핑합니다.</td> 
   </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 ID]</td> 
  <td>계약을 연결할 레코드의 ID를 입력하거나 매핑합니다.</td> 
   </tr> 
 </tbody> 
</table>

#### 참여 만들기

이 작업 모듈은 HubSpot의 CRM 오브젝트와 참여(예: 메모, 작업 또는 활동)를 만듭니다. 참여는 CRM에 기록해야 하는 연락처와의 모든 상호 작용입니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL이 활성화되었습니까?]</td> 
   <td>새 참여가 만들어질 때 활성화될 경우 이 옵션을 활성화하십시오. 타임라인에 참여하려면 참여가 활성화되어야 합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 유형]</td> 
  <td>만들려는 참여 유형을 선택합니다.
  <ul>
  <li><b>이메일</b><p></p><a href="#email-metadata" class="MCXref xref" >이메일 메타데이터</a>을(를) 계속합니다.</p></li>
  <li><b>호출</b><p><a href="#call-metadata" class="MCXref xref" >메타데이터 호출</a>을 계속합니다.</p></li>
  <li><b>회의</b><p><a href="#meeting-fields" class="MCXref xref" >모임 필드</a>을(를) 계속합니다.</p></li>
  <li><b>작업</b><p><a href="#task-fields" class="MCXref xref" >작업 필드</a>로 계속합니다.</p></li>
  <li><b>참고</b><p>본문 필드에 메모 텍스트를 입력합니다.</p></li>
  </ul>
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">타임스탬프</td> 
   <td>참여에 대한 타임스탬프를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">소유자 ID</td> 
   <td>계약을 할당할 사용자의 소유자 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">UID</td> 
   <td>여러 객체 유형에서 사용할 수 있는 참여 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">포털 ID</td> 
   <td>포털의 ID를 입력하거나 매핑합니다. 이 기능은 조직에 여러 개의 포털이 있는 경우에 유용합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">연결된 연락처</td> 
   <td>이 계약을 연결할 각 연락처에 대해 <b>항목 추가</b>를 클릭하고 연락처 ID를 입력하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">연계된 회사</td> 
   <td>이 참여를 연결할 각 회사에 대해 <b>항목 추가</b>를 클릭하고 회사 ID를 입력하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">연계된 거래</td> 
   <td>이 계약을 연결할 각 거래에 대해 <b>항목 추가</b>를 클릭하고 거래 ID를 입력하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">연계된 티켓</td> 
   <td>이 참여를 연결할 각 티켓에 대해 <b>항목 추가</b>를 클릭하고 티켓 ID를 입력하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">첨부 파일</td> 
   <td>이 참여를 연결할 각 첨부 파일에 대해 <b>항목 추가</b>를 클릭하고 첨부할 파일의 파일 ID를 입력하십시오.</td> 
  </tr> 
 </tbody> 
</table>

##### 이메일 메타데이터

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL From &gt; Email]</p> </td> 
   <td> <p>이메일을 보낼 이메일 주소를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL First Name]</td> 
   <td>이메일을 보낼 사람의 이름을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 성]</td> 
  <td>이메일을 보낼 사람의 성을 입력하거나 매핑합니다.
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">까지</td> 
   <td>전자 메일을 보낼 각 전자 메일 주소에 대해 <b>항목 추가</b>를 클릭하고 전자 메일 주소를 입력하거나 매핑하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">참조</td> 
   <td>참조하려는 각 전자 메일 주소에 대해 <b>항목 추가</b>를 클릭하고 전자 메일 주소를 입력하거나 매핑하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">숨은 참조</td> 
   <td>Bcc로 보낼 각 전자 메일 주소에 대해 <b>항목 추가</b>를 클릭하고 전자 메일 주소를 입력하거나 매핑하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">제목</td> 
   <td>이메일 제목 텍스트 입력 또는 매핑</td> 
  </tr> 
  <tr> 
   <td role="rowheader">HTML</td> 
   <td>HTML 형식의 이메일을 보내려면 HTML 태그를 포함한 이메일 본문을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">텍스트</td> 
   <td>텍스트 전용 이메일을 보내려면 이메일 본문의 텍스트를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

##### 메타데이터 호출

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL To Number]</p> </td> 
   <td> <p>전화를 걸 전화 번호를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL From Number]</td> 
   <td>전화를 걸 전화 번호를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 상태]</td> 
  <td>호출 상태를 선택합니다.
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">본문</td> 
   <td>통화에 대한 세부 정보 또는 메모를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">외부 ID</td> 
   <td>이 필드는 HubSpot에서 수행한 호출의 내부 ID를 나타냅니다. 별도의 작업이 필요하지 않습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">기간</td> 
   <td>호출 길이(밀리초)를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">외부 계정 ID</td> 
   <td>이 필드는 HubSpot에서 수행한 호출의 내부 계정 ID를 나타냅니다. 별도의 작업이 필요하지 않습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">레코딩 URL</td> 
   <td>기록 파일의 URL을 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

##### 모임 필드

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Title]</p> </td> 
   <td> <p>모임의 제목이나 제목을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>모임 설명 또는 세부 정보의 텍스트를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시작 시간]</td> 
  <td>회의 시작 시간을 UNIX 타임스탬프로 입력하거나 매핑합니다.
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">종료 시간</td> 
   <td>회의 종료 시간을 UNIX 타임스탬프로 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

##### 작업 필드

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Subject]</p> </td> 
   <td> <p>작업의 제목 또는 제목을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>작업 설명 또는 세부 정보의 텍스트를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">상태</td> 
   <td>작업 상태를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 유형에 대한 [!UICONTROL]</td> 
  <td><code>CONTACT</code> 또는 <code>COMPANY</code>을(를) 입력하십시오.
  </td> 
   </tr> 
 </tbody> 
</table>

#### 참여 삭제

이 작업 모듈은 해당 ID로 계약을 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 ID]</td> 
   <td>삭제할 계약의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### 참여 보기

이 트리거 모듈은 포털에 새 참여가 생성되면 시나리오를 시작합니다. 이 모듈은 지난 30일 동안 생성된 레코드 또는 가장 최근에 생성된 레코드 10,000개만 반환합니다.

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
   <td>시나리오 실행 주기 동안 최대 회사 수 [!DNL Workfront Fusion]이(가) 반환해야 합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since]</td> 
   <td>이벤트를 보려는 가장 빠른 날짜를 입력하거나 매핑합니다. <code>MM/DD/YYYY h:mm</code> 형식을 사용합니다.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**이벤트 및 알림**

### 이벤트 및 알림

* [타임라인 이벤트 만들기/업데이트](#create--update-a-timeline-event)
* [타임라인 이벤트 유형 나열](#list-timeline-event-types)
* [달력 이벤트 보기](#watch-calendar-events)
* [알림 보기](#watch-notifications)

#### 타임라인 이벤트 만들기/업데이트

이 작업 모듈은 타임라인 이벤트를 만들거나 업데이트합니다. 이 모듈은 사용자 식별자, HubSpot API 키, 클라이언트 ID 및 클라이언트 암호를 포함하는 개발자 연결에서만 사용할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 응용 프로그램 ID]</td> 
   <td>이 이벤트가 속한 응용 프로그램의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이벤트 ID]</td> 
   <td>이 이벤트의 ID를 입력하거나 매핑합니다. 이벤트 ID는 시스템에서 생성되지 않습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이벤트 유형 ID]</td> 
   <td>이 이벤트의 이벤트 유형 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>이벤트를 만들 연락처의 이메일 주소를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 개체 ID]</td> 
   <td>이벤트를 만들 연락처의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 타임스탬프]</td> 
   <td>이 이벤트의 타임스탬프를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사용자 지정 데이터]</td> 
   <td>이 이벤트에 추가할 사용자 지정 데이터의 각 항목에 대해 <b>항목 추가</b>를 클릭하고 항목의 이름과 값을 입력합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### 타임라인 이벤트 유형 나열

이 검색 모듈은 특정 애플리케이션에 대한 모든 타임라인 이벤트 목록을 반환합니다. 이 모듈은 사용자 식별자, HubSpot API 키, 클라이언트 ID 및 클라이언트 암호를 포함하는 개발자 연결에서만 사용할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 응용 프로그램 ID]</td> 
   <td>이 이벤트가 속한 애플리케이션의 ID를 입력하거나 매핑합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### 달력 이벤트 보기

이 트리거 모듈은 새 이벤트가 캘린더에 추가되면 시나리오를 시작합니다. 시작 날짜와 종료 날짜 사이에 최대 500개의 작업이 포함됩니다. 이 모듈은 사용자 식별자, HubSpot API 키, 클라이언트 ID 및 클라이언트 암호를 포함하는 개발자 연결에서만 사용할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이벤트 유형]</td> 
   <td>소셜 이벤트, 콘텐츠 이벤트 또는 모든 이벤트를 시청할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 파일 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시작 날짜]</td> 
   <td>시작 날짜를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 종료 날짜]</td> 
   <td>종료 날짜를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### 알림 보기

이 트리거 모듈은 변경 사항에 대한 새 알림이 전송될 때 시나리오를 시작합니다.  시작 날짜와 종료 날짜 사이에 최대 500개의 작업이 포함됩니다. 이 모듈은 사용자 식별자, HubSpot API 키, 클라이언트 ID 및 클라이언트 암호를 포함하는 개발자 연결에서만 사용할 수 있습니다. HubSpot에는 개발자 애플리케이션당 하나의 웹후크 URL만 있을 수 있습니다.

이 모듈에 대한 웹후크를 만들려면 웹후크 필드 옆에 있는 **추가**&#x200B;를 클릭하고 다음 필드를 채우십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 응용 프로그램 ID]</td> 
   <td>이 웹후크에 사용할 애플리케이션 ID를 입력합니다. HubSpot 개발자 포털에서 ID를 찾을 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 가입]</td> 
   <td> <p>보려는 각 알림 유형에 대해 <b>항목 추가</b>를 클릭하고 구독 유형을 선택하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이전 구독을 강제로 제거]</td> 
   <td>이 웹후크에 첨부된 이전 구독을 분리하거나 삭제하려면 이 옵션을 활성화하십시오.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**파일**

### 파일

* [[!UICONTROL 폴더 만들기]](#create-a-folder)
* [파일 삭제](#delete-a-file)
* [[!UICONTROL 폴더 삭제]](#delete-a-folder)
* [목록 파일](#list-files)
* [[!UICONTROL 파일 이동]](#move-a-file)
* [파일 업로드](#upload-a-file)
* [파일 보기](#watch-files)

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

#### 파일 삭제

이 작업 모듈은 파일 관리자에서 파일 및 모든 관련 데이터와 썸네일을 영구적으로 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 ID]</td> 
   <td>삭제할 파일의 ID를 입력하거나 매핑합니다.</td> 
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
   <td>삭제하려는 폴더의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### 목록 파일

이 검색 모듈은 파일 관리자에 저장된 파일 목록을 반환합니다.

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
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 파일 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 ID]</td> 
   <td>나열할 파일이 포함된 폴더의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>파일 이름에 특정 문자가 들어 있는 파일만 포함하려면 파일 이름에 포함할 문자를 입력하거나 매핑합니다.</td> 
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

#### 파일 업로드

이 작업 모듈은 파일을 파일 관리자에 업로드합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source 파일]</td> 
   <td> <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 액세스 유형] </td> 
   <td>파일을 private으로 할지, public으로 할지, indexable로 만들지 또는 public과 indexable로 할지 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 ID] </td> 
   <td>파일을 업로드할 폴더의 ID를 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 덮어쓰기]</td> 
   <td>폴더에 파일이 이미 있는 경우 덮어쓰려면 이 옵션을 활성화합니다.</td> 
  </tr> 
 </tbody> 
</table>

### 파일 보기

이 트리거 모듈은 새 파일이 파일 관리자에 저장될 때 시나리오를 시작합니다.

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
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 파일 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더 ID]</td> 
   <td>보려는 파일이 포함된 폴더의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>파일 이름에 특정 문자가 들어 있는 파일만 포함하려면 파일 이름에 포함할 문자를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**작업**

### 작업

* [캘린더 작업 만들기](#create-a-calendar-task)
* [캘린더 작업 삭제](#create-a-calendar-task)
* [작업 이벤트 보기](#watch-task-events)

#### 캘린더 작업 만들기

이 작업 모듈은 캘린더에 대한 새 작업을 만듭니다. 이 모듈에서 사용되는 연결은 유료 마케팅 계정이 있는 사용자의 자격 증명을 사용해야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이름]</td> 
   <td>새 달력 작업의 이름을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 설명]</td> 
   <td>새 달력 작업에 대한 설명을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소유자 ID]</td> 
   <td>이 작업에 할당된 사용자의 소유자 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이벤트 날짜]</td> 
   <td>이 작업의 날짜를 입력하거나 매핑합니다.<p>지원되는 날짜 및 시간 형식 목록을 보려면 [!DNL Adobe Workfront Fusion]</a>의 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 변환을 참조하십시오.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 범주]</td> 
   <td>이벤트 유형을 선택합니다.<ul><li><b>블로그 게시물</b><p>콘텐츠 그룹 ID를 입력합니다. 블로그 페이지의 ID입니다.</p></li><li><b>이메일</b><p>사용할 이메일 템플릿에 경로를 입력하거나 매핑합니다.</li><li><b>랜딩 페이지</b><p>사용할 랜딩 페이지 템플릿에 경로를 입력하거나 매핑합니다.</li><li><b>사용자 정의</b></li><ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 상태]</td> 
   <td>이벤트가 "할 일" 상태인지 또는 "완료" 상태인지 여부를 입력합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campaign GUID]</td> 
   <td>이 이벤트가 속한 캠페인의 내부 HubSpot ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### 캘린더 작업 삭제

이 작업 모듈은 캘린더 작업을 삭제합니다. 이 모듈에서 사용되는 연결은 유료 마케팅 계정이 있는 사용자의 자격 증명을 사용해야 합니다.

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
   <td>삭제할 작업의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### 작업 이벤트 보기

이 트리거 모듈은 캘린더에 새 작업 이벤트가 있을 때 시나리오를 시작합니다. 이 모듈에서 사용되는 연결은 유료 마케팅 계정이 있는 사용자의 자격 증명을 사용해야 합니다. 모듈은 최대 500개의 이벤트를 반환합니다.

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
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 파일 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시작 날짜]</td> 
   <td>이벤트를 보려는 가장 빠른 날짜를 입력하거나 매핑합니다. <code>MM/DD/YYYY h:mm</code> 형식을 사용합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 종료 날짜]</td> 
   <td>이벤트를 보려는 최신 날짜를 입력하거나 매핑합니다. <code>MM/DD/YYYY h:mm</code> 형식을 사용합니다.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**사용자**

### 사용자

* [소유자 가져오기](#get-an-owner)
* [목록 소유자](#list-owners)

#### 소유자 가져오기

이 작업 모듈은 소유자에 대한 세부 정보를 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소유자 ID]</td> 
   <td> <p>세부 정보를 반환할 소유자의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 목록 소유자

이 검색 모듈은 HubSpot 계정에 있는 모든 소유자 목록을 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**티켓**

### 티켓

<!--* [Create a Ticket]-->
* [티켓 삭제](#delete-a-ticket)
  <!--* [Create a Ticket]-->
  <!--* [Create a Ticket]-->
  <!--* [Create a Ticket]-->
  <!--* [Create a Ticket]-->

<!-- Create a Ticket Need to find a working connection-->

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

<!-- Get a Ticket  Need to find a working connection-->

<!-- List Tickets  Need to find a working connection-->

&lt;!— 티켓 업데이트 작동 중인 연결을 찾아야 합니다—>

<!-- Watch Tickets Need to find a working connection-->

+++

+++**Forms**

### 양식

* [양식을 통해 업로드된 파일 가져오기](#get-a-file-uploaded-via-form)
* [Forms 나열](#list-forms)
  <!--* [Submit Data to a Form]-->
  <!--* [Watch Submissions for a Form]-->

#### 양식을 통해 업로드된 파일 가져오기

이 작업 모듈은 양식을 통해 업로드된 파일을 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 URL]</td> 
   <td>검색할 파일의 URL을 입력하거나 매핑합니다. 이는 양식 메타데이터에서 찾을 수 있습니다.</td> 
  </tr> 
 </tbody> 
</table>

#### 목록 Forms

이 작업 모듈은 이 모듈에 사용된 연결과 연결된 계정에서 만든 모든 양식을 반환합니다.

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
   <td>한 실행 주기에서 모듈이 반환할 최대 양식 수를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

<!--#### Submit Data to a Form Need to find a working connection-->



&lt;!—#### 양식에 대한 제출 보기 — 작업 연결을 찾아야 합니다.>—>

+++

+++**소셜 미디어(브로드캐스트)**

### 소셜 미디어(브로드캐스트)

* [브로드캐스트 메시지 취소](#cancel-a-broadcast-message)
* [브로드캐스트 메시지 만들기](#create-a-broadcast-message)
* [브로드캐스트 메시지 보기](#watch-broadcast-messages)

#### 브로드캐스트 메시지 취소

이 작업 모듈은 트윗 또는 Facebook 게시물과 같은 예약된 브로드캐스트를 취소합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 브로드캐스트 ID]</td> 
   <td>취소할 브로드캐스트의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### 브로드캐스트 메시지 만들기

이 작업 모듈은 지정된 소셜 미디어 채널에 메시지를 만들고 즉시 게시합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 채널 ID]</td> 
   <td>이 브로드캐스트에 사용할 채널의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>이 브로드캐스트의 제목을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>브로드캐스트의 텍스트를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사진 URL]</td> 
   <td>브로드캐스트에 포함할 사진의 URL을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 썸네일 URL]</td> 
   <td>이 브로드캐스트에 사용할 썸네일의 URL을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 트리거 위치]</td> 
   <td>브로드캐스트를 전송할 날짜 및 시간을 입력하거나 매핑합니다. 비워 두면 브로드캐스트가 즉시 전송됩니다.<p>지원되는 날짜 및 시간 형식 목록을 보려면 [!DNL Adobe Workfront Fusion]</a>의 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 변환을 참조하십시오.</p></td> 
  </tr> 
 </tbody> 
</table>

#### 브로드캐스트 메시지 보기

이 트리거 모듈은 메시지가 HubSpot에서 지정된 소셜 미디어 채널로 게시되면 시나리오를 시작합니다.

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
   <td role="rowheader">[!UICONTROL 상태별 필터]</td> 
   <td>메시지가 특정 상태에 있을 때만 시나리오를 시작하려면 상태를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">채널별 [!UICONTROL 필터]</td> 
   <td>메시지가 특정 채널에 있을 때만 시나리오를 시작하려면 채널을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 브로드캐스트 ID]</td> 
   <td>메시지가 특정 날짜 또는 그 이후일 때만 시나리오를 시작하려면 <code>MM/DD/YYYY</code> 형식으로 날짜를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**블로그 게시물**

### 블로그 게시물

<!--* [Create a Blog Post]-->
* [블로그 게시물 삭제](#delete-a-blog-post)
  <!--* [List Blog Posts]-->
* [블로그 게시물 Publish/게시 취소](#publish--unpublish-a-blog-post)
  <!--* [Watch Blog Posts]-->

<!--
#### Create a Blog Post May need connection
-->


#### 블로그 게시물 삭제

이 작업 모듈은 단일 블로그 게시물을 삭제합니다.

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
   <td>삭제하려는 블로그 게시물의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

<!--#### List Blog Posts May need connection

This search module retrieves posts from a HubSpot blog.-->

#### Publish / 블로그 게시물 게시 취소

이 작업 모듈은 블로그 게시물 게시를 예약하거나 취소합니다.

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
   <td>예약하거나 취소할 블로그 게시물의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td>블로그 게시물을 예약할지 또는 이전에 예약된 블로그 게시물을 취소할지 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

<!--#### Watch Blog PostsMay need connection-->

+++

<!--+++**Workflows**>

<!--### Workflows May need connection

#### Add a Contact to a Workflow


#### Remove a Contact from a Workflow

-->

<!--+++-->

+++**구독**

### 구독수

* [이메일 구독 업데이트](#update-email-subscription)
* [포털에 대한 구독 타임라인 보기](#watch-subscriptions-timeline-for-a-portal)

#### 이메일 구독 업데이트

이 작업 모듈은 HubSpot의 이메일 구독을 업데이트합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>업데이트할 구독의 이메일 주소를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 상태]</td> 
   <td>구독을 업데이트하려는 각 상태에 대해 <b>항목 추가</b>를 클릭하고 상태의 ID와 전자 메일 주소를 해당 상태에 구독할지 여부를 입력합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Portal 가입 법적 상태]</td> 
   <td>GDPR에 대한 이 구독의 법적 근거를 기록하려면 이 구독의 법적 상태를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Portal 가입 법적 근거 설명]</td> 
   <td>GDPR에 대한 이 구독의 법적 근거에 대한 메모를 추가하려면 메모 텍스트를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### 포털에 대한 구독 타임라인 보기

이 트리거 모듈은 새 이메일 타임라인 구독이 포털에 추가되면 시나리오를 시작합니다.

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
   <td role="rowheader">[!UICONTROL 시작 타임스탬프]</td> 
   <td>특정 날짜 또는 그 이후의 결과를 반환하려면 형식으로 날짜를 입력합니다 <code>MM/DD/YYYY.</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 종료 타임스탬프]</td> 
   <td>특정 날짜 또는 그 이전 날짜의 결과를 반환하려면 형식으로 날짜를 입력합니다 <code>MM/DD/YYYY.</code></td> 
  </tr> 
 </tbody> 
</table>

+++

<!--+++**Associations**-->

<!--### Associations-->

<!--#### Associate CRM Objects  May need connection

This action module associates two CRM objects.-->

<!--#### Associate Multiple CRM Objects  May need connection-->



<!--#### Delete an Association May need connection-->



<!--#### Delete Multiple Associations between CRM Objects May need connection-->



<!--#### List Associations for a CRM Object May need connection-->

<!--+++-->

+++**기타**

### 기타

#### [!UICONTROL API 호출 만들기]

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

+++

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
