---
product-area: requests
navigation-topic: create-requests
title: 제출된 요청 찾기
description: 본인 또는 다른 사용자가 제출한 요청이나 제출하지 않고 초안으로 저장한 요청을 찾을 수 있는 Adobe Workfront의 영역에 대해 알아봅니다.
author: Alina
feature: Work Management
exl-id: cfa2383a-9594-4867-9b48-11b8ea281486
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 1%

---

# 제출된 요청 찾기

사용자 또는 다른 사용자가 제출한 다음 유형의 요청 또는 시작했으나 제출을 완료하지 않은 요청을 찾을 수 있습니다. Adobe Workfront의 다음 영역에서 이러한 요청을 찾을 수 있습니다.

* **제출된 섹션**: 사용자 또는 다른 사용자가 제출한 모든 요청이며 적어도 보기에 액세스할 수 있습니다.
* **초안 섹션** : 시작했지만 완료되지 않았고 제출하지 않은 모든 요청. 초안 요청에 대한 자세한 내용은 [Adobe Workfront 요청 만들기 및 제출](../../../manage-work/requests/create-requests/create-submit-requests.md).

   >[!TIP]
   >
   >고유한 초안 요청만 볼 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스 개요*</td> 
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문제에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>요청 이상에 대한 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 제출된 요청 찾기

사용자 또는 다른 사용자가 제출한 요청을 찾으려면 다음을 수행하십시오.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서
1. 클릭 **제출됨** 왼쪽 패널에서 를 클릭하여 제출된 모든 요청을 확인합니다.

   최대 2000개의 요청을 볼 수 있으며 여러 페이지에 표시할 수 있습니다.

   >[!TIP]
   >
   >제출된 요청 목록에서 열을 사용자 지정할 수 없습니다.

   ![](assets/nwe-submitted-requests-new-list-350x57.png)

1. 기본적으로 다음 열이 표시됩니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td> <p>요청의 이름입니다.</p> <p>요청 이름을 클릭하여 엽니다. </p> <p><b>팁</b>

   문제가 작업 또는 프로젝트로 변환될 때 유지되지 않으면 문제 이름이 흐리게 표시되어 더 이상 클릭할 수 없습니다. 변환 문제에 대한 자세한 내용은 <a href="../../../manage-work/issues/convert-issues/convert-issues.md" class="MCXref xref">Adobe Workfront의 변환 문제 개요</a>. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">전환 대상:</td> 
      <td> <p>요청을 변환한 작업 또는 프로젝트일 수 있는 해결 객체의 이름입니다. </p> <p>작업 또는 프로젝트의 이름을 클릭하여 엽니다. </p> <p>요청이 변환되지 않은 경우 이 필드는 비어 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">경로</td> 
      <td>원래 요청이 제출된 요청 큐, 항목 그룹 및 큐 항목의 이름입니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">상태</td> 
      <td>해결 객체(작업 또는 프로젝트)의 요청 또는 현재 상태</td> 
     </tr> 
     <tr> 
      <td role="rowheader">시작 날짜</td> 
      <td>요청을 제출한 날짜나 요청을 변환할 때 삭제한 경우 확인 개체가 생성된 날짜입니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">마지막 업데이트 날짜</td> 
      <td> <p>요청이 마지막으로 업데이트된 날짜입니다.</p> <p>Submitted 요청 목록은 기본적으로 이 필드로 정렬됩니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 열 헤더를 클릭하여 정렬합니다.

   >[!TIP]
   >
   >제출된 요청 목록에서 멀리 탐색하면 선택한 정렬 옵션이 유지됩니다.

