---
product-area: projects
navigation-topic: manage-tasks
title: 작업 이동
description: Adobe Workfront에서 작업을 다른 프로젝트 또는 다른 상위 작업으로 이동할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 2%

---

# 작업 이동

<!--Audited: 5/2025-->


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


Adobe Workfront에서 다음 개체 간에 작업을 이동할 수 있습니다.

* 프로젝트에 대한 임시 작업입니다.
* 프로젝트에서 다른 프로젝트로의 작업입니다.
* 다른 프로젝트의 다른 상위 프로젝트 아래에 있는 프로젝트의 작업입니다.
* 동일한 프로젝트 내의 다른 상위 작업

작업 수준에서 작업을 이동하거나 작업 목록에서 작업을 이동할 수 있습니다.

단일 작업을 이동하거나 작업 목록에서 한 번에 여러 작업을 이동할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>새로운 기능: 표준 </p> 
 <p>또는</p>  
<p>현재: 작업 시간 이상 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 권한 관리</p> <p>작업을 추가할 수 있는 권한으로 프로젝트에 대한 상위 권한 기여</p>  </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 작업 이동에 대한 고려 사항

작업을 이동할 때는 다음 사항을 고려하십시오.

* 시스템 또는 그룹 관리자는 사용자가 설정 영역에서 작업 및 기록된 시간 문제를 이동할 수 있도록 허용 기본 설정을 구성하는 방법에 따라 기록된 시간이 있는 작업을 이동하지 못하도록 할 수 있습니다. 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)을 참조하십시오.

* 한 프로젝트에서 다른 프로젝트로 작업을 이동하면 작업 날짜가 다시 계산될 수 있습니다. 재계산에는 새 프로젝트가 사용하는 일정 및 프로젝트의 일정 시작 정보가 고려됩니다.

* 이동 프로세스 중에 작업과 연관된 일부 항목을 이동된 작업으로 이동할 수 있습니다. 그러나 기본적으로 다음 객체는 이동된 작업으로 전송됩니다.

   * 문제
   * 기록된 시간
   * 사용자 댓글
   * 사용자 정의 양식 및 사용자 정의 필드 정보
   * 하위 작업

* 기본적으로 다음 항목은 작업과 함께 이동하지 않습니다.

   * 마일스톤

## 목록에서 작업 이동

{{step1-to-projects}}

1. **프로젝트** 페이지에서 이동할 작업이 포함된 프로젝트를 선택합니다.
1. 작업 목록을 표시하려면 왼쪽 패널의 **작업**&#x200B;을(를) 클릭하십시오.
1. **플랜 모드** 아이콘 ![플랜 모드 아이콘](assets/plan-mode.png)을 클릭하고 **자동 저장** 전환이 사용하도록 설정되어 있는지 확인한 다음 이동할 작업을 선택하십시오.

   ![자동 저장 옵션](assets/autosave-icon.png)

   >[!IMPORTANT]
   >
   >**자동 저장** 전환을 사용하지 않도록 설정하면 작업을 이동할 수 없습니다.

1. (선택 사항 및 조건부) 선택한 작업을 동일한 프로젝트 내에서 이동하려면 선택한 작업을 클릭한 다음 프로젝트에서 이동하려는 위치로 끌어서 놓습니다. 작업 계층 변경 사항은 즉시 저장되고 각 작업과 연관된 정보가 작업과 함께 이동됩니다.

1. (조건부) 이동할 작업을 선택하고 다음 중 하나를 수행합니다.

   * 작업 목록 맨 위에 있는 **자세히** 메뉴 ![자세히 아이콘](assets/main-more-icon.png)을 클릭한 다음 **이동**&#x200B;을 클릭합니다.
   * 선택한 작업을 마우스 오른쪽 단추로 클릭한 다음 **이동**&#x200B;을 클릭합니다.
   * 작업 하나를 선택할 때 목록에서 작업 이름 옆에 있는 **자세히** 메뉴 ![](assets/more-icon-task-list.png)을(를) 클릭한 다음 **이동**&#x200B;을(를) 클릭합니다.

   **작업 이동** 상자가 표시됩니다.

