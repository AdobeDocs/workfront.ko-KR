---
content-type: reference
product-area: projects
navigation-topic: convert-issues
title: 해결 가능한 객체 해결 및 해결 방법 개요
description: 해결 가능한 개체는 해결 개체에 연결되어 있는 문제입니다. 해결 개체는 프로젝트, 작업 또는 다른 문제입니다.
author: Alina
feature: Work Management
exl-id: 2ff034ec-6116-42af-a55f-1fb24fc12b2f
source-git-commit: 4c4a8703cca33066f72f8f2088029382edbafc29
workflow-type: tm+mt
source-wordcount: '1732'
ht-degree: 1%

---

# 해결 가능한 객체 해결 및 해결 방법 개요

해결 가능한 개체는 해결 개체에 연결되어 있는 문제입니다. 해결 개체는 프로젝트, 작업 또는 다른 문제입니다.

문제를 작업 또는 프로젝트로 변환하면 해당 문제가 작업 또는 프로젝트의 해결 가능한 개체가 됩니다.

작업, 프로젝트 또는 문제인 해결 개체에 문제를 수동으로 연결할 수도 있습니다. 자세한 내용은 [문제 해결을 다른 문제, 작업 또는 프로젝트에 수동으로 연결](../../../manage-work/issues/convert-issues/manually-tie-resolution-of-issue-to-ptis.md).

원래 문제는 이 시나리오에서 작업, 프로젝트 또는 문제의 해결 가능한 개체가 됩니다.

## 해결 가능한 개체를 처리하도록 Adobe Workfront 설정 {#set-up-adobe-workfront-to-handle-resolvable-objects}

Workfront 관리자 또는 그룹 관리자는 시스템 또는 그룹에서 해결 가능한 개체를 처리하는 방법을 결정할 수 있습니다.

작업 또는 프로젝트로 변환할 때 해결 가능한 개체를 유지하거나 작업 또는 프로젝트가 만들어지면 삭제할 수 있습니다. 문제를 변환하는 과정에서 이러한 설정을 변경할 수 있도록 선택할 수 있습니다. 이렇게 하면 문제를 변환한 사용자가 문제를 변환하면서 유지할 것인지 삭제할 것인지 선택할 수 있습니다.

>[!NOTE]
>
>해결 가능한 개체는 항상 해결 방법 및 상태가 연관된 해결 객체의 해상도 및 상태에 따라 달라질 수 있는 문제입니다. 문제, 작업 또는 프로젝트일 수 있는 객체 해결

