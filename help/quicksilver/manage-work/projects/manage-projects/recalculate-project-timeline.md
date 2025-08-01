---
product-area: projects
navigation-topic: manage-projects
title: 프로젝트 타임라인 다시 계산
description: 타임라인을 다시 계산하면 관리자는 프로젝트와 관련된 다양한 요소가 프로젝트의 타임라인에 미치는 영향을 확인할 수 있습니다. 프로젝트의 타임라인은 계획된 일자와 예상 일자를 나타냅니다.
author: Alina
feature: Work Management
exl-id: ec5d9a07-e45a-4aa2-9f41-9421ca5d5920
source-git-commit: d846f2f90a8ca2a38c1b18897341cb50f4c5aef4
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 0%

---

# 프로젝트 타임라인 다시 계산

<!--Audited: 06/2025-->

타임라인을 다시 계산하면 관리자는 프로젝트와 관련된 다양한 요소가 프로젝트의 타임라인에 미치는 영향을 확인할 수 있습니다. 프로젝트의 타임라인은 계획된 일자와 예상 일자를 나타냅니다.

일정, 직원 휴가 및 프로젝트 범위를 벗어나는 기타 항목을 변경하는 것은 프로젝트 타임라인에 즉시 영향을 주지 않습니다. 타임라인이 다시 계산되면 프로젝트 타임라인이 영향을 받습니다. 외부 영향은 다시 계산이 발생할 때까지 프로젝트에 영향을 주지 않습니다.

이 문서에서는 타임라인 재계산이 발생하는 방법에 대해 설명합니다.

프로젝트 작업에 관련된 모든 사용자에 대해 특별한 액세스 권한 없이 자동 타임라인 재계산이 수행됩니다. 또한 타임라인을 수동으로 다시 계산할 수 있습니다.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

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
   <td> <p>표준 </p> 
    <p>플랜 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p>시스템 관리자가 시스템의 모든 프로젝트에 대한 타임라인을 다시 계산</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 관리</p>  </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 자동 재계산

기본적으로 프로젝트 타임라인은 프로젝트 범위가 변경될 때 매일 또는 매일 밤 자동으로 다시 계산됩니다. Workfront 관리자는 설정의 프로젝트 환경 설정 영역에서 타임라인 설정을 관리하여 매일 밤 또는 모든 범위 변경 시 타임라인을 자동으로 계산할지 여부를 결정합니다. 자세한 내용은 [프로젝트에 대한 타임라인 다시 계산 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md)을 참조하십시오.

>[!IMPORTANT]
>
>* 프로젝트의 타임라인이 15년을 초과하는 경우 해당 프로젝트에 대해 자동 재계산이 비활성화되며 수동 업데이트 유형만 선택할 수 있습니다. 프로젝트의 날짜를 15년 미만으로 변경하는 경우 타임라인이 자동으로 계산되기 전에 한 번 수동으로 다시 계산해야 합니다.
>* 미리보기 및 사용자 지정 새로 고침 샌드박스 환경의 경우 야간 다시 계산이 비활성화되고 프로젝트 타임라인이 자동으로 다시 계산되지 않습니다. 미리보기 및 사용자 지정 새로 고침 샌드박스 환경에 대한 프로젝트 타임라인을 수동으로 다시 계산해야 합니다.
>* 프로젝트가 복잡한 경우 자동 타임라인 재계산이 수행되지 않을 수 있습니다.
>  &#x200B;> 복잡한 프로젝트의 예로는 여러 종속성, 많은 작업 수, 여러 프로젝트 간 전임 작업 또는 여러 작업 들여쓰기가 있는 프로젝트가 있을 수 있습니다.
>  &#x200B;> Workfront은 프로젝트 페이지의 프로젝트 이름 오른쪽에 프로젝트 타임라인을 수동으로 다시 계산해야 한다는 경고를 표시합니다. 프로젝트에 대한 관리 권한이 있는 사용자만 타임라인을 수동으로 다시 계산할 수 있습니다.
>
>   ![](assets/project-warning-to-manually-recalculate-timeline.png)
>

