---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '기간 유형 개요: 작업 중심'
description: 작업 제어 는 Adobe Workfront에서 작업에 대해 설정할 수 있는 기간 유형입니다. Workfront의 기간 유형에 대한 일반적인 정보는 작업 기간 및 기간 유형 개요를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 1%

---

# 기간 유형 개요: 작업 기반

작업 제어 는 Adobe Workfront에서 작업에 대해 설정할 수 있는 기간 유형입니다. Workfront의 기간 유형에 대한 일반적인 내용은 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## 투입 중심 기간 유형 개요

Workfront 또는 그룹 관리자는 시스템 또는 그룹의 기본 기간 유형을 작업 기반 으로 설정할 수 있습니다. 이 경우 이 기간 유형을 사용하여 새 작업이 모두 생성됩니다. 시스템 수준 또는 그룹 수준 프로젝트 환경 설정의 일부로 작업 및 문제 환경 설정 변경에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

이 시나리오에서는 프로젝트 관리자로 작업이 실제로 투입 주도적 작업인지 여부를 고려하지 않는 한 프로젝트 계획을 임의로 축소시킬 위험이 있습니다.

작업 기반:

* 작업에서 사용할 수 있는 자원의 수를 기준으로 계획 기간을 결정합니다. 기간은 계획 시간과 같습니다. 계획 기간은 계획 시간 을 지정자 수로 나눈 시간과 같습니다.

   태스크에 적용되는 투입 수준은 노무 및 기간 분리를 결정합니다.

* 여러 리소스가 할당될 때 작업에서 걸린 총 시간 수를 추적합니다.

   자원이 추가되면 작업의 계획 기간이 줄어듭니다. (&quot;많은 손으로 작업을 수행하는 방식&quot;의 원칙은 이 기간 유형이 작업의 계획 기간에 미치는 영향을 나타냅니다.)

다음 섹션에서는 Workfront이 투입 중심 작업의 계획 기간을 계산하는 방법과 이 기간 유형을 사용하여 작업에 리소스를 추가하는 효과에 대한 자세한 정보를 제공합니다.

## 투입 제어 기간 유형 배합표의 개요

지속 기간 유형이 투입 중심인 태스크에 대한 계획 기간 계산 공식은 태스크에 지정된 각 자원의 할당 비율에 따라 달라집니다. 작업 기반 작업의 경우, Workfront은 작업의 계획 시간을 계산하며 항상 작업 기간과 동일합니다.

```
Planned Hours (in hours) = Duration (in days)
```

작업 지속 시간을 수동으로 조정할 수 있습니다.

Workfront에서는 작업일에 8시간이 있다고 가정합니다. Workfront 또는 그룹 관리자는 설정의 프로젝트 환경 설정에서 작업당 일반 시간 설정을 사용하여 작업당 시간 수를 정의합니다. 시스템 수준 프로젝트 환경 설정의 일부로 작업 및 문제 환경 설정 변경에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!TIP]
>
>Workfront은 작업에 할당된 각 리소스에 대한 일정을 고려하여 해당 작업에 대한 각 리소스에 대한 할당 비율을 결정합니다. 사용자에게 일정 만들기 및 지정에 대한 자세한 내용은 [예약 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

다음 시나리오를 고려하십시오.

* [자원이 작업에 100% 할당됨](#resources-are-allocated-100-to-the-task)
* [자원은 작업에 대한 다양한 시간 백분율에 대해 할당됩니다](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### 자원이 작업에 100% 할당됨 {#resources-are-allocated-100-to-the-task}

이 공식은 모든 자원이 작업에 100%를 할당한다고 가정합니다.

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

이 계산에서는 일반 작업일의 시간 수가 8이라고 가정합니다. 방정식에 이 값이 포함되므로 계획 기간이 일 단위로 표시됩니다.

### 자원은 작업에 대한 다양한 시간 백분율에 대해 할당됩니다 {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

지정된 각 자원에는 고유한 할당 레벨이 있을 수 있으므로 실제 공식은 이러한 할당 값을 고려합니다.

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

이 계산에서는 일반 작업일의 시간 수가 8이라고 가정합니다. 방정식에 이 값이 포함되므로 계획 기간이 일 단위로 표시됩니다.

## 작업에 리소스를 더 추가하는 효과

작업 중심 기간 유형을 사용하여 태스크에 담당자를 추가하거나 제거할 때 기간 및 계획 시간은 변경되지 않습니다. 하지만 계획 기간은 변경됩니다.

다음 예에서는 System Setup의 Project Preferences에서 General Hours per Work Day가 8로 설정됩니다. 기간이 3일이므로 계획 시간은 24로 설정됩니다(3일 x8시간 = 24시간).

>[!NOTE]
>
>고정 일자 태스크 제약 사용 시 할당을 추가하거나 제거할 때 계획 기간은 동일하게 유지되며 대신 기간 및 계획 시간이 조정됩니다. 고정 일자 이외의 작업 제약 조건을 사용할 경우 계획 기간이 조정됩니다.

다음 표에서는 작업에 리소스를 추가하여 계획 기간이 어떻게 변경되는지를 보여 줍니다.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong>할당자 수(각각 100% 할당됨)</strong> </p> </th> 
   <th> <p><strong>기간</strong> </p> </th> 
   <th> <p><strong>계획된 시간</strong> </p> </th> 
   <th><strong>계획된 기간</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> </td> 
   <td> <p>1</p> </td> 
   <td> <p>3일</p> </td> 
   <td> <p>24시간</p> <p>(3일 x 8시간 근무일 = 24시간 계획 시간)</p> </td> 
   <td> <p>3일</p> <p>(24시간/1할당자 = 3일)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3일</p> </td> 
   <td> <p>24시간</p> <p>(3일 x 8시간 근무일 = 24시간 계획 시간)</p> </td> 
   <td> <p>1.5일</p> <p>(24시간/2명의 담당자 = 12시간 또는 1.5일)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3일</p> </td> 
   <td> <p>24시간</p> <p>(3일 x 8시간 근무일 = 24시간 계획 시간)</p> </td> 
   <td> <p>1일</p> <p>(24시간/3명의 담당자 = 8시간 또는 1일)</p> </td> 
  </tr> 
 </tbody> 
</table>

## 작업의 기간 유형을 작업량 제어로 변경합니다.

작업의 기간 유형 변경에 대한 자세한 내용은 [작업의 기간 유형 업데이트](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Effort Driven</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong><strong>Changes</strong>.</li>
</ol>
-->
