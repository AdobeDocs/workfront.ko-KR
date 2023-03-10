---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 작업 로드 밸런서에서 사용자 할당 관리
description: 리소스 관리자는 사용자에게 작업을 할당하고 작업 로드 밸런서에서 일별, 주별 또는 월별 할당을 관리할 수 있습니다.
author: Alina
feature: Resource Management
exl-id: 9649e482-af24-4516-9a69-ef12b2f1d579
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '2787'
ht-degree: 0%

---

# 작업 로드 밸런서에서 사용자 할당 관리

리소스 관리자는 사용자에게 작업을 할당하고 작업 로드 밸런서에서 일별, 주별 또는 월별 할당을 관리하여 사용 가능한 스케줄에 맞는 시간을 할당할 수 있습니다.

## 액세스 요구 사항 {#access-requirements}

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>팀 또는 자원 영역에서 작업 로드 밸런서를 사용할 계획 </p>
   <p>프로젝트의 작업 로드 밸런서를 사용할 때 작업 </p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>다음에 대한 액세스 편집:</p> 
    <ul> 
     <li> <p>리소스 관리</p> </li> 
     <li> <p>프로젝트</p> </li> 
     <li> <p>작업</p> </li> 
     <li> <p>문제</p> </li> 
    </ul> <p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>할당을 관리할 작업 및 문제에 [할당]을 포함하는 Contribute 권한 이상입니다. </p> <p>또는 </p> <p>할당을 업데이트하는 것 외에도 계획 시간을 업데이트할 작업에 대한 권한을 관리합니다. 작업 로드 밸런서에서 계획 시간 업데이트에 대한 자세한 내용은 <a href="#update-task-planned-hours-when-managing-user-allocations">사용자 할당을 관리할 때 작업 계획 시간 업데이트</a> 섹션에 자세히 설명되어 있습니다. </p> <p>작업 권한에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md">작업 공유 </a><span> 문제 권한에 대한 자세한 내용은</span> <span href="../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md">문제 공유 </a></span>. </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 사용자 할당 이해

사용자 할당은 사용자가 지정된 일 또는 요일, 주 또는 월에 작업 항목을 완료하는 데 소비해야 하는 시간을 나타내는 시간(시)의 금액입니다. 작업 항목의 계획 시간에 포함됩니다.

이 문서에서는 작업 또는 문제에 할당된 사용자에 대한 일별, 주별 또는 월별 시간별 할당을 업데이트하는 방법에 대해 설명합니다. 사용자에 대한 전체 할당 및 작업에 대한 작업 역할을 관리하는 방법에 대한 자세한 내용은 [작업에 대한 사용자 및 역할 할당 시간 관리](../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md) .

