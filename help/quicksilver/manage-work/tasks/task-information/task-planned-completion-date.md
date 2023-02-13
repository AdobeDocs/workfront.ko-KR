---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 작업 계획 완료 일자 개요
description: 작업의 계획 완료 날짜는 작업이 완료되도록 설정된 날짜입니다.
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 1%

---

# 작업 계획 완료 일자 개요

작업의 계획 완료 날짜는 작업이 완료되도록 설정된 날짜입니다.

작업의 계획 완료 날짜를 지정하거나, 특정 기준에 따라 계산하도록 Adobe Workfront에 둘 수 있습니다. 

프로젝트의 계획 완료 일자는 프로젝트가 시작 일자에서 스케줄링될 때 프로젝트의 계획 완료 일자를 결정합니다. 프로젝트 계획 완료 일자에 대한 자세한 내용은 [프로젝트 계획 완료 일자 설정](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>태스크의 계획 완료 일자는 다음과 같은 방법으로 태스크의 커밋 일자 또는 태스크 예상 완료 일자와 다릅니다.
>
>* 커밋 날짜는 작업에 할당된 사람이 작업을 완료했을 것으로 수동으로 추정하는 날짜입니다. 자세한 내용은 다음 문서를 참조하십시오.
   * [커밋 날짜 개요](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
   * [커밋 일자와 계획 완료 일자 간의 상호 작용](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
* 예상 완료 날짜는 Workfront에서 계산된 날짜이며 작업 지연, 작업 또는 이전 작업의 일정 및 기타 요소를 고려하여 작업이 현실적으로 완료될 수 있는 실제 날짜를 결정합니다. 자세한 내용은 [프로젝트, 작업 및 문제에 대한 예상 완료 일자 개요](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>


## 작업의 계획 완료 날짜 수동으로 설정

작업의 계획 완료 날짜를 업데이트하려면 작업에 대한 편집 액세스 권한 및 작업 관리 권한이 있어야 합니다.

작업의 계획 완료 날짜 설정은 작업에 지정하는 작업 제약 조건 유형에 따라 다릅니다. 

Workfront의 다음 영역에서 계획 완료 일자를 수동으로 설정할 수 있습니다.

* 작업 편집 상자에서 작업을 만들거나 편집할 때 자세한 내용은 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* 작업 세부 정보 영역에서 자세한 내용은 [작업 세부 정보 개요 영역의 작업 정보 관리](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* 작업을 볼 때 계획 완료 일자가 표시되는 홈 영역입니다. 자세한 내용은 [홈 영역에서 작업 항목 업데이트 또는 편집](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* 작업 헤더에서 자세한 내용은 [새 개체 머리글](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* 계획 완료 일자 필드가 뷰에 표시되는 경우 작업 목록 또는 보고서에서

   자세한 내용은 [목록의 작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

다음 작업 제약 중 하나를 선택하면 계획 완료 일자를 수동으로 지정할 수 있습니다. 

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>작업 제한 유형</strong> </p> </th> 
   <th> <p><strong>계획 완료 일자 수동 변경 효과</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>다음까지 완료:</p> <p>다음보다 늦지 않게 완료</p> <p>다음 이후에 완료:</p> </td> 
   <td> <p><span class="s1">기간을 동일하게 유지하기 위해 계획 시작 일자가 조정됩니다.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>고정 일자</p> </td> 
   <td> <p>계획 시작 일자를 동일하게 유지하기 위해 기간을 조정합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront에서 작업에 대한 계획된 완료 날짜를 자동으로 계산하는 방법

시스템에서 자동으로 계산되는 경우, 다음은 작업의 계획 완료 날짜에 영향을 줄 수 있습니다.

* 작업 제한 사항

   작업 제한에 대한 자세한 내용은 문서를 참조하십시오 [작업 제한 개요](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* 작업 선행 관계

   작업 전임자에 대한 자세한 내용은 문서를 참조하십시오 [작업 선행 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* 프로젝트 완료 일자, 프로젝트를 완료 일자부터 스케줄링합니다.
* 작업의 기본 할당자의 일정 시간

   기본 할당자가 작업 기간 동안 예약된 시간이 있으면 작업 계획 날짜는 **작업 기간의 사용자 시간 비우기 고려** 이 설정에 대해 선택되어 있습니다 **사용자 해제 시간** 필드. 새 프로젝트는 프로젝트 환경 설정 영역에서 이 설정을 상속하지만 프로젝트 수준에서 설정을 편집할 수 있습니다.

   예를 들어, 가능한 한 빨리 제약 조건이 있는 작업이 6월 1일에 시작하여 6월 3일에 완료되도록 예약되어 있고 기본 할당자가 6월 2일에 타임오프로 표시된 경우 계획 완료 날짜는 6월 4일이 됩니다.

   에 대한 정보 **사용자 해제 시간** 기본 설정에 따라 문서를 참조하십시오 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) 또는 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

* 작업이 승인과 연결된 경우 승인 설정과 연관된 시간입니다. 자세한 내용은 [전역 승인 설정 구성](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

자동으로 설정되면 계획 완료 일자는 다음 계산에 따라 결정됩니다. 

```
Planned Completion Date = Planned Start Date + Duration
```

예를 들어 작업의 시작 날짜가 9월 16일이고 기간이 10일인 경우 계획 완료 날짜는 9월 26일입니다.

>[!NOTE]
 계획 시간 및 기간을 자동으로 조정하려면 프로젝트에 대한 갱신 유형을 자동 및 변경 시 또는 자동으로 설정해야 합니다.\
업데이트 유형에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트 업데이트 유형을 선택합니다](../../../manage-work/projects/manage-projects/select-project-update-type.md).