* [프로젝트 타임라인 자동 다시 계산](#automatic-recalculation-of-project-timelines)
* [프로젝트 타임라인의 자동 재계산을 트리거하는 작업](#actions-that-trigger-an-automatic-recalculation-of-project-timelines)



### 프로젝트 타임라인 자동 재계산 {#automatic-recalculation-of-project-timelines}

Workfront은 다음 조건이 모두 충족되는 프로젝트에 대해서만 매일 타임라인을 다시 계산합니다.

* 현재 상태
* 프로젝트 업데이트 유형이 자동 또는 자동으로 설정되고 변경 시 로 설정됩니다.

  자세한 내용은 [프로젝트 업데이트 형식 개요](../../../manage-work/projects/planning-a-project/project-update-type-overview.md)를 참조하십시오.

* 지난 3개월 내에 마지막 업데이트 날짜가 있습니다. Workfront 관리자는 이 기본 기능을 변경할 수 있습니다. 자세한 내용은 [프로젝트에 대한 타임라인 다시 계산 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md)을 참조하십시오.

* 프로젝트 타임라인의 마지막 계산 날짜가 현재 역일 내에 없습니다. 즉, 프로젝트 타임라인의 마지막 계산 날짜가 현재 날짜의 00:00 이전입니다.

프로젝트의 타임라인이 업데이트되는 빈도를 구성할 수 있습니다. 프로젝트 타임라인이 업데이트되면 프로젝트에 대한 변경 사항을 기반으로 다시 계산됩니다.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
or changes made to another project that the timeline is dependent on
</MadCap:conditionalText>
-->


<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: above, the last part is drafted because of this: I don't think this is right because we told people that in the case of cross-project predecessors, the timeline must be calculated manually for the successor to see the updates in the predecessor's project. Drafting for now.)</p>
-->

자세한 내용은 [프로젝트 업데이트 형식 선택](../../../manage-work/projects/manage-projects/select-project-update-type.md)을 참조하세요.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;content moved to the article linked above)</p>
<p>You can configure how the timeline for your project is updated:</p>
<ol>
<li value="1">Go to the project for which you want to configure how the timeline is updated.</li>
<li value="2"> <p>  Click the <strong>More</strong> icon <img src="assets/more-icon.png"> to the right of the project name, then click&nbsp; <strong>Edit</strong>. </p> <p>The <strong>Edit Project</strong> dialog box is displayed.</p> </li>
<li value="3"> <p>Click<strong>Settings.</strong><br><img src="assets/screen-shot-2013-09-18-at-10.36.16-am-350x347.png" alt="" style="width: 350;height: 347;"></p> </li>
<li value="4">In the <strong>Update Type</strong> drop-down list, select from the following options:<br><strong>- Automatic and On Change:</strong> (Default setting) The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. The project timeline is also updated each night. <br>This is the recommended setting for this field because it ensures that the project timeline is always up to date.<br>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed.
<div>
<p><img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"></p>
</div><br>This indicates that the recalculation is not yet finished, and the dates are subject to change. <br><strong>- Change Only:</strong> The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur.<br>You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on.<br><strong>- Automatic Only:</strong> The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on.<br><note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note><br><strong>- Manual Only:</strong> The project timeline is updated only when you select the option to Recalculate Timelines, as described in <a href="#manual-recalculation" class="MCXref xref">Manual recalculation</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).<br>For more information about the project Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a><note type="note">
If the timeline of a project is longer than 15 years, the automatic recalculation is disabled. If you change the dates on the project to less than 15 years, you must manually recalculate your timeline one time before it is calculated automatically.
</note></li>
<li value="5">Click <strong>Save Changes.</strong></li>
</ol>
</div>
-->

### 프로젝트 타임라인의 자동 재계산을 트리거하는 작업 {#actions-that-trigger-an-automatic-recalculation-of-project-timelines}

프로젝트 수명의 다양한 범위 변경 사항은 다음 작업을 포함하여 프로젝트 타임라인을 자동으로 다시 계산합니다.

* 작업 상태를 업데이트하는 중입니다.
* 작업을 다른 프로젝트로 이동.
* 작업의 계획된 일자 또는 계획된 완료 일자 업데이트.
* 작업의 기간 유형, 작업 제한 또는 할당자 수 업데이트.
* 작업 전임 작업 관계를 업데이트하는 중입니다.
* 작업의 계획된 완료 일자에 시간을 추가하는 작업에 승인 추가.\
  승인 설정에 대한 자세한 내용은 [전역 승인 설정 구성](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)을 참조하세요.

## 수동 재계산 {#manual-recalculation}

프로젝트 소유자는 개별 프로젝트에 대한 타임라인을 수동으로 다시 계산할 수 있습니다. Workfront 관리자는 Workfront의 모든 타임라인을 수동으로 다시 계산할 수 있습니다.

