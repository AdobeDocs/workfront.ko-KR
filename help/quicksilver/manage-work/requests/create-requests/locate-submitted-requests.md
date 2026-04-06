---
product-area: requests
navigation-topic: create-requests
title: 제출된 요청 보기
description: 귀하 또는 다른 사람이 제출한 요청 또는 제출한 적이 없고 초안으로 저장된 요청을 볼 수 있는 Adobe Workfront 영역에 대해 알아봅니다.
author: Alina
feature: Requests
topic: Collaboration
role: User
exl-id: cfa2383a-9594-4867-9b48-11b8ea281486
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: ca8f1375d641531eaf11e3889ccb67a6fbe1788f
workflow-type: tm+mt
source-wordcount: '1441'
ht-degree: 2%

---

# 제출된 요청 보기

<!--
Remove production and preview references at release
-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

귀하 또는 다른 사람이 제출한 요청 또는 시작했지만 제출하지 않은 요청을 볼 수 있습니다. 완료되지 않은 요청은 초안으로 저장됩니다.

Adobe Workfront의 다음 영역에서 제출된 요청을 찾을 수 있습니다.

* Workfront의 요청 영역
* 홈의 내 요청 위젯

요청 영역에는 보기를 선택한 방법에 따라 다음 요청이 표시됩니다.

* 기존 경험을 사용할 때 Workfront 요청
* 새 경험을 사용할 때 Workfront 및 Planning 요청이 함께 표시됩니다.

  >[!NOTE]
  >
  >* 자신의 초안 요청만 볼 수 있습니다.
  >* 새 요청 경험에서 제출된 요청과 초안이 동일한 목록에 있습니다.
  >* 기존 경험에서 생성된 초안은 새 요청 경험에 표시되지 않습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>모든 Adobe Workfront 또는 Adobe Workflow 패키지</p> 
   <p>모든 Adobe Workfront Planning 패키지</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>기여자 이상</p>
   <p>요청 이상</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td><p>문제에 대한 액세스 편집</p></td> 
  </tr>
  <tr>
   <td role="rowheader">개체 권한</td> 
   <td><p>요청에 대한 권한 이상 보기</p></td> 
  </tr> 
  <!--
  tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
  </tr> 
  -->
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 요청 영역에서 제출된 요청 보기

요청 영역 또는 홈의 내 요청 위젯에서 제출된 요청을 볼 수 있습니다.

내 요청에 대한 자세한 내용은 [내 요청 위젯 사용](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)을 참조하세요.

제출된 요청 보기는 새 요청 경험을 사용하는지 아니면 기존 요청 경험을 사용하는지에 따라 다릅니다.

