---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 프로젝트 진행 상태 개요
description: Adobe Workfront은 타임라인 전체에서 프로젝트의 진행률을 확인하여 프로젝트의 진행 상태를 결정합니다. 작업의 진행 상태 값을 기반으로 프로젝트의 상태를 결정하도록 Workfront을 구성할 수 있습니다. 프로젝트 진행 상태에 대해 이 문서에서 자세히 알아보십시오.
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
source-git-commit: 4e3cafafb121371249fb73f2f001477bdbad2d77
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 1%

---

# 프로젝트 진행 상태 개요

<!--Audited: 12/2023-->

Adobe Workfront은 타임라인 전체에서 프로젝트의 진행률을 확인하여 프로젝트의 진행 상태를 결정합니다. 작업의 진행 상태 값을 기반으로 프로젝트의 상태를 결정하도록 Workfront을 구성할 수 있습니다. 프로젝트 상태 구성에 대한 자세한 내용은 문서 [프로젝트 상태 및 상태 형식 개요](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md)를 참조하십시오.

다음은 Workfront에서 프로젝트의 진행 상태입니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>정시</td> 
   <td> 다음과 같은 경우 프로젝트의 진행 상태는 <strong>정시</strong>입니다.<ul><li>예상 완료 일자와 예상 완료 일자가 모두 프로젝트의 계획된 완료 일자와 같거나 이전인 경우</li></ul> <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p> </td> 
  </tr> 
  <tr> 
   <td>위험 상태</td> 
   <td> 다음 중 <strong>모두</strong>이(가) true인 경우 프로젝트의 진행 상태는 <strong>위험</strong>입니다.<ul><li>예상 완료 일자와 예상 완료 일자는 모두 미래입니다.</li><li> 예상 및 예상 완료 일자가 모두 계획된 완료 일자보다 늦습니다.</li><li> 예상 완료 일자가 예상 완료 일자보다 늦음</li></ul><p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>지연됨</td> 
   <td> 다음 중 <strong>모두</strong>이(가) true인 경우 프로젝트의 진행 상태는 <strong>늦음</strong>입니다.<ul><li>예상 완료 일자와 예상 완료 일자는 모두 미래입니다.</li><li> 예상 완료 일자와 예상 완료 일자가 모두 프로젝트의 계획된 완료 일자보다 늦습니다</li><li> 예상 완료 일자는 예상 완료 일자 이후입니다.</li></ul> <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>지연</td> 
   <td> 
     다음 중 <strong>어느 하나</strong>이(가) true인 경우 프로젝트의 진행 상태는 <strong>Late</strong>입니다.<ul><li>프로젝트가 완료되고 실제 완료 일자가 계획된 완료 일자보다 늦습니다. <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>프로젝트가 완료되지 않았고 계획된 완료 일자가 과거입니다. <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

다음 사항을 고려하십시오.

* 프로젝트의 예상 완료 일자는 가장 최근 예상 완료 일자의 중요 경로에 있는 작업에 의해 결정됩니다.
* 프로젝트의 예상 완료 날짜는 가장 늦은 예상 완료 날짜가 있는 중요 경로의 작업에 의해 결정됩니다.

프로젝트의 중요 경로에 대한 자세한 내용은 [프로젝트 중요 경로 개요](../../../manage-work/tasks/manage-tasks/critical-path.md)를 참조하십시오.

예상 완료 날짜에 대한 자세한 내용은 [프로젝트, 작업 및 문제의 예상 완료 날짜 개요](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)를 참조하십시오.