1. 이 문서의 [작업 수준에서 작업 이동](#move-a-task-at-the-task-level) 섹션에 설명된 대로 작업을 계속 이동합니다.

   <!--
   is this still accurate?!
   -->

## 작업 수준에서 작업 이동 {#move-a-task-at-the-task-level}

작업 목록에서 작업을 이동할 수 있을 뿐만 아니라 작업을 연 후 작업 수준에서 작업을 이동할 수 있습니다.

1. 검색하여 Workfront 시스템에서 작업을 찾습니다.
1. 작업 이름을 클릭하여 엽니다.
1. 작업 이름 옆에 있는 **자세히** 드롭다운 메뉴 ![자세히 아이콘](assets/main-more-icon.png)을 클릭한 다음 **이동**&#x200B;을 클릭합니다. **작업 이동** 사이드 패널이 표시됩니다.

1. (선택 사항) **작업 이름**&#x200B;을(를) 업데이트합니다. 작업이 새 위치에서 새 이름으로 이동합니다.

   >[!TIP]
   >
   >목록에서 여러 작업을 이동하도록 선택하면 **작업 이름** 필드가 흐리게 표시되어 편집할 수 없습니다. **작업 이름** 필드 위로 마우스를 가져가면 선택한 모든 작업 목록이 표시됩니다.
   >
   >
   >![작업 이름 표시](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. **대상 프로젝트 선택** 필드에 작업을 이동할 프로젝트의 이름을 입력합니다. 동일한 프로젝트 내에서 작업을 이동하려면 현재 프로젝트의 이름을 입력합니다.

   >[!TIP]
   >
   >* 프로젝트 이름은 대소문자를 구분합니다.
   >* 참조 번호 를 입력하거나 프로젝트의 ID를 입력하여 프로젝트를 검색할 수 있습니다. 이렇게 하면 이름이 동일한 프로젝트를 구별하는 데 도움이 될 수 있습니다.
   >* 100개의 프로젝트만 목록에 표시됩니다.

1. (조건부) 프로젝트에 액세스할 수 없는 경우 **액세스 요청**&#x200B;을 클릭합니다.
1. (조건부) 대상 프로젝트의 작업 중 하나에 작업을 추가할 수 있는 액세스 권한이 있는 경우 액세스 요청 없이 작업을 대상 프로젝트로 계속 이동합니다.

   ![액세스를 요청하지 않고 작업 이동](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >Workfront 관리자가 이러한 프로젝트에 작업을 추가할 수 없도록 방지하면 선택한 프로젝트가 승인 보류 중, 완료 또는 정지된 경우에도 유사한 메시지가 표시됩니다. 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

1. (선택 사항) **옵션** 섹션에서 아래 표에 나열된 항목을 선택 해제하여 이동된 작업에서 제거합니다. 기본적으로 모든 옵션이 선택되어 있습니다.

   >[!IMPORTANT]
   >
   >**옵션** 목록에서 항목을 선택 취소하면 데이터가 손실됩니다. 기존 작업의 정보가 제거되어 복구할 수 없습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">모두 선택</td> 
      <td>작업을 새 위치로 이동할 때 작업에서 모든 정보를 제거하려면 이 옵션을 선택 취소합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">제한</td> 
      <td> <p>작업 제한 사항은 프로젝트 일정 모드 설정에 따라 가능한 한 빨리 또는 가능한 한 늦게 설정됩니다.</p> <p> 선택하면 작업의 현재 제한 사항이 작업과 함께 전송됩니다. </p> 
      <p>주: 일자별 제한조건이 있는 태스크를 다른 프로젝트로 이동하거나 복사할 때 태스크의 제한조건 일자가 신규 프로젝트 일자를 벗어나면 태스크 제한조건이 가능한 한 빨리 또는 가능한 한 늦게 변경되거나 프로젝트의 계획된 시작 일자 또는 계획된 완료 일자가 조정됩니다.

   다음은 날짜별 제한의 예입니다.
   <ul>
      <li> 시작 일자</li>
      <li> 다음까지 완료</li>
      <li> 다음 이후에 시작</li>
      <li> 다음 이전에 시작</li>
      </ul>

   자세한 내용은 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">작업 제한 개요</a>를 참조하십시오.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">할당</td> 
      <td> <p>모든 할당이 작업에서 제거됩니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">승인 진행</td> 
      <td>모든 승인 프로세스가 작업에서 제거됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">진행</td> 
      <td>작업 상태가 신규로 설정됩니다. 그렇지 않으면 기존 작업 상태가 유지됩니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">재무 정보</td> 
      <td>작업의 재무 정보가 제거되고 Workfront이 작업 비용 유형을 비용 없음으로 업데이트하고 작업 수익 유형을 청구 불가능으로 업데이트합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">모든 전임 작업</td> 
      <td> <p>이 옵션을 선택하면 작업을 다른 프로젝트로 이동할 때 종속성이 프로젝트 간 전임 작업이 됩니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">문서</td> 
      <td> <p>작업에 첨부된 문서가 이동된 작업으로 전송되지 않습니다. 여기에는 버전, 증명 및 연결된 문서가 포함됩니다.</p> <p>여기에는 문서 승인이 포함되지 않습니다. 작업을 이동할 때 문서 승인은 이동할 수 없습니다.</p> 
      <p>참고: 작업과 함께 문서를 이동하지 않도록 선택하면 문서가 삭제되고 30일 동안 휴지통에 보관됩니다. 관리자는 이를 복원할 수 있으며 이동된 작업에 복원됩니다. </p>

   <p>작업을 이동한 후 삭제하면 복원된 문서가 복원한 관리자의 사용자 페이지에 있는 문서 영역에 배치됩니다.</p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">미리 알림</td> 
      <td>작업 미리 알림이 이동된 작업으로 전송되지 않습니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">경비</td> 
      <td>작업에 기록된 경비는 이동된 작업으로 이전되지 않습니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">권한</td> 
      <td> <p>Workfront은 작업의 공유 목록에 표시되는 모든 엔티티의 이름을 제거합니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>



1. (선택 사항) **상위 선택** 섹션에서 이동된 작업의 상위가 될 대상 프로젝트의 작업을 선택합니다.

   >[!TIP]
   >
   >목록에서 여러 작업을 이동하도록 선택할 때 선택한 모든 작업이 선택한 상위의 하위 작업이 됩니다.

   다음 중 하나를 수행하여 상위 항목을 선택합니다.

   * 작업 목록에서 프로젝트 계획의 상위 항목 중 하나를 선택합니다.
   * 검색 아이콘 ![검색 아이콘](assets/search-icon.png)을 클릭하고 이름별로 상위 작업을 검색합니다.

   작업이 목록에 표시됩니다.

   ![검색 기능이 있는 작업을 이동할 때 상위 작업 선택 &#x200B;](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

   >[!NOTE]
   >
   >상위 작업을 선택하지 않으면 작업이 하위 작업이 아닌 기본 작업으로 이동되고 대상 프로젝트의 작업 목록 끝에 배치됩니다.

1. **작업 이동**&#x200B;을 클릭합니다. 작업이 상위 작업 또는 프로젝트의 마지막 작업으로 하위 작업으로 지정된 프로젝트로 이동합니다.
