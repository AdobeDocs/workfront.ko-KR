---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: 리소스 계획자의 프로젝트 및 역할 뷰의 시간, FTE 및 비용 정보 개요
description: 리소스 계획자의 프로젝트 및 역할 뷰의 시간, FTE 및 비용 정보 개요
author: Alina
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '2973'
ht-degree: 0%

---

# 리소스 계획자의 프로젝트 및 역할 뷰의 시간, FTE 및 비용 정보 개요

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

프로젝트에서 수행해야 하는 작업에 대한 자원 예산을 책정하는 것은 자원 계획자의 주요 기능입니다. 리소스의 사용 가능한 시간을 보고 리소스를 할당된 프로젝트에 시간을 할당할 수 있습니다.

리소스 계획자의 예산 책정 자원에 대한 자세한 내용은 [프로젝트 및 역할 보기를 사용하는 자원 계획자의 예산 자원](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)

이 문서에서는 Resource Planner에서 리소스 예산을 짜기 전에 알아야 하는 몇 가지 주요 개념에 대해 설명합니다.

## 예산 책정 리소스 개요

Resource Planner를 사용하여 자원을 예산책정할 때 다음 사항을 고려하십시오.

* 자원 할당에 예산을 편성할 수 있습니다. 이 경우 자원이 프로젝트에서 작업을 완료하는 데 사용할 수 있는 시간, FTE 또는 비용을 지정할 수 있습니다. 자원에 대한 시간 또는 비용을 예산하는 경우 자원에 대한 가용 시간, FTE 또는 비용은 예산책정된 금액만큼 감소합니다. 그 결과 예산을 책정하는 프로젝트를 따르는 프로젝트에 대한 가용 시간, FTE 또는 비용 금액이 해당 프로젝트에서 해당 사용자와 역할에 대해 감소합니다.

   >[!IMPORTANT]
   >
   >15년 동안 자원을 편성할 수 있습니다. 기간이 15년을 초과하는 프로젝트에 대한 자원을 예산을 책정하는 경우 예산 정보가 정확하지 않을 수 있습니다.

