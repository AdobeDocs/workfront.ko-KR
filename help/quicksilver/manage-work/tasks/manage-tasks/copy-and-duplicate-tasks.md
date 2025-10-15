---
product-area: projects
navigation-topic: manage-tasks
title: 작업 복사 및 복제
description: 프로젝트에서 다른 프로젝트로 작업을 복사하거나 동일한 프로젝트 내에서 작업을 복제할 수 있습니다.
author: Alina
feature: Work Management
exl-id: daf89062-cf58-4c39-83ff-727d969a9630
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '1679'
ht-degree: 1%

---

# 작업 복사 및 복제

프로젝트에서 다른 프로젝트로 작업을 복사하거나 동일한 프로젝트 내에서 작업을 복제할 수 있습니다.

한 번에 하나 이상의 작업 또는 상위 작업을 복사하거나 복제할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>표준</p> 
   <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 권한 관리</p> <p>프로젝트에 대한 상위 권한 기여</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a task</p> <p>Contribute or higher permissions to the project</p> 
   <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 작업 복사 시 고려 사항

작업을 복사할 때에는 다음 사항을 고려하십시오.

* 한 프로젝트에서 다른 프로젝트로 작업을 복사할 때 작업 날짜가 다시 계산될 수 있습니다. 재계산에는 새 프로젝트가 사용하는 일정 및 프로젝트의 일정 시작 정보가 고려됩니다.
* 사용자 정의 양식이 작업과 함께 복사됩니다. 사용자 정의 필드의 정보는 작업을 복사할 때 사용자 정의 데이터를 복사하도록 선택한 경우에만 복사된 작업으로 전송됩니다.
* 복사 프로세스 중에 작업과 연관된 일부 항목을 복사된 작업에 복사하도록 선택할 수 있습니다. 그러나 기본적으로 다음 객체는 복사된 작업으로 전송되지 않습니다.
   * 문제
   * 기록된 시간
   * 사용자 댓글 <!--not sure about this, enable only if requested by users and verified by Product: System activity comments transfer to the new task if they relate to information that you specifically select to be copied. For example, if you select to copy Expenses to the new task, system comments that identify adding expenses to the task will transfer to the copied task. -->
* 다음 항목은 기본적으로 복사된 작업으로 이동합니다.

   * 마일스톤은 복사된 작업으로 전송되고 원래 작업에서 제거됩니다.
   * 하위 작업이 새 작업으로 전송됩니다.

* 한 번에 하나의 작업을 복사할 수도 있고 목록에서 작업을 편집할 때 한 번에 여러 작업을 복사할 수도 있습니다.

## 목록의 작업 복사 {#copy-tasks-in-a-list}

1. 복사할 작업이 포함된 프로젝트로 이동합니다.

   또는

   작업 보고서로 이동합니다.

1. (조건부) 작업이 포함된 프로젝트를 연 경우 왼쪽 패널에서 **작업**&#x200B;을 클릭합니다.
1. **플랜 모드** 아이콘 ![](assets/qs-list-mode-or-save-mode-icon-small.png)을 클릭하고 **자동 저장** 옵션이 활성화되어 있는지 확인하십시오.

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >변경 사항을 자동으로 저장할 때만 목록에서 작업을 복사할 수 있습니다. 작업을 편집할 때 옵션을 저장하는 방법에 대한 자세한 내용은 [목록에서 작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)을 참조하십시오.

1. 복사할 작업을 선택하고 다음 중 하나를 수행합니다.

   * 작업 목록 맨 위에 있는 **추가 메뉴**&#x200B;를 클릭한 다음 **복사 위치**&#x200B;를 클릭합니다.
   * 선택한 작업을 마우스 오른쪽 단추로 클릭한 다음 **복사 위치**&#x200B;를 클릭합니다.
   * 작업 하나를 선택할 때 목록에서 작업 이름 옆에 있는 **자세히** 메뉴 ![](assets/more-icon-task-list.png)을(를) 클릭한 다음 **복사 위치**&#x200B;를 클릭합니다.

   ![](assets/copy-task-in-list-nwe-350x131.png)

