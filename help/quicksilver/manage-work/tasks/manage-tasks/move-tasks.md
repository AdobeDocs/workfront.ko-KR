---
product-area: projects
navigation-topic: manage-tasks
title: 작업 이동
description: 작업을 다른 프로젝트 또는 Adobe Workfront의 다른 상위 작업으로 이동할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: 23a08c929b0a227c7a555af70ff731ef2df7a179
workflow-type: tm+mt
source-wordcount: '1360'
ht-degree: 2%

---

# 작업 이동

다음 개체 간에 Adobe Workfront에서 작업을 이동할 수 있습니다.

* 프로젝트에 대한 임시 작업입니다.
* 프로젝트에서 다른 프로젝트로 하는 작업입니다.
* 다른 프로젝트의 다른 부모 아래에 있는 프로젝트의 작업입니다.
* 동일한 프로젝트 내의 다른 상위 항목에 있는 작업입니다.

작업 수준에서 작업을 이동하거나 작업 목록에서 작업을 이동할 수 있습니다.

## 액세스 요구 사항

이 문서에서 작업을 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 권한 관리</p> <p>작업을 추가할 수 있는 기능을 사용하여 프로젝트에 대한 권한을 더 이상 부여하십시오</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 목록에서 작업 이동

작업 목록에 표시된 작업을 이동하려면 다음을 수행합니다.

1. 이동할 작업이나 작업이 포함된 프로젝트로 이동합니다.
1. 클릭 **작업** 왼쪽 패널에 작업 목록을 표시합니다.
1. 다음을 확인합니다. **자동 저장** 토글이 활성화되면 이동할 작업이나 작업을 선택합니다.

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >작업을 이동할 때 **자동 저장** 토글이 비활성화되어 있습니다.

1. (선택 사항 및 조건부) 선택한 작업을 동일한 프로젝트 내에서 이동하려면 선택한 작업을 클릭하고 선택한 작업을 드래그하여 프로젝트에서 이동하려는 위치에 놓습니다.

   작업을 프로젝트의 올바른 위치에 놓으면 작업 계층에 대한 변경 사항이 즉시 저장됩니다. 각 작업과 연관된 모든 정보는 작업과 함께 이동됩니다.

1. (조건부) 이동할 작업을 선택하고 다음 중 하나를 수행합니다.

   * 을(를) 클릭합니다. **자세히** 메뉴 ![](assets/qs-more-menu.png) 작업 목록의 맨 위에서 을 클릭합니다. **이동 위치**.
   * 선택한 작업을 마우스 오른쪽 단추로 클릭한 다음 **이동 위치**.
   * 작업 하나를 선택하면 **자세히** 메뉴 ![](assets/more-icon-task-list.png) 목록의 작업 이름 옆에 있는 **이동 위치**.

   ![](assets/move-task-in-list-nwe-350x119.png)

   작업 이동 상자가 표시됩니다

