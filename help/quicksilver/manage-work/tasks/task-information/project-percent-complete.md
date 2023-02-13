---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 프로젝트 완료율 개요
description: 프로젝트의 완료 퍼센트 값은 프로젝트의 계획 기간 또는 계획 시간 작업을 기준으로 계산됩니다. Adobe Workfront 관리자 또는 그룹 관리자는 프로젝트 환경 설정 영역에서 정보를 구성할 때 시스템에서 완료율을 계산할 때 고려할 값을 정의합니다. 프로젝트 환경 설정 구성에 대한 자세한 내용은 시스템 전체 프로젝트 환경 설정 구성을 참조하십시오.
author: Alina
feature: Work Management
exl-id: d2395569-9fe5-42e7-a392-cff49eb519d9
source-git-commit: 31533bd7ee1890a8343d32770d623d5d9a6007d2
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# 프로젝트 완료율 개요

프로젝트의 완료 퍼센트 값은 프로젝트의 기간 또는 계획 시간 작업을 기준으로 계산됩니다. Adobe Workfront 관리자 또는 그룹 관리자는 프로젝트 환경 설정 영역에서 정보를 구성할 때 시스템에서 완료율을 계산할 때 고려할 값을 정의합니다.

프로젝트 환경 설정 구성에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

상위 태스크의 완료율은 각 하위 태스크의 기간 또는 계획 시간을 기준으로 합니다.

마찬가지로, 프로젝트의 완료율은 프로젝트의 각 주요 작업의 기간 또는 계획 시간을 기반으로 합니다.

기본 작업은 상위 작업과 하위 항목이 없는 독립 실행형 작업입니다.

>[!TIP]
>
>기본 작업은 프로젝트 계획에서 들여쓰지 않습니다.

## Workfront이 완료율을 계산하는 방법

