---
product-area: projects
navigation-topic: manage-tasks
title: 작업 목록 내의 동시 변경 사항 저장 개요
description: 목록에서 작업을 편집할 때 별도의 저장 설정을 사용하여 목록에서 작업을 편집할 때 변경 내용을 수동으로 저장할지 여부를 지정할 수 있습니다.
author: Alina
feature: Work Management
exl-id: dff52425-4711-40a8-8f40-205d75c506ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# 작업 목록 내의 동시 변경 사항 저장 개요

목록에서 작업을 편집할 때 별도의 저장 설정을 사용하여 목록에서 작업을 편집할 때 변경 내용을 수동으로 저장할지 여부를 지정할 수 있습니다.

작업 목록에서 작업 편집에 대한 자세한 내용은 문서를 참조하십시오 [목록의 작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

두 사용자가 동일한 작업을 변경하는 경우 충돌이 발생할 수 있습니다.

작업 목록에서 작업을 편집할 때는 다음 사항을 고려하십시오.

* Adobe Workfront에서는 프로젝트 업데이트 유형이 자동 또는 자동 또는 변경일 경우 변경 내용을 자동으로 저장하도록 선택하면 작업 변경 사항을 즉시 저장합니다. 프로젝트 업데이트 유형에 대한 자세한 내용은 [프로젝트 업데이트 유형을 선택합니다](../../../manage-work/projects/manage-projects/select-project-update-type.md).
* Workfront은 다른 사용자가 시스템의 다른 곳에서 수행할 수 있는 변경 사항을 사용하여 매분마다 작업 중인 목록의 정보를 업데이트합니다. 이렇게 하면 항상 작업에 대한 최신 정보를 얻을 수 있습니다.

여러 사용자가 동일한 작업을 편집할 때 다음 시나리오가 있습니다.

* **한 사용자는 작업 목록에 변경 내용을 자동으로 저장하고 다른 사용자는 수동으로 저장합니다**: 사용자 B가 동일한 작업을 편집하는 동안 사용자(사용자 A)가 변경 사항을 수동으로 저장하지만 변경 사항을 자동으로 저장하는 경우 사용자 B가 수행한 라이브 변경 사항이 사용자 A의 목록에서 1분마다 업데이트됩니다. 두 사용자가 수행한 변경 내용 간에 충돌이 있으면 사용자가 수동으로 저장(사용자 A)하면 변경 사항을 저장하기 전에 경고 메시지가 표시됩니다. 경고 메시지에 충돌하는 변경 사항이 있는 항목이 표시됩니다. 이때 사용자 A는 변경 사항을 유지할지(사용자 B의 변경 사항을 덮어씁니다) 또는 취소할지(사용자 B의 변경 사항을 유지합니다.) 선택할 수 있습니다.

>[!NOTE]
>
>변경한 내용을 취소하도록 선택하면 다른 사용자가 편집한 내용과 충돌하는 변경 사항뿐만 아니라 모든 변경 사항에 적용됩니다.

* **여러 사용자가 작업 목록의 변경 내용을 수동으로 저장하고 있습니다**: 목록의 작업을 변경하는 여러 사용자가 동시에 수동으로 저장하는 경우, Workfront에서는 먼저 저장하는 사용자가 수행한 변경 사항을 저장합니다. 이러한 변경 내용을 저장하면 충돌이 발생하지 않습니다. Workfront는 다른 모든 사용자가 수행한 변경 사항을 이미 저장한 정보와 비교하고, 정보를 저장하기 전에 다른 사용자에게 충돌하는 변경 사항에 대한 경고를 표시합니다.

>[!IMPORTANT]
>
>변경 내용을 다른 모든 변경 사항에 대해 유지하도록 선택하면 변경한 작업이 다른 사용자가 삭제되지 않는 한 모든 변경 내용이 저장됩니다. 이 경우 경고 메시지는 삭제된 작업에 대한 변경 사항이 유실되었음을 알려줍니다.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
<p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - when replaced with the above live section; does it need an edit??) </p>
<div>
<p>When editing tasks in a list, you can select whether you want each change to be saved automatically or if you want to manually save multiple changes at one time by clicking the Save button. This depends on whether you enable the Autosave setting in the task list or not. </p>
<p>For information about editing tasks in a task list, see the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref" xrefformat="{para}">Edit tasks</a>. </p>
<p>Sometimes, conflicts might appear if two users are making changes on the same tasks. </p>
<p>Consider the following when editing tasks in a task list: </p>
<ul>
<li>Workfront saves the changes you make to tasks immediately when you have enabled the Autosave setting. </li>
<li>Workfront updates the information on the list you are working on every minute with changes that other users might make anywhere else in the system. This ensures that you always get the latest information on the tasks. </li>
</ul>
<p>The following scenarios exist when multiple users are editing the same tasks:</p>
<ul>
<li>One user has Autosave disabled and another has it enabled: If a user (User A) has disabled the Autosave setting and is editing the task list while User B is editing the same tasks but they have enabled the Autosave setting, the live changes made by User B are updated on the list for User A every minute. If there are conflicts between the changes made by the two users, the user with the Autosave setting disabled (User A) sees a warning message before they can save their changes, that shows the items that have those conflicting changes. At this time, User A can choose whether they should keep their changes (which overwrites the changes made by User B), or discard them (which keeps the changes made by User B.) </li>
</ul> <note type="note">
When you select to discard the changes you made, this applies to all the changes and not just to those that have conflicts with the edits made by another user.
</note>
<ul>
<li>Several users have disabled the Autosave setting: If several users that have disabled the Autosave setting are making changes at the same time, Workfront saves the changes made by the user who saves first. Saving these changes should not encounter any conflicts. Workfrontthen compares the changes made by all the other users with the information that it already saved and displays a warning about the conflicting changes to the other users before they can save their information. </li>
</ul> <note type="important">
When you select to keep your changes over all other changes, your changes are saved, unless the tasks you made changes to were deleted by another user. In this case, the warning message informs you that the changes you made to the deleted tasks are lost.
</note>
</div>
</div>
-->
