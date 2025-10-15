---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '기간 유형 개요: 계산된 작업'
description: 계산된 작업은 Adobe Workfront에서 작업에 설정할 수 있는 기간 유형입니다. Workfront의 기간 유형에 대한 일반 정보는 작업 기간 및 기간 유형 개요를 참조하십시오.
author: Alina
feature: Work Management
exl-id: f521c2f5-8d58-44c0-af18-6940ad0950ea
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 1%

---

# 기간 유형 개요: 계산된 작업

계산된 작업은 Adobe Workfront에서 작업에 설정할 수 있는 기간 유형입니다. Workfront의 기간 유형에 대한 일반적인 정보는 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)를 참조하십시오.

## 계산된 작업 기간 유형 개요

계산된 작업 시간에 따라 작업을 완료하는 데 필요한 작업량(계획된 시간)이 결정됩니다. 작업에 할당된 리소스를 작업의 전체 기간에 할당할 때 계산된 작업 기간 유형을 사용하는 것이 좋습니다.

Workfront 또는 그룹 관리자는 시스템 또는 그룹의 기본 기간 유형을 계산된 작업으로 설정할 수 있습니다. 이 경우 모든 새 작업은 이 기간 유형으로 만들어집니다. 시스템 수준 또는 그룹 수준 프로젝트 환경 설정의 일부로 작업 및 문제 환경 설정을 변경하는 방법에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)을 참조하십시오.

자원이 작업에 추가되면 프로젝트 관리자는 계획된 작업량 증가를 예상할 수 있습니다. 예를 들어, 세 개의 리소스로 구성된 1시간 계획 회의는 세 개의 총 필수 작업 시간을 나타내고, 10개의 리소스로 구성된 1시간 계획 회의는 10개의 필수 작업 시간을 나타냅니다. 각 자원이 100% 할당된 작업에 할당된다고 가정한다.

## 계산된 작업 기간 유형을 사용할 때 필요한 작업 시간을 계산하는 공식 검토

작업에 대해 계산된 작업 기간 유형을 사용할 때 Workfront은 다음 두 가지 공식을 사용하여 각 작업에 대한 작업량을 계산합니다. 공식은 각 자원이 작업에 할당된 시간의 백분율과 각 작업에 할당한 자원의 수에 따라 다릅니다.

* 간소화된 공식: 작업에 하나의 자원이 지정되어 있고 가용 시간의 100% 동안 작업에 할당되어 있다고 가정할 경우, 각 작업에 대한 작업 필요 값은 다음 공식을 사용하여 계산됩니다.

```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```

* 복합 공식: 다양한 할당으로 각 자원을 지정하는 경우 공식은 이러한 할당을 고려하여 다음 변형에 대한 계정을 만듭니다.

```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```

## 작업에서 리소스 추가 또는 제거의 효과 검토

계산된 작업 기간 유형의 작업에 피할당자를 추가하거나 제거할 때 기간은 수동으로 편집할 수 있습니다. 피할당자가 작업에 추가되거나 제거되면 계획된 시간이 변경됩니다.

다음 예에서는 [설정]의 [프로젝트 환경 설정]에서 [근무일당 일반 시간]이 8로 설정되어 있습니다. 각 작업의 기간은 1일입니다. 할당자 수가 변경되면 계획된 시간은 주어진 작업의 할당자 수에 따라 변경됩니다.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>피할당자 수(각각 100% 할당됨)</strong> </p> </th> 
   <th> <p><strong>기간</strong> </p> </th> 
   <th> <p><strong>계획된 시간</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>1</p> </td> 
   <td> <p>1일</p> </td> 
   <td> <p>8시간</p> <p>(1일 x 근무일당 8시간 x 피할당자 1명 = 계획된 시간 8시간)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>2</p> </td> 
   <td> <p>1일</p> </td> 
   <td> <p>16시간</p> <p>(1일 x 근무일당 8시간 x 피할당자 2명 = 계획된 시간 16시간)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>3</p> </td> 
   <td> <p>1일</p> </td> 
   <td> <p>24시간</p> <p>(1일 x 근무일당 8시간 x 피할당자 3명 = 계획된 시간 24시간)</p> </td> 
  </tr> 
 </tbody> 
</table>

이 경우, 각 할당자는 계산된 작업 작업에 100% 할당됩니다.

![](assets/calcwork-350x71.png)

## 작업의 기간 유형을 계산된 작업으로 변경

작업의 기간 유형 변경에 대한 자세한 내용은 [작업의 기간 유형 업데이트](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)를 참조하십시오.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Work</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