* [사용자 할당 개요](#user-allocation-overview)
* [사용자 할당을 재설정하는 기준](#criteria-that-reset-user-allocations)

### 사용자 할당 개요 {#user-allocation-overview}

사용자 할당을 작업 로드 밸런서에서 시간 또는 백분율 값으로 표시할 수 있습니다. 시간 또는 백분율을 조정할 수 있습니다.

사용자 할당은 작업 항목의 계획 시간 수에 포함됩니다. 계획된 시간에 대한 자세한 내용은 [계획 시간 개요](../../manage-work/tasks/task-information/planned-hours.md).

작업 계획 시간은 작업에 지정된 사용자에 대한 작업 기간 내의 모든 일 간에 균등하게 분배됩니다. 예를 들어, 작업에 기간 5일과 총 10시간의 계획 시간이 있는 경우, 작업에 대한 일별 할당 수는 2시간입니다. 주간 할당은 10시간입니다. 즉, 사용자는 매일 2시간 동안 작업 수행을 위해 할당됩니다. 그러나 작업 로드 밸런서를 사용하여 사용자에 대한 일별 할당을 수동으로 변경할 수 있습니다.

>[!CAUTION]
>
>작업 로드 밸런서는 작업 항목당 최대 1000개의 계획된 시간과 항목의 지속 기간 최대 1000일만 표시합니다. 작업 로드 밸런서의 할당은 1000시간 또는 1000일 제한에 도달한 후 0으로 표시됩니다. 더 많은 계획 시간 또는 1000일 이상의 지속 시간을 수용하도록 작은 하위 태스크로 작업을 나누는 것이 좋습니다.

작업 로드 밸런서에서 작업 또는 문제에 대한 일별, 주별 또는 월별 할당을 찾을 때 다음 사항을 고려하십시오.

* 사용자의 작업 항목에 대한 일별, 주별 및 월별 할당을 볼 수 있습니다. 주 또는 월 뷰를 활성화하여 주별 또는 월별 할당을 표시합니다.
* 작업 로드 밸런서를 사용하여 작업이나 문제에 대한 사용자의 일별, 주별 또는 월별 할당을 수정할 수 있습니다. 작업 로드 밸런서의 보기 조정에 대한 자세한 내용은 [작업 로드 밸런서 탐색](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

   >[!NOTE]
   >
   >사용자 할당을 관리할 때 항상 사용할 시간대(일별, 주별 또는 월별)를 결정하고 동일한 작업 항목에 대해 간에 전환하지 않는 것이 좋습니다. 일별 할당을 이전에 갱신한 동일한 사용자에 대한 주별 할당을 갱신하면 사용자의 일별 할당이 변경됩니다.

* 근무 일수와 비근무 일수에 대한 할당을 갱신할 수 있습니다.
* 작업 항목의 계획 시작 및 계획 완료 날짜에 대한 타임스탬프와 프로젝트 일정이 자동으로 계산될 때 작업 항목의 시간 스탬프가 중요합니다.

>[!INFO]
>
> 예를 들어, 작업의 기간은 2일 및 2이며, 사용자가 포함된 기간의 첫 날에 계획된 시작 시간은 오후 12시이고 프로젝트 일정은 오후 5시에 끝나는 것입니다. 첫 날의 사용자 용량은 5시간입니다. 두 번째 날의 사용자 용량은 8시간입니다(예약이 오전 9시에 시작하는 경우).
>
>Workfront은 다음 공식을 사용하여 지속 시간 2일 동안 2시간의 할당을 계산합니다.
>
>
```
>
>   Daily allocation hours = (Total Planned Hours / Total of available hours) * Daily available hours
>```
>
>  이 예에서는 각 날의 일별 할당 시간은 다음과 같습니다.
>   
>  (2 / 13) * 5 = 첫 번째 날에 대한 0.77 할당 시간
>
>  (2 / 13) * 8 = 두 번째 날에 대한 1.23 할당 시간
>
>  위의 계산에서 13은 작업에 사용할 수 있는 총 시간입니다. 5 + 8 = 13



* 지정된 사용자의 시간대와 다른 시간대에 있는 서로 다른 시간대에 있는 두 명의 사용자가 동일한 작업 항목을 보는 두 사용자에게 할당 금액이 다르게 표시될 수 있습니다.

* 사용자가 시간대를 예약하면 해당 일 또는 해당 날의 일부가 회색 배경으로 표시됩니다. Workfront 관리자가 사용자의 시간 오프를 고려하여 설정 영역에서 사용자 시간 초과 설정을 활성화한 경우 할당된 시간이 타임라인에서 다음 사용 가능한 날짜로 이동합니다. 이 설정을 비활성화하면 할당된 시간은 해제 시간으로 표시된 날에 유지되며 사용자는 초과 할당으로 표시됩니다. 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   >[!TIP]
   >
   >사용자가 작업 항목에 지정된 후 휴가가 표시된 경우, 이동한 할당을 표시하려면 프로젝트의 타임라인을 재계산해야 합니다. 자세한 내용은 [프로젝트 타임라인 다시 계산](../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* 작업에 할당된 사용자가 여러 개 있는 경우, 계획 시간의 양이 각 사용자에게 먼저 균등하게 분배된 다음 작업 기간 내에 각 날에 균등하게 분배됩니다. 이 배포는 각 사용자의 작업에 대한 할당이 됩니다.

   예를 들어, 다음 시나리오가 있을 수 있습니다.

   * 기간이 2일이고 계획 시간 10개가 한 사용자에게 할당된 작업의 경우, 사용자에 대한 일별 할당은 기본적으로 각 날에 대해 5시간입니다.
   * 기간이 2일이고 계획 시간 10이 2명의 사용자에게 할당된 작업의 경우, 각 사용자에 대한 일별 할당은 기본적으로 각 날에 대해 2.5시간입니다.

* 계획 완료 일자 이전에 완료된 작업이나 문제는 남은 일수에 대해 할당된 시간 수를 처리하여 사용자의 전체 할당에 계산되지 않습니다. 할당 표시 아이콘 및 예상 날짜 표시 설정이 모두 사용되도록 설정된 경우에만 표시됩니다. 작업 로드 밸런서에서 설정 활성화에 대한 자세한 내용은 [작업 로드 밸런서 탐색](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

   ![](assets/allocations-struck-through-highlighted-350x39.png)

* 사용자가 너무 많이 할당되면 할당된 시간이 사용자 필드에 빨간색 배경이 표시됩니다.
* 사용자가 할당된 시간이 부족하거나 예약된 사용 가능한 시간에 동일한 시간을 할당하면 해당 시간은 파란색 배경으로 표시됩니다.
* 사용자 라인의 차트 뷰에 사용자 할당을 표시할 수 있습니다. 사용자 할당을 위한 차트 보기를 활성화하는 방법에 대한 내용은 문서의 &quot;작업 로드 밸런서 탐색&quot; 섹션을 참조하십시오 [작업 로드 밸런서 탐색](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

   ![](assets/user-allocation-chart-350x237.png)

### 사용자 할당을 재설정하는 기준 {#criteria-that-reset-user-allocations}

모든 작업 변경 사항이 재배포할 수정된 할당을 트리거하는 것은 아닙니다. 그러나 이미 조정된 리소스에 대한 할당을 재설정하고 각 할당자에 대한 작업 항목 기간 동안 모든 일에 균등하게 재배포할 수 있는 특정 작업이 있습니다.

>[!NOTE]
>
>작업 항목에 대한 할당 자동 분포를 수정하지 않은 경우, 작업 항목에 대한 할당 수, 작업 기간 또는 계획 시간의 양이 변경될 때 시간이 모든 담당자 간에 균등하게 재배포됩니다.

* [조정된 할당을 재설정하는 작업](#actions-that-reset-adjusted-allocations)
* [조정된 할당을 재설정하지 않는 작업](#actions-that-do-not-reset-adjusted-allocations)

#### 조정된 할당을 재설정하는 작업 {#actions-that-reset-adjusted-allocations}

다음 작업은 다음에 설명된 대로 사용자를 수동으로 조정한 후 사용자에 대한 일별, 주별 또는 월별 할당을 재설정하거나 수정합니다 [사용자 할당 수정](#modify-user-allocations) 섹션:

* 지속 기간의 일수를 단축하는 작업 항목의 길이를 단축하면 손실된 일수에서 조정된 할당 시간이 작업 항목의 마지막 날의 할당 금액에 추가됩니다.
* 발령 또는 작업 품목에 대한 계획 시간 금액을 변경하면, 신규 계획 시간 수는 작업 항목의 전체 기간 동안 균일하게 재분배됩니다.
* 작업 항목에 담당자를 추가하거나 제거하면 작업의 계획 시간이 변경되므로 조정된 값이 균일하게 재배포됩니다.

#### 조정된 할당을 재설정하지 않는 작업 {#actions-that-do-not-reset-adjusted-allocations}

작업 항목에 대한 다음 변경 사항은 재설정하거나 수정할 조정된 할당을 트리거하지 않습니다.

* 작업 항목의 일수를 이동하지만 지속 기간의 일 수가 변경되지 않으면 조정된 할당 값은 동일하게 유지되며 새 날짜로 이동합니다.
* 작업 항목의 지속 기간을 늘리면 해당 기간의 일 수가 늘어나면 조정된 할당된 시간은 조정된 일 동안 동일하게 유지됩니다. 할당된 시간이 0인 작업 항목에 추가 일이 추가됩니다.
* 작업 항목에 담당자를 추가하거나 제거해도 항목의 계획 시간이 변경되지 않으므로 조정된 값은 동일하게 유지됩니다.

## 작업 로드 밸런서에서 계획 시간 찾기

사용자에게 할당된 작업 또는 문제의 계획 시간을 찾아 작업 로드 밸런서를 사용하여 작업 또는 문제에 대한 사용자 할당을 수정할 수 있습니다.

작업 로드 밸런서에서 계획 시간을 볼 때 다음 사항을 고려하십시오.

* 작업 로드 밸런서 왼쪽의 작업 또는 문제 이름 옆에 작업 또는 문제에 대한 총 계획된 시간이 표시됩니다.

* 작업 로드 밸런서 왼쪽의 프로젝트 이름 옆에 프로젝트에 대한 총 계획 시간이 표시됩니다. 이는 작업 로드 밸런서에서 프로젝트에 나열된 모든 작업 및 문제에 대한 총 계획 시간을 나타내며 프로젝트의 모든 계획 시간이 아닙니다.
* 모든 작업 및 모든 프로젝트에 대해 일별 또는 주별 할당된 시간은 수동으로 할당 표시 설정을 활성화할 때만 표시됩니다. 작업 로드 밸런서에서 설정 활성화에 대한 자세한 내용은 [작업 로드 밸런서 탐색](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 사용자 할당 수정 {#modify-user-allocations}

사용자에게 작업을 할당하는 과정에서 작업 로드 밸런서에서 사용자 할당을 수정하여 할당된 시간이 초과되지 않도록 하거나 리소스 간의 정확한 시간 균형을 확보할 수 있습니다. 사용자가 초과 할당되었는지 여부를 식별하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [사용자 할당 개요](#user-allocation-overview) 참조하십시오.

1. 사용자에게 작업과 문제가 할당되었는지 확인합니다. 작업 로드 밸런서에서 사용자에게 작업을 할당하는 방법에 대한 내용은 다음을 참조하십시오 [작업 로드 밸런서에서 작업 할당 개요](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).
1. 작업 로드 밸런서로 이동합니다.
1. (선택 사항) **주** 또는 **월** 사용자를 위한 주별 또는 월별 할당을 관리하려면

   ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

1. 에서 **지정된 작업 시간** 영역에서 수동으로 할당을 수정할 사용자를 찾은 다음 사용자 이름의 왼쪽에 있는 오른쪽 화살표를 클릭하여 사용자를 확장합니다.

   ![](assets/wb-highlight-on-name-caret-350x106.png)

1. 프로젝트를 확장하고 사용자가 할당된 작업 항목을 표시하려면 프로젝트 이름의 왼쪽에 있는 오른쪽 화살표 를 클릭합니다.

   >[!TIP]
   >
   >작업 및 문제에 대해서만 사용자 할당을 수정할 수 있습니다. 프로젝트에 대한 사용자 할당은 수정할 수 없습니다.

1. (선택 사항) **할당 표시 아이콘** ![](assets/show-allocations-icon-small.png) 모든 작업 항목에 대한 할당을 표시하려면

   작업 및 프로젝트의 이름은 작업 또는 프로젝트에 대한 사용자의 할당으로 대체됩니다.

1. (선택 사항) **설정** 아이콘 ![](assets/gear-icon-settings.png) 다음 옵션 중 하나를 선택합니다.

   1. **문제의 시간 포함**. 이를 통해 작업 할당 외에 문제 할당을 관리할 수 있습니다.
   1. **완료된 작업 보기** . 이 항목은 할당을 관리하는 타임라인 동안 완료되고 예약된 항목을 표시합니다.
   1. **남은 시간 표시** 선택 사항입니다. 사용자 라인의 각 사용자에 대한 총 시간(시간)이 변경됩니다. 이 설정이 활성화되면 작업 로드 밸런서에는 할당된 시간 대신 각 사용자가 작업에 사용할 수 있는 시간이 표시됩니다.

      >[!TIP]
      >
      >이 설정이 활성화될 때 할당을 수정하면 사용자 라인의 총 숫자가 줄어듭니다.

   1. **프로젝트** 에서 **색상 테마 선택** 섹션을 참조하십시오. 이렇게 하면 각 프로젝트 및 해당 작업 항목이 고유한 색상으로 표시되고 프로젝트에 속하는 항목을 쉽게 이해할 수 있습니다.
   1. **백분율** 에서 **에 사용자 할당 표시** 섹션을 참조하십시오. 할당은 백분율 값으로 표시됩니다. 일정에 따른 사용자 용량은 100%로 간주됩니다. 예를 들어, 사용자가 하루 8시간의 예약과 연결되어 있는 경우 8시간은 100% 수용량과 같습니다. 사용자를 하루에 4시간 동안 작업하도록 할당하려면 사용자의 할당을 50%로 업데이트합니다.

      >[!NOTE]
      >
      >Workfront 관리자는 설정의 리소스 관리 영역에서 사용자 능력을 계산하기 위해 시스템에서 사용할 일정을 결정합니다. 자세한 내용은 [리소스 관리 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).


1. 을(를) 클릭합니다. **자세히** 메뉴 ![](assets/qs-more-menu.png) 작업 항목의 경우 **할당 편집**.

![](assets/more-menu-on-task-wb-nwe.png)

또는

작업 또는 문제 표시줄에서 일, 주 또는 월을 두 번 클릭합니다.

할당 상자는 편집할 수 있게 됩니다.

1. 각 일별, 주별 또는 월별 할당의 상자 내부를 클릭하여 사용자가 매일, 주 또는 월별로 할당받을 시간 또는 백분율 값을 수동으로 업데이트한 다음 **저장** 아이콘 ![](assets/checkmark-icon.png).

   >[!TIP]
   >
   >을(를) 클릭합니다. **취소** 아이콘 ![](assets/cancel-allocations-wb.png) 조정한 할당을 제거하려면

   ![](assets/wb-contouring-with-check-and-x-boxes-350x63.png)

   사용자 업데이트에 대한 할당입니다.

   >[!TIP]
   >
   >계획 완료 일자 이전에 완료된 작업이나 문제는 남은 일수에 대해 할당된 시간 수를 처리하여 사용자의 전체 할당에 계산되지 않습니다. 할당 표시 아이콘 및 예상 날짜 표시 설정이 모두 사용되도록 설정된 경우에만 표시됩니다.

   다음 시나리오가 있습니다.

   * 단순 또는 문제가 아닌 기간 유형이 있는 작업의 경우, 확인 표시 아이콘을 누르기 전에 총 할당이 계획 시간과 일치해야 합니다.
   * 단순 기간 유형이 있는 작업의 경우, 할당의 총 합계가 계획 시간보다 높거나 낮을 수 있으며, 일치하지 않더라도 확인 표시 아이콘을 클릭할 수 있습니다. 또한 작업에 대한 계획 시간(시)도 업데이트됩니다. 작업 로드 밸런서에서 작업에 대한 계획 시간을 업데이트할 수 있는 올바른 권한과 액세스 권한이 있어야 합니다.

      >[!TIP]
      >
      >작업의 단순 기간 유형을 나타내기 위해 할당 조정을 시작할 때 작업 이름의 오른쪽에 잠금 아이콘이 표시됩니다.

      ![](assets/lock-icon-on-simple-task-in-the-balancer-350x119.png)
   작업 로드 밸런서에서 계획 시간을 갱신하기 위해 충족해야 하는 조건에 대한 자세한 내용은 이 문서에서 다음 섹션을 참조하십시오. [사용자 할당을 관리할 때 작업 계획 시간 업데이트](#update-task-planned-hours-when-managing-user-allocations). 작업 기간 유형에 대한 자세한 내용은 [작업 기간 및 기간 유형 개요](../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (조건부) 작업이 두 명 이상의 사용자에게 할당된 경우 작업에 지정된 각 사용자에 대해 이러한 단계를 반복하여 각 사용자에 대한 할당을 업데이트합니다.

   작업 로드 밸런서를 볼 수 있는 액세스 권한이 있고, 동일한 사용자와 관리하는 동일한 프로젝트를 볼 수 있는 모든 사용자는 이제 관리하는 사용자에 대해 업데이트된 할당을 봅니다.

## 사용자 할당을 관리할 때 작업 계획 시간 업데이트 {#update-task-planned-hours-when-managing-user-allocations}

작업에 대한 작업 로드 밸런서에서 사용자 할당을 관리할 때 작업의 계획 시간을 갱신할 수 있습니다. 이 문제는 갱신된 할당된 시간의 합계가 해당 작업에 대한 계획된 시간의 최초 합계와 일치하지 않을 때 발생합니다.

>[!IMPORTANT]
>
>* 작업에 대한 계획 시간 업데이트는 프로젝트의 진행 상태에 영향을 줄 수 있습니다.
>* 일별 할당을 변경하여 수동으로 계획 시간을 갱신하면 나중에 작업에서 지정을 제거할 때 계획 시간에 영향을 줄 수 있습니다. 자세한 내용은 [계획 시간 개요](../../manage-work/tasks/task-information/planned-hours.md).
>
>* 작업 로드 밸런서에서 할당을 업데이트하여 문제에 대한 계획 시간을 업데이트할 수 없습니다.
>


다음 조건이 있을 경우 이 작업이 가능합니다.

* 작업 로드 밸런서에서 계획된 시간을 관리할 수 있는 올바른 권한과 액세스 권한이 있습니다. 여기에는 다음 항목이 포함되어 있습니다.

   * 작업에 대한 권한을 관리합니다.
   * 액세스 레벨의 리소스 관리 영역에서 작업 로드 밸런서 액세스에서 계획 시간을 갱신합니다.

   작업 로드 밸런서를 사용하는 데 필요한 액세스에 대한 자세한 내용은 이 문서에서 다음 섹션을 참조하십시오. [액세스 요구 사항](#access-requirements) .

* 작업에 단순 기간 유형이 있습니다.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;the statement above might include other duration types in the future)</p>
  -->