1. 섹션에 설명된 대로 작업을 계속 이동합니다 [작업 수준에서 작업 이동](#move-a-task-at-the-task-level) 이 문서에서 4단계부터 시작합니다.

   <!--
   is this still accurate?!
   -->

## 작업 수준에서 작업 이동 {#move-a-task-at-the-task-level}

작업 목록에서 작업을 이동하는 것 외에도 작업을 연 후 작업 수준에서 이동할 수도 있습니다. 

1. Workfront 시스템에서 작업을 검색하여 찾습니다.
1. 작업 이름을 클릭하여 엽니다.
1. 을(를) 클릭합니다. **자세히** 드롭다운 메뉴 ![](assets/qs-more-menu.png) 작업 이름 옆에 있는 **이동 위치**. 작업 이동 상자가 표시됩니다.

   ![](assets/move-task-at-task-level-nwe-350x222.png)

1. (선택 사항) **작업 이름**. 작업이 새 위치에 새 이름으로 이동합니다. Workfront은 작업의 원래 이름을 기록하지 않습니다.

   >[!TIP]
   >
   >이 필드는 목록에서 여러 작업을 이동할 때 흐리게 표시되어 편집할 수 없습니다. 작업 이름 필드를 마우스로 가리키면 선택한 모든 작업 목록이 표시됩니다.
   >
   >
   >![](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. 이름 입력 **대상 프로젝트** 작업을 이동할 위치 **대상 프로젝트 선택** 필드.

   동일한 프로젝트 내에서 작업을 이동하려면 현재 프로젝트의 이름을 입력합니다.

   >[!TIP]
   >
   >* 프로젝트 이름은 대/소문자를 구분합니다.
   >* 참조 번호 입력을 시작하거나 프로젝트 ID를 입력할 수도 있습니다. 이렇게 하면 이름이 같은 프로젝트를 구분하는 데 도움이 될 수 있습니다.
   >* 목록에 100개의 프로젝트만 표시됩니다.


1. (조건부) 클릭 **액세스 요청** 프로젝트에 대한 액세스를 요청하려면 선택한 프로젝트에 대한 액세스 권한이 없는 경우 선택합니다.
1. (조건부) 대상 프로젝트의 작업 중 하나에 작업을 추가할 수 있는 액세스 권한이 있으면 액세스를 요청하지 않고 작업을 선택한 대상 프로젝트로 계속 이동합니다.

   ![](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >Workfront 관리자가 이러한 프로젝트에 작업을 추가할 수 없을 때 선택한 프로젝트가 승인 보류 중, 완료 또는 사용 중지 상태인 경우 유사한 메시지가 표시됩니다. 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (선택 사항) **옵션** 왼쪽 패널에서

   또는

   아래로 스크롤하여 **옵션** 작업 이동 상자의 섹션을 선택한 다음 아래 테이블에 나열된 항목을 선택 취소하고 이동한 작업에서 제거합니다. 기본적으로 모든 옵션이 선택됩니다.

   >[!IMPORTANT]
   옵션 목록에서 항목을 선택 해제하면 데이터가 손실됩니다. 기존 작업의 정보가 제거되어 복구할 수 없습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">모두 선택</td> 
      <td>새 위치로 이동할 때 작업에서 모든 정보를 제거하려면 이 옵션을 선택 취소합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">제한</td> 
      <td> <p>작업 제약 조건은 프로젝트 예약 모드 설정에 따라 가능한 한 빨리 또는 최대한 늦게 설정됩니다.</p> <p> 선택하면 작업의 현재 제약 조건이 작업과 함께 전송됩니다. </p> 
      <p><b>메모</b>

   일자 특정 제약 조건이 있는 태스크를 다른 프로젝트로 이동하거나 복사하거나 태스크의 제약 일자가 신규 프로젝트의 일자 이외의 경우 태스크 제약은 가능한 한 빨리 또는 최대한 늦게 또는 프로젝트의 계획 시작 또는 계획 완료 일자가 조정됩니다.

   다음은 특정 날짜 제한의 예입니다.
   <ul>
      <li> 시작 일자:</li>
      <li> 다음까지 완료:</li>
      <li> 다음 이후에 시작:</li>
      <li> 다음 이전에 시작</li>
      </ul>

   작업 제한 및 작업 제한 또는 프로젝트 날짜가 영향을 받을 수 있는 방법에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">작업 제한 개요</a> 특정 제약 조건을 찾습니다.</p> </td>
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
      <td>작업 상태는 새로 만들기 입니다. 그렇지 않으면 기존 작업 상태가 유지됩니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">재무 정보</td> 
      <td>태스크의 재무 정보가 제거되고 Workfront이 태스크 원가 유형을 원가 없음으로 갱신하고 태스크 수익 유형을 청구 가능으로 갱신합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">모든 선행 작업</td> 
      <td> <p>선택하면 작업을 다른 프로젝트로 이동할 때 종속성이 프로젝트 간 전임자가 됩니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">문서</td> 
      <td> <p>작업에 첨부된 문서는 이동된 작업에 전송되지 않습니다. 여기에는 버전, 증명 및 연결된 문서가 포함됩니다.</p> <p>여기에는 문서 승인이 포함되지 않습니다. 작업을 이동할 때는 문서 승인을 이동할 수 없습니다.</p> 
      <b>메모</b>

   작업과 함께 문서를 이동하지 않도록 선택하면 문서가 삭제되고 30일 동안 휴지통에 보관됩니다. 관리자는 해당 파일을 복원할 수 있으며 이동된 작업에서 복원됩니다.

   작업이 이동한 후 삭제되면 복원된 문서가 복원되는 관리자의 사용자 페이지의 문서 영역에 배치됩니다.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">미리 알림</td> 
      <td>작업 미리 알림은 이동된 작업에 전송되지 않습니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">경비</td> 
      <td>작업에 로그된 비용은 이동된 작업에 전송되지 않습니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">권한</td> 
      <td> <p>Workfront은 작업의 공유 목록에 표시되는 모든 엔티티의 이름을 제거합니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>



1. (선택 사항) **상위 선택** 왼쪽 패널에서

   또는

   로 스크롤합니다. **상위 선택** 섹션을 선택한 다음 대상 프로젝트에서 이동된 작업의 상위 작업이 될 작업을 선택합니다.

   >[!TIP]
   목록에서 여러 작업을 이동하도록 선택하면 선택한 모든 작업이 선택한 상위의 하위 작업이 됩니다.

   다음 중 하나를 수행하여 상위를 선택합니다.

   * 작업 목록에서 프로젝트 계획에서 상위 중 하나를 선택합니다.
   * 검색 아이콘을 클릭합니다 ![검색 아이콘](assets/search-icon.png) 이름으로 상위 작업을 검색합니다.

   작업이 목록에 나타납니다.

   ![검색 기능이 있는 작업을 이동할 때 상위 작업 선택 ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. 라디오 단추를 찾은 후 상위의 라디오 단추를 선택합니다.

   상위 작업을 선택하지 않으면 작업은 하위 작업이 아닌 기본 작업으로 이동되며 대상 프로젝트의 작업 목록 끝에 배치됩니다.

1. 클릭 **작업 이동**

   또는

   클릭 **작업 이동** 목록에서 여러 작업을 선택하는 경우.
이동된 작업은 이제 지정된 프로젝트에 있으며 상위 작업의 하위 작업이거나 프로젝트의 마지막 작업입니다.