1. 4단계부터 [작업 수준에서 작업 복사](#copy-a-task-at-the-task-level) 섹션에 설명된 대로 작업 복사를 계속하십시오.

   <!--
      (NOTE: is this still accurate?!)
   -->

## 작업 수준에서 작업 복사 {#copy-a-task-at-the-task-level}

작업 목록에서 작업을 복사할 수 있을 뿐만 아니라 작업을 연 후에도 복사할 수 있습니다.

1. 검색하여 Workfront 시스템에서 작업을 찾습니다.
1. 작업 이름을 클릭하여 엽니다.
1. 작업 이름 옆에 있는 **자세히** 드롭다운 메뉴 ![](assets/qs-more-menu.png)을(를) 클릭한 다음 **복사 위치**&#x200B;를 클릭합니다.

   ![](assets/taskcopy-to-at-the-task-level-nwe-350x200.png)

   작업 복사 상자가 표시됩니다.

1. (선택 사항) **작업 이름**&#x200B;을(를) 업데이트합니다.

   >[!TIP]
   >
   >목록에서 여러 작업을 복사하도록 선택하면 이 필드는 흐리게 표시되어 편집할 수 없습니다. 작업 이름 필드 위로 마우스를 가져가면 선택한 모든 작업 목록이 표시됩니다.
   >
   >![](assets/copy-task-multiple-tasks-box-with-list-of-task-names-nwe-350x130.png)

1. **대상 프로젝트 선택** 필드에 작업을 복사할 **대상 프로젝트**&#x200B;의 이름을 입력하십시오.

   >[!TIP]
   >
   >* 프로젝트 이름은 대소문자를 구분합니다.
   >* 참조 번호 입력을 시작하거나 프로젝트의 ID를 입력할 수도 있습니다. 이렇게 하면 이름이 동일한 프로젝트를 구별하는 데 도움이 될 수 있습니다.
   >* 100개의 프로젝트만 목록에 표시됩니다.

   기본적으로 현재 프로젝트 이름이 표시됩니다. 동일한 프로젝트 내에서 작업을 복사하려면 이 필드를 변경하지 마십시오.

1. (조건부) 선택한 프로젝트에 대한 액세스 권한이 없는 경우 **액세스 권한 요청**&#x200B;을 클릭하여 프로젝트에 대한 액세스 권한을 요청하십시오.
1. (조건부) 대상 프로젝트의 작업 중 하나에 작업을 추가할 수 있는 액세스 권한이 있는 경우 액세스 권한 요청 없이 선택한 대상 프로젝트에 작업을 계속 복사합니다.

   ![](assets/copy-task-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >Workfront 관리자가 이러한 프로젝트에 작업을 추가할 수 없을 때 선택한 프로젝트가 승인 보류 중, 완료 또는 정지된 경우에도 유사한 메시지가 표시됩니다. 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

1. 왼쪽 패널에서 **옵션**&#x200B;을 클릭한 다음 작업과 함께 복사하지 않으려는 작업 특성을 선택 취소합니다. 기본적으로 모든 옵션이 선택되어 있습니다.

   >[!TIP]
   >
   >**모두 선택**&#x200B;을 선택한 후 선택을 취소하면 모든 옵션이 선택 해제됩니다.

   다음 옵션에서 선택을 해제하여 복사된 작업으로 전송하지 않습니다. 다음 표에서는 옵션을 선택 해제할 때 발생하는 상황을 설명합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">제한</td> 
      <td> <p>작업 제한 사항은 프로젝트 일정 모드 설정에 따라 가능한 한 빨리 또는 가능한 한 늦게 설정됩니다.</p> <p> 선택하면 작업의 현재 제한 사항이 복사된 작업으로 전송됩니다. </p> <p>주: 일자별 제한조건이 있는 태스크를 다른 프로젝트로 이동하거나 복사할 때 태스크의 제한조건 일자가 신규 프로젝트의 일자를 벗어나면 태스크 제한조건이 가능한 한 빨리 또는 가능한 한 늦게 변경되거나 프로젝트의 계획된 시작 일자 또는 계획된 완료 일자가 조정됩니다. 날짜별 제한의 몇 가지 예는 다음에서 시작되어야 함, 다음에서 완료되어야 함, 다음 날짜까지 시작, 다음 날짜까지 시작 등입니다. 작업 제한 및 작업 제한 또는 프로젝트 날짜가 영향을 받는 방법에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">작업 제한 개요</a>를 참조하고 특정 제한 사항을 찾으십시오.</p> </td> 
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
      <td>작업 상태가 신규입니다. 그렇지 않으면 복사된 작업이 기존 작업의 상태를 유지합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">재무 정보</td> 
      <td>작업의 재무 정보가 제거됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">모든 전임 작업</td> 
      <td> <p>즉, 종속성이 복사된 작업으로 이전되지 않습니다. </p> <p>이 옵션을 선택하면 복사된 작업 그룹 내의 전임 작업은 유지되고 다른 작업은 삭제됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">문서</td> 
      <td> <p>작업에 첨부된 문서는 복사된 작업으로 전송되지 않습니다. 여기에는 버전, 증명 및 연결된 문서가 포함됩니다.</p> <p>여기에는 문서 승인이 포함되지 않습니다. 작업을 복사할 때 문서 승인은 복사할 수 없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">미리 알림</td> 
      <td>작업 미리 알림이 복사된 작업으로 전송되지 않습니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">경비</td> 
      <td>작업에 기록된 경비는 복사된 작업으로 이전되지 않습니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">권한</td> 
      <td>Workfront은 작업의 공유 목록에 표시되는 모든 엔티티의 이름을 제거합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 정의 데이터</td> 
      <td> <p>사용자 정의 필드의 값이 지워지고 사용자 정의 양식이 복사된 작업으로 전송됩니다. </p> <p>선택하면 양식과 사용자 정의 필드 값이 모두 복사된 작업으로 전송됩니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 왼쪽 패널에서 **상위 선택**&#x200B;을 클릭한 다음 대상 프로젝트에서 복사된 작업의 상위가 될 작업을 선택합니다.

   >[!TIP]
   >
   >목록에서 여러 작업을 복사하도록 선택하면 선택한 모든 작업이 선택한 상위의 1차 하위 구성요소가 됩니다.

   다음 중 하나를 수행하여 상위 항목을 선택합니다.

   * 작업 목록에서 프로젝트 계획의 상위 항목 중 하나를 선택합니다.
   * 검색 아이콘 ![검색 아이콘](assets/search-icon.png)을 클릭하고 이름별로 상위 작업을 검색합니다.

   작업이 목록에 표시됩니다.

   ![검색 기능이 있는 작업을 이동할 때 상위 작업 선택 ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. 상위 항목을 찾으면 해당 라디오 단추를 선택합니다.

   상위 작업을 선택하지 않으면 작업이 하위 작업이 아닌 기본 작업으로 복사되고 대상 프로젝트의 작업 목록 끝에 배치됩니다.

1. **작업 복사** 클릭

   또는

   목록에서 작업을 여러 개 선택하면 **작업 복사**를 클릭합니다.
복사된 작업이 이제 지정된 프로젝트에 있으며 선택한 상위 작업의 하위 작업 또는 프로젝트의 마지막 작업입니다.

## 작업 복제

동일한 프로젝트에서 동일한 작업이 필요한 경우 작업 목록에서 작업을 빠르게 복제할 수 있습니다.

* [작업 중복에 대한 고려 사항](#considerations-for-duplicating-tasks)
* [작업 복제](#duplicate-tasks)

### 작업 중복에 대한 고려 사항 {#considerations-for-duplicating-tasks}

* 작업 번호별로 목록을 정렬한 경우에만 작업 목록에서 작업을 복제할 수 있습니다.
* 새 작업의 이름이 원래 작업과 동일합니다.
* 새 작업에 복제되는 정보는 선택할 수 없습니다. 원래 작업의 거의 모든 정보는 기본적으로 상위 관계를 포함하여 중복 작업으로 전송됩니다.
* 다음 항목은 새 작업으로 전송되지 않습니다.

   * 기록된 시간
   * 참고
   * 문제
   * 복사된 작업 그룹과 동일한 그룹에 있는 전임 작업만 후속 작업과 함께 복사됩니다.

     **예**

     예를 들어 작업 2와 전임 작업 1을 동시에 복사하면 작업 2의 사본과 작업 1의 사본이 있습니다. 작업 1의 복사본이 작업 2의 전신이 됩니다. 그러나 전임 작업을 복사하지 않고 작업 2만 복사하면 해당 복사에는 전임 작업이 없습니다.

* 상위 작업을 복제하면 하위 작업이 선택되지 않은 경우에도 모든 하위 작업이 복제됩니다.
* 하나 이상의 작업을 동시에 복제할 수 있습니다.

  하지만 동시에 순차적이 아닌 여러 작업을 복제할 수는 없습니다.

* 이정표가 새 작업으로 이동되고 원래 작업에서 제거됩니다.

### 작업 복제

1. 복제할 작업이 포함된 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **작업**&#x200B;을 클릭합니다.
1. 다음 중 하나를 수행하십시오.

   * (조건부) **플랜 모드** 아이콘 ![](assets/qs-list-mode-or-save-mode-icon-small.png)을(를) 클릭하고 **자동 저장** 옵션이 활성화되어 있는지 확인한 다음, 복제할 작업을 선택하고 **추가 메뉴** ![](assets/qs-more-menu-29x11.png) > **복제**&#x200B;를 클릭합니다.

     ![](assets/duplicate-tasks-in-list-nwe-350x196.png)

   * (조건부) **플랜 모드** 아이콘 ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **수동 저장** > **표준** 또는 **타임라인 계획 수립**&#x200B;을 클릭한 후 다음을 수행합니다.

      1. 복제할 작업을 선택하고 **복제**&#x200B;를 클릭합니다.
      1. (선택 사항) 변경 내용을 취소하고 작업을 복제하지 않으려면 **실행 취소**&#x200B;를 클릭하십시오.
      1. (선택 사항 및 조건부) 이전에 **실행 취소**&#x200B;를 클릭한 경우 **다시 실행**&#x200B;을 클릭하여 변경 내용을 유지하고 작업을 복제합니다.

      1. 변경 내용을 저장하려면 **저장**&#x200B;을 클릭하세요.

         작업이 복제되고 원래 작업과 동일한 프로젝트에 추가됩니다.
