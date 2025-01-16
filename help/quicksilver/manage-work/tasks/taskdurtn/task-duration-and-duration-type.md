---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 작업 기간 및 기간 유형 개요
description: 작업 기간은 작업의 계획된 완료 일자와 계획된 시작 일자 간의 차이입니다. 기간은 작업을 완료하는 데 사용할 수 있는 기간을 나타냅니다.
author: Alina
feature: Work Management
recommendations: noDisplay, noCatalog
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '1649'
ht-degree: 1%

---

# 작업 기간 및 기간 유형 개요

<!-- Audited: 12/2023 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

작업 기간은 작업의 계획된 완료 일자와 계획된 시작 일자 간의 차이입니다. 기간은 작업을 완료하는 데 사용할 수 있는 기간을 나타냅니다.

작업의 기간 유형은 작업에 할당된 리소스 수, 총 작업량 및 작업의 총 기간 간의 관계를 식별합니다.

## 작업 기간 개요

작업의 실제 시작 및 실제 완료 일자가 프로젝트, 기본 담당자 또는 기본 일정의 일정을 벗어나는 경우 작업 기간은 0입니다.

>[!BEGINSHADEBOX]

**예**
오전 9시에 시작하여 오후 12시에 끝나는 일정과 오후 2시에 시작하여 오후 4시에 끝나도록 예정된 작업이 있는 경우 작업의 기간은 0입니다.


>[!ENDSHADEBOX]

다음은 Adobe Workfront에서 기간을 계산할 때 발생하는 두 가지 시나리오입니다.

* 작업이 한 명의 사용자에게 할당된 경우:

   1. Workfront은 프로젝트 또는 작업에 할당된 사용자의 일정을 고려합니다.

      Workfront 또는 그룹 관리자는 작업이 한 사용자에게 할당될 때 Workfront에서 사용하는 일정을 결정합니다. 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

   1. 사용자 또는 프로젝트에 일정이 없는 경우 Workfront은 시스템 기본 일정을 사용합니다.

      단계는 Workfront에서 기간을 계산하는 데 사용하는 일정을 파악한 후 첫 번째 시나리오와 유사합니다.

* 작업이 여러 사용자에게 할당된 경우:

   1. Workfront은 프로젝트 또는 기본 피할당자의 일정을 고려합니다.

      Workfront 또는 그룹 관리자는 작업이 여러 사용자에게 할당될 때 Workfront에서 사용하는 일정을 결정합니다. 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

   1. 기본 담당자 또는 프로젝트에 일정이 없는 경우 Workfront은 시스템 기본 일정을 사용합니다.

  단계는 Workfront에서 기간을 계산하는 데 사용하는 일정을 파악한 후 첫 번째 시나리오와 유사합니다.

>[!NOTE]
>
>프로젝트에 대한 기본 피할당자의 휴가를 고려할 때 작업의 계획된 일자가 조정될 수 있지만 작업의 기간은 동일하게 유지됩니다. 프로젝트를 계획할 때 기본 피할당자의 휴무 시간을 고려하는 방법에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

## 작업 기간 단위

정규 시간과 계획된 시작 일자와 계획된 완료 일자 사이의 경과 시간 모두에 작업 기간을 표시할 수 있습니다.

목록의 작업 기간을 업데이트할 때 Workfront에서 시간 단위를 표시하기 위해 다음 약자를 사용할 수 있습니다.

| 시간 단위 | 약어 |
|---|---|
| 분 | M |
| 시간 | H |
| 일. 이것이 기본값입니다. | D |
| 주 | 주 |
| 개월 | T, MO |
| 경과 시간(분) | EM |
| 경과 시간 | EH |
| 경과 일수 | 에드 |
| 경과 주수 | EW |
| 경과 기간(월) | ET |

{style="table-layout:auto"}

>[!BEGINSHADEBOX]

**예**

작업의 기간을 3일 경과로 나타내려면 작업 목록 의 기간 필드에 &quot;3 ED&quot;를 입력합니다.  작업을 편집할 때 또는 작업 세부 정보 섹션에서 사용 가능한 드롭다운 메뉴에서 기간 단위 기본 옵션을 선택할 수도 있습니다. 작업 편집에 대한 자세한 내용은 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md)을 참조하세요.


