---
product-area: projects
navigation-topic: convert-issues
title: Adobe Workfront의 문제 전환 개요
description: 문제가 제출된 후 문제를 완료하기 위해 추가 작업을 수행해야 하는 경우 문제를 프로젝트 또는 작업으로 변환할 수 있습니다.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 97c83b65-208b-4e3f-b4cc-681237d82aa3
source-git-commit: 55c714436fe59c84251c7f4e2a46614feae92cd6
workflow-type: tm+mt
source-wordcount: '1506'
ht-degree: 2%

---

# Adobe Workfront의 문제 전환 개요

문제가 제출된 후 문제를 완료하기 위해 추가 작업을 수행해야 하는 경우 문제를 프로젝트 또는 작업으로 변환할 수 있습니다.

문제를 작업으로 변환하는 방법에 대한 자세한 내용은 [Adobe Workfront에서 문제를 작업으로 변환](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)을 참조하십시오.

문제를 프로젝트로 변환하는 방법에 대한 자세한 내용은 [Adobe Workfront에서 문제를 프로젝트로 변환](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)을 참조하십시오.

## 문제 전환 시 고려 사항

* 문제를 작업 또는 프로젝트로 전환할 때 이 문서에 별도로 명시되지 않는 한 문제의 대부분의 정보가 작업 또는 프로젝트로 전달됩니다.
* [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)에 설명된 대로 Workfront 관리자 또는 그룹 관리자가 이미 문제, 해결 방법, 프로젝트 또는 작업으로 전환될 때 기본 연락처의 액세스 권한에 대한 환경 설정을 설정했습니다.
* Workfront은 전환 중에 문제와 관련된 모든 승인을 제거합니다.
* Workfront은 작업 또는 프로젝트로 전환할 때 문제의 해결 중 오브젝트를 덮어씁니다. 새 작업 또는 문제는 전환 후 문제의 새 해결 오브젝트가 됩니다.
* 다음 사항을 고려하십시오.

   * 변환 중에 문제 및 해결 방법을 생성 중인 프로젝트 또는 작업에 계속 연결할 것인지 여부를 묻는 메시지가 표시될 수 있습니다.
   * 문제를 유지하면 프로젝트, 작업 또는 문제에 변경 사항이 있거나 Workfront이 타임라인을 다시 계산할 때 프로젝트 또는 작업의 상태 및 완료율이 문제의 상태 및 완료율을 자동으로 업데이트합니다.

  >[!NOTE]
  >
  >   문제 상태가 마감됨(작업 또는 프로젝트 마감 결과)이 되면 마감 후 작업 또는 프로젝트가 어떤 상태로 변경되는지에 관계없이 문제는 마감됨 상태로 유지됩니다.


* 문제를 작업 또는 프로젝트로 전환할 때 문제에 할당된 사용자의 홈 영역에서 문제가 제거됩니다.

* 문제를 전환할 때 원래 문제에 대한 권한이 전환된 개체(작업 또는 프로젝트)로 전송되지 않습니다.

