---
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: 커밋 일자 개요
description: 커밋 일자는 작업 또는 문제에 할당된 사용자가 작업 또는 문제를 완료하기 위해 커밋하는 일자입니다. 이는 업무를 직접 담당하는 사용자가 부여한 보다 현실적인 준공 일자 추정치인 만큼 계획된 준공 일자와 다르다.
author: Alina
feature: Work Management
exl-id: 47072433-bb8e-4210-947a-8bfa41ec47a9
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# 커밋 일자 개요

<!--Audited: 05/2025-->

<!-- <span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

커밋 일자는 작업 또는 문제에 할당된 사용자가 작업 또는 문제를 완료하기 위해 커밋하는 일자입니다. 이는 업무를 담당하는 사용자만이 부여한 완료일에 대한 보다 현실적인 추정치이기 때문에 업무 또는 문제의 계획된 완료일과 다릅니다.

계획된 완료 날짜에 대한 자세한 내용은 [작업 계획된 완료 날짜에 대한 개요](../../../manage-work/tasks/task-information/task-planned-completion-date.md)를 참조하십시오.

## 커밋 일자 개요

커밋 일자를 사용할 때는 다음 사항을 고려하십시오.

* 작업과 문제에만 커밋 일자가 있습니다.
* 커밋 일자는 Adobe Workfront에서 자동으로 설정되지 않습니다. 작업 또는 문제를 만들 때 할당된 커밋 일자가 없습니다.
* 작업 또는 문제에 할당된 경우 다음 중 하나를 수행하여 커밋 일자를 설정할 수 있습니다.

   * Workfront에서 작업 또는 문제에 대한 작업, 문제 시작 또는 작업 시작을 클릭하여 커밋 일자를 작업 또는 문제의 기존 계획된 완료 일자와 일치하도록 설정할 수 있습니다. 자세한 내용은 [처리 중 단추를 시작 단추로 바꾸기](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md)를 참조하십시오.
   * 작업 또는 문제가 완료될 시기에 따라 커밋 일자를 직접 수동으로 설정하십시오. 이는 프로젝트 관리자가 작업 또는 문제를 특정 날짜까지 완료할 수 있도록 프로젝트 관리자에 대한 예상 및 약속입니다. 자세한 내용은 [작업 및 문제에 대한 커밋 일자 업데이트](/help/quicksilver/manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md)를 참조하십시오.

>[!NOTE]
>
>커밋 일자를 변경하려면 작업의 작업 소유자여야 합니다. 다음 사용자는 작업의 커밋 일자를 변경할 수 없습니다.
>
>* 프로젝트 소유자
>* 프로젝트 스폰서
>* 리소스 관리자
>* 시스템 관리자
>* 작업에 대한 다른 모든 할당자
>* 작업에 대한 권한이 있는 다른 모든 사용자
>
>작업 소유자에 대한 자세한 내용은 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md)을 참조하세요.

## 작업 및 문제의 커밋 일자 찾기

Workfront의 다음 영역에서 작업 및 문제의 커밋 일자를 찾을 수 있습니다.

* 세부 정보 페이지
* Workfront 또는 그룹 관리자가 레이아웃 템플릿에 요약 패널을 추가하면 다음이 표시됩니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 요약 패널 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)을 참조하십시오.
* Workfront 또는 그룹 관리자가 작업 또는 문제를 레이아웃 템플릿에 추가한 후의 헤더. 자세한 내용은 [레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)을 참조하십시오.

## 커밋 일자 변경으로 트리거된 알림 및 업데이트 {#notifications-and-updates-triggered-by-changing-the-commit-date}

작업 또는 문제 피할당자가 수동으로 커밋 일자를 프로젝트 소유자가 설정한 계획된 완료 일자와 다른 일자로 변경하면 프로젝트 소유자 및 다른 사용자에게 이 변경을 알리는 다수의 알림 및 업데이트가 있습니다.

>[!NOTE]
>
>커밋 일자를 변경해도 계획된 일자는 자동으로 변경되지 않고, 계획된 일자를 변경해도 커밋 일자는 자동으로 변경되지 않습니다.

작업 또는 문제에 대한 커밋 일자를 수동으로 설정하면 다음 변경 사항이 트리거됩니다.