해결 가능한 객체 처리를 위한 환경 설정 설정에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: drafted and just pointed the user to the article linked above)&nbsp;</p>
<p>To establish the system default for what happens to the issue as it is being converted to a task or a project:</p>
<ol>
<li value="1">Log in to Workfront as a Workfront administrator <span>or group administrator.</span></li>
<li value="2"> <p>  From the main menu, click <strong>Setup</strong>. </p> <p> <img src="assets/qs-main-menu-expanded-with-menu-highlight-350x521.png" style="width: 350;height: 521;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Expand <strong>Project Preferences</strong>.</li>
<li value="4">Click <strong>Tasks & Issues</strong>.</li>
<li value="5">Go to the <strong>Issues</strong> area of the setup.<br><img src="assets/qs-setup-project-preferences-issues-area-350x214.png" style="width: 350;height: 214;"><br>Consider editing any of the following settings:
<ul>
<li><p><strong>Automatically update Resolvable Issue status when the status of the Resolving Object changes:</strong> Select this option to tie the resolution of the original issue to the resolution of its Resolving Object. In order for this setting to have any effect, the options to <strong>Keep the original issue and tie its resolution to the task</strong> or<strong>project</strong> must be selected.</p>
<ul>
<li>When this setting is enabled, you can create custom statuses with the same key for both issues and projects or tasks. When the project or task (as a resolvable object) turns into the custom status, the change also reflects on the status of the issue. The status key must be the same for the issue and project or task statuses.</li>
<li><p>When this setting is disabled, resolving object statuses are automatically set to the default status, instead of the custom ones. For more information about the default statuses, see <a href="#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p><note type="note">
The default status of the issue is controlled by the status of the project or task, regardless of whether this option is selected or not.
</note></li>
</ul></li>
<li><strong>When converting an issue to a TASK...:</strong> The settings in this section determine what happens during the conversion process from issue to task:
<ul>
<li><strong>Keep the original issue and tie its resolution to the task:</strong> When converting the issue, it remains visible as an issue until the task is complete. The status of the issue automatically changes to Closed when the task completes.</li>
<li><strong>Allow Primary Contact to have access to the task:</strong> Gives the primary contact (issue creator) access to the task to review the task, make updates, and stay informed of its progress.</li>
<li><strong>Allow these settings to be changed during conversion:</strong> Allows the user who is converting the issue to change these options during the conversion of an issue to a task. </li>
</ul></li>
<li><strong>When converting an issue to a PROJECT...:</strong> The settings in this section determine what happens during the conversion process from issue to project:
<ul>
<li><strong>Keep the original issue and tie its resolution to the project:</strong> When converting the issue, it remains visible as an issue until the project is complete. The status of the issue automatically changes to Closed when the project completes.</li>
<li><strong>Allow Primary Contact to have access to the project:</strong> Gives the primary contact (issue creator) access to the project to review the project, make updates, and stay informed of its progress.</li>
<li><strong>Allow these settings to be changed during conversion:</strong> Allows the user who is converting the issue to change these options during the conversion of an issue to a project. </li>
</ul></li>
</ul></li>
<li value="6">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## 프로젝트나 작업으로 변환하는 동안 해결 가능한 개체를 처리합니다

Workfront 또는 그룹 관리자가 시스템 또는 그룹 수준 문제 환경 설정을 구성한 방식에 따라 프로젝트나 작업으로 문제를 변환하는 동안 해결할 수 있는 개체를 처리할 수 있습니다.

다음 시나리오가 있습니다.

* Workfront 또는 그룹 관리자가 **원래 문제를 유지하고 해결 방법을 작업에 연결합니다** 그리고 **원래 문제를 그대로 두고 그 해결책을 프로젝트에 연결합니다** 선택 및 **전환 중에 이러한 설정을 변경할 수 있도록 허용합니다** 선택하지 않으면 문제를 작업 또는 프로젝트로 변환할 때 이러한 설정을 변경할 수 없습니다.\
   ![](assets/qs-setup-project-preferences-issues-area-some-boxes-unselected-350x217.png)

* Workfront 또는 그룹 관리자가 **원래 문제를 유지하고 해결 방법을 작업에 연결합니다** 그리고 **원래 문제를 그대로 두고 그 해결책을 프로젝트에 연결합니다** 선택 또는 선택 취소 및 **전환 중에 이러한 설정을 변경할 수 있도록 허용합니다** 선택한 경우 문제를 작업 또는 프로젝트로 변환할 때 이러한 설정을 변경할 수 있습니다.\
   ![](assets/qs-options-to-keep-issue-when-coverting-it-inside-the-issue-350x113.png)

