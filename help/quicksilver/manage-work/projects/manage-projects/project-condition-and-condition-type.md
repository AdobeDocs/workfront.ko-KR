---
title: 프로젝트 조건 및 조건 유형 개요
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: 프로젝트 조건 은 프로젝트가 진행되는 방식을 시각적으로 나타냅니다. 이 변수는 프로젝트의 계획, 예상 및 예상 날짜 간의 관계에 의해 결정되는 보고 가능한 변수입니다.
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# 프로젝트 조건 및 조건 유형 개요

프로젝트 조건 은 프로젝트가 진행되는 방식을 시각적으로 나타냅니다. 이 변수는 프로젝트의 계획, 예상 및 예상 날짜 간의 관계에 의해 결정되는 보고 가능한 변수입니다.

## 프로젝트 조건 개요

프로젝트의 조건을 이해하려면 다음 사항을 고려하십시오.

* 프로젝트 소유자는 프로젝트의 조건이 수동으로 설정되었는지 또는 자동으로 설정되었는지 결정할 수 있습니다. 프로젝트의 조건은 다음과 같은 방법으로 설정할 수 있습니다.

   * 수동으로, 프로젝트 관리에 액세스할 수 있는 사용자와 프로젝트의 조건 유형이 수작업으로 설정된 경우.
   * 프로젝트의 조건 유형이 진행 상태로 설정되어 있으면 자동으로 Adobe Workfront이 지정합니다. 프로젝트의 진행 상태는 프로젝트의 작업 진행 상태에 의해 결정됩니다. 프로젝트의 진행 상태에 대한 자세한 내용은 [프로젝트 진행 상태 개요](../../../manage-work/projects/planning-a-project/project-progress-status.md).

   프로젝트의 조건 유형을 업데이트하는 방법에 대한 자세한 내용은 다음을 참조하십시오 [프로젝트의 조건 유형 설정](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md).

* Workfront에서 프로젝트의 상태를 자동으로 예측할 수 있도록 허용하는 경우 작업 진행 상태가 프로젝트의 실제 진행 상황과 진행 상태를 반영하도록 작업에 선행 작업을 사용하는 것이 좋습니다.
* 프로젝트 소유자는 조건 유형을 진행 상태에서 수동으로 변경하여 진행 상태를 사용하는 대신 수동 조건 유형을 사용하도록 프로젝트를 변경할 수 있습니다.

   >[!NOTE]
   >
   >작업 날짜 및 진행 상태에 관계없이 다음 상태 중 하나에 있는 프로젝트는 항상 Target 상태로 표시됩니다.
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

## Workfront이 진행 상태를 기반으로 프로젝트 조건을 업데이트하는 방법

프로젝트의 조건 유형이 수작업으로 설정되면 프로젝트의 조건이 프로젝트의 진행 상태와 독립적인지를 결정할 수 있습니다.

그러나 작업의 진행 상태에 따라 프로젝트의 실제 진행 상황을 명확하게 나타낼 수 있도록 프로젝트의 조건 유형을 진행 상태로 설정하는 것이 좋습니다. Workfront이 프로젝트의 진행 상태를 계산하는 방법에 대한 자세한 내용은 다음을 참조하십시오 [프로젝트 진행 상태 개요](../../../manage-work/projects/planning-a-project/project-progress-status.md).

이 경우 프로젝트 조건의 값은 다음과 같습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>프로젝트 조건</td> 
   <td>프로젝트 진행 상태</td> 
   <td>Workfront 조건 표시기</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>대상</td> 
   <td> <li>프로젝트 진행 상태 설정 시 프로젝트 조건은 다음과 같습니다 <strong>Target 시</strong>.</li> </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>위험 상태</td> 
   <td>프로젝트의 진행 상태가 <strong>뒤</strong> 또는 <strong>위험</strong>로 설정되면 프로젝트의 조건이 <strong>위험</strong>.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>문제 발생</td> 
   <td>프로젝트의 진행 상태가 <strong>늦게</strong>로 설정되면 프로젝트의 조건이 <strong>문제 발생</strong>. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>환경에 맞게 조건을 사용자 지정할 수 있으므로 환경에서 조건에 대한 옵션을 세 개 이상 찾을 수 있습니다. 조건 이름은 위에 나열된 이름과 다를 수 있습니다. 의 조건 사용자 지정에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 조건 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## 프로젝트 조건, 프로젝트 조건 갱신 및 마지막 조건 참고에 대한 보고서

프로젝트 보고서 보기에서 프로젝트 조건과 관련된 다음 필드를 표시할 수 있습니다.

* **프로젝트 조건:** 프로젝트의 현재 조건을 표시합니다.
* **프로젝트 조건 업데이트**: 프로젝트 소유자가 프로젝트의 업데이트 스트림에 새 조건과 함께 제공한 최신 업데이트를 표시합니다.\
   조건 업데이트에 대한 댓글은 **조건 업데이트** column; 기본 업데이트만 표시됩니다.

* **마지막 조건 참고**: 객체 소유자가 객체에 마지막으로 입력한 업데이트를 표시합니다. 이 필드는 개체의 최근 활동이나 상호 작용을 표시하는 데 유용합니다.\
   다음 **마지막 조건 참고** 개체의 마지막 메모 텍스트가 삭제된 경우 열이 비어 있습니다. 객체에 새 메모를 입력하면 마지막 메모가 되고 열에 다시 표시됩니다.

보고서를 만드는 방법에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
