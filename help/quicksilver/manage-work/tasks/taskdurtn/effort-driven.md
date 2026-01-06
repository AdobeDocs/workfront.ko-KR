---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '기간 유형 개요: 작업량 고정'
description: 작업량 고정 유형은 Adobe Workfront에서 작업에 대해 설정할 수 있는 기간 유형입니다. Workfront의 기간 유형에 대한 일반 정보는 작업 기간 및 기간 유형 개요를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 1%

---

# 기간 유형 개요: 작업량 고정

작업량 고정 유형은 Adobe Workfront에서 작업에 대해 설정할 수 있는 기간 유형입니다. Workfront의 기간 유형에 대한 일반적인 정보는 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)를 참조하십시오.

## 작업량 고정 기간 유형 개요

Workfront 또는 그룹 관리자는 시스템 또는 그룹의 기본 기간 유형을 작업량 고정(Effort Driven)으로 설정할 수 있습니다. 이 경우 모든 새 작업은 이 기간 유형으로 만들어집니다. 시스템 수준 또는 그룹 수준 프로젝트 환경 설정의 일부로 작업 및 문제 환경 설정을 변경하는 방법에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)을 참조하십시오.

이 시나리오에서는 프로젝트 관리자로서 해당 작업이 실제로 작업주도형 작업인지 숙고하는 시간을 갖지 않는 한 프로젝트 계획을 임의로 단축할 위험이 있다.

노력 기반 사용:

* 작업에 사용할 수 있는 리소스 수에 따라 계획된 기간을 결정합니다. 기간은 계획된 시간과 같습니다. 계획된 기간은 계획된 시간을 할당자의 수로 나눈 시간과 같습니다.

  작업에 적용되는 노력 수준은 분업과 기간을 결정한다.

* 여러 자원이 배정될 때 작업에 소요된 총 시간을 추적합니다.

  리소스가 추가되면 작업의 계획된 기간이 줄어듭니다. (많은 사람이 가볍게 작업한다는 원칙은 이 기간 유형이 작업의 계획된 기간에 미치는 영향을 보여줍니다.)

다음 섹션에서는 Workfront이 작업량 고정 작업의 계획된 지속 시간을 계산하는 방법과 이 기간 유형의 작업에 리소스를 추가하는 것의 영향에 대해 자세히 설명합니다.

## 투입 고정 기간 유형 공식 개요

기간 유형이 투입 고정 작업인 작업의 계획된 기간을 계산하는 공식은 작업에 할당된 각 자원의 할당 비율에 따라 달라집니다. 작업량 고정 작업의 경우 Workfront은 작업의 계획된 시간을 계산하며 이 시간은 항상 작업의 기간과 동일합니다.

```
Planned Hours (in hours) = Duration (in days)
```

작업 기간을 수동으로 조정할 수 있습니다.

Workfront은 근무일에 8시간이 있다고 가정합니다. Workfront 또는 그룹 관리자는 설정의 프로젝트 환경 설정에서 일반 근무일당 시간 설정을 사용하여 근무일당 시간을 정의합니다. 시스템 수준 프로젝트 환경 설정의 일부로 작업 및 문제 환경 설정을 변경하는 방법에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)을 참조하십시오.

>[!TIP]
>
>Workfront은 작업에 할당된 각 자원의 일정을 고려하여 작업의 각 자원에 대한 할당 비율을 결정합니다. 일정을 만들고 사용자에게 할당하는 방법에 대한 자세한 내용은 [일정 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)를 참조하세요.

다음 시나리오를 고려하십시오.

* [리소스가 작업에 100% 할당됨](#resources-are-allocated-100-to-the-task)
* [자원이 작업에 다양한 시간 비율로 할당됩니다.](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### 자원이 작업에 100% 할당됨 {#resources-are-allocated-100-to-the-task}

이 공식은 모든 자원이 작업에 100% 할당된다고 가정합니다.

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

이 계산에서는 정상 근무일의 시간 수가 8이라고 가정합니다. 방정식에 이 값이 포함되므로 계획된 기간 이 일 단위로 표시됩니다.

### 자원이 작업에 다양한 시간 비율로 할당됩니다. {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

할당된 각 자원은 고유한 할당 레벨을 가질 수 있으므로 실제 공식은 다음 할당 값을 고려합니다.

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

이 계산에서는 정상 근무일의 시간 수가 8이라고 가정합니다. 방정식에 이 값이 포함되므로 계획된 기간 이 일 단위로 표시됩니다.

## 작업에 더 많은 리소스 추가 효과

작업량 고정 기간 유형이 있는 작업에 피할당자를 추가하거나 제거할 때 기간 및 계획된 시간은 변경되지 않습니다. 그러나 계획된 기간은 변경되지 않습니다.

다음 예제에서는 시스템 설정의 프로젝트 환경 설정에서 근무일당 일반 시간을 8로 설정합니다. 기간이 3일이므로 계획된 시간은 24(3일 x 근무일당 8시간 = 24 계획된 시간)로 설정됩니다.

>[!NOTE]
>
>고정 일자 작업 제한 사항을 사용할 때 피할당자를 추가하거나 제거할 때 계획된 기간은 동일하게 유지되며, 대신 기간 및 계획된 시간이 조정됩니다. 고정 일자 이외의 작업 제한 사항을 사용할 경우 계획된 기간이 조정됩니다.

다음 표는 작업에 리소스를 추가하면 계획된 기간이 어떻게 변경되는지 보여줍니다.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong>피할당자 수(각각 100% 할당됨)</strong> </p> </th> 
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
   <td> <p>24시간</p> <p>(3일 x 근무일당 8시간 = 24시간 계획된 시간)</p> </td> 
   <td> <p>3일</p> <p>(24시간 계획된 시간 / 할당자 1명 = 3일)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3일</p> </td> 
   <td> <p>24시간</p> <p>(3일 x 근무일당 8시간 = 24시간 계획된 시간)</p> </td> 
   <td> <p>1.5일</p> <p>(24시간 계획 / 담당자 2명 = 12시간 또는 1.5일)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3일</p> </td> 
   <td> <p>24시간</p> <p>(3일 x 근무일당 8시간 = 24시간 계획된 시간)</p> </td> 
   <td> <p>1일</p> <p>(24시간 계획 / 담당자 3명 = 8시간 또는 1일)</p> </td> 
  </tr> 
 </tbody> 
</table>

## 작업의 기간 유형을 작업량 고정 항목으로 변경

작업의 기간 유형 변경에 대한 자세한 내용은 [작업의 기간 유형 업데이트](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)를 참조하십시오.

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