문제를 작업 및 프로젝트로 변환하는 방법에 대한 자세한 내용은 [Adobe Workfront의 변환 문제 개요](../../../manage-work/issues/convert-issues/convert-issues.md).

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Tie the resolution of an issue to a project, task or </h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: created new article for this section; draft when the article is live and see if you need to make a link from this one to the new article) </p>
<div>
<p>You can manually tie the resolution of an issue to the resolution of a project, task, or issue without converting the issue. The issue becomes one of the Resolvable Objects of the project, task, or issue you select. When you do this, a change in the status of the project, task, or issue triggers a change in the status of the original issue, so you cannot manually edit the status of the original issue. <br>For more information about how the status of the Resolving Object affects the Resolvable Object, see <a href="#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p>
<p>You must have Manage permissions on the original issue and View permissions on the project, task, or issue to do this. </p>
<p>To tie the resolution of an issue to the resolution of a project, task, or issue:</p>
<ol>
<li value="1">Navigate to an issue whose resolution you want to tie to a task or a project.</li>
<li value="2"> <p>  Click the <strong>Issue Details</strong> > <strong>Overview</strong> area. </p> <p> <img src="assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png" style="width: 350;height: 462;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Edit</strong> icon <img src="assets/edit-icon.png"> in the upper-right corner of the Issue Details section. </p> </li>
<li value="4">At the bottom of the form,  click in the <strong>Resolved By</strong> field,  and select from the following types of resolving objects:
<ul>
<li><strong>Project</strong></li>
<li><strong>Task</strong></li>
<li><p><strong>Issue</strong></p></li>
</ul><p>The field for the resolving object displays. </p></li>
<li value="5">After selecting the object, start typing the name of a specific project, task, or issue in the available field and select it when it appears in the drop-down list. </li>
<li value="6">Click <strong>Save</strong>&nbsp;<strong>Changes</strong>.<br>The original issue becomes the Resolvable Object for the project, task, or issue you selected in step 4 and 5.<br><note type="note">
One project, task, or issue may have multiple issues as Resolvable Objects.
</note></li>
</ol>
</div>
</div>
-->

## 해결 가능한 객체의 상태를 해결 객체의 상태와 동기화합니다 {#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object}