* [작업에서 완료율 업데이트](#update-the-percent-complete-on-a-task)
* [Workfront이 상위 작업에서 완료율을 계산하는 방법](#how-workfront-calculates-percent-complete-on-a-parent-task)
* [Workfront이 프로젝트에 대한 완료율을 계산하는 방법](#how-workfront-calculates-percent-complete-on-a-project)

### 작업에서 완료율 업데이트 {#update-the-percent-complete-on-a-task}

작업 완료율을 수동으로 수정할 수 있습니다. 이것은 계산이 아닙니다.

Workfront에서는 개별 작업의 완료율을 사용하여 상위 작업의 완료율 또는 프로젝트 완료율을 계산합니다.

작업 완료율 업데이트에 대한 자세한 내용은 [작업에 대한 완료율 보기 및 갱신](../../../manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

### Workfront이 상위 작업에서 완료율을 계산하는 방법 {#how-workfront-calculates-percent-complete-on-a-parent-task}

시스템 또는 그룹 레벨의 프로젝트 환경설정에서 선택한 Workfront 또는 그룹 관리자의 작업에 따라 상위 작업에 대한 완료 백분율이 기간 또는 계획 시간 작업을 기반으로 계산됩니다.

다음 시나리오를 고려하십시오.

* 시스템에서 계획 시간을 기준으로 완료 퍼센트를 계산하는 경우 상위 태스크 완료율은 다음 공식을 사용하여 계산됩니다.

   `Parent Task Percent Complete = (((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of Parent)*100`

   상위의 총 계획 시간은 각 1차 하위 구성요소의 모든 계획 시간의 합계를 나타냅니다.

   ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

* 시스템에서 지속 기간을 기준으로 완료 퍼센트를 계산하는 경우, 상위 태스크 완료율은 다음 공식을 사용하여 계산됩니다.

   `Parent Task Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/ Total Duration of Parent)*100`

   ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

   >[!IMPORTANT]
   >
   >상위 작업의 총 기간은 하위 작업의 모든 기간의 합계입니다. 예를 들어, 각 기간이 1일 및 2일인 두 하위 작업이 있는 상위 작업은 두 하위 작업이 같은 날에 시작할 수 있더라도 총 3일의 기간을 갖습니다.


### Workfront이 프로젝트에 대한 완료율을 계산하는 방법 {#how-workfront-calculates-percent-complete-on-a-project}

시스템 또는 그룹 수준의 프로젝트 환경 설정에서 선택한 Workfront 또는 그룹 관리자가 프로젝트에 대한 완료 백분율은 프로젝트에 있는 주요 작업의 기간 또는 계획 시간을 기반으로 계산됩니다.

* 시스템에서 계획 시간을 기준으로 완료 퍼센트를 계산하는 경우 프로젝트 완료 퍼센트는 다음 공식을 사용하여 계산됩니다.

   `Project Percent Complete =(((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of the Project)*100`

   프로젝트의 총 계획 시간은 프로젝트에 있는 모든 주요 작업의 계획 시간 합계입니다.

   ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

   >[!NOTE]
   >
   >작업 1 또는 작업 2는 상위 작업 또는 독립형 작업만 될 수 있습니다. 1차 하위 구성요소 작업의 계획 시간 및 완료 퍼센트는 이 계산에서 사용되지 않습니다.

* 시스템에서 지속 기간을 기준으로 완료 퍼센트를 계산하는 경우 프로젝트 완료 퍼센트는 다음 공식을 사용하여 계산됩니다.

   `Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

   >[!IMPORTANT]
   >
   >Duration of the Project는 완료율이 표시되는 기본 작업의 모든 기간의 합계입니다. 예를 들어, 지속 기간이 2일인 독립 실행형 태스크가 있는 프로젝트 및 완료된 기간이 5일인 상위 태스크는 두 작업이 같은 날에 시작할 수 있더라도 총 7일의 기간을 갖습니다.

   ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

   >[!NOTE]
   >
   >작업 1 또는 작업 2는 상위 작업 또는 독립형 작업만 될 수 있습니다. 1차 하위 구성요소 작업의 기간 및 완료율은 이 계산에서 사용되지 않습니다.

## 지속 시간을 사용하는 프로젝트의 완료율 예

작업 기간 을 사용하여 프로젝트의 완료율을 계산할 때 다음 예를 생각해 보십시오.

![](assets/project-with-tasks-percent-complete-duration-calculation.png)

다음 정보는 프로젝트의 완료율을 계산하는 데 사용됩니다

* 독립형 작업의 완료율(작업 1 - 20%)
* 상위 작업의 완료율(작업 2 - 25%)
* 작업 기간 1(5일)
* 작업 기간 2(2일)
* 프로젝트 기간(7일)


지속 시간을 사용하여 프로젝트의 완료 비율을 계산하려면

`Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

또는

`(((5*0.2)+(2*0.25))/7)*100= 21.43%`


<!--drafted, this was the old example:

When using the Planned Duration of the tasks to calculate the percent complete of a project, consider the following example:

percent_complete_on_project_example.png

Only the parent task (Task 1) and the standalone task (Task 8) are used to calculate the percent complete of the project.

The secondary parents of Task 1 are used to calculate the percent complete of the main parent (Task 1).

To calculate the percent complete of the main parent (Task 1), first calculate the percent complete of its secondary parents:

Task 5 Percent Complete = ((14 * 0.75 + 12 * 0.25)/(12 + 14))*100 = 51.92%

Task 2 Percent Complete = ((5 * 0.7 + 2 * 0.5)/(5 + 2))*100 = 64.29 %

Then, to calculate the percent complete of the main parent (Task 1), use the following formula:

Task 1 Percent Complete =((56 * 0.5192 + 7 * 0.6429)/63)*100 = 53.29%

To calculate the percent complete of the project, you will need to have the following numbers ready:

Task 1 Duration (63 hours) and Percent Complete (53.29%)
Task 8 Duration (100 hours) and Percent Complete (4%)
Now, to calculate the percent complete of the project, use the following formula:

Project Percent Complete =((100 * 0.04 + 63 * 0.5329))/163)*100 = 23.05%
-->