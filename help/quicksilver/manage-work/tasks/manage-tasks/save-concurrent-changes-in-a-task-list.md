---
product-area: projects
navigation-topic: manage-tasks
title: 작업 목록 내 동시 변경 사항 저장 개요
description: 목록에서 작업을 편집할 때 목록에서 작업을 편집할 때 변경 사항을 수동으로 자동 저장할지 여부를 나타내는 별도의 저장 설정을 사용할 수 있습니다.
author: Alina
feature: Work Management
exl-id: dff52425-4711-40a8-8f40-205d75c506ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# 작업 목록 내 동시 변경 사항 저장 개요

목록에서 작업을 편집할 때 목록에서 작업을 편집할 때 변경 사항을 수동으로 자동 저장할지 여부를 나타내는 별도의 저장 설정을 사용할 수 있습니다.

작업 목록에서 작업을 편집하는 방법에 대한 자세한 내용은 문서 [목록에서 작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)을 참조하십시오.

경우에 따라 두 사용자가 동일한 작업을 변경할 때 충돌이 발생할 수 있습니다.

작업 목록에서 작업을 편집할 때 다음 사항을 고려하십시오.

* 프로젝트 업데이트 유형이 자동, 자동 또는 변경 시 인 경우 변경 사항을 자동으로 저장하도록 선택하면 Adobe Workfront은 작업에 수행한 변경 사항을 즉시 저장합니다. 프로젝트 업데이트 형식에 대한 자세한 내용은 [프로젝트 업데이트 형식 선택](../../../manage-work/projects/manage-projects/select-project-update-type.md)을 참조하세요.
* Workfront은 다른 사용자가 시스템의 다른 곳에서 변경할 수 있는 변경 사항으로 매분 작업 중인 목록의 정보를 업데이트합니다. 이를 통해 항상 작업에 대한 최신 정보를 얻을 수 있습니다.

여러 사용자가 동일한 작업을 편집할 때 다음과 같은 시나리오가 있습니다.

* **한 사용자가 작업 목록에 변경 사항을 자동으로 저장하고 다른 사용자가 수동으로 저장함**: 사용자 B가 동일한 작업을 편집하지만 변경 사항을 자동으로 저장하는 동안 사용자 A가 변경 사항을 수동으로 저장하는 경우 사용자 B의 실시간 변경 사항이 사용자 A의 목록에 매 분 업데이트됩니다. 두 사용자의 변경 사항이 충돌하는 경우 수동으로 저장하는 사용자(사용자 A)에게 변경 사항을 저장하기 전에 경고 메시지가 표시됩니다. 경고 메시지는 충돌하는 변경 사항이 있는 항목을 보여 줍니다. 이때 사용자 A는 변경 내용을 유지해야 할지(사용자 B의 변경 내용을 덮어씀) 아니면 버려야 할지(사용자 B의 변경 내용을 유지함) 선택할 수 있습니다.

>[!NOTE]
>
>변경한 내용을 취소하도록 선택하면 다른 사용자가 편집한 내용과 충돌하는 경우뿐만 아니라 모든 변경 내용에 적용됩니다.

* **여러 사용자가 수동으로 작업 목록에 변경 내용을 저장하고 있습니다**: 목록의 작업을 변경하는 여러 사용자가 동시에 수동으로 저장하는 경우 Workfront에서는 먼저 저장한 사용자가 변경한 내용을 저장합니다. 이러한 변경 사항을 저장하면 충돌이 발생하지 않습니다. 그런 다음 Workfront는 다른 모든 사용자가 변경한 내용을 이미 저장한 정보와 비교하며 다른 사용자가 정보를 저장하기 전에 충돌하는 변경 내용에 대한 경고를 표시합니다.

>[!IMPORTANT]
>
>다른 모든 변경 사항에 대해 변경 사항을 유지하기로 선택한 경우 변경한 작업이 다른 사용자에 의해 삭제되지 않는 한 모든 변경 사항이 저장됩니다. 이 경우 경고 메시지는 삭제된 작업에 대한 변경 내용이 손실되었음을 알려줍니다.

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