* 템플릿을 사용하여 문제를 프로젝트로 전환할 때 템플릿의 대부분의 정보가 새 프로젝트로 전송됩니다. 그러나 문제의 일부 정보가 새 프로젝트로 이전될 수도 있습니다. 자세한 내용은 이 문서의 [템플릿을 사용하여 문제를 프로젝트로 전환할 때의 프로젝트 필드 개요](#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template) 섹션을 참조하십시오.
* 문제를 전환하는 동안 일부 문서 또는 해당 정보가 문제가 전환된 새 객체로 이동하지는 않습니다. 문서 또는 문서 링크가 첨부된 문제를 변환할 때 다음 항목이 포함됩니다.

   * 문서
   * Google Drive 또는 SharePoint과 같은 서드파티 서비스에 대한 링크를 문서화합니다.
   * 버전
   * **원래 문제를 유지하고 해결 방법을 이 작업에 연결** 옵션을 선택하지 않은 경우에만 증명이 포함됩니다.
   * 문서 및 문서 링크가 첨부된 문제를 변환할 때 문서 승인이 포함되지 않습니다.
* 문제를 전환할 때는 5분 처리 제한이 있습니다. 문제에 많은 문서가 첨부되어 있고 전환하지 못하는 경우, 일부 문서를 제거하고 다시 시도해야 할 수 있습니다.
* 문제를 전환에 유지하기로 결정했으며 해당 전환에 문서가 첨부된 경우 문서 및 해당 버전이 프로젝트 또는 작업에 복사됩니다. 증명 및 문서 승인은 프로젝트 또는 작업에 복사되지 않습니다.
* 전환에 문제를 유지하지 않기로 결정했으며 해당 전환에 문서가 첨부된 경우 문서, 문서 버전 및 증명이 프로젝트 또는 작업으로 전송됩니다. 문서 승인은 프로젝트 또는 작업으로 이전되지 않습니다.
* 전환 중에 문제를 보관하는지 여부에 관계없이 Google 드라이브와 같은 타사 서비스의 원래 문제와 연결된 문서 및 폴더가 있는 경우 해당 링크가 새 개체에 복사됩니다.
* 문제 주석은 문제에서 전환된 작업 또는 프로젝트에도 복사되지만, 태그가 지정된 사용자는 전송되지 않습니다.
* 문제의 사용자 정의 양식 정보를 전환 중인 프로젝트 또는 작업으로 전송하려면 문제에서 전송할 동일한 필드가 포함된 프로젝트 또는 작업 사용자 정의 양식이 있어야 합니다. 자세한 내용은 [개체를 변환할 때 사용자 정의 양식 데이터 전송](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md)을 참조하십시오.

## 템플릿을 사용하여 문제를 프로젝트로 전환할 때의 프로젝트 필드 개요 {#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template}

문제를 프로젝트로 전환할 때 빈 프로젝트로 전환하거나 템플릿을 사용할 수 있습니다.

자세한 내용은 [문제를 Adobe Workfront의 프로젝트로 변환](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)을 참조하십시오.

템플릿을 사용할 때 템플릿에서 채워지는 일부 필드는 전환된 문제에서 생성된 프로젝트로 전송됩니다. 다른 필드는 전환된 문제에서 프로젝트로 전송됩니다.

다음 표에는 프로젝트 정보 및 템플릿 전송 여부와 문제 전송 여부가 나와 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>설명</td> 
   <td> <p>문제가 새 프로젝트로 이전되는 설명. </p> <p> 문제에 대한 설명이 없는 경우 템플릿의 설명이 프로젝트로 전송됩니다. </p> <p>문제와 템플릿에 대한 설명 필드가 모두 비어 있으면 프로젝트에서 필드가 비어 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>상태</td> 
   <td>템플릿의 그룹에 대해 선택된 기본 상태입니다. 템플릿이 그룹과 연결되어 있지 않으면 프로젝트 상태는 [설정]의 [프로젝트 환경 설정] 영역에서 Workfront 관리자가 설정한 기본 상태로 설정됩니다. 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">시스템 전체 프로젝트 환경 설정 구성</a>을 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td>우선순위</td> 
   <td><p>문제에서 전송.</p>
   <p>변환된 프로젝트에 템플릿을 사용하는 경우 우선순위를 수동으로 변경할 수 있는 옵션이 있습니다. 변경하지 않기로 선택한 경우 문제의 우선순위가 프로젝트로 이전됩니다. 
    </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td> <p>문제의 URL이 새 프로젝트로 전송됩니다. </p> <p> 문제에 지정된 URL이 없는 경우 템플릿의 URL이 프로젝트로 전송됩니다. </p> <p>문제와 템플릿에 대한 URL 필드가 모두 비어 있으면 프로젝트에서 필드가 비어 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>프로젝트 상태 유형</td> 
   <td>템플릿에서 전송합니다.</td> 
  </tr> 
  <tr> 
   <td>프로젝트 상태</td> 
   <td>Workfront 관리자가 설정 영역에서 결정한 시스템 수준 기본 설정과 일치합니다. 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">프로젝트 기본값으로 사용자 지정 조건 설정</a>을 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td>일정 기준</td> 
   <td>템플릿에서 전송합니다.</td> 
  </tr> 
  <tr> 
   <td>프로젝트 일자</td> 
   <td> 
    <ul> 
     <li> <p><b>계획된 시작 일자</b>: 템플릿 일정의 시간대에 따라 템플릿 일정의 작업 시간을 기준으로 가장 가까운 작업 시간을 미리 선택해야 합니다. 일정: 부터 필드가 완료: 부터로 설정된 경우 이 필드가 비활성화됩니다. </p> </li> 
     <li> <p><b>계획된 완료 일자</b>: 템플릿 일정의 시간대에 따라 템플릿 일정의 작업 시간을 기준으로 가장 가까운 작업 시간을 미리 선택해야 합니다. 일정 시작 일자 필드가 시작 일자로 설정된 경우 이 필드가 비활성화됩니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>포트폴리오</td> 
   <td>템플릿에서 전송합니다. 그렇지 않으면 이 필드는 비어 있습니다.</td> 
  </tr> 
  <tr> 
   <td>프로그램</td> 
   <td>템플릿에서 전송합니다. 그렇지 않으면 이 필드는 비어 있습니다.</td> 
  </tr> 
  <tr> 
   <td>그룹</td> 
   <td><p> 다음과 같은 시나리오가 있습니다.</p>
     <ul><li>변환 중에 그룹이 지정된 경우 해당 그룹이 프로젝트의 그룹이 됩니다</li>
     <li>템플릿을 사용하여 프로젝트로 변환할 때 템플릿에 그룹이 있고 변환 중에 그룹을 지정하지 않으면 템플릿 그룹이 새 프로젝트의 그룹이 됩니다</li>
      <li> 템플릿에 그룹이 없고 전환하는 동안 그룹을 지정하지 않으면 원래 문제의 프로젝트 그룹이 새 프로젝트의 그룹이 됩니다</li> </ul>
      </td> 
  </tr> 
  <tr> 
   <td>회사</td>    
   <td>  템플릿에서 전송합니다. 그렇지 않으면 이 필드는 비어 있습니다.</td>

</tr> 
  <tr> 
   <td>프로젝트 소유자</td> 
   <td>템플릿의 템플릿 소유자 필드에서 전송합니다. 그렇지 않으면 변환을 수행하는 로그인한 사용자로 설정됩니다. </td> 
  </tr> 
  <tr> 
   <td>프로젝트 스폰서</td> 
   <td>템플릿의 템플릿 스폰서 필드에서 전송합니다. 그렇지 않으면 이 필드는 비어 있습니다.</td> 
  </tr> 
  <tr> 
   <td>리소스 관리자</td> 
   <td>템플릿에서 전송합니다. 그렇지 않으면 이 필드는 비어 있습니다.</td> 
  </tr> 
  <tr> 
   <td>작업 설정</td> 
   <td>템플릿에서 전송합니다.</td> 
  </tr> 
  <tr> 
   <td>문제 설정</td> 
   <td>템플릿에서 전송합니다. </td> 
  </tr> 
  <tr> 
   <td>액세스</td> 
   <td> <p>템플릿에 대한 액세스 섹션에서 전송합니다. </p> </td> 
  </tr> 
  <tr> 
   <td>승인</td> 
   <td>템플릿에서 전송합니다. 문제와 관련된 승인은 전환 중에 제거됩니다. </td> 
  </tr> 
 </tbody> 
</table>

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a project</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the <strong>Issues</strong> icon on a project. </li>
<li value="2"> <p>Click the issue to be converted to access the issue.</p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu, then click <strong>Convert to Project</strong>. </p>  </li>
<li value="4"> <p>In the submenu that displays, do one of the following:</p>
<ul>
<li>Click <strong>New Project</strong></li>
<li>Under <strong>New from Template</strong>, click the name of a project template you want to use</li>
</ul> </li>
<li value="5"> <p>Specify a name for the project.</p> <p>The default name is the name of the issue you are converting.</p> </li>
<li value="6">(Optional and conditional) If you are creating this project from a template, update the available fields in the Convert to Project box.<br>For more information about editing fields on projects, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the available options:</p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this project</strong>When deselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li><strong>Allow <User Name> to have access to this project</strong>If unselected, the user who entered the issue has no access to the new task.</li>
</ul> <note type="note">
<div>
<p>The options that are available here depend on how the Workfront administrator has configured them for everyone in the system or for your group. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options available here depend on which group you selected for the new project in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a><span class="preview">.</span></p>
</div>
</note> </li>
<li value="8">(Optional) In the <strong>Custom Forms</strong> section, attach any custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new project, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.</li>
<li value="9"> <p>Click <strong>Save Changes.</strong></p> <p> <img src="assets/qs-issue-convert-to-project-before-saving-ui-350x366.png" style="width: 350;height: 366;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> <p>The issue is now a project, if you decided to delete the original issue.<br>Or<br>The issue is now linked to the new project and it will complete when the project completes, if you decided to keep the original issue. </p> <p>Some issue fields transfer to the project. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. </p> </li>
<li value="10"> <p>(Optional) Set any further project details ​(project owner, project dates) and tasks as necessary.</p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a task</h2> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the Issues icon on a project.  </li>
<li value="2"> <p>Click the issue you want to convert to go to the issue's landing page. </p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu on the issue, then <strong>Convert to Task</strong>.  </p>  </li>
<li value="4"> <p>Name the task.</p> </li>
<li value="5"> <p>Identify the project where the task will reside. </p> <p>You can select a different project from the project that the issue is on.</p> </li>
<li value="6"> <p>In the <strong>Project</strong> box, start typing the name of the project where you want to put the new task, then press <strong>Enter</strong> when it appears.</p> <p>By default, this box the name of the project containing the issue that you are converting.</p> </li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the following options. </p> <p>The Workfront administrator or group administrator must enable these preferences before they are visible during the conversion of issues: </p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this task</strong> </p> <p>If unselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li> <p><strong>Allow <User Name> to have access to this task</strong> </p> <p>If unselected, the user who entered the issue has no access to the new task.</p> </li>
<li> <p><strong>Keep the planned completion date of the issue</strong> </p> <p>If unselected, the Planned Completion Date of the new task is calculated from the Planned Start Date of the task. The Planned Start Date of the new task is set according to the system preferences for new tasks.</p> </li>
</ul> <note type="note">
<div>
<p>The options that display here depend on how the Workfront administrator configured them for everyone in the system. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options that display here depend on which group is associated with the project you selected in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a>.</p>
</div>
</note> </li>
<li value="8">(Optional) Attach custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new task, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.<br><p><img src="assets/qs-issue-convert-to-task-before-saving-ui-350x367.png" style="width: 350;height: 367;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></p></li>
<li value="9"> <p>Click <strong>Save Changes</strong> when all task settings are set.</p> <p>The issue is now a task on the designated project, if you decided to delete the original issue.</p> <p>Or</p> <p>The issue is now linked to the new task on the project you chose, and it will complete once the task completes, if you decided to keep the original issue.</p> <p>Some issue fields transfer to the task. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. <br></p> </li>
<li value="10"> <p>(Optional) Continue editing the task (assignments, dates) as necessary. </p> </li>
</ol>
</div>
-->

## 프로젝트 및 작업에 대한 원래 문제 정보 보기 {#view-original-issue-information-on-projects-and-tasks}

프로젝트 및 작업 목록과 보고서 또는 프로젝트 세부 정보 영역에서 원래 문제 정보를 볼 수 있습니다. 보고서 작성에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.

다음 표는 변환된 프로젝트 및 작업에서 표시되는 문제 필드를 보여 줍니다.

| 문제 필드 | 프로젝트 또는 작업 필드 | 프로젝트 목록 또는 보고서 | 프로젝트 세부 정보 영역 | 작업 목록 또는 보고서 | 작업 세부 정보 영역 |
|---|---|---|---|---|---|
| 문제 이름 | 전환된 문제 이름 | ✔ | ✔ | ✔ | ✔ |
| 기본 담당자 | 전환된 문제 작성자 이름 | ✔ | `✔` | ✔ |  |
| 입력 일자 | 전환된 문제 입력 일자 | ✔ |  | ✔ |  |


>[!CAUTION]
>
>문제의 기본 담당자가 변경되거나 문제가 전환된 후 프로젝트 또는 작업에서 문제가 연결 해제되는 경우 전환된 문제 작성자 이름이 업데이트되지 않고 문제가 전환된 시점의 문제의 원래 기본 담당자가 표시됩니다.
