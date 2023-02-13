---
product-area: projects
navigation-topic: create-tasks
title: 프로젝트에서 작업 만들기
description: 프로젝트를 만든 후에만 프로젝트에서 작업을 만들 수 있습니다.
author: Alina
feature: Work Management
exl-id: 96f80e7b-6ad5-40ae-861d-8d97c570f2ac
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 1%

---

# 프로젝트에서 작업 만들기

프로젝트를 만든 후에만 프로젝트에서 작업을 만들 수 있습니다.

예를 들어 프로젝트를 생성한 후 작업을 추가하고 수정하여 프로젝트 계획을 구성할 수 있습니다. 프로젝트 만들기에 대한 자세한 내용은 [프로젝트 만들기](../../../manage-work/projects/create-projects/create-project.md).

프로젝트에 없는 개인 작업을 만드는 방법에 대한 자세한 내용은 문서의 &quot;개인 작업 만들기&quot; 섹션을 참조하십시오 [홈 영역에서 작업 항목 만들기](../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

이 문서에서는 처음부터 작업을 만드는 방법을 설명합니다. 다음과 같은 방법으로 작업을 만들 수도 있습니다.

* 기존 작업을 복사하거나 복제하여 자세한 내용은 [작업 복사 및 복제](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* 한 프로젝트에서 다른 프로젝트로 작업을 이동하는 방법 자세한 내용은 [작업 이동](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## 액세스 요구 사항

<!--drafted for P&P - replace the table:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront license*</p> </td> 
   <td><p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to tasks, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Grant access to tasks</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront 라이선스*</p> </td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. 작업 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">작업에 대한 액세스 권한 부여</a>. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 추가 기능을 사용하여 프로젝트에 사용 권한을 제공합니다.</p> <p>작업을 만들면 작업에 대한 관리 권한을 자동으로 받게 됩니다</p> <p> 작업 권한에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">작업 공유 </a>. </p> <p>추가 권한 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 프로젝트에서 작업 만들기

1. 작업을 만들 프로젝트로 이동합니다.
1. 클릭 **작업** 왼쪽 패널에 표시됩니다.
1. (조건부) 현재 민첩한 보기에서 작업 목록을 보고 있는 경우 **목록 보기** 아이콘 ![](assets/list-view-in-agile-view-for-tasks.png) 오른쪽 위 모서리에서 작업 목록을 표시합니다.
1. (선택 사항) **계획 모드** 아이콘 ![](assets/nwe-plan-mode-icon-task-list.png) 을(를) 선택합니다. **수동 저장**, 다음 중 하나를 선택합니다. **표준** 또는 **타임라인 계획**. 이 확인란을 선택하면 **자동 저장** 옵션이 기본적으로 활성화되어 있습니다.

   ![](assets/nwe-autosave-off-manual-highlighted-350x58.png)

   >[!TIP]
   >
   >수동 저장을 선택하면 변경 사항을 취소할 수 있습니다.

1. 다음 중 하나를 수행하여 새 작업을 만듭니다.

   * 클릭 **새 작업** 작업 목록의 맨 위에
   * 클릭 **추가 작업** 작업 목록 맨 아래에

   ![](assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png)

1. (조건부) **새 작업** 다음을 수행합니다.

   1. 내 제한된 필드 목록에 있는 필드 중 하나를 지정합니다 **새 작업** 상자를 클릭한 다음 **작업 만들기** 작업을 신속하게 만들려면

      또는

      작업의 모든 필드를 업데이트하려면 **추가 옵션** 열다 **작업 만들기** 상자.

      ![](assets/nwe-create-task-small-screen-350x272.png)

      다음 **작업 만들기** 상자가 열립니다.

      ![](assets/create-task-larger-box-nwe-350x244.png)

       

      >[!NOTE]
      >
      >Workfront 관리자가 레이아웃 템플릿을 설정하는 방법에 따라 작업 만들기 상자의 필드에 사용자 환경의 다른 필드가 표시될 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 세부 사항 보기 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   1. 작업 만들기 상자의 왼쪽 패널에서 다음 영역에 대한 정보를 지정합니다.

      * 작업 이름
      * 개요
      * 할당
      * 사용자 지정 Forms
      * 재무
      * 설정

         작업의 모든 작업 관련 필드 정의에 대한 자세한 내용은 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
   1. (조건부 및 선택 사항) 작업을 반복하려면 **되풀이 빈도** 필드. 반복 작업 만들기에 대한 자세한 내용은 [반복 작업 만들기](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).
   1. (선택 사항) **문서** 왼쪽 패널에서 문서를 새 작업에 첨부한 다음 **파일 추가 또는 연결** 컴퓨터, 다른 서비스에서 작업에 문서를 추가하거나 컴퓨터나 다른 서비스에서 문서 및 폴더를 연결하는 데 사용됩니다.


1. (조건부) **추가 작업** 5단계에서 인라인 편집을 사용하여 작업 정보를 입력한 다음 Enter 키를 누릅니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this stays accurate)</p>
   -->

   특히 목록에 여러 작업을 추가할 때 이 옵션을 사용하는 것이 좋습니다.

   ![](assets/ctp4-350x26.png)

1. (조건부) 다음 중 하나를 수행합니다.

   * 클릭한 경우 **새 작업** 5단계에서 **작업 만들기** 변경 사항을 저장하고 새 작업을 프로젝트에 추가합니다.

      <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?)</p>   
     -->

   * 클릭한 경우 **추가 작업** 5단계에서 다음을 수행합니다.

      <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?) </p>   
     -->

      1. 브라우저에서 아무 곳이나 클릭하여 변경 내용을 제출하거나 Enter 키를 누릅니다.
      1. (선택 사항) 작업 목록에서 새로 만든 작업을 선택한 다음 **들여쓰기**.

         이렇게 하면 새 작업이 이전 작업의 하위 또는 하위 태스크가 됩니다.

         하위 작업에 대한 자세한 내용은 [작업 개요](../../../manage-work/tasks/task-information/tasks-overview.md).

      1. (조건부) **자동 저장** 옵션 **추가 작업**&#x200B;를 채울 수 있습니다.

         * 클릭 **실행 취소** 언제든지 마지막 변경 내용을 취소하거나 **취소** 작업 목록에 수행한 모든 변경 사항을 취소합니다.
         * 이전에 클릭한 경우 **실행 취소**&#x200B;를 클릭합니다. **다시 실행** 마지막으로 취소한 변경 내용을 다시 적용하려면 다음을 취소하십시오.
         * 클릭 **저장** 작업 목록에 변경 내용을 저장하려면 다음을 수행합니다.
