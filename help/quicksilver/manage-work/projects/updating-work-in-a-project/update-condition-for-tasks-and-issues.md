---
product-area: projects
navigation-topic: update-work-in-a-project
title: 작업 및 문제에 대한 조건 업데이트
description: 작업 또는 문제의 조건은 진행 방식을 나타내는 플래그입니다. 작업 항목의 상태와는 다릅니다. 작업 항목은 항목의 현재 개발 단계를 나타냅니다.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 0%

---

# 작업 및 문제에 대한 조건 업데이트

작업 또는 문제의 조건은 진행 방식을 나타내는 플래그입니다. 작업 항목의 상태와는 다릅니다. 작업 항목은 항목의 현재 개발 단계를 나타냅니다.

작업의 조건 또는 문제를 자동 또는 수동으로 설정할 수 있습니다.

Adobe Workfront 관리자는 [사용자 지정 조건 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)

<!--You can manually update the Condition of a task or issue if you are assigned to it or if you have permissions to it, as described in the [Access requirements](#access-requirements) section of this article.-->

## 액세스 요구 사항 {#access-requirements}

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the current licenses:
   <ul><li><p>Standard for tasks</p></li>
   <li><p>Contributor or higher for issues</p></li></ul>


   For legacy licenses:
   <ul><li><p>Work or higher for tasks</p></li>
   <li><p>Request or higher for issues</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
    <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>작업의 경우 작업 이상</p>
   <p>문제에 대한 요청 이상</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 보기 이상의 액세스 권한</p> <p>작업 및 문제에 대한 액세스 편집 </p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 및 문제에 대한 권한을 보고 해당 조건을 확인합니다</p>
   <p>작업 및 문제에 대한 권한을 관리하여 조건 업데이트</p>
    <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 작업 및 문제 조건 찾기

조건은 작업 또는 문제와 관련된 플래그로 표시됩니다. 또한 레이블 대신 보고서에 표시할 수 있는 숫자와 연결할 수도 있습니다. 조건과 숫자를 연결하는 방법에 대한 자세한 내용은 [사용자 지정 조건 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

다음 영역에서 작업 및 문제 조건을 찾을 수 있습니다.

* 작업이나 문제에 지정되면 업데이트 내의 작업 및 문제 업데이트 영역입니다.
* 보기 또는 그룹에 조건 필드를 표시할 때의 보고서 및 목록입니다.

>[!NOTE]
>
>&quot;condition&quot;이라는 단어가 분개 입력 보고서의 필드 이름 필드에 표시되면 이는 항목의 조건이 갱신되었음을 나타냅니다. 조건 필드가 분개 입력 보고서에서 추적되면 신규 및 이전 번호 값이 해당 이름 대신 조건에 연관된 번호를 표시합니다. 조건이 원래 작업 또는 문제에 대해 정의되지 않은 경우 나중에 갱신하면 갱신을 캡처하는 분개 입력에 조건 필드의 이전 번호 값이 -2,147,483,648로 표시됩니다.

## 상태를 업데이트하여 조건 자동 업데이트

작업이나 문제가 할당되면 **작업** , 작업 시작 또는 문제 시작 또는 해당 상태를 업데이트하거나, 작업 또는 문제의 조건이 **원활하게 진행**.

사용자 지정 조건을 기본 조건으로 사용하는 방법에 대한 자세한 내용은 문서를 참조하십시오  [사용자 지정 조건을 작업 및 문제에 대한 기본값으로 설정](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) 및 [사용자 지정 조건을 프로젝트의 기본값으로 설정](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

작업 상태 변경에 대한 자세한 내용은 [작업 상태 업데이트](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

문제 상태 변경에 대한 자세한 내용은 [문제 상태 업데이트](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Work On It 단추를 작업 시작 또는 문제 시작 단추로 설정하는 방법에 대한 자세한 내용은 [Work On It 단추를 시작 단추로 바꿉니다.](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## 수동으로 조건 업데이트

해당 작업에 조건을 설정할 수 있으려면 작업 또는 문제에 할당받거나 관리 권한이 있어야 합니다.

작업 또는 문제의 조건 업데이트는 작업 또는 문제에 지정되었는지 여부에 따라 다릅니다.

* 업데이트 탭이나 작업 또는 문제 목록에 지정된 경우 조건을 업데이트할 수 있습니다.
* 작업 또는 문제 목록에 지정되어 있지 않지만 해당 작업에 대한 관리 권한이 있는 경우에만 조건을 업데이트할 수 있습니다. 이 경우 작업이나 문제의 업데이트 탭에서 조건을 업데이트할 수 없습니다.

작업 또는 문제의 조건을 수동으로 설정하려면 다음을 수행하십시오.

1. 조건을 설정할 태스크나 문제로 이동합니다.

   또는

   관리 권한이 있지만 자신에게 할당되지 않은 작업 또는 문제 목록으로 이동합니다.

1. 다음과 같이 문제 또는 작업의 조건을 변경합니다.

   * 작업 또는 문제에 할당되고 이 작업에 대한 관리 권한이 있는 경우, **업데이트** 탭, **새 업데이트 시작**&#x200B;에서 을(를) 선택합니다. **조건** 작업 진행 방식을 가장 잘 반영하려면 **새 업데이트 시작** 영역(선택 사항) 을 클릭한 다음 **업데이트**.

      ![](assets/change-condition-update-comment-350x141.png)

      >[!NOTE]
      >
      >환경에 맞게 조건을 사용자 지정할 수 있으므로 환경에서 조건에 대한 옵션을 세 개 이상 찾을 수 있습니다. 조건 이름은 위에 나열된 이름과 다를 수 있습니다. Workfront의 조건 사용자 지정에 대한 자세한 내용은 [사용자 지정 조건 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

      작업 항목을 업데이트할 때 사용할 수 있는 추가 기능에 대한 자세한 내용은 [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p></li>   
     -->