* [새 요청 경험에서 제출된 요청 보기](#view-submitted-requests-in-the-new-requesting-experience)
* [기존 요청 경험에서 제출된 요청 보기](#view-submitted-requests-in-the-legacy-requesting-experience)

### 새 요청 경험에서 제출된 요청 보기

>[!NOTE]
>
>* Workfront Planning이 있는 경우 Workfront 및 Planning 요청이 동일한 목록에 나타납니다. Workfront 요청은 `Issue`개체 유형&#x200B;**열에 값**&#x200B;을(를) 표시합니다.
>* 기본적으로 요청 영역의 목록에 최대 50개의 요청이 표시됩니다. 더 많은 요청을 보려면 목록 맨 아래로 스크롤합니다.

홈의 요청 영역 및 내 요청 위젯에서 제출된 요청을 볼 수 있습니다.

>[!NOTE]
>
>새 요청 환경을 활성화하면 다음 객체에는 요청 영역 및 내 요청 위젯의 요청 목록에 있는 링크가 있습니다.
>
>* 제목 필드의 Planning 및 Workfront 요청.
>* 생성된 객체 필드의 Planning 요청에서 생성된 Planning 레코드.
>* 미리 보기 환경의 만들어진 개체 필드에 있는 Workfront 요청에서 전환된 <span class="preview">Workfront 작업 및 문제. </span>

사용자 또는 다른 사용자가 새 요청 경험에서 제출한 요청을 보려면 다음 작업을 수행하십시오.

{{step1-to-requests}}

1. 화면 오른쪽 상단의 **새 경험 사용** 설정이 켜져 있는지 확인하십시오.

   요청 목록이 표시됩니다.

1. (선택 사항) 요청을 검색하려면 목록의 오른쪽 위 모서리에 있는 검색 막대에 입력을 시작합니다. 입력하면 검색 결과가 표시됩니다.
1. (선택 사항) 정보가 요청 목록에 표시되는 방식을 관리하려면 목록에 대해 다음 보기 요소를 갱신합니다.

   * 보기
   * 필터
   * 열

   <div class="preview">

   * **그룹화**
   * 셀 서식 지정
   * 행 높이

   </div>

   요청 목록에서 정보를 관리하는 방법에 대한 자세한 내용은 [고급 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)을 참조하십시오.

1. (선택 사항) **상태** 열을 확인하여 요청 상태를 확인합니다. 새 요청 경험에서 사용할 수 있는 상태는 다음과 같습니다.

   * **초안**: 이 요청은 아직 제출되지 않았습니다.
   * **검토 보류 중**: (Planning만 해당) 이 요청에는 승인자가 있으며 승인자 중 해당 요청을 연 사람이 없습니다.
   * **검토 중**: (계획만 해당) 이 요청에는 승인자가 있으며 한 명 이상의 승인자가 요청을 열었지만 결정된 사항이 없습니다.
   * **거부됨**: (Planning만 해당) 이 요청에는 승인자가 있으며 거부되었습니다. 이 요청은 레코드를 만들지 않습니다.
   * **진행 중**:
      * Workfront 요청: 요청이 전환되었으며 작업이 진행 중입니다.
      * Workfront Planning 요청: 요청 완료는 특정 계획 필드에 매핑되며 필드 값이 아직 완료 값과 일치하지 않습니다.

        자세한 내용은 Adobe Workfront Planning에서 요청 양식 만들기 및 관리 문서에서 [구성 세부 정보 설정](/help/quicksilver/planning/requests/create-request-form.md#set-up-configuration-details)을 참조하십시오.
   * **완료**: 요청이 완료되었습니다.

### 기존 요청 경험에서 제출된 요청 보기

귀하 또는 다른 사용자가 이전 요청 경험에서 제출한 요청을 보려면 다음을 수행하십시오.

{{step1-to-requests}}

1. (조건부) 조직에서 Workfront Planning 패키지를 구입한 경우 **Workfront** 탭을 클릭하여 Workfront 요청을 봅니다.
1. 제출된 모든 요청을 보려면 왼쪽 패널의 **제출됨**&#x200B;을 클릭합니다.

   최대 2000개의 요청을 볼 수 있으며 여러 페이지에 표시될 수 있습니다.

   >[!TIP]
   >
   >제출된 요청 목록의 열은 사용자 정의할 수 없습니다.

   ![제출된 새 목록](assets/nwe-submitted-requests-new-list-350x57.png)


1. 기본적으로 다음 열이 표시됩니다.

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">이름</td> 
         <td> <p>요청의 이름입니다.</p> <p>요청 이름을 클릭하여 엽니다. </p> <p><b>팁</b>

   작업 또는 프로젝트로 전환할 때 문제가 유지되지 않으면 문제의 이름이 흐리게 표시되어 더 이상 클릭할 수 없습니다. 문제 변환에 대한 자세한 내용은 <a href="../../../manage-work/issues/convert-issues/convert-issues.md" class="MCXref xref">Adobe Workfront의 문제 변환 개요</a>를 참조하십시오. </p> </td>
   </tr> 
      <tr> 
         <td role="rowheader">전환 대상:</td> 
         <td> <p>요청이 전환된 작업 또는 프로젝트일 수 있는 해결 중 오브젝트의 이름. </p> <p>작업 또는 프로젝트의 이름을 클릭하여 엽니다. </p> <p>요청이 전환되지 않은 경우 이 필드는 비어 있습니다. </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader">경로</td> 
         <td>요청이 원래 제출된 요청 대기열, 주제 그룹 및 대기열 주제의 이름입니다. </td> 
      </tr> 
      <tr> 
         <td role="rowheader">상태</td> 
         <td>요청 또는 해결 중 오브젝트(작업 또는 프로젝트)의 현재 상태</td> 
      </tr> 
      <tr> 
         <td role="rowheader">입력 일자</td> 
         <td>요청이 제출된 날짜 또는 전환 시 요청이 삭제된 경우 해결 중 오브젝트가 생성된 날짜입니다. </td> 
      </tr> 
      <tr> 
         <td role="rowheader">마지막 업데이트 날짜</td> 
         <td> <p>요청이 마지막으로 업데이트된 날짜.</p> <p>Submitted 요청 목록은 기본적으로 이 필드별로 정렬됩니다. </p> </td> 
      </tr> 
      </tbody> 
      </table>

1. (선택 사항) 정렬할 열의 헤더를 클릭합니다.

   >[!TIP]
   >
   >제출된 요청 목록에서 멀리 이동하면 선택한 정렬 옵션이 유지됩니다.

1. (선택 사항) 목록에서 요청을 선택한 다음 **요약 열기** 아이콘 ![텍스트가 있는 요약 열기](assets/open-summary-with-text-nwe.png)를 클릭하여 요약 패널을 열고 요청에 대한 추가 정보를 표시하거나 설명, 문서를 추가하거나 할당합니다. 요약 패널에 대한 자세한 내용은 [요약 개요](../../../workfront-basics/the-new-workfront-experience/summary-overview.md)를 참조하십시오.

   >[!TIP]
   >
   >요약 패널이 이미 열려 있는 경우 요약 열기 아이콘이 요약 닫기로 변경됩니다.

1. (선택 사항 및 조건부) 오른쪽 상단의 **X** 아이콘 또는 **요약 닫기** 아이콘 ![텍스트가 있는 요약 닫기](assets/close-summary-with-text-nwe.png)를 클릭하여 요약 패널을 닫습니다.

   문제가 작업 또는 프로젝트로 전환되고 전환 프로세스에서 문제가 삭제된 경우 요약 패널이 비어 있습니다. 문제 변환에 대한 자세한 내용은 [Adobe Workfront의 문제 변환 개요](../../../manage-work/issues/convert-issues/convert-issues.md)를 참조하십시오.

1. 목록의 오른쪽 상단에 있는 **필터 아이콘** ![필터 아이콘](assets/filter-nwepng.png)에서 아래 표에 나열된 필터를 선택하십시오.

   >[!TIP]
   >
   >요청 영역의 제출됨 섹션에서 필터를 수정할 수 없습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">모두</td> 
      <td>상태 또는 제출한 사람에 관계없이 모든 제출된 요청.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">열기</td> 
      <td> <p>누가 제출했는지에 상관없이 현재 열려 있는 모든 제출된 요청. 직접 제출하지 않은 경우 적어도 볼 수 있는 권한이 있는 요청만 여기에 표시됩니다. </p> <p>실제 완료 일자가 없거나 해결 중인 객체에 실제 완료 일자가 없는 요청은 열기 하위 탭에 나열됩니다.</p> <p><b>팁</b>

   Closed와 동일하지 않은 모든 상태에 있는 요청은 Open으로 간주됩니다.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">내 요청</td> 
      <td>상태에 관계없이 제출한 요청. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">내 진행 중 요청</td> 
      <td> <p>제출한 요청이 아직 열려 있습니다. </p> <p>실제 완료 일자가 없거나 해결 중인 객체에 실제 완료 일자가 없는 요청은 [내 진행 중인 요청] 하위 탭에 나열됩니다. </p> <p><b>팁</b>

   Closed와 동등한 상태가 아닌 요청은 Open으로 간주됩니다.</p> </td>
   </tr> 
    </tbody> 
   </table>

1. (선택 사항) 이름으로 요청을 검색하려면 목록 맨 위에 있는 **필터 페이지** 아이콘 ![검색 아이콘](assets/search-icon.png)을 클릭합니다. 목록이 검색 기준과 일치하는 결과로 업데이트됩니다.

   <!--

   1. (Conditional) To display only Workfront Request queues, search or filter for `Issue` object types.</span>
   -->

   <!--
   <li> <p>Click the <strong>Complete</strong> subtab to view requests that have been completed.</p> <p>(NOTE: this step will stay drafted even after release. We can't see Completed at this time!) <br>Requests with an Actual Completion Date or whose resolving object has an Actual Completion Date are listed in the Complete subtab.<br>Once a request receives an Actual Completion Date, it stays in the Recently Completed area for 10 business days. After that, it is moved to the Completed area. <br>For information about resolving and resolvable objects, see the article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </li>
   -->

   <!--
   <li>(Optional) Select an option from the <strong>Sort by</strong> drop-down menu to sort the requests by the following criteria:   (NOTE: this step will stay drafted even after release. We can't see Completed at this time!)  
   <ul>
   <li><strong>Assigned To</strong>: Requests are sorted alphabetically by the name of the assignee using the following criteria: 
   <ul>
   <li>All requests assigned to users are sorted first, in the order of the users' names.</li>
   <li>Requests assigned to job roles are sorted secondly, in the order of the job roles' names and are listed after all the requests assigned to users.</li>
   <li>Requests that are assigned to teams are sorted last, in the order of the teams' names and are listed after all the requests assigned to users and those assigned to job roles.</li>
   <li>All unassigned requests are listed last, in the order of their Entry Date. </li>
   </ul></li>
   <li><strong>Submitted On</strong>: Requests are sorted chronologically by the date when they were submitted.</li>
   <li><strong>Recently Updated</strong> (this is the default): Requests are sorted chronologically by the date of their last update.</li>
   <li><strong>Name</strong>: Requests are sorted alphabetically by name. </li>
   <li><strong>Priority</strong>: Requests are sorted in the order of their priority.</li>
   <li><strong>Queue</strong>: Requests are sorted alphabetically by the name of the requests queue where they were submitted. </li>
   <li><strong>Status</strong>: Requests are sorted alphabetically by their status. </li>
   </ul></li>
   -->

1. 모든 초안 요청을 보려면 **초안**&#x200B;을 클릭하십시오. Workfront은 이 폴더의 각 요청 대기열에 대해 초안을 무제한으로 저장합니다. 이미 초안이 있는 대기열 주제에 대한 새 요청을 입력하면 기존 초안을 사용하라는 메시지가 표시됩니다. 자세한 내용은 [초안에서 요청 만들기](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)를 참조하십시오.

   <!--
   Planning tab has been removed and no longer visible in legacy Requests area: 
   (Optional and conditional) If your organization purchased a Workfront Planning package, click the **Planning** tab, then click **Submitted** in the left panel to view Workfront Planning requests. 
      Use **Filters** and **Columns** to update the information in the Planning request list. 
      ![Planning tab submitted section in Requests area](assets/workfront-planning-tab-submitted-section-in-requests-area.png)
      For information, see [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md).
   -->


1. (선택 사항) **상태** 열을 확인하여 요청 상태를 확인합니다. 새 요청 경험에서 사용할 수 있는 상태는 다음과 같습니다.

   * **초안**. 이 요청은 아직 제출되지 않았습니다.
   * **진행 중**
   * **완료**


