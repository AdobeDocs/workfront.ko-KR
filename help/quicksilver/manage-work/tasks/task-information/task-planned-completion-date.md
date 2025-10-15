---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 작업 계획 완료 일자 개요
description: 작업의 계획된 완료 일자는 작업이 완료되도록 설정된 일자입니다.
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 1%

---

# 작업 계획 완료 일자 개요

작업의 계획된 완료 일자는 작업이 완료되도록 설정된 일자입니다.

작업의 계획된 완료 일자 를 지정하거나 특정 기준에 따라 Adobe Workfront에 맡겨 계산할 수 있습니다.

프로젝트의 작업의 계획된 완료 일자에 따라 프로젝트가 시작 일자부터 예약된 경우 프로젝트의 계획된 완료 일자가 결정됩니다. 프로젝트 계획 완료 날짜에 대한 자세한 내용은 [프로젝트 계획 완료 일자 설정](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)을 참조하십시오.

>[!NOTE]
>
>작업의 계획된 완료 일자는 다음과 같은 방식으로 작업의 커밋 일자 또는 작업의 예상 완료 일자와 다릅니다.
>
>* 커밋 일자는 작업에 할당된 사용자가 작업을 완료할 것으로 수동으로 예상하는 일자입니다. 자세한 내용은 다음 문서를 참조하십시오.
>
>   * [커밋 일자 개요](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [커밋 일자와 계획된 완료 일자 간의 상호 작용](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* 예상 완료 일자 는 Workfront에서 계산한 일자로, 작업 지연, 작업 또는 전임 작업의 타임라인 및 기타 요소를 고려하여 작업이 실제로 완료될 수 있는 실제 일자를 결정합니다. 자세한 내용은 [프로젝트, 작업 및 문제의 예상 완료 일자 개요](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)를 참조하십시오.
>

## 작업의 계획된 완료 일자 수동 설정

작업의 계획된 완료 일자를 업데이트하려면 작업에 대한 편집 액세스 권한과 작업에 대한 관리 권한이 있어야 합니다.

작업의 계획된 완료 일자 설정은 작업에 할당하는 작업 제한 유형에 따라 다릅니다.

Workfront의 다음 영역에서 계획된 완료 일자 를 수동으로 설정할 수 있습니다.

* 작업을 만들거나 편집할 때 작업 편집 상자에서 확인할 수 있습니다. 자세한 내용은 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md)을 참조하세요.
* 작업 세부 정보 영역입니다. 자세한 내용은 [작업 세부 정보 개요 영역에서 작업 정보 관리](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)를 참조하십시오.
* 요약 패널에서 작업을 볼 때 계획된 완료 일자 가 표시되는 경우 홈 영역에 표시됩니다. 자세한 내용은 [홈 영역에서 작업 항목 업데이트 또는 편집](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md)을 참조하세요.
* 작업 헤더에서. 자세한 내용은 [새 개체 헤더](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md)를 참조하십시오.
* 뷰에 계획된 완료 일자 필드가 표시되는 경우 작업 목록 또는 보고서에서

  자세한 내용은 [목록의 작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)을 참조하세요.

다음 태스크 제한조건 중 하나를 선택하면 계획된 완료 일자를 수동으로 지정할 수 있습니다.

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
   <td> <p>다음까지 완료</p> <p>다음보다 늦지 않게 완료</p> <p>다음 이후에 완료</p> </td> 
   <td> <p><span class="s1">기간을 동일하게 유지하기 위해 계획된 시작 날짜가 조정되었습니다.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>고정 일자</p> </td> 
   <td> <p>계획된 시작 일자를 동일하게 유지하기 위해 기간이 조정됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront에서 작업에 대한 계획된 완료 일자를 자동으로 계산하는 방법

시스템에서 자동으로 계산되는 경우 다음 사항은 작업의 계획된 완료 일자에 영향을 줄 수 있습니다.

* 작업 제한 사항

  작업 제한에 대한 자세한 내용은 [작업 제한 개요](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) 문서를 참조하십시오.

* 작업 전임 작업 관계

  작업 전임 작업에 대한 자세한 내용은 [작업 전임 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) 문서를 참조하십시오.

* 프로젝트 완료 일자(프로젝트가 완료 일자부터 예약된 경우).
* 작업의 기본 피할당자의 휴무 일정입니다.

  작업 기간 동안 기본 피할당자에게 휴무가 예약되어 있는 경우 **사용자 휴무** 필드에 대해 **작업 기간에서 사용자 휴무 고려** 설정을 선택하면 작업의 계획된 날짜가 그에 따라 조정됩니다. 새 프로젝트는 프로젝트 환경 설정 영역에서 이 설정을 상속하지만 프로젝트 수준에서 설정을 편집할 수 있습니다.

  예를 들어, &quot;가능한 한 빨리&quot; 제한이 있는 작업이 6월 1일에 시작하여 6월 3일에 완료되도록 예약되어 있고 기본 피할당자가 6월 2일에 휴무로 표시된 경우, 작업 계획 완료 일자는 6월 4일이 됩니다.

  **사용자 휴가** 기본 설정에 대한 자세한 내용은 [시스템 전체 프로젝트 기본 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) 또는 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md) 문서를 참조하십시오.

* 작업이 승인과 연결된 경우 승인 설정과 연결된 시간입니다. 자세한 내용은 [전역 승인 설정 구성](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)을 참조하세요.

자동으로 설정된 경우 다음 계산에 따라 계획된 완료 일자가 결정됩니다.

```
Planned Completion Date = Planned Start Date + Duration
```

예를 들어 작업의 시작 일자가 9월 16일이고 기간이 10일인 경우 계획된 완료 일자는 9월 26일입니다.

>[!NOTE]
>
> 계획된 시간 및 기간을 자동으로 조정하려면 프로젝트의 업데이트 유형을 자동 및 변경 시 또는 자동으로 설정해야 합니다.\
>업데이트 유형에 대한 자세한 내용은 문서 [프로젝트 업데이트 유형 선택](../../../manage-work/projects/manage-projects/select-project-update-type.md)을 참조하십시오.
