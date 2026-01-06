---
title: 프로젝트 상태 및 상태 유형 개요
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: 프로젝트 상태는 프로젝트가 진행되는 방식을 시각적으로 보여 줍니다. 프로젝트의 계획, 예상, 추정 일자 간의 관계에 의해 결정되는 보고 가능한 변수이다.
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# 프로젝트 상태 및 상태 유형 개요

<!-- Audited: 12/2023 -->

프로젝트 상태는 프로젝트가 진행되는 방식을 시각적으로 보여 줍니다. 프로젝트의 계획, 예상, 추정 일자 간의 관계에 의해 결정되는 보고 가능한 변수이다.

## 프로젝트 상태 개요

프로젝트의 상태를 이해하려면 다음 사항을 고려하십시오.

* 프로젝트 소유자는 프로젝트의 상태를 수동으로 설정할지 자동으로 설정할지를 결정할 수 있습니다. 프로젝트의 상태는 다음과 같은 방법으로 설정할 수 있습니다.

   * 프로젝트 관리에 대한 액세스 권한이 있고 프로젝트의 상태 유형이 수동으로 설정된 경우 사용자가 수동으로 생성합니다.
   * 프로젝트의 상태 유형이 진행 상태로 설정된 경우 Adobe Workfront에서 자동으로 수행합니다. 프로젝트의 진행 상태는 프로젝트에 대한 작업의 진행 상황에 따라 결정됩니다. 프로젝트의 진행 상태에 대한 자세한 내용은 [프로젝트 진행 상태 개요](../../../manage-work/projects/planning-a-project/project-progress-status.md)를 참조하십시오.

  프로젝트의 상태 유형을 업데이트하는 방법에 대한 자세한 내용은 [프로젝트의 상태 유형 설정](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md)을 참조하십시오.

* Workfront에서 프로젝트의 상태를 자동으로 추정하도록 허용할 때 작업 진행 상태가 프로젝트의 실제 진행 상황 및 진행 상황에 반영되도록 작업에 전임 작업을 사용하는 것이 좋습니다.
* 프로젝트 소유자는 상태 유형을 진행 상태에서 수동으로 변경하여 진행 상태를 사용하는 대신 수동 상태 유형을 사용하도록 프로젝트를 변경할 수 있습니다.

  >[!NOTE]
  >
  >다음 상태의 프로젝트는 작업 및 진행 날짜에 관계없이 항상 [대상에]로 표시됩니다.
  >
  >* 아이디어
  >* 요청됨
  >* 승인됨
  >* 거부됨

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set the Condition Type for a project</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted here and moved it to a separate article: /Content/Manage work/Projects/Manage projects/set-condition-type-for-project.htm)</p>
<ol>
<li value="1">Go to the project for which you want to update the Condition Type. </li>
<li value="2"> <p>  Click the <strong>More</strong> menu <img src="assets/qs-more-menu.png"> to the right of the project name, then click <strong>Edit</strong>.  <br> </p> </li>
<li value="3">In the <strong>Condition Type</strong> field, choose one of the following:
<ul>
<li><p><strong>Manual:</strong> The project owner sets the Condition on the project manually.</p><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In this case, the project owner can update the Condition of the project in the project header, or the Project Details section. </p></li>
<li><p><strong>Progress Status:</strong> Workfront sets the Condition based on the Progress Status of the project. <br></p></li>
</ul></li>
<li value="4">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Workfront이 진행 상태를 기반으로 프로젝트 상태를 업데이트하는 방법

프로젝트의 상태 유형을 수동으로 설정하면 프로젝트의 진행 상태와 독립적으로 프로젝트의 상태를 확인할 수 있습니다.

하지만 작업의 진행 상황을 기반으로 프로젝트의 실제 진행 상황을 명확하게 나타낼 수 있도록 프로젝트의 상태 유형을 진행 상태로 설정하는 것이 좋습니다. Workfront에서 프로젝트의 진행 상태를 계산하는 방법에 대한 자세한 내용은 [프로젝트 진행 상태 개요](../../../manage-work/projects/planning-a-project/project-progress-status.md)를 참조하십시오.

이 경우 프로젝트 조건의 값은 다음과 같을 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>프로젝트 상태</strong></td> 
   <td><strong>프로젝트 진행 상태</strong></td> 
   <td><strong>Workfront 조건 표시기</strong></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>대상</td> 
   <td>정시의 프로젝트 진행 상태일 때 프로젝트의 상태는 <strong>On Target</strong>입니다. </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>위험 상태</td> 
   <td>프로젝트의 진행 상태가 <strong>늦어짐</strong> 또는 <strong>위험</strong>인 경우 프로젝트의 상태는 <strong>위험</strong>입니다.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>문제 발생</td> 
   <td>프로젝트의 진행 상태가 <strong>지연</strong>인 경우 프로젝트의 상태는 <strong>문제 발생</strong>입니다. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>사용자 환경에 맞게 조건을 사용자 정의할 수 있으므로 사용자 환경에서 조건에 대한 세 가지 이상의 옵션을 찾을 수 있습니다. 조건의 이름은 위에 나열된 조건과 다를 수 있습니다. 에서 조건을 사용자 지정하는 방법에 대한 자세한 내용은 문서 [사용자 지정 조건 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)을 참조하십시오.

## 프로젝트 상태, 프로젝트 상태 업데이트 및 마지막 상태 메모에 대한 보고서

프로젝트 보고서 보기에서 프로젝트의 상태와 관련된 다음 필드를 표시할 수 있습니다.

* **프로젝트 상태:**&#x200B;은(는) 프로젝트의 현재 상태를 표시합니다.
* **프로젝트 상태 업데이트**: 프로젝트 소유자가 새 상태와 함께 프로젝트의 업데이트 스트림에 제공한 최신 업데이트를 표시합니다.\
  조건 업데이트에 대한 댓글은 **조건 업데이트** 열에 표시되지 않고 기본 업데이트만 표시됩니다.

* **마지막 상태 메모**: 개체 소유자가 개체에 마지막으로 입력한 업데이트를 표시합니다. 이 필드는 객체에 대한 소유자의 가장 최근 활동이나 상호 작용을 표시하는 데 유용합니다.\
  개체의 마지막 메모의 메모 텍스트를 삭제한 경우 **마지막 조건 메모** 열이 비어 있습니다. 객체에 새 메모를 입력하면 마지막 메모가 되고 열에 다시 표시됩니다.

보고서를 만드는 방법에 대한 자세한 내용은 문서 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하십시오.
