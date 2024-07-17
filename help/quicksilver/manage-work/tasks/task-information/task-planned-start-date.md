---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 작업 계획 시작 일자 개요
description: 작업의 계획된 시작 일자는 작업 생성자가 작업에 대한 작업을 시작해야 한다고 결정하는 일자입니다. 계획된 작업 일자는 프로젝트의 일자 및 타임라인에 영향을 줍니다. 프로젝트 계획 시작 일자에 대한 자세한 내용은 프로젝트 계획 시작 일자 개요를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 2%

---

# 작업 계획 시작 일자 개요

작업의 계획된 시작 일자는 작업 생성자가 작업에 대한 작업을 시작해야 한다고 결정하는 일자입니다. 계획된 작업 일자는 프로젝트의 일자 및 타임라인에 영향을 줍니다. 프로젝트 계획 시작 날짜에 대한 자세한 내용은 [프로젝트 계획 시작 날짜의 개요](../../../manage-work/projects/planning-a-project/project-planned-start-date.md)를 참조하십시오.

## 작업의 계획된 시작 일자

작업의 계획된 시작 일자를 지정하거나 특정 기준에 따라 작업을 Adobe Workfront에 맡겨 계산할 수 있습니다. 

* [작업의 계획된 시작 날짜를 수동으로 설정](#manually-set-the-planned-start-date-of-a-task)
* [작업에 대한 계획된 시작 일자 계산 방법](#how-the-planned-start-date-is-calculated-for-a-task)

### 작업의 계획된 시작 일자 수동 설정 {#manually-set-the-planned-start-date-of-a-task}

작업의 계획된 시작 일자 설정은 작업에 할당하는 작업 제한 유형에 따라 다릅니다. 

[프로젝트에서 작업 만들기](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) 문서에 설명된 대로 작업을 만들 때 계획된 시작 날짜를 수동으로 설정할 수 있습니다.

다음 작업 제한조건 중 하나를 선택하면 계획된 시작 일자를 수동으로 지정할 수 있습니다. 

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>작업 제한 유형</strong> </p> </th> 
   <th> <p><strong>계획된 완료 일자 수동 변경의 영향</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>일자에 시작</p> <p>다음 이후에 시작</p> <p>다음 이전에 시작</p> </td> 
   <td> <p><span class="s1">기간을 동일하게 유지하기 위해 계획된 완료 날짜가 조정되었습니다.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>고정 일자</p> </td> 
   <td> <p>계획된 완료 일자를 동일하게 유지하기 위해 기간이 조정됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 작업에 대한 계획된 시작 일자 계산 방법 {#how-the-planned-start-date-is-calculated-for-a-task}

시스템에서 자동으로 계산되는 경우 다음 사항은 작업의 계획된 시작 일자에 영향을 줄 수 있습니다.

* 설정 의 작업 및 문제 영역에 있는 시작 날짜 환경 설정

  Workfront 또는 그룹 관리자는 새 작업이 프로젝트의 계획된 시작 일자와 동일한 날짜에 시작되는지 또는 작업을 만든 날짜에 시작되는지를 결정할 수 있습니다.

  작업 및 문제 환경 설정에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)을 참조하십시오.

* 작업 제한 사항

  작업 제한에 대한 자세한 내용은 [작업 제한 개요](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) 문서를 참조하십시오.

* 작업 전임 작업 관계

  작업 전임 작업에 대한 자세한 내용은 [작업 전임 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) 문서를 참조하십시오.

* 프로젝트 시작 일자(프로젝트가 시작 일자부터 예약된 경우).
* 작업의 기본 피할당자의 휴무 일정입니다.

  작업 기간 동안 기본 피할당자에게 휴무가 예약되어 있는 경우 **사용자 휴무** 필드에 대해 **작업 기간에서 사용자 휴무 고려** 설정을 선택하면 작업의 계획된 날짜가 그에 따라 조정됩니다. 새 프로젝트는 프로젝트 환경 설정 영역에서 이 설정을 상속하지만 프로젝트 수준에서 설정을 편집할 수 있습니다.

  예를 들어, &#39;가능한 한 빨리&#39;라는 제한 사항이 있는 작업이 6월 1일에 시작하여 6월 3일에 완료되도록 예약되어 있고 기본 피할당자가 6월 1일에 휴무로 표시된 경우, 작업 계획 시작 일자는 6월 2일이 됩니다.

  **사용자 휴가** 기본 설정에 대한 자세한 내용은 [시스템 전체 프로젝트 기본 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) 또는 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md) 문서를 참조하십시오.

자동으로 설정되는 경우 계획된 시작 일자는 다음 계산에 따라 결정됩니다. 

```
Planned Start Date = Planned Completion Date - Task Duration
```

예를 들어 작업의 완료 일자가 9월 16일이고 기간이 10일인 경우 계획된 시작 일자는 9월 6일입니다.

>[!NOTE]
>
> 계획된 시간 및 기간을 자동으로 조정하려면 프로젝트의 업데이트 유형도 &#39;자동 및 변경 시&#39; 또는 &#39;자동&#39;으로 설정해야 합니다.\
>업데이트 유형에 대한 자세한 내용은 문서 [프로젝트 업데이트 유형 선택](../../../manage-work/projects/manage-projects/select-project-update-type.md)을 참조하십시오.