* 프로젝트 타임라인에 관계없이 Resource Planner에 표시되는 시간 기간 동안 자원에 대한 시간, FTE 또는 비용을 예측할 수 있습니다. 예를 들어, 프로젝트의 타임라인에서 자원을 사용할 수 없을 수도 있지만(계획 시간과 연관된 경우) 다른 시간 동안 사용할 수 있을 수도 있다는 것을 나타내려면 계획 시간이 0인 기간에 대해 예산을 책정하여 작업할 수 있습니다. 이렇게 한 후 리소스 가용성에 맞게 프로젝트의 타임라인을 수동으로 변경할 수 있습니다.

   >[!NOTE]
   >
   >Job 역할이나 사용자에 대해 Hours, FTE 또는 Cost 를 수동으로 예산을 편성하는 것이 좋습니다. 자동 옵션을 사용하여 계획 시간, FTE 또는 비용의 양이 항상 예산 책정된 시간, FTE 또는 원가와 일치해야 하는 경우에만 프로젝트 및 자원에 대한 시간을 예측할 수 있습니다.\
   >Resource Planner에서 예산 편성에 대한 자동 옵션을 사용하는 방법에 대한 자세한 내용은 문서의 &quot;예산 프로젝트 및 역할 자동&quot; 섹션을 참조하십시오 [Adobe Workfront Resource Planner를 사용하여 리소스 가용성 및 할당 검토](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

* 예산 책정 FTE 또는 비용은 예산 책정 시간과 동일합니다. Adobe Workfront은 예산을 편성하는 자원에 대해 시간 대신 FTE 및 비용 값을 사용합니다.

   Resource Planner에서 원가를 계산하는 방법을 이해하는 방법에 대한 자세한 내용은 다음을 참조하십시오 [리소스 계획자에서 비용 계산](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

* 자원 계획자에서 자원에 대한 예산 할당은 다음과 같은 방법으로 수행됩니다.

   * 수동으로

      또는

   * 에서 프로젝트 및 역할 옵션을 사용하여 자동으로 **프로젝트별 보기** 및 **역할별 보기** 보기.
   자세한 내용은 [프로젝트 및 역할 보기를 사용하는 자원 계획자의 예산 자원](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

* 사용자가 작업 역할을 변경하거나, 삭제되거나, 비활성화되거나, 리소스 풀에서 제거되면, 역할에 대해 책정된 시간이 변경되지 않고 역할의 나머지 사용자에게 다시 분배됩니다. Job 역할과 연관된 사용자가 더 이상 없을 경우 역할에 대한 예산책정된 시간이 0이 됩니다.

프로젝트 및 역할 옵션에 대한 자세한 내용은 섹션을 참조하십시오 [리소스 플래너의 시간, FTE 및 비용 값 이해](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner) 참조하십시오.

## 리소스 플래너의 시간, FTE 및 비용 값 이해 {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

자원 예산을 책정하고 자원 계획자에서 예산 책정된 시간 정보를 갱신하기 전에 다음 개념을 숙지해야 합니다

* **계획 시간, FTE 또는 비용**: 작업 및 문제에 대해 정의된 대로 수행해야 하는 작업입니다.
* **사용 가능한 시간, FTE 또는 비용**: 사용자와 연관된 일정에 따라 사용자나 작업 역할을 작업할 수 있는 시간입니다.

이 정보는 각 리소스(사용자 또는 역할)와 각 프로젝트에 대한 리소스 계획자에 표시됩니다.

프로젝트의 프로젝트 및 역할 보기에 표시되는 항목에 대한 자세한 내용은 문서를 참조하십시오 [리소스 플래너 탐색 개요](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Resource Planner에서 원가를 계산하는 방법을 이해하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [리소스 계획자에서 비용 계산](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

>[!NOTE]
>
>원가별 예산편성은 시간 또는 FTE별 예산편성과 동일하지만, Workfront에서 리소스 계획자에 대한 비용을 계산하는 방법을 이해해야 합니다.
>
>Resource Planner에서 비용을 계산하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [리소스 계획자에서 비용 계산](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

다음 테이블은 프로젝트 또는 역할 뷰를 적용할 때 리소스 계획자에 표시되는 할당 및 가용성 정보를 보여 줍니다. 시간, FTE 또는 비용별로 이 정보를 볼 수 있습니다.

* [AVL(사용 가능) 열](#the-avl-available-column)
* [PLN(계획됨) 열](#the-pln-planned-column)
* [BDG(예산책정) 열](#the-bdg-budgeted-column)
* [VAR(분산) 열](#the-var-variance-column)
* [NET 열](#the-net-column)

### AVL(사용 가능) 열 {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>표시 기준</strong> </td> 
   <td><strong>설명</strong> </td> 
  </tr> 
  <tr> 
   <td>프로젝트 </td> 
   <td> <p>선택한 기간 동안 프로젝트의 모든 사용자가 일정에 따라 작업할 수 있는 시간, FTE 또는 비용의 총계 </p> </td> 
  </tr> 
  <tr> 
   <td>역할</td> 
   <td> <p>이 역할에 연관된 모든 사용자가 자신의 일정 및 해당 일정에 따라 작업할 수 있는 시간, FTE 또는 비용의 합계 <strong>FTE 가용성 비율</strong> 해당 특정 역할에 대해 선택한 기간 동안 사용할 수 있습니다. </p> <p>다음 사항을 고려하십시오. </p> 
    <ul> 
     <li>작업 역할과 연관된 사용자가 없는 경우 작업 역할에 대한 사용 가능한 시간 값은 0입니다. </li> 
     <li>사용자가 기본 작업 역할과 연관되지만 <strong>FTE 가용성 비율</strong> 롤의 경우 작업 역할 사용 가능 시간 값은 0입니다.</li> 
     <li>사용자가 기타 역할 및 <strong>FTE 가용성 비율</strong> 롤이 0%인 경우, 기타 역할은 자원 계획자에 나열되지 않으며 사용자는 기본 역할에만 표시됩니다.</li> 
    </ul> <p>에 대한 자세한 정보 <strong>FTE 가용성 비율</strong> job 역할에 대해서는 문서를 참조하십시오 <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">사용자 프로필 편집</a>.</p> <p>Resource Planner에서 Job 역할 가용성을 계산하는 방법에 대한 자세한 내용은 문서의 "리소스 계획자에서 Job 역할에 대한 사용 가능한 시간 및 FTE 계산" 섹션을 참조하십시오 <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">리소스 계획자에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>사용자</td> 
   <td> <p>사용자가 선택한 기간 동안의 일정에 따라 작업할 수 있는 시간, FTE 또는 비용입니다. 이 숫자는 다음과 관련된 시간을 뺀 것입니다.</p> 
    <ul> 
     <li>예외 예약</li> 
     <li>사용자 해제 시간</li> 
     <li>기타 프로젝트에 대해 책정된 시간 </li> 
    </ul> <p>사용자 변경에 대한 사용 가능한 시간, FTE 또는 비용은 다음과 같이 변경됩니다. </p> 
    <ul> 
     <li>시스템 레벨의 리소스 관리 기본 설정을 기반으로 스케줄 및 FTE를 계산하는 방법<br><p>사용자 및 Job 역할 가용성 계산에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">리소스 계획자에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요</a>.</p>
     Workfront에서 리소스 관리 환경 설정 구성에 대한 자세한 내용은 다음을 참조하십시오 <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">리소스 관리 환경 설정 구성</a></li> 
    </ul> 
    <ul> 
     <li>a <strong>프로젝트 계획 우선 순위</strong>: 사용자의 작업 예산이 책정된 경우<br>프로젝트 계획 우선 순위가 사용자의 사용 가능한 시간에 미치는 영향에 대한 자세한 내용은 <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">리소스 플래너 탐색 개요 </a>. </li> 
    </ul> <p>사용자가 비활성화하도록 예약되어 있는 경우 비활성화 일자 이후의 일수(일수), FTE 또는 비용이 0입니다. <br>사용자 비활성화에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">사용자 비활성화 또는 다시 활성화</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



### PLN(계획됨) 열 {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>표시 기준</strong> </td> 
   <td><strong>설명</strong> </td> 
  </tr> 
  <tr> 
   <td>프로젝트</td> 
   <td> <p>다음을 포함하여 프로젝트 아래에 나열된 모든 Job 역할 또는 사용자의 계획된 시간, FTE 또는 비용의 합계입니다. <strong>역할 없음</strong> 또는 <strong>사용자 없음</strong> 섹션에 나열된 상태로 남아 있습니다. </p> <p><b>메모</b>

일별 사용자 할당을 수동으로 조정하면 Resource Planner에서 주별, 월별 또는 분기별 계획 시간 값이 변경될 수 있습니다. 작업 로드 밸런서를 사용하여 작업 및 문제에 대한 일별 사용자 할당을 수동으로 조정할 수 있습니다. 자세한 내용은 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">작업 로드 밸런서에서 사용자 할당 관리</a>.</p> </td>
</tr> 
  <tr> 
   <td>역할</td> 
   <td> <p>선택한 기간 동안 롤에 할당된 모든 작업에서 계획된 시간의 합계입니다. </p> <p>다음 <strong>역할 없음</strong> 섹션에는 할당되지 않고 팀에 할당된 작업과 연관된 계획 시간(해당 시간이 팀에 나열됨)이 표시됩니다 <strong>사용자 없음</strong> 섹션) 또는 작업 역할과 연관되지 않은 사용자에게 할당됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td>사용자</td> 
   <td> <p>선택한 기간 동안 특정 역할의 사용자에게 할당된 모든 작업의 계획 시간 </p> <p>다음 <strong>사용자 없음</strong> 섹션에는 지정되지 않았거나 팀에 할당된 작업과 관련된 계획된 시간이 표시됩니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

계획 시간을 볼 때 다음 사항을 고려하십시오.

* 프로젝트 및 역할 뷰의 리소스 계획자에서 작업 할당에 대한 정보를 볼 수는 없지만 계획 시간 값은 프로젝트의 작업에 대한 계획 시간에서 가져옵니다.
* 계획 시간은 지정된 각 자원에 대해 작업 기간 내의 각 날에 균등하게 분배됩니다. 태스크 기간은 계획 시작 및 완료 일자를 기준으로 하며 해당 기간 내의 모든 달력 일자를 포함합니다.\
   Workfront은 사용자 또는 프로젝트에 계획 시간을 배포할 때 사용자 또는 프로젝트의 일정을 고려합니다. 이 경우 계획 시간은 주말, 휴가 일수 및 스케줄 예외를 제외한 작업의 기간 내에 각 날에 균등하게 분배됩니다.\
   예를 들어, 주별 리소스 계획자를 표시하고 프로젝트에서 여러 주에 걸쳐 있는 작업이 있는 경우, 주 단위 계획 시간 수는 해당 주 내의 일 수가 태스크 지속 기간의 일부인 기간에 따라 달라집니다. 이 기능은 월 또는 분기별로 리소스 계획자를 표시할 때와 작업이 여러 달 또는 분기에 걸쳐 있을 때 비슷하게 작동합니다.\
   주말 일, 예약 예외 및 휴가 일은 이 배포에서 제외됩니다.
* 각 자원에 대한 계획 시간 계산에는 다음 태스크 범주가 포함됩니다.

   * 프로젝트의 리소스 풀, 작업 역할 또는 팀에서 사용자에게 할당된 작업\
      작업이 팀에 할당되면 해당 할당이 **역할 없음** 및 **사용자 없음** 섹션에 자세히 설명되어 있습니다. 팀과 연관된 계획 시간 을 볼 수 있지만 작업과 연관된 역할이나 사용자가 없으므로 시간을 계산할 수 없습니다.

   * 할당되지 않은 작업

* 자원 계획자의 계획 시간은 다음과 연관된 계획 시간을 포함하지 않습니다.

   * 상위 작업
   * 리소스 풀이 없는 사용자에게 할당된 작업
   * 문제, **문제 발생 시간 포함** 설정이 비활성화되어 있습니다.

* 작업 기간이 0인 경우 계획 시간이 자원 계획자에 표시되지 않습니다.
* 비활성화된 사용자와 연결된 계획된 시간이 표시되지 않습니다.

### BDG(예산책정) 열 {#the-bdg-budgeted-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>표시 기준</strong> </td> 
   <td><strong>설명</strong> </td> 
  </tr> 
  <tr> 
   <td>프로젝트</td> 
   <td> <p>선택한 기간 동안 프로젝트에 대해 예산을 책정하는 시간, FTE 또는 비용을 추정하는 수동 입력입니다. </p> <p>프로젝트 보기에서 프로젝트에 대해 예산을 책정하는 시간은 프로젝트 아래에 나열된 작업 역할에 배포됩니다. 각 역할에 대한 계획 시간 금액은 예산책정된 시간이 역할에 분배되는 방식을 결정합니다. 예산책정된 시간은 더 높은 계획 시간 값이 있는 역할에 분배됩니다. </p> <p>역할 보기에서 프로젝트에 대해 예산을 책정하는 시간은 프로젝트의 역할이나 사용자에게 배포되지 않습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>역할</td> 
   <td> <p>선택한 기간 동안 역할에 대해 예산을 편성하는 시간을 예상하는 수동 입력입니다. </p> <p>Job 롤과 연관된 사용자가 없을 경우 Job 롤에 대한 예산책정된 시간을 예측할 수 없습니다. </p> <p>역할 보기에서 역할에 대해 예산을 책정하는 시간은 역할 아래에 나열된 프로젝트에 분산됩니다. 각 프로젝트에 대한 계획 시간의 양은 예산책정된 시간이 프로젝트에 분배되는 방식을 결정합니다. 예산책정된 시간은 더 높은 계획 시간 값이 있는 프로젝트에 분배됩니다.</p> <p>프로젝트 보기에서는 역할에 대해 예산을 편성하는 시간이 프로젝트 또는 역할과 연관된 사용자에게 배포되지 않습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>사용자</td> 
   <td> <p>선택한 기간 동안 사용자에 대해 예산을 책정하 는 시간을 예상하는 수동 입력입니다. </p> <p> <p><b>참고</b>   태스크에 지정되지 않지만, 자원 그룹과 연관된 사용자의 예산 책정된 시간을 예측할 수 있습니다. 이러한 사용자는 자원 계획자에도 표시되기 때문입니다. 하지만 작업에 할당되지 않은 경우 계획 시간은 0이어야 합니다. </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

예산책정된 시간 작업 시 다음 사항을 고려합니다.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(Duplicated below ??)
</MadCap:conditionalText>
-->

* 프로젝트에 대한 리소스 관리 및 재무 데이터에 대한 편집 액세스 권한 및 재무 관리 권한이 있는 경우에만 리소스를 예측할 수 있습니다.

   예산 책정 리소스에 필요한 액세스에 대한 자세한 내용은 문서를 참조하십시오 [Adobe Workfront의 예산 리소스에 대한 액세스 필요](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* 기본적으로 자원 계획자의 예산책정된 시간은 모든 자원 및 모든 프로젝트에 대해 0입니다.
* 사용자 및 역할에 대한 예산책정된 시간을 수동으로 추정하거나 프로젝트 또는 작업 롤의 링크 중 하나를 사용할 수 있습니다 **자세히** 메뉴를 사용하여 계획 시간 수에 따라 갱신합니다.\
   프로젝트 및 역할 옵션에 대한 자세한 내용은 섹션을 참조하십시오 [리소스 계획자의 프로젝트 및 역할 뷰의 시간, FTE 및 비용 정보 개요](#Budget) 참조하십시오.

* 시간, FTE 또는 비용을 편성할 수 있는 가장 작은 기간은 1주일입니다. 하루 동안의 시간, FTE 또는 비용을 계산할 수 없습니다.
* 예산책정된 시간은 지정된 각 자원에 대해 작업 기간 내에 각 일별로 균등하게 분배됩니다. 태스크 기간은 계획 시작 및 완료 일자를 기준으로 하며 해당 기간 내의 모든 달력 일자를 포함합니다.\
   Workfront은 사용자 또는 프로젝트에 예산책정된 시간을 분배할 때 사용자 또는 프로젝트의 일정을 고려합니다. 이 경우, 예산책정된 시간은 주말을 제외한 작업의 기간 내에 각 일별로 동일하게 분산되며, 타임오프 및 스케줄 예외를 포함합니다.\
   예를 들어, 주별 자원 계획자를 표시하고 여러 주에 걸쳐 있는 작업이 있는 경우, 주 단위 예산 책정된 시간 수는 해당 주 내의 일 수가 태스크 지속 기간의 일부인지에 따라 달라집니다. 주말 요일은 이 배포에서 제외됩니다. 이 기능은 월 또는 분기별로 리소스 계획자를 표시할 때와 작업이 여러 달 또는 분기에 걸쳐 있을 때 비슷하게 작동합니다.

* 신규 보고서에 대한 보고서 객체로 예산책정된 시간을 선택하여 예산책정된 시간을 보고할 수 있습니다.\
   Workfront에서 보고할 수 있는 객체에 대한 자세한 내용은 문서의 &quot;객체에 대한 보고서&quot; 섹션을 참조하십시오 [Adobe Workfront의 개체 이해](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
   예산책정된 시간 보고서 작성에 대한 자세한 내용은 문서를 참조하십시오 [보고서: 예산책정 시간](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md).

* 나중에 비활성화된 사용자에 대해 이전에 예산책정된 시간은 표시되지 않습니다.

### VAR(분산) 열 {#the-var-variance-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>표시 기준</strong> </td> 
   <td><strong>설명</strong> </td> 
  </tr> 
  <tr> 
   <td>프로젝트</td> 
   <td> <p>시간, FTE 또는 원가 분산은 프로젝트에 대한 모든 계획 시간을 달성하는 데 필요한 충분한 예산책정 시간이 있는지 여부를 표시합니다. </p> <p>프로젝트 시간, FTE 또는 원가 분산은 다음 공식을 사용하여 계산됩니다.</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>역할</td> 
   <td> <p>시간, FTE 또는 원가 분산은 역할에 할당된 계획 시간을 달성하는 데 충분한 예산 책정된 시간, FTE 또는 비용이 있는지 여부를 표시합니다. </p> <p>역할 시간, FTE 또는 원가 분산은 다음 공식을 사용하여 계산됩니다.</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>사용자</td> 
   <td> <p>시간, FTE 또는 원가 분산은 사용자에게 지정된 계획 시간을 달성할 수 있는 충분한 예산책정 시간이 있는지 여부를 표시합니다. </p> <p>사용자 시간, FTE 또는 원가 차이는 다음 공식을 사용하여 계산됩니다.</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>시간, FTE 또는 원가 차이가 빨간색으로 표시되는 경우 완료해야 하는 실제 작업의 계획 시간보다 적은 예산책정된 시간이 표시됩니다. 이 경우, 예산책정된 시간이 작업을 완료하기에 충분하지 않을 수 있습니다.

### NET 열  {#the-net-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>표시 기준</strong> </td> 
   <td><strong>설명</strong> </td> 
  </tr> 
  <tr> 
   <td>프로젝트</td> 
   <td> 
    <div> 
     <p>프로젝트 순 시간, FTE 또는 원가는 다음 중 하나를 표시할 수 있습니다. </p> 
     <ul> 
      <li> <p>사용 가능한 시간 또는 원가와 프로젝트에 대한 예산 책정된 시간 또는 원가의 차이:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>NET 계산 설정에서 계획(PLN) 값 사용 설정을 사용할 경우, 사용 가능한 시간 또는 비용과 프로젝트에 대한 계획 시간 또는 비용 간의 차이: </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>팁</b></p>        
  <p>이 옵션은 선택한 항목 표시 섹션에서 보기를 사용자 지정하는 경우에만 적용됩니다.</p>
  <p>자세한 내용은 <a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >Adobe Workfront Resource Planner를 사용하여 리소스 가용성 및 할당 검토</a> </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>역할</td> 
   <td> 
    <div> 
     <p>Net Hours, FTE 또는 Cost 역할에는 다음 중 하나가 표시될 수 있습니다. </p> 
     <ul> 
      <li> <p>사용 가능한 시간 또는 비용과 역할에 대한 예산 책정된 시간 또는 비용 간의 차이:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>NET 계산 설정에서 계획(PLN) 값 사용 설정을 사용할 경우 역할에 대한 가용 시간 또는 비용과 계획 시간 또는 비용 간의 차이입니다.</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>팁</b> <span>

이 옵션은 선택한 항목 표시 섹션에서 보기를 사용자 지정하는 경우에만 적용됩니다.</span> </p> <p><span>자세한 내용은 </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Adobe Workfront Resource Planner를 사용하여 리소스 가용성 및 할당 검토</a> </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>사용자</td> 
   <td> 
    <div> 
     <p>사용자 순 시간, FTE 또는 비용은 다음 중 하나를 표시할 수 있습니다. </p> 
     <ul> 
      <li> <p>사용 가능한 시간 또는 원가와 사용자의 예산 책정된 시간 또는 원가 간의 차이:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>NET 계산 설정에서 계획(PLN) 값 사용 설정을 사용할 경우, 사용 가능한 시간 또는 비용과 사용자의 계획 시간 또는 비용 간의 차이:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>팁</b> <span>

이 옵션은 선택한 항목 표시 섹션에서 보기를 사용자 지정하는 경우에만 적용됩니다.</span> </p> <p><span>자세한 내용은 </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Adobe Workfront Resource Planner를 사용하여 리소스 가용성 및 할당 검토</a> </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**NET Hours, FTE 또는 Cost가 빨간색으로 표시되는 경우 예산책정된 항목을 처리할 사용 가능한 시간이나 예산이 충분하지 않습니다** 또는 작업과 연관된 계획 시간 또는 원가 이 경우 리소스가 너무 할당됩니다.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the table below is ideal but it does not transfer to Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours, FTE, or Cost)</strong> </td>
<td><strong>Displayed by</strong> </td>
<td><strong>Description</strong> </td>
</tr>
<tr>
<td rowspan="3">AVL <br>(Available Hours, FTE, or Cost)</td>
<td>Project </td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users on the project are available to work according to their schedule, for the time frame selected. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users associated with this role are available to work according to their schedule and their <strong>Percentage of FTE Availability</strong> for that specific role, for the time frame selected. </p> <p>Consider the following: </p>
<ul>
<li>If no user is associated with a job role, then the value for the Available Hours for the job role is zero. </li>
<li>If a user is associated with a Primary Job Role, but the <strong>Percentage of FTE Availability</strong> for the role is 0%, the job role Available Hours value is zero.</li>
<li>If the user is associated with Other Roles and the <strong>Percentage of FTE Availability</strong> for the roles is 0%, the Other Roles are not listed in the Resource Planner and the user displays only under their Primary Role.</li>
</ul> <p>For more information about the <strong>Percentage of FTE Availability</strong> for a job role, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> <p>For more information about how the job role availability is calculated in the Resource Planner, see the section "Calculate the Available Hours and FTE for a job role in the Resource Planner" in the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>Hours, FTEs, or Cost that the user is available to work, according to their schedule, for the time frame selected. This number subtracts the hours associated with the following:</p>
<ul>
<li>schedule exceptions</li>
<li>time off of the user</li>
<li>hours budgeted for other projects. </li>
</ul> <p>The Available Hours, FTEs, or Cost for a user change according the following: </p>
<ul>
<li>how their schedule and FTE are calculated based on the Resource Management Preferences at the system level.<br>For more information about calculating user and job role availability, see the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</li>
</ul>
<ul>
<li>the <strong>Project Planning Priority</strong>, if the user is budgeted for work.<br>For more information about how Project Planning Priority affects the Available Hours of a user, see <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Resource Planner navigation overview </a>. </li>
</ul> <p>If the user is scheduled for deactivation, the Available Hours, FTEs, or Cost for the days after the deactivation date are zero. <br>For more information about deactivating users, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</p> </td>
</tr>
<tr>
<td rowspan="4">PLN <br>(Planned Hours, FTE, or Cost)</td>
<td>Project</td>
<td> <p>The total of the Planned Hours, FTEs, or Cost from all the job roles or users listed under the project, including in the <strong>No Role</strong> or <strong>No User</strong> sections, for the time frame selected, and as displayed in the Project Details tab of the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of the Planned Hours from all the tasks assigned to the role, during the time frame selected. </p> <p>The <strong>No Role</strong> section will show the Planned Hours associated with tasks that are either unassigned, assigned to teams (whose hours are listed in the <strong>No User</strong> section), or assigned to users who are not associated with a job role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Planned Hours from all the tasks assigned to the user in a specific role, during the time frame selected. </p> <p>The <strong>No User</strong> section will show the Planned Hours associated with tasks that are either unassigned or assigned to teams. </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<ul>
<li>Although you cannot see information about task allocations in the Resource Planner in the Project and Role views, the amount of Planned Hours comes from the Planned Hours on the tasks in the projects. </li>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks excluding weekends, time-off days, and schedule exceptions.<br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> The following categories of tasks are included in calculating the Planned Hours for each resource:
<ul>
<li> tasks assigned to users in Resource Pools, job roles, or teams on the project<br>If tasks are assigned to teams, their allocation will appear under <strong>No Role</strong> and <strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks. </li>
<li> unassigned tasks </li>
</ul></li>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>tasks assigned to users with no Resource Pools</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> </td>
</tr>
<tr>
<td rowspan="4"> BDG <br>(BudgetedHours, FTE, or Cost) </td>
<td>Project</td>
<td> <p>A manual entry to estimate how many hours, FTE, or Cost you budget for a project, for a selected time frame. </p> <p>In the Project view, the hours you budget for the project are distributed to the job roles listed under the project. The amount of Planned Hours for each role determines how the Budgeted Hours are distributed to the roles. The Budgeted Hours are distributed to the roles with higher Planned Hours values. </p> <p>In the Role view, the hours you budget for the project are not distributed to the roles or the users on the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>A manual entry to estimate how many hours you budget for a role, for a selected time frame. </p> <p>If no user is associated with the job role, you cannot estimate the Budgeted Hours for the job role. </p> <p>In the Role view, the hours you budget for the role are distributed to the projects listed under the role. The amount of Planned Hours for each project determines how the Budgeted Hours are distributed to the projects. The Budgeted Hours are distributed to the projects with higher Planned Hours values.</p> <p>In the Project view, the hours you budget for the role are not distributed to the projects or the users associated with the role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>A manual entry to estimate how many hours you budget for a user, for a selected time frame. </p> <p> <note type="note">  You can estimate the Budgeted Hours for users who are not assigned to tasks, but are associated with a Resource Pool on a project because these users also appear in the Resource Planner. Their Planned Hours should be zero, however, if they are not assigned to tasks.
</note> </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when working with Budgeted Hours:</p> <li>
<ul>
<li> <p>You can budget resources only when you have Edit access to Resource Management and Financial Data and Manage Finance permissions on the projects.</p> <p>For information about the access needed for budgeting resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this bullet: Duplicated below)</p>
</li>
</ul> </li>
<ul>
<li>By default, the Budgeted Hours in the Resource Planner are zero for all resources and for all the projects.</li>
<li>You can manually estimate the Budgeted Hours for users and roles, or you can use one of the links in the Project or Job Role <strong>More</strong> menus to update them according to the number of Planned Hours.<br>For more information about project and role options, see the section <a href="#Budget" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a> in this article.</li>
<li> The smallest period of time you can budget hours, FTE, or Cost for is a week. You cannot budget hours, FTE, or Cost for a day. </li>
<li> Budgeted Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time. <br>Workfront takes into account the schedule of the user or of the project when distributing Budgeted Hours to users or projects. In this case, Budgeted Hours are equally distributed to each day within the Duration of tasks excluding weekends, but including time-off and schedule exceptions. <br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks, the number of Budgeted Hours per week depends on how many days within that week are part of the task Duration. Weekend days are excluded from this distribution. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters. </li>
<li>You can report on Budgeted Hours, by selecting Budgeted Hour as your report object for a new report.<br>For information about what objects you can report on in Workfront, see the section "Report on objects" in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. <br>For information about building a Budgeted Hour report, see the article <a href="../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Report: Budgeted Hour</a>.</li>
<li>Hours previously budgeted for users who were later deactivated do not display. <br></li>
</ul> </td>
</tr>
<tr>
<td rowspan="4">VAR <br>(Hour, FTE, or ,Cost Variance)</td>
<td>Project</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the project to accomplish all the Planned Hours for the project. </p> <p>The Project Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours, FTE, or Cost for the role to accomplish the Planned Hours assigned to it. </p> <p>The Role Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Hours, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the user to accomplish the Planned Hours assigned to them. </p> <p>The User Hours, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
When the Hours, FTE, or Cost Variance displays in red, you have estimated less Budgeted Hours than the Planned Hours of the actual work that needs to be completed. In this case, the Budgeted Hours might not be enough to complete the work.
</note> </td>
</tr>
<tr>
<td rowspan="4"> NET <br>(Net Hours, FTEs, or Cost) </td>
<td>Project</td>
<td>
<div>
<p>The project Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the project:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the project, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>Role</td>
<td>
<div>
<p>The role Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the role:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the role, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span class="preview"><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>User</td>
<td>
<div>
<p>The user Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the user:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the user, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
<span>When the NET Hours,&nbsp;FTE, or Cost display in red, there is not enough Available time or budget to cover either the Budgeted</span> or the Planned time or cost associated with the work. In this case, the resources are overallocated.
</note> </td>
</tr>
</tbody>
</table>
-->
