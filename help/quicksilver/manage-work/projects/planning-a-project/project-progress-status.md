---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 프로젝트 진행 상태 개요
description: Adobe Workfront은 타임라인에서 프로젝트의 진행 상태를 확인하여 프로젝트의 진행 상태를 결정합니다. 작업의 진행 상태 값을 기반으로 프로젝트의 조건을 결정하도록 Workfront을 구성할 수 있습니다. 프로젝트 조건 구성에 대한 자세한 내용은 프로젝트 조건 및 조건 유형 개요 문서를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 1%

---

# 프로젝트 진행 상태 개요

Adobe Workfront은 타임라인에서 프로젝트의 진행 상태를 확인하여 프로젝트의 진행 상태를 결정합니다. 작업의 진행 상태 값을 기반으로 프로젝트의 조건을 결정하도록 Workfront을 구성할 수 있습니다. 프로젝트 조건 구성에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트 조건 및 조건 유형 개요](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

다음은 Workfront에 있는 프로젝트의 진행 상태입니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>시간</td> 
   <td> <p>예상 완료 일자와 예상 완료 일자가 모두 프로젝트의 계획 완료 일자보다 이전이거나 같으면 프로젝트의 진행 상태가 됩니다 <strong>시간</strong>.</p> <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p> </td> 
  </tr> 
  <tr> 
   <td>위험 상태</td> 
   <td> <p>예상 완료 일자와 예상 완료 일자가 모두 미래(미래)이지만 프로젝트의 계획 완료 일자 및 예상 완료 일자보다 늦은 경우 프로젝트 진행 상태는 예상 완료 일자보다 이후입니다 <strong>위험</strong>. </p> <p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>지연됨</td> 
   <td> <p>예상 완료 일자와 예상 완료 일자가 모두 미래(미래)이지만 프로젝트의 계획 완료 일자보다 늦은 경우 예상 완료 일자가 예상 완료 일자보다 이후인 경우 프로젝트 진행 상태는 다음과 같습니다 <strong>뒤</strong>.</p> <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>지연</td> 
   <td> 
    <ul> 
     <li> <p>프로젝트가 완료되고 실제 완료 일자가 계획 완료 일자보다 늦은 경우 프로젝트의 진행 상태는 다음과 같습니다 <strong>늦게</strong>. </p> <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>프로젝트가 완료되지 않고 프로젝트의 계획 완료 일자가 지난 경우 프로젝트 진행 상태는 다음과 같습니다 <strong>늦게</strong>. </p> <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

다음 사항을 고려하십시오.

* 프로젝트의 예상 완료 일자는 가장 최근의 예상 완료 일자가 있는 위기 경로의 작업에 의해 결정됩니다.
* 프로젝트의 예상 완료 일자는 가장 최근의 예상 완료 날짜가 있는 위기 경로의 작업에 의해 결정됩니다.

프로젝트의 중요 경로에 대한 자세한 내용은 [프로젝트 중요 경로 개요](../../../manage-work/tasks/manage-tasks/critical-path.md).

예상 완료 날짜에 대한 자세한 내용은 [프로젝트, 작업 및 문제에 대한 예상 완료 일자 개요](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
