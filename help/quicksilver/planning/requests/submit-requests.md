---
title: Adobe Systems Workfront Planning 요청 제출
description: 다른 사용자가 Adobe Systems Workfront Planning의 레코드 종류 페이지에서 요청 양식에 대한 링크를 공유한 후 요청 양식과 연결된 레코드 종류에 대한 레코드를 만들기 위한 요청을 추가할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '2019'
ht-degree: 0%

---

# Adobe Systems Workfront Planning 요청을 제출하여 레코드 만들기

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview">이 페이지 상의 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객이 미리 보기 환경에서만 사용할 수 있습니다. 프로덕션에 대한 월별 릴리스 후에는 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 조직에[ 대한 빠른 릴리스 활성화 또는 비활성화를 참조하세요](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

{{planning-important-intro}}

작업 영역 관리자가 Adobe Systems Workfront Planning에서 레코드 종류에 대한 요청 양식을 작성한 후 이 양식을 사용하여 양식과 연결된 레코드 종류에 대한 레코드를 만드는 요청을 제출할 수 있습니다.

다음 영역에서 Workfront Planning 요청 요청을 제출할 수 있습니다.

* Workfront의 요청 영역에서.
* 직접 링크에서 공유된 요청 양식으로.

  이 문서에서는 Workfront의 요청 영역 또는 공유 링크에서 레코드 종류에 새 레코드를 추가하기 위한 요청을 제출하는 방법을 설명합니다.
* 레코드 종류 페이지에서 새 레코드를 추가하거나 요청 할 때. 자세한 내용은 레코드[ 만들기 섹션을 참조하세요](/help/quicksilver/planning/records/create-records.md).

Workfront 사용자 및 외부 사용자는 레코드 유형 계획에 요청을 제출하고 레코드를 만들 수 있습니다. <!--double check on the external users-->

작업 영역 관리자가 요청 양식을 만들어 레코드 종류와 연결하는 방법에 대한 자세한 내용은 Adobe Systems Workfront Planning[의 요청 양식 만들기 및 관리를 참조하십시오](/help/quicksilver/planning/requests/create-request-form.md).

## 액세스 요구 사항

+++ 액세스 요구 사항을 보려면 확장합니다.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 제품</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Systems Workfront 플랜*</p></td>
   <td>
<p>다음 Workfront 플랜 중 하나:</p>
<ul><li>선택</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다</p>
   </td>
<tr>
   <td role="rowheader"><p>Adobe Systems Workfront 계획 패키지*</p></td>
   <td>
<p>어떤 </p>  
<p>각 Workfront Planning 플랜에 포함된 항목에 대한 자세한 내용은 Workfront 계정 관리자 관리자에게 문의하십시오. </td>
<tr>
   <td role="rowheader"><p>Adobe Systems Workfront 플랫폼</p></td>
   <td>