* [개별 프로젝트 또는 일괄적으로 타임라인 다시 계산](#recalculate-timelines-for-individual-projects-or-in-bulk)
* [프로젝트 편집 상자에서 타임라인을 수동으로 일괄적으로 다시 계산](#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box)
* [시스템의 모든 프로젝트에 대한 타임라인 다시 계산(Workfront 관리자만)](#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only)

### 개별 프로젝트에 대한 타임라인 또는 일괄적으로 다시 계산 {#recalculate-timelines-for-individual-projects-or-in-bulk}

프로젝트 페이지나 프로젝트 목록 또는 보고서에서 Workfront의 프로젝트 타임라인을 다시 계산할 수 있습니다.

1. 타임라인을 다시 계산할 프로젝트로 이동한 다음 프로젝트 이름 왼쪽에 있는 **자세히** 아이콘 ![추가 메뉴](assets/qs-more-menu.png)를 클릭합니다.

   또는

   프로젝트 목록 또는 보고서로 이동하여 하나 또는 여러 프로젝트를 선택한 다음 목록 맨 위에 있는 **자세히** 아이콘 ![추가 메뉴](assets/qs-more-menu.png)를 클릭합니다.

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >프로젝트의 복잡성에 따라 최적의 성능을 보장하기 위해 타임라인을 일괄 재계산할 때 많은 수의 프로젝트를 선택하지 않는 것이 좋습니다. 프로젝트를 너무 복잡하게 만들 수 있는 몇 가지 사항은 여러 종속성 또는 할당이거나 사용자 정의 필드의 수가 많을 수 있습니다.

1. **타임라인 다시 계산**&#x200B;을 클릭합니다. 타임라인이 다시 계산되고 성공 메시지가 화면에 표시됩니다.

   >[!TIP]
   >
   >타임라인 재계산이 완료되기 전에 일부 계획된 또는 예상 일자가 흐리게 표시될 수 있습니다. 이는 재계산이 아직 완료되지 않았으며 날짜는 변경될 수 있음을 의미합니다.

### 프로젝트 편집 상자에서 수동으로 타임라인 일괄 재계산 {#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box}

여러 프로젝트를 일괄적으로 편집하여 타임라인을 수동으로 다시 계산할 수 있습니다.

>[!TIP]
>
>프로젝트의 복잡성에 따라 최적의 성능을 보장하기 위해 일괄 편집할 때 많은 수의 프로젝트를 선택하지 않는 것이 좋습니다. 프로젝트를 너무 복잡하게 만들 수 있는 몇 가지 사항은 여러 종속성 또는 할당이거나 사용자 정의 필드의 수가 많을 수 있습니다.

1. 프로젝트 목록으로 이동합니다.
1. 목록에서 여러 프로젝트를 선택한 다음 **편집**&#x200B;을 클릭합니다.
1. **설정**&#x200B;을 클릭한 다음 **타임라인 다시 계산**&#x200B;을 선택합니다.

1. **변경 내용 저장**&#x200B;을 클릭합니다.

### 시스템의 모든 프로젝트에 대한 타임라인 다시 계산(Workfront 관리자만) {#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only}

Workfront 관리자는 타임라인 다시 계산 진단을 실행하여 Workfront 시스템의 모든 타임라인을 즉시 다시 계산할 수 있습니다. 이를 통해 모든 프로젝트 관리자는 계획된 일자와 예상 일자 모두에 대한 외부 변경 사항의 영향을 즉시 확인할 수 있습니다.

전체 Workfront 사이트의 타임라인 다시 계산에 대한 자세한 내용은 [프로젝트에 대한 타임라인 다시 계산 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md)에서 전체 Workfront 인스턴스의 타임라인 다시 계산 섹션을 참조하십시오.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Project Update Types</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to thisa rticle: /Content/Manage work/Projects/Planning a Project/project-update-type-overview.htm)</p>
<p>For information about how to update the project's Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>. </p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<p>You can select how each project calculates its timeline by choosing between the following Update Types:</p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<ul>
<li> <p><strong>Automatic and On Change:</strong>&nbsp;This is the default setting. The project timeline is updated each time a change occurs&nbsp;in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.&nbsp; <br>This is the recommended setting as it ensures that the project timeline is always up to date.</p> <p>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. </p> <p> <img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"> </p> <p>This indicates that the recalculation is not yet finished, and the dates are subject to change. </p> </li>
<li><strong>Change Only:</strong>&nbsp;The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur. <br>You might want to select this option if you are concerned about system performance and if&nbsp;changes rarely occur in the project or in other projects that the timeline is dependent on.</li>
<li> <p><strong>Automatic Only:</strong>&nbsp;The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.</p> <note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note> </li>
<li><strong>Manual Only:</strong>&nbsp;The project timeline is updated only&nbsp;when you select the option to <strong>Recalculate Timelines</strong>, as described in the section "Manual Recalculation" in&nbsp;the article <a href="#" class="MCXref xref selected">Recalculate project timelines</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</li>
</ul>
</div>
-->