>[!ENDSHADEBOX]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

작업 기간을 표시할 때는 다음 사항을 고려하십시오.

* 경과 시간은 작업 기간에 대한 시간 단위입니다. 휴일, 주말 및 휴무를 포함하는 작업의 계획된 시작 일자와 계획된 완료 일자 사이의 시간입니다. 즉, 경과 시간은 역일이 경과된 때이다.
* 일은 시스템에 정의된 근무일을 나타내며 설정 영역에서 구성할 수 있습니다. 대부분의 경우 하루는 8시간으로 구성됩니다.
* 정규 시간(일 또는 근무일)은 휴일, 주말 및 휴무를 고려하여 작업 기간에서 제외합니다.
* 작업 기간을 주 단위로 표시하면 Workfront은 Workfront 관리자가 설정의 프로젝트 환경 설정 영역에서 설정한 주당 일반 근무일 및 근무일당 일반 시간 설정을 기반으로 기간을 계산합니다.
* Workfront은 기간(월)을 계산할 때 한 달에 대해 4주의 기본 기간을 사용합니다.

## 작업 기간 유형 개요

작업의 기간 유형을 관리하면 작업의 요구 사항에 따라 일관된 자원 할당을 설정할 수 있습니다.

기간 유형은 다음 질문에 답변하는 데 도움이 됩니다.

* 얼마나 바쁜가요?
* 그 일은 얼마나 큰가요?
* 얼마나 걸리나요?

![duration_type_triangle.png](assets/duration_type_triangle.png)

## 기간 유형 정의

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="row"><p><strong>기간 유형</strong></p></th> 
   <th scope="col"> <p><strong>함수</strong> </p> </th> 
   <th scope="col"> <p><strong>리소스가 영향을 미치는 방식</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th scope="col"> <p><strong>계산된 할당</strong> </p> </th> 
   <td scope="col"> <p>작업의 각 할당자에 대한 할당 비율을 계산합니다. </p> <p>이 기간 유형을 선택하면 작업에 대해 개별 기간 및 계획된 시간을 입력할 수 있습니다. Workfront은 계획된 시간을 작업 기간 내의 시간 수로 나눈 다음 작업에 할당된 리소스 수로 나누어 각 할당자에 대한 할당을 계산합니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">기간 유형 개요: 계산된 할당</a>을 참조하십시오.</p> </td> 
   <td scope="col">작업에 할당자를 추가하거나 제거할 때 기간 및 계획된 시간은 변경되지 않습니다. </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>계산된 작업</strong> </p> </th> 
   <td scope="col"> <p>작업을 완료하는 데 필요한 계획된 시간(작업량)을 결정합니다.</p> <p>일반적으로 작업에 할당된 리소스가 작업의 전체 기간 동안 할당되는 경우 사용됩니다.</p> <p>이 기간 유형을 선택하면 작업에 대해 개별 기간을 입력할 수 있습니다. Workfront은 해당 기간의 일 수에 일정의 작업 시간 수와 작업에 대한 할당자 수를 곱하여 작업에 대한 계획된 시간을 계산합니다. </p> <p>각 할당자의 할당 백분율을 수동으로 작업에 변경하여 계획된 시간의 양을 줄일 수 있습니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">기간 유형 개요: 계산된 작업</a>을 참조하세요.</p> </td> 
   <td scope="col"> <p>피할당자가 작업에 추가되면 계획된 시간이 늘어납니다. </p> <p>피할당자가 작업에서 제거되면 계획된 시간이 감소합니다.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>작업량 고정</strong></p> </th> 
   <td scope="col"> <p>리소스 수에 따라 계획된 시간을 결정합니다.</p> <p>이 기간 유형을 선택하면 작업에 대해 개별 기간을 입력할 수 있습니다. Workfront은 해당 기간의 일 수에 일정의 작업 시간을 곱한 후 이를 작업에 대한 할당자 수로 나누어 작업의 계획된 시간을 계산합니다. </p> <p>작업에 대한 각 할당자의 할당 백분율을 수동으로 변경할 수 있지만 계획된 시간 수는 동일하게 유지됩니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">기간 유형 개요: 작업량 고정</a>을 참조하십시오.</p> </td> 
   <td scope="col"> <p>피할당자가 작업에서 제거되면 계획된 시간이 증가합니다.</p> <p>피할당자가 작업에 추가되면 계획된 시간이 줄어듭니다. </p> <p>피할당자 수 또는 일정이 변경되더라도 기간은 변경되지 않습니다. </p> <p>기간은 계획된 시간과 같습니다. 계획된 기간은 계획된 시간을 할당자의 수로 나눈 시간과 같습니다.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>단순</strong> </p> </th> 
   <td scope="col"> <p>각 할당자에 할당된 시간을 기반으로 하여 계획된 시간과 기간(이 기간 유형에 대해 동일함)을 결정합니다. </p> <p>Workfront은 각 할당자에 대해 계획된 할당 시간을 합산하여 계획된 시간을 계산합니다. </p> <p>각 할당자가 할당된 시간을 수동으로 변경할 수 있으며 계획된 시간 수 및 기간 금액이 그에 따라 변경됩니다. 모든 피할당자에 대해 할당된 총 시간 수를 선택하는 경우 해당 시간은 각 피할당자 간에 균등하게 분할됩니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">기간 유형 개요: 단순</a>을 참조하세요.</p> </td> 
   <td scope="col"> <p>할당된 총 시간 수를 선택하면 시간이 할당자 간에 균등하게 분배됩니다. 그러나 프로젝트 관리자는 각 할당자에 대해 시간을 수동으로 조정할 수 있습니다. </p> <p>단순 기간 유형 인라인 또는 작업 수준에서 작업의 계획된 시간 및 기간을 편집할 수 있습니다. </p> <p>애자일 팀이 작업에 할당되면 기간 유형이 자동으로 단순으로 설정되며 변경할 수 없습니다. 애자일 팀의 작업 기간은 0분 이상이어야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 새 작업의 기간 유형