<p>Workfront Planning에 액세스하려면 조직의 Workfront 인스턴스가 Adobe Systems 통합 환경에 온보딩되어 있어야 합니다.</p>
<p>자세한 내용은 Adobe Systems Unified Experience for Workfront<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">를 참조하십시오</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Systems Workfront 라이선스*</p></td>
   <td>
   <p>외부, 기여자, Light 또는 Standard 라이선스</p>
   <p>Workfront Planning은 기존 Workfront 라이선스에 사용할 수 없습니다</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Adobe Systems Workfront Planning에 대한 액세스 수준 컨트롤은 없습니다</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>개체 사용 권한</p></td>
   <td>
   <p>작업 영역 및 레코드 종류에 대한 보기 이상의 권한(Workfront 사용자인 경우)</p> 
  </td>
  </tr>
 </tbody>
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서[의 액세스 요구 사항을 참조하십시오](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## 전제 조건

Workfront Planning 요청 양식에 요청을 제출하려면 다음 사항을 충족해야 합니다.

* Workfront Planning에는 다음 사항이 있어야 합니다.

   * 작업 영역
   * 레코드 종류입니다.
   * 레코드 종류와 연결된 요청 양식입니다.

     자세한 내용은 Adobe Systems Workfront Planning[의 요청 양식 만들기를 참조하십시오](/help/quicksilver/planning/requests/create-request-form.md).

* 요청 양식은 사용자가 액세스할 수 있는 방식으로 공유해야 합니다. 다음과 같은 시나리오가 있습니다.

   * 내부적으로 양식은 작업 영역에 대한 보기 이상의 권한이 있는 사용자와 공유되어야 합니다.

     Workfront 사용자는 링크 에서 양식에 액세스하거나 Workfront의 요청 영역에서 요청 양식을 찾을 수 있습니다.

   * Workfront 계정 계정이 없는 경우 양식에 대한 링크 링크가 외부 사용자와 공유된 것입니다.

     Workfront 사용자는 외부 사용자와 공유된 링크 파일에도 액세스할 수 있습니다.

* 양식에 대한 링크 만료되지 않아야 합니다.

## Workfront Planning에 요청을 제출할 때 고려해야 할 사항

* 요청 제출 후에는 Workfront에서 편집할 수 없습니다.
* 제출된 각 요청 양식이 승인과 연결되어 있지 않거나 모든 승인자가 승인을 부여한 경우 사용하는 양식과 연결된 레코드 종류에 대한 레코드가 만들어집니다.
* 요청 양식을 제출하여 생성된 레코드는 Workfront Planning의 다른 방법을 통해 추가된 레코드와 구별할 수 없습니다.

  자세한 내용은 레코드[ 만들기 섹션을 참조하세요](/help/quicksilver/planning/records/create-records.md).
* 제출된 요청은 Workfront의 요청 영역에 있는 제출됨 섹션의 계획 탭 에 표시됩니다.
* 특정 필드 유형이 요청 양식에 표시되는 방식이나 양식이 제출된 후 요청 세부 정보 페이지에 표시되는 방식에는 제한이 있습니다.

  자세한 내용은 Adobe Systems Workfront Planning[의 요청 양식 만들기 및 관리를 참조하십시오](/help/quicksilver/planning/requests/create-request-form.md).

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Workfront의 요청 영역에서 Workfront Planning에 요청 제출

{{step1-to-requests}}

1. **화면의 오른쪽 상단 모서리에 있는 새 경험** 설정으로 전환을 활성화합니다.
이 설정을 활성화하면 Workfront의 요청**영역에서 Workfront Planning 요청 양식을 사용할 수 있습니다**.

   >[!TIP]
   >
   >이 설정은 다음이 설정된 경우에만 사용할 수 있습니다.
   >
   >* 회사에서 Workfront Planning 패키지를 구매했습니다.
   >* Workfront 인스턴스 가 Adobe Systems Unified Experience에 온보딩됩니다.
   >* 하나 이상의 작업 영역 보기에 액세스할 수 있습니다.
   >

1. 새로 만들기 요청&#x200B;**을 클릭합니다**.

   ![통합 Workfront 및 Planning 카드가 있는 새로 만들기 요청 상자](assets/new-request-box-with-unified-workfront-and-planning-cards.png)

   **새로 만들기 요청** 상자가 열리고 다음 정보가 표시됩니다.

   * 가장 최근에 액세스한 6개의 Workfront 요청 대기열 및 계획 요청 양식이 최근 섹션에 표시됩니다.
   * 50개의 추가 Workfront 요청 대기열 및 Planning 요청 양식이 **모든 요청 양식** 섹션에 알파벳순으로 표시됩니다. 기본적으로 표시되지 않는 요청 큐를 검색할 수 있습니다.

1. 다음 중 하나를 수행하십시오.

   * 최근 또는 모든 요청 양식 섹션에서 계획 요청 양식 중 하나에 대한 카드를 클릭합니다
   * 시작 검색 상자에 Planning 요청 양식의 이름을 입력한 다음 목록에 표시되면 카드 클릭합니다.

   요청 양식이 열립니다.

1. 요청 양식에서 사용할 수 있는 필드를 업데이트합니다. 빨간색 별표가 있는 필드는 필수입니다.
1. Submit(제출&#x200B;**)을 클릭합니다**.

   요청 양식이 닫히고 [요청] **** 영역으로 돌아갑니다.

   양식이 제출되고 다음 상황이 발생합니다.

   * 요청 양식이 승인과 연결되지 않은 경우 요청이 Workfront 요청 영역의 제출됨 섹션에 있는 계획 탭에 추가되고 양식과 연결된 레코드 종류에 새 레코드가 추가됩니다.

   * 요청 양식이 승인과 연결된 경우 요청이 Workfront 요청 영역의 제출됨 섹션에 있는 계획 탭에 추가됩니다. 새 레코드는 모든 승인자가 승인한 후에만 레코드 종류 페이지 에 추가됩니다.

     자세한 내용은 요청 양식[에 승인 추가를 참조하십시오](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     ![통합 작업 과정 계획 탭 토글이 있는 요청 영역](assets/requests-area-with-toggle-for-unified-workflow-planning-tab-open.png)

     >[!IMPORTANT]
     >
     >하나 이상의 작업 영역 액세스 권한이 있는 모든 사용자는 요청 영역에서 계획 탭 을 볼 수 있습니다. 사용자 또는 다른 사용자가 최소한 보기 권한이 있는 작업 영역에 제출한 요청만 볼 수 있습니다. Workfront 관리자는 시스템의 모든 작업 영역 영역에 제출된 모든 요청을 볼 수 있습니다.

   * 요청은 소유자, 승인자 및 작업 영역에 대한 최소한 보기 권한이 있는 사용자에게만 표시됩니다.

   * 요청이 성공적으로 제출되었거나 검토를 위해 전송되었다는 인앱 및 이메일 알림 수신.
   * 요청 양식이 승인과 연결된 경우 승인자는 요청을 검토하고 승인하기 위한 인앱 및 이메일 알림을 받습니다.

     >[!NOTE]
     >
     >이메일 및 인앱 알림은 조직의 Workfront 인스턴스 가 Adobe Systems 통합 경험에 온보딩된 경우에만 표시됩니다.
     >
     >이메일 확인 또는 승인 알림에 요청 링크가 있습니다.

1. (선택 사항) 확인 메시지에서 요청&#x200B;**보기를 클릭하여**&#x200B;요청을 열거나 X **아이콘을 클릭하여**&#x200B;확인을 닫습니다.

1. (선택 사항) **요청을 보려면 [요청]****영역에서 [계획**] 탭 을 클릭합니다.
계획 요청 양식에 제출된 보기 액세스 권한이 있는 모든 요청이 목록에 표시됩니다.
1. (선택 사항) 다음 중 하나를 수행합니다.

   * 필터를&#x200B;**클릭하고**&#x200B;계획 탭에서 보려는 요청에 대한 조건을 추가하기 시작합니다.

     ![계획 요청 탭에서 필터 편집](assets/filters-editing-box-in-requests-planning-tab.png)

     다음 필드를 기준으로 필터링할 수 있습니다.

      * **작업 영역**: 요청 양식이 연결된 작업 영역입니다.
      * **레코드 종류**: 요청 양식이 연결된 레코드 종류입니다.
      * **시작 날짜**: 요청 제출 날짜입니다.
      * **요청 양식**: 요청을 제출하는 데 사용되는 요청 양식의 이름입니다.
      * **상태**: 요청의 상태입니다.
      * **입력자**: 요청을 추가한 사용자 이름입니다. Workfront **외부의 누군가가 요청 을 추가한 경우 입력자** 필드에 가 표시됩니다 `N/A`.

        여러 필터를 And **또는** Or **로**조인할 수 있습니다.
필터 조건을 추가하면 요청 목록이 자동으로 필터링됩니다.

   * 열을&#x200B;**클릭하고**&#x200B;요청 목록에서 열을 숨기기, 표시 또는 다시 정렬합니다.

     >[!TIP]
     >
     >더 이상 열을 추가할 수 없습니다.
     >
     >제목&#x200B;**필드는**&#x200B;표시할 수 없습니다.

     ![](assets/columns-editing-box-in-requests-planning-tab.png)


1. 목록에서 요청 이름을 클릭합니다.

   요청 세부 사항 페이지 페이지가 열립니다.

   ![요청 세부 사항 페이지](assets/request-details-page.png)


1. (조건부) 요청 양식이 승인과 연결되어 있지 않거나 요청 승인된 경우 요청 이름을 클릭한 다음 레코드&#x200B;**필드에서**&#x200B;레코드 이름을 클릭합니다.

   레코드의 페이지 가 Workfront Planning에서 열립니다.

   >[!TIP]
   >
   >* 레코드의 기본 필드가 요청 양식에서 업데이트되지 않은 경우 요청의 레코드 필드에 있는 레코드 이름이 제목&#x200B;**없음으로**&#x200B;표시됩니다.
   >
   >* 요청 양식이 승인과 연결된 경우 승인을 받아야 요청 페이지에서 레코드에 액세스할 수 있습니다.

1. (선택 사항) 레코드 유형의&#x200B;**이름을**&#x200B;클릭합니다.

   레코드 유형 페이지 가 Workfront Planning에서 열립니다.

## 공유 링크에서 요청 양식으로 Workfront Planning에 요청 제출

1. Workfront Planning 레코드 유형에서 나와 공유된 링크 로 이동합니다.

1. 양식에서 사용 가능한 필드를 업데이트합니다. 별표가 있는 필드는 필수입니다.

   >[!TIP]
   >
   >   **제목** 필드를 사용할 수 있는 경우 요청 제출 후 Workfront Planning에 표시되지 않습니다.
   >
   >Workfront Planning의 레코드 유형에 새 레코드가 추가될 때 새 레코드를 식별할 수 있도록 요청 시 가능한 한 많은 필드를 업데이트하는 것이 좋습니다.

1. Submit(제출&#x200B;**)을 클릭합니다**.

   양식이 제출되고 다음 상황이 발생합니다.

   * 요청 양식이 승인과 연결되지 않은 경우 요청이 Workfront 요청 영역의 제출됨 섹션에 있는 계획 탭에 추가되고 양식과 연결된 레코드 종류에 새 레코드가 추가됩니다.

   * 요청 양식이 승인과 연결된 경우 요청이 Workfront 요청 영역의 제출됨 섹션에 있는 계획 탭에 추가됩니다. 새 레코드는 모든 승인자가 승인한 후에만 레코드 종류 페이지 에 추가됩니다.

     자세한 내용은 요청 양식[에 승인 추가를 참조하십시오](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     ![요청의 계획 탭](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     >하나 이상의 작업 영역 액세스 권한이 있는 모든 사용자는 요청 영역에서 계획 탭 을 볼 수 있습니다. 사용자 또는 다른 사용자가 최소한 보기 권한이 있는 작업 영역에 제출한 요청만 볼 수 있습니다. Workfront 관리자는 시스템의 모든 작업 영역 영역에 제출된 모든 요청을 볼 수 있습니다. <!--ensure this is correct; asking team in slack-->

   * 요청이 성공적으로 제출되었거나 검토를 위해 전송되었다는 인앱 및 이메일 알림 수신.
   * 요청 양식이 승인과 연결된 경우 승인자는 요청을 검토하고 승인하기 위한 인앱 및 이메일 알림을 받습니다.

     >[!NOTE]
     >
     >이메일 및 인앱 알림은 조직의 Workfront 인스턴스 가 Adobe Systems 통합 경험에 온보딩된 경우에만 표시됩니다.

   * <span class="preview"> 요청 요청이 승인되고 레코드가 생성되면 승인자 및 승인 날짜 필드에는 레코드의 승인에 대한 정보가 표시됩니다.</span>

1. (선택 사항) 요청&#x200B;**보기 클릭하여** Workfront에서 요청 엽니다.

   <!--Or-->

   <!--Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.-->

1. (선택 사항) Planning **탭>**>**주 메뉴** 요청을&#x200B;**클릭하여**&#x200B;요청 확인한 후 요청 이름을 클릭합니다.

   요청 세부 사항 페이지 페이지가 열립니다.

   ![요청 세부 사항 페이지](assets/request-details-page.png)

1. (조건부) 요청 양식이 승인과 연결되어 있지 않거나 요청 승인된 경우 요청 이름을 클릭한 다음 레코드&#x200B;**필드에서**&#x200B;레코드 이름을 클릭합니다.

   레코드의 페이지 가 Workfront Planning에서 열립니다.

   >[!TIP]
   >
   >* 레코드 이름이 요청 양식에 추가되지 않은 경우 요청의 레코드 필드에 있는 레코드 이름이 제목&#x200B;**없음으로**&#x200B;표시됩니다.
   >
   >* 요청 양식이 승인과 연결된 경우 승인을 받아야 요청 페이지에서 레코드에 액세스할 수 있습니다.

1. (선택 사항) 레코드 유형의&#x200B;**이름을**&#x200B;클릭합니다.

   레코드 유형 페이지 가 Workfront Planning에서 열립니다.