* [객체 해결 시 문제가 될 때 상태 동기화](#synchronize-statuses-when-the-resolving-object-is-an-issue)
* [객체 해결이 작업 또는 프로젝트일 때 상태 동기화](#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project)

### 객체 해결 시 문제가 될 때 상태 동기화 {#synchronize-statuses-when-the-resolving-object-is-an-issue}

문제가 다른 문제에 수동으로 연결되어 있으면 두 번째 문제(개체 해결)의 상태가 첫 번째 문제(해결 가능한 개체)의 상태 변경을 트리거합니다. 첫 번째 문제의 상태는 두 번째 문제가 로 변경된 상태와 일치합니다. 이는 기본 및 사용자 지정 문제 상태에 모두 적용됩니다.

### 객체 해결이 작업 또는 프로젝트일 때 상태 동기화 {#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project}

작업 또는 프로젝트의 해결 가능한 개체가 문제가 되면 작업 및 프로젝트의 상태 변경 사항이 문제 상태로 변경됩니다. 기본 상태는 사용자 지정 상태와 다르게 트리거됩니다. 이 경우

* [해결 가능 객체의 기본 상태와 해결 가능 객체의 기본 상태 동기화](#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object)
* [해결 가능 객체의 사용자 정의 상태와 해결 가능 객체의 사용자 정의 상태 동기화](#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object)

#### 해결 가능 객체의 기본 상태와 해결 가능 객체의 기본 상태 동기화 {#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object}

객체 해결(프로젝트 또는 작업)에서 기본 상태가 변경될 때마다 &quot;객체 변경 사항 해결&quot; 옵션의 상태가 선택된 경우 자동으로 해결 가능 문제 상태 업데이트&quot;가 선택되는지의 여부와 관계없이 해결 가능 객체(문제)의 상태가 변경될 때마다 그에 따라 변경됩니다. 이러한 변경을 트리거하기 위해 기본 상태만 이미 매핑되었습니다.

작업에 대한 다음 기본 상태는 문제가 작업의 해결 개체로 설정된 경우 문제의 기본 상태에 다음 변경 사항을 트리거합니다.

| **작업 상태** | **문제 상태** |
|---|---|
| 신규 | 신규 |
| 진행 중 | 진행 중 |
| 완료 | 마감됨 |

프로젝트에 대한 다음 기본 상태는 문제가 프로젝트의 해결 가능 개체로 설정된 경우 문제에 대한 기본 상태에 다음 변경 사항을 트리거합니다. 일부 프로젝트 상태는 문제 상태에 대한 변경 사항을 트리거하지 않습니다. 문제는 프로젝트가 다음 상태 중 하나로 전환되기 전의 상태로 유지됩니다.

| **프로젝트 상태** | **문제 상태** |
|---|---|
| 계획 수립 | 신규 |
| 현재 | 진행 중 |
| 보류 중 | 보류 중 |
| 요청됨 | 문제 상태 변경을 트리거하지 않습니다 |
| 승인됨 | 문제 상태 변경을 트리거하지 않습니다 |
| 거부됨 | 문제 상태 변경을 트리거하지 않습니다 |
| 아이디어 | 문제 상태 변경을 트리거하지 않습니다 |
| 중단 | 마감됨 |
| 완료됨 | 마감됨 |

>[!NOTE]
>
>문제 상태가 닫힘 (작업 또는 프로젝트를 닫은 결과)이 된 후 작업 또는 프로젝트가 변경되는 상태에 관계없이 문제가 닫힘 상태로 유지됩니다.

#### 해결 가능 객체의 사용자 정의 상태와 해결 가능 객체의 사용자 정의 상태 동기화 {#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object}

작업 또는 프로젝트의 상태를 사용자 지정 상태로 변경하면 다음 두 가지 조건이 충족되는 경우에만 문제 상태가 사용자 지정 문제 상태로 변경됩니다.

* 객체 변경 해결(Resolved Issue) 옵션 상태가 선택된 경우 &quot;Automatically update Resolved Issue status(객체 변경 사항 해결)&quot; 옵션을 선택합니다. 이 설정을 활성화하는 방법에 대한 자세한 내용은 [해결 가능한 개체를 처리하도록 Adobe Workfront 설정](#set-up-adobe-workfront-to-handle-resolvable-objects).

* 프로젝트 또는 작업의 사용자 지정 상태는 문제의 사용자 지정 상태와 동일한 세 문자 코드를 갖습니다.

문제와 프로젝트 또는 작업 모두에 대해 동일한 키로 사용자 지정 상태를 만들 수 있습니다. 프로젝트 또는 작업(해결 개체)이 사용자 지정 상태로 변경되면 변경 사항도 문제의 상태에 반영됩니다. 문제 및 프로젝트 또는 작업 상태에 대해 상태 키는 동일해야 합니다.

예를 들어, &quot;Current&quot;와 같은 세 문자 코드 &quot;LCD&quot;를 사용하여 &quot;Launch&quot;라는 프로젝트 사용자 지정 상태를 만듭니다. 또한 &quot;In Progress&quot;와 같은 문자 코드 &quot;LCD&quot;와 함께 &quot;Project Launch&quot;라는 사용자 정의 상태를 만듭니다. 프로젝트를 &quot;시작됨&quot;으로 표시하면 문제가 자동으로 상태를 &quot;프로젝트 시작됨&quot;으로 변경합니다. Resolvable Issue 상태는 개체 변경 해결(Resolving Object changes) 설정이 활성화되지 않은 경우 자동으로 업데이트 해결 가능 문제 상태가 설정되면 문제 상태가 대신 &quot;진행 중&quot;(기본 상태)으로 변경됩니다.

사용자 지정 상태 만들기에 대한 자세한 내용은 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## 해결 가능 객체의 완료율을 해결 가능 객체의 완료율과 동기화합니다

작업 또는 프로젝트에 의해 문제가 해결되면 다음 중 하나가 발생하면 문제 완료율이 해결된 문제에 대해 업데이트됩니다. 

* 작업 또는 프로젝트에 대한 변경 사항을 저장할 때.
* 프로젝트의 타임라인이 다시 계산됩니다.

및 문제가 다른 문제로 해결되면 두 문제 중 하나가 업데이트될 때 완료율이 업데이트됩니다.

## 작업 또는 프로젝트에서 해결 가능한 개체 찾기

해결 객체를 찾는 것은 작업 및 프로젝트에 대해 동일합니다.

1. 문제를 프로젝트 또는 작업으로 변환하여 만든 프로젝트 또는 작업으로 이동합니다.
1. 을(를) 클릭합니다. **프로젝트 세부 사항** 또는 **작업 세부 사항** 아이콘을 클릭하고 클릭하여 확장합니다.
1. 클릭 **개요**.
1. 탭 하단에서 을(를) 찾습니다. **이 문제가 해결됩니다.** 필드: 프로젝트 또는 작업의 해결 가능한 개체인 문제가 이 필드에 나열됩니다.

   >[!NOTE]
   >
   >문제는 다른 문제로 변환할 수 없지만 수동으로 문제 해결과 연결할 수 있습니다. 프로젝트, 작업 또는 문제는 해결 가능한 개체로서 여러 문제를 가질 수 있습니다. 프로젝트, 작업 또는 문제가 해결되면 해결 가능한 개체(문제)도 해결됩니다. 해결된 프로젝트, 작업 또는 문제가 다시 열리는 경우에도 해결 가능한 문제가 닫혀 있습니다.

## 목록에서 개체 해결 문제 식별

문제 목록에서 이 아이콘을 찾아 상태 아이콘을 통해 개체 확인으로 레이블이 지정된 문제를 식별할 수 있습니다 **상태 아이콘** 또는 **플래그** 열:

![](assets/ro1.png)

## 보고서에서 해결 가능한 객체 정보 보기 및 해결

프로젝트, 작업 또는 문제에 대한 보기 또는 보고서에서 해결 가능 또는 해결 객체 관련 정보를 표시할 수 있습니다.\
다음 표는 표시할 수 있는 필드와 표시할 수 있는 보기를 보여 줍니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>보기의 필드</strong> </th> 
   <th><strong>문제 보기</strong> </th> 
   <th><strong>작업 보기</strong> </th> 
   <th><strong>프로젝트 보기</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>해결 가능 여부 있음</strong>: 를 표시합니다 <strong>True</strong> 프로젝트 또는 작업에 관련된 해결 가능한 문제가 있는 경우 값과 <strong>False</strong> 값을 지정한 경우 이해할 수 있도록 해줍니다.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td><strong>원래 문제 이름, 원래 문제 항목 날짜, 작성자 이름</strong>: 원래 문제의 이름 및 시작 날짜와 텍스트 모드 사용자 지정 보기에서 문제를 만든 사용자의 이름을 표시합니다.<br>원래 문제에 대한 정보를 표시하기 위해 프로젝트나 작업 보고서나 목록에 대한 텍스트 모드 사용자 지정 보기를 만드는 방법에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md" class="MCXref xref">보기: 작업 및 프로젝트 목록에 원래 문제 정보 표시</a>.<br></td> 
   <td> </td> 
   <td> ✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>해결 방법:</strong> 프로젝트나 작업 보고서 또는 목록에 대한 텍스트 모드 사용자 지정 보기에 있는 모든 해결 가능 객체 목록을 표시합니다.</p> <p>이 보기 빌드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-resolvable-objects-task-project-report.md" class="MCXref xref">보기: 작업 또는 프로젝트 보고서의 해결 가능한 개체</a></p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td><strong>변환된 문제 작성자</strong>: 문제를 처음 기록한 사용자의 정보를 표시하여 나중에 작업으로 변환했습니다. </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>프로젝트 해결</strong>: 원래 문제로부터 변환되었거나 문제의 해결 개체로 수동으로 지정된 프로젝트 해결에 대한 정보를 표시합니다.</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>작업 해결</strong>: 원래 문제로부터 변환되었거나 문제의 해결 개체로 수동으로 지정된 해결 작업에 대한 정보를 표시합니다.</td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>문제 해결</strong>: 문제의 해결 개체로 수동으로 지정된 문제 해결에 대한 정보를 표시합니다.</td> 
   <td> ✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
