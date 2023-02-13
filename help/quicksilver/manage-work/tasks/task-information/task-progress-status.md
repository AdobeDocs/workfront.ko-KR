---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 작업 진행 상태 개요
description: Adobe Workfront은 해당 타임라인에서 작업의 진행 상태를 확인하여 작업의 진행 상태를 결정합니다. 작업의 진행 상태 값을 기반으로 프로젝트의 조건을 결정하도록 Workfront을 구성할 수 있습니다. 프로젝트 조건 구성에 대한 자세한 내용은 프로젝트 조건 및 조건 유형 개요 문서를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 38e5f89e-bdfa-433c-9371-3c3003ada3a3
source-git-commit: 65f25a3b1198f491f7357efef11e2ae075e9721a
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 1%

---

# 작업 진행 상태 개요

Adobe Workfront은 해당 타임라인에서 작업의 진행 상태를 확인하여 작업의 진행 상태를 결정합니다. 작업의 진행 상태 값을 기반으로 프로젝트의 조건을 결정하도록 Workfront을 구성할 수 있습니다. 프로젝트 조건 구성에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트 조건 및 조건 유형 개요](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

## 작업의 진행 상태를 결정하는 기준

프로젝트의 진행 상태에 대한 자세한 내용은 [프로젝트 진행 상태 개요](../../../manage-work/projects/planning-a-project/project-progress-status.md).

작업 진행 상태 추적에 대한 자세한 내용은 [작업 추적 모드 개요](../../../manage-work/tasks/task-information/task-tracking-mode.md).

다음 기준은 작업의 진행 상태를 결정합니다.

<table> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>진행 상태</strong> </p> </th> 
   <th> <p><strong>기준 결정</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td scope="col"> <p> </p> <p><strong>정시</strong> </p> </td> 
   <td scope="col"> <p>작업이 고려됩니다 <strong>시간</strong> 모든 계획 일자가 예상 일자와 일치하는 경우 이 진행 상태는 프로젝트가 스케줄 보다 우선하며 예상 일자가 계획 일자 이전일 수도 있음을 의미합니다.</p> <p>예상 날짜에 대한 자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">프로젝트, 작업 및 문제에 대한 예상 완료 일자 개요</a>.</p> <p>작업 계획 완료 날짜에 대한 자세한 내용은 다음 문서를 참조하십시오.</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">작업 계획 시작 일자 개요</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">작업 계획 완료 일자 개요</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><p></p> <p><strong>위험 상태</strong> </p> </td> 
   <td><p>작업이 고려됩니다 <strong>위험</strong> 예상 완료 일자가 계획 완료 일자 이후이고 예상 완료 일자 이후인 경우 작업에 제약 조건이 있을 경우 이 문제가 발생할 수 있습니다 <strong>다음 작업을 완료해야 함</strong> 또는 <strong>시작 시기</strong> 그러나 작업의 완료율 또는 이전 관계를 보면 지정된 날짜에 완료하거나 시작할 수 없음을 알 수 있습니다. </p><p> 작업 제약 조건 설정 <strong>다음 작업을 완료해야 함</strong> 계획된 완료 일자를 특정 일자로 수동으로 설정합니다. 이 경우 예상 완료 일자는 계획 완료 일자와 일치합니다. 이 제한의 경우, Workfront은 작업을 분석하여 완료된 백분율을 기반으로 언제 완료되는지 계산합니다. 이 계산은 예상 만기 일자로 저장됩니다. 예상 완료 일자 이후인 경우 작업이 지연될 위험이 있습니다. </p> <p> 작업 제약 조건 설정 <strong>시작 시기</strong> 계획된 시작 일자를 특정 일자로 수동으로 설정합니다. 이 경우 예상 시작 일자는 계획 시작 일자와 일치합니다. 이 제한 사항의 경우 Workfront은 작업을 분석하여 선행 관계를 기반으로 시작되는 시기를 계산합니다. 이 계산은 예상 시작 날짜로 저장됩니다. 지정된 시작 날짜에 작업을 시작할 수 없는 강제 선행 작업이 있는 경우 예상 시작 일자는 예상 완료 일자 이후일 수 있습니다. 그 일은 지각할 위험이 있다고 여겨진다. </p> <p>참고: 일반적으로 예상 날짜는 <strong>시작 시기</strong> 또는 <strong>다음 작업을 완료해야 함</strong> 이 사용됩니다. 이러한 경우 예상 일자는 완료 퍼센트 및 기타 요소(이전 관계)를 기준으로 계속 계산되며, 예상 일자는 수동으로 설정된 계획 일자와 일치해야 합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>지연됨</strong> </p> </td> 
   <td> <p>작업은 다음과 같습니다 <strong>뒤</strong> 예상 완료 일자가 계획 완료 일자 이후이거나 예상 완료 일자 이전인 경우</p> <p>예상 완료 날짜는 이전 진행 상태에 따라 작업이 완료되는 시점을 실시간으로 보는 것입니다. 작업이 늦게 시작되었지만 계획 및 예상 완료 일자가 아직 미래이고 작업이 제시간에 완료될 수 있으므로 작업이 아직 지연으로 간주되지는 않습니다.</p> <p>참고: 다음 <strong>뒤</strong> 및 <strong>위험</strong> 진행 상태는 거의 동일합니다. 하지만, <strong>위험</strong> 계획 일자 중 하나 또는 둘 다에 일부 강제 태스크 제약(완료, 시작, 고정 일자)이 있음을 나타냅니다. 태스크에 강제 제약 조건이 없는 경우 예상 일자는 예상 일자와 동일하며 태스크의 현재 진행 상태에 따라 완료 일자에 대한 시스템 계산을 반영합니다. 계획 완료 날짜와 예상 완료 날짜가 아직 미래에는 있기 때문에 작업이 아직 지연으로 간주되지 않습니다. 작업이 제 시간에 완료될 수도 있습니다.<br>예상 및 예상 날짜에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">예상 일자와 예상 일자 구분 </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>지연</strong> </p> </td> 
   <td> <p>작업은 <strong>늦게</strong> 계획 완료 일자가 오늘 일자 이전인 경우<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## 시간 경과에 따라 작업 진행 상태 업데이트 방법

프로젝트에서 다른 날짜 유형은 시간이 지남에 따라 작업이 진행되는 방식을 알려줍니다.

* 정시

   ![](assets/on-time-progress-status-350x233.png)

* 위험 상태

   ![](assets/at-risk-progress-status-350x233.png)

* 지연됨

   ![](assets/behind-progress-status-350x233.png)

* 지연

   ![](assets/late-progress-status-350x233.png)