새 작업의 기간 유형이 시스템에 설정된 기간 유형과 일치합니다. 기본 기간 유형은 계산된 지정입니다. Workfront 관리자 또는 그룹 관리자는 시스템 또는 프로젝트와 연결된 그룹에 대한 기본 기간 유형을 업데이트할 수 있습니다. 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)을 참조하십시오.

## 상위 작업의 원래 기간

원래 작업 기간은 작업이 상위 작업이 되기 전에 원래 있었던 기간(분)입니다.

작업이 상위가 되면 가장 이른 하위의 계획된 시작 일자와 마지막 하위의 계획된 완료 일자 사이의 기간이 상위 작업에 롤업되고 상위 작업의 기간이 됩니다. 이렇게 하면 원래 작업의 기간이 대체됩니다.

하위 항목이 경과 일수의 기간 단위를 사용하고 상위 항목이 기간 단위 일을 사용하는 경우 Workfront에서 상위 작업의 기간을 계산하는 방식에 불일치가 있을 수 있습니다.

다음 사항을 고려하십시오.

* 기간 단위 경과 일수는 달력 일을 나타내며, 항상 일별 24시간으로 구성됩니다.
* 기간 단위 일수는 시스템에 정의된 근무일을 나타내며, 구성 가능합니다. 대부분의 경우 하루에 8시간으로 구성되어 있습니다.
* 상위 작업의 기간을 계산하는 공식은 다음과 같습니다.

  `Parent task duration = Planned Completion Date of the child task that is planned to end the latest - Planned Start Date of the child task that starts the earliest`

* 상위 작업의 기간을 계산할 때 시스템은 먼저 위의 공식으로 기간을 계산한 다음 일정을 적용합니다.


자세한 내용은 [원래 기간 및 원래 계획된 시간의 개요](/help/quicksilver/manage-work/tasks/task-information/task-original-duration-and-original-planned-hours.md)를 참조하십시오.

## 작업의 기간 유형 변경

작업의 기간 유형 변경에 대한 자세한 내용은 [작업의 기간 유형 업데이트](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)를 참조하십시오.
