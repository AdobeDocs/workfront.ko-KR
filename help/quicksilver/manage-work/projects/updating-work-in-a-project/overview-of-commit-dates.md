---
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: 커밋 일자 개요
description: 커밋 일자는 작업 또는 문제에 할당된 사용자가 작업 또는 문제를 완료하기로 커밋하는 일자입니다. 이는 업무를 담당하는 사용자만이 부여한 준공기일을 보다 현실적으로 추정한 것이어서 계획된 준공기일과 다르다. 계획된 완료 일자에 대한 자세한 내용은 태스크 계획 완료 일자 개요를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 47072433-bb8e-4210-947a-8bfa41ec47a9
source-git-commit: c50ff48bbc492199b39db17b8c445207209bb6a5
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 0%

---

# 커밋 일자 개요

{{preview-and-fast-release}}

커밋 일자는 작업 또는 문제에 할당된 사용자가 작업 또는 문제를 완료하기로 커밋하는 일자입니다. 이는 업무를 담당하는 사용자만이 부여한 준공기일을 보다 현실적으로 추정한 것이어서 계획된 준공기일과 다르다. 계획된 완료 일자에 대한 자세한 내용은 [작업 계획 완료 일자 개요](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

## 커밋 일자 개요

커밋 일자를 사용할 때는 다음 사항을 고려하십시오.

* 작업과 문제에만 커밋 일자가 있습니다.
* 커밋 일자는 Adobe Workfront에서 자동으로 설정되지 않습니다.\
  작업 또는 문제를 만들 때 작업 또는 문제에 할당된 커밋 일자가 없습니다.
* 작업 또는 문제에 할당된 경우 다음 중 하나를 수행하여 커밋 일자를 설정할 수 있습니다.

   * Workfront에서 작업 또는 문제에 대한 작업, 문제 시작 또는 작업 시작을 클릭하여 커밋 일자를 작업 또는 문제의 기존 계획된 완료 일자와 일치하도록 설정할 수 있습니다. [처리 중] 단추를 [시작] 단추로 바꾸는 방법에 대한 자세한 내용은  [처리 중 단추를 시작 단추로 바꾸기](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).
   * 작업 또는 문제가 완료될 수 있다고 생각되는 시기에 따라 커밋 일자를 직접 수동으로 설정하십시오. 이는 프로젝트 관리자가 작업 또는 문제를 특정 날짜까지 완료할 수 있도록 프로젝트 관리자에 대한 예상 및 약속입니다.

>[!NOTE]
>
>커밋 일자를 변경하려면 작업의 작업 소유자여야 합니다. 다음 사용자는 작업의 커밋 일자를 변경할 수 없습니다.
>
>* 프로젝트 소유자
>* 프로젝트 스폰서
>* 리소스 관리자
>* 시스템 관리자
>* 작업에 대한 다른 모든 할당자
>* 작업에 대한 권한이 있는 다른 모든 사용자입니다.
>
>작업 소유자에 대한 자세한 내용은 섹션을 참조하십시오 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) 이 문서에서 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## 커밋 일자 변경으로 트리거된 알림 및 업데이트 {#notifications-and-updates-triggered-by-changing-the-commit-date}

작업 또는 문제 할당자가 프로젝트 소유자가 설정한 계획된 완료 일자와 다른 커밋 일자를 선택하면 프로젝트 소유자 및 다른 사용자에게 이 변경 사항을 알리는 다수의 알림 및 업데이트가 있습니다.

>[!NOTE]
>
>커밋 일자를 변경해도 계획된 일자는 자동으로 변경되지 않고, 계획된 일자를 변경해도 커밋 일자는 자동으로 변경되지 않습니다.

작업 또는 문제에 대한 커밋 일자를 설정하면 다음 변경 사항이 트리거됩니다.

* 커밋 일자는 작업 또는 문제의 업데이트 스트림에 채워집니다.

  <span class="preview">![](assets/update-stream-confirmation-that-commit-date-changed-nwe-350x73.png)</span>

  Workfront 관리자가 설정의 업데이트 피드 영역에서 이 업데이트를 활성화하면 작업 또는 문제의 업데이트 영역에 커밋 일자 변경이 표시됩니다. 자세한 내용은 [시스템 추적 업데이트](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

* 이제 작업이 완료될 가능성이 더 정확하게 표시되므로 작업 또는 문제의 예상 완료 일자가 동일한 일자로 설정됩니다.

  예상 완료 일자에 대한 자세한 내용은 [프로젝트, 작업 및 문제의 예상 완료 일자 개요](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

  ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

* 프로젝트 소유자는 기존 주석 달기 경험을 사용하는 경우 작업의 업데이트 탭에서 이 변경 사항이 프로젝트 타임라인에 영향을 주는지 여부를 확인하고 동일한 영역에서 작업의 계획된 완료 일자를 업데이트할 수 있습니다.

  이 기능은 새 댓글 달기 환경에서 지원되지 않습니다. 자세한 내용은 [새 댓글 달기 환경](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

  >[!TIP]
  >
  >  문제 일자는 프로젝트 타임라인에 영향을 주지 않으므로 프로젝트 소유자는 문제의 계획된 완료 일자를 업데이트할 수 없습니다.

  프로젝트 소유자가 변경 사항을 수락하지 않으려는 경우 새 날짜를 제안하는 사용자에게 댓글을 달아 커밋 일자를 원래 계획된 일자로 다시 변경하거나 새 날짜를 선택하는 것이 좋습니다. 프로젝트 소유자가 변경을 수락하면 항목에 할당된 사용자가 제공한 커밋 일자와 일치하도록 계획된 완료 일자를 수동으로 조정할 수 있습니다. 다음을 클릭할 수도 있습니다. **계획된 일자를 다음으로 설정: &lt; date >** 업데이트 영역에서 계획된 완료 일자를 새 커밋 일자와 일치하도록 자동으로 설정합니다.

  이 변경 사항을 수락하려면 작업 및 프로젝트를 관리할 액세스 권한이 있어야 합니다.

  >[!NOTE]
  >
  >작업의 계획된 완료 일자 변경을 수락하여 프로젝트의 타임라인이 어떻게 영향을 받는지 확인하려면 다음을 클릭하십시오. **프로젝트 타임라인**. 이렇게 하면 작업 목록이 열리고 여기에서 날짜 변경 사항과 프로젝트 타임라인을 평가할 수 있습니다.
  >
  >
  >![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)  >
  >

* 알림 영역의 프로젝트 소유자에게는 작업 커밋 일자가 변경되었다는 알림이 표시됩니다.

  ![](assets/in-product-notification-commit-date-changed-nwe-350x149.png)

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tip below is actually wrong and the updates feeds should not control this setting, but at this time it does, according to this issue in Hub: https://hub.workfront.com/issue/61e1aa5e0002a186fdd0a73a10db0fc3/updates?email-source=comm</p>
  -->

  >[!TIP]
  >
  >Workfront 관리자가 설정의 업데이트 피드 영역에 커밋 일자 표시를 활성화할 경우에만 커밋 일자가 변경되었다는 알림이 프로젝트 소유자에게 전송됩니다. 자세한 내용은 [시스템 추적 업데이트](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).



작업 항목을 업데이트할 때 사용할 수 있는 추가 기능에 대한 자세한 내용은  [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

작업 및 문제에 대한 커밋 일자 업데이트에 대한 자세한 내용은 다음을 참조하십시오. [작업 및 문제에 대한 커밋 일자 업데이트](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

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