* 작업 또는 문제의 업데이트 섹션에 있는 시스템 활동 및 모두 탭에 커밋 일자 변경이 채워집니다.

  ![커밋 일자 변경 알림](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)

  Workfront 관리자가 설정의 업데이트 피드 영역에서 이 업데이트를 활성화하면 작업 또는 문제의 업데이트 영역에 커밋 일자 변경 사항이 표시됩니다. 자세한 내용은 [시스템 추적 업데이트](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md)를 참조하십시오.

  프로젝트 소유자가 변경 사항을 수락하지 않으려는 경우 업데이트 섹션의 설명 탭을 사용하여 새 날짜를 제안하는 사용자에게 다시 댓글을 달거나 커밋 날짜를 원래 계획된 날짜로 다시 변경하도록 요청하거나 새 날짜를 선택하는 것이 좋습니다.

  프로젝트 소유자가 변경을 수락하는 경우 작업 또는 문제를 편집하여 항목에 할당된 사용자가 제공한 커밋 일자와 일치하도록 계획된 완료 일자를 수동으로 조정할 수 있습니다.

  편집하려면 작업 또는 문제를 관리할 수 있는 액세스 권한이 있어야 합니다.

  >[!TIP]
  >
  >시스템 또는 그룹 관리자에게 업데이트하기 쉽도록 요약 패널 또는 헤더에 커밋 일자 필드를 추가하도록 요청할 수 있습니다.
  >
  >자세한 내용은 다음 문서를 참조하십시오.
  >
  >* [요약 개요](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
  >* [레이아웃 템플릿을 사용하여 요약 패널 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
  >* [레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)

<!--this is no longer possible: 
>[!NOTE]
>
>If you want to see how the timeline of the project is affected by accepting to change the Planned Completion Date of the task, click **Project Timeline**. This opens the task list where you can evaluate the date changes and the project timeline.
>
>
>![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)  >
>
-->


* 이제 작업이 완료될 가능성이 더 정확하게 표시되므로 작업 또는 문제의 예상 완료 일자가 동일한 일자로 설정됩니다.

  자세한 내용은 [프로젝트, 작업 및 문제의 예상 완료 일자 개요](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)를 참조하십시오.

  ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

* 알림 영역의 프로젝트 소유자에게는 작업 또는 문제 커밋 일자가 변경되었다는 알림이 표시됩니다.

  ![커밋 일자 변경 알림](assets/in-product-notification-commit-date-changed-nwe-350x149.png)

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tip below is actually wrong and the updates feeds should not control this setting, but at this time it does, according to this issue in Hub: https://hub.workfront.com/issue/61e1aa5e0002a186fdd0a73a10db0fc3/updates?email-source=comm</p>
  -->

  >[!TIP]
  >
  >Workfront 관리자가 설정의 업데이트 피드 영역에 커밋 일자 표시를 활성화할 경우에만 커밋 일자가 변경되었다는 알림이 프로젝트 소유자에게 전송됩니다. 자세한 내용은 [시스템 추적 업데이트](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md)를 참조하십시오.

작업 항목을 업데이트할 때 사용할 수 있는 추가 기능에 대한 자세한 내용은 [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)를 참조하십시오.

작업 및 문제의 커밋 일자 업데이트에 대한 자세한 내용은 [작업 및 문제의 커밋 일자 업데이트](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md)를 참조하십시오.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update Commit Dates on tasks and issues</h2>
<p>(NOTE: moved to its own article) </p>
<p>Updating the Commit Date is identical for tasks and issues.</p>
<ol>
<li value="1"> <p>Go to a task or issue that you are assigned to as the <strong>Task Owner</strong>.</p> <p>For more information about finding out who the Task Owner for an issue or task is, see the section <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments" class="MCXref xref">Edit tasks</a> in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> </li>
<li value="2"> <p>Click Work on it in the task or issue header</p> <p>Or</p> <p>Click <strong>Start Task</strong> or <strong>Start Issue</strong> if the Work on it button has been customized in your environment to indicate that you are now working on the work item. </p> <p>At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.</p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <strong>Undo</strong> in the lower-left corner of the screen. The Commit Date is removed. </p> <p>For information about replacing the Work On It button with a Start button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <note type="tip">
The option to undo your selection to start your work is not available when you click
<span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>.
</note> </li>
<li value="4"> <p> Expand the <strong>This will be done by</strong> date picker, and select a new Commit Date.</p>
<div>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>Updates</strong> in the left panel, then click the <strong>Start a new update</strong>><strong>Commit Date</strong></p>
<p>Or</p>
<p>Click <strong>Task Details</strong> or <strong>Issue Details</strong> in the left panel, then double click <strong>Commit Date</strong> and select a new date from calendar. </p>
</div>
<p>The Commit Date and the Planned Completion date are no longer the same.</p>
<p>Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.</p>
<p>The changes are saved automatically.</p>
<p>The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. For information about the notifications and updates that are triggered by this change, see the section <a href="#notifications-and-updates-triggered-by-changing-the-commit-date" class="MCXref xref">Notifications and updates triggered by changing the Commit Date</a> in this article.</p>
</div> </li>
</ol>
</div>
-->