1. (선택 사항) 목록에서 요청을 선택한 다음 **요약 열기** 아이콘 ![](assets/open-summary-with-text-nwe.png) 요약 패널을 열고 요청에 대한 추가 정보를 표시하려면 주석, 문서를 추가하거나 지정합니다. 요약 패널에 대한 자세한 내용은 [요약 개요](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

   >[!TIP]
   >
   >요약 패널이 이미 열려 있으면 요약 열기 아이콘이 요약 닫기로 변경됩니다.

1. (선택 사항 및 조건부) **X** 오른쪽 위 모서리나 **요약 닫기** 아이콘 ![](assets/close-summary-with-text-nwe.png) 을 클릭하여 요약 패널을 닫습니다.

   문제가 작업 또는 프로젝트로 변환되고 변환 프로세스에서 문제가 삭제된 경우 요약 패널이 비어 있습니다. 변환 문제에 대한 자세한 내용은 [Adobe Workfront의 변환 문제 개요](../../../manage-work/issues/convert-issues/convert-issues.md).

1. 에서 **필터 아이콘** ![](assets/filter-nwepng.png) 목록의 오른쪽 위에서 아래 표에 나열된 필터 중 하나를 선택합니다.

   >[!TIP]
   >
   >요청 영역에서 필터를 수정할 수 없습니다. 또한 요청 영역의 보기를 수정하거나 변경하는 옵션이 없습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">모두</td> 
      <td>상태 또는 제출자에 관계없이 제출된 모든 요청.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">열기</td> 
      <td> <p>제출한 사람에 관계없이 현재 열려 있는 모든 제출된 요청입니다. 직접 제출하지 않은 경우 여기에 표시할 수 있는 권한 이상의 요청만 있습니다. </p> <p>실제 완료 일자가 없거나 객체 해결에 실제 완료 일자가 없는 요청은 개설 하위 탭에 나열됩니다.</p> <p><b>팁</b>

   Closed와 같지 않은 모든 상태에 있는 요청은 열린 것으로 간주됩니다.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">내 요청</td> 
      <td>상태에 관계없이 제출한 요청. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">내 열린 요청</td> 
      <td> <p>아직 열려 있는 요청을 제출했습니다. </p> <p>실제 완료 일자가 없거나 객체 해결에 실제 완료 일자가 없는 요청은 내 개설 요청 하위 탭에 나열됩니다. </p> <p><b>팁</b>

   Closed와 같은 상태에 있지 않은 요청은 열린 것으로 간주됩니다.</p> </td>
   </tr> 
    </tbody> 
   </table>

1. (선택 사항) **페이지 필터링** 아이콘 ![](assets/search-icon.png) 목록의 맨 위에서 이름별로 요청을 검색합니다. 목록이 검색 기준과 일치하는 결과로 업데이트됩니다.

   <!--
   <li value="9" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Click the&nbsp;<strong>Complete</strong> subtab to view requests that have been completed.</p> <p>(NOTE: this step will stay drafted even after release. We can't see Completed at this time!) <br>Requests with an Actual Completion Date or whose resolving object has an Actual Completion Date are listed in the Complete subtab.<br>Once a request receives an Actual Completion Date, it stays in the Recently Completed area for 10 business days. After that, it is moved to the Completed area. <br>For information about resolving and resolvable objects, see the article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </li>
   -->

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Optional) Select an option from the <strong>Sort by</strong> drop-down menu to sort the requests by the following criteria:&nbsp; &nbsp;(NOTE:&nbsp;this step will stay drafted even after release. We can't see Completed at this time!) &nbsp;
   <ul>
   <li><strong>Assigned To</strong>: Requests are sorted alphabetically by the name of the assignee using the following criteria:&nbsp;
   <ul>
   <li>All requests assigned to users are sorted first, in the order of the users' names.</li>
   <li>Requests assigned to job roles are sorted secondly, in the order of the job roles' names and are listed after all the requests assigned to users.</li>
   <li>Requests that are assigned to teams are sorted last, in the order of the teams' names and are listed after all the requests assigned to users and those assigned to job roles.</li>
   <li>All unassigned requests are listed last, in the order of their Entry Date. </li>
   </ul></li>
   <li><strong>Submitted On</strong>: Requests are sorted chronologically by the date when they were submitted.</li>
   <li><strong>Recently Updated</strong> (this is the default): Requests are sorted chronologically by the date of their last update.</li>
   <li><strong>Name</strong>: Requests are sorted alphabetically by name.&nbsp;</li>
   <li><strong>Priority</strong>: Requests are sorted in the order of their priority.</li>
   <li><strong>Queue</strong>: Requests are sorted alphabetically by the name of the requests queue where they were submitted.&nbsp;</li>
   <li><strong>Status</strong>: Requests are sorted alphabetically by their status.&nbsp;</li>
   </ul></li>
   -->

1. 클릭 **초안** 모든 초안 요청을 조회하려면 Workfront은 이 폴더의 각 요청 큐에 대해 무제한으로 초안을 저장합니다. 이미 초안이 있는 큐 항목에 대한 새 요청을 입력하면 기존 초안을 사용하라는 메시지가 표시됩니다. 자세한 내용은 [초안에서 요청 만들기](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).

 

 

 
