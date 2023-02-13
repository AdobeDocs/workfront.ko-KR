---
product-area: resource-management
navigation-topic: resource-scheduling
title: 예약 영역에서 미할당 작업 및 문제를 자동으로 지정
description: 예약 도구를 사용할 때 Adobe Workfront에서 사용 가능한 사용자 간에 현재 작업 할당을 분석하고 아직 할당되지 않은 작업 또는 문제에 대해 지능적인 논리적 할당을 제안할 수 있도록 할 수 있습니다. 제안된 지정을 완료하기 전에 수정할 수 있습니다.
author: Alina
feature: Resource Management
exl-id: 087fe3ef-9b85-491b-9fdc-436a01822ede
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1579'
ht-degree: 0%

---

# 예약 영역에서 미할당 작업 및 문제를 자동으로 지정

>[!IMPORTANT]
>  
><span class="preview">이 문서에 설명된 예약 기능은 2023년 1월 23.1 릴리스부터 Adobe Workfront에서 더 이상 사용되지 않고 제거됩니다.   </span>
>  
> <span class="preview"> 이 문서는 2023년 초에 23.1 릴리스 직후 제거됩니다. 지금은 이에 따라 책갈피를 업데이트하는 것이 좋습니다. </span>
> 
><span class="preview"> 이제 작업 로드 밸런서를 사용하여 자원에 대한 작업 일정을 예약할 수 있습니다. </span>
>  
> <span class="preview">작업 로드 밸런서를 사용하여 리소스를 예약하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [작업 로드 밸런서](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!-- 

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

예약 도구를 사용할 때 Adobe Workfront에서 사용 가능한 사용자 간에 현재 작업 할당을 분석하고 아직 할당되지 않은 작업 또는 문제에 대해 지능적인 논리적 할당을 제안할 수 있도록 할 수 있습니다. 제안된 지정을 완료하기 전에 수정할 수 있습니다.

Workfront은 현재 선택한 날짜 범위 내의 [지정되지 않음] 영역에서 사용할 수 있는 작업 및 문제를 살펴보고 각 항목에 대한 할당을 한 번에 제안합니다. 필터를 만들어 [지정되지 않음] 영역에서 사용할 수 있는 항목의 수를 제한할 수 있습니다.

시스템 관리자는 Workfront이 시스템 수준에서 리소스 가용성을 계산하는 방법을 결정합니다(시간 및 FTE 가용성을 고려). 이 시스템 전체 설정에 따라 기본 예약이나 사용자의 일정을 사용하여 리소스 가용성이 계산됩니다. 자세한 내용은 [Workfront에서 예약 영역에 대한 리소스 시간 및 FTE 가용성을 계산하는 방법을 구성합니다](../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>프로젝트, 작업 및 문제에 대한 보기 이상의 액세스 권한</p> <p><strong>메모</strong>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트, 작업 및 업데이트 문제에 대한 권한 이상을 제공할 수 있습니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건 {#prerequisites}

Workfront은 독점 알고리즘을 사용하여 할당 제안을 결정합니다. 최상의 결과를 얻으려면 Workfront에서 다음 정보가 정확한지 확인하십시오.

* 다음을 포함한 작업 및 문제 정보:

   * 역할 할당\
      역할에 할당되지 않은 작업 및 문제에 대한 제안이 없습니다.
   * 계획된 시간\
      현재 작업이나 문제에 계획된 시간이 없는 경우, Workfront에서는 자동으로 작업을 할당할 때 작업당 4시간의 계획된 시간을 가정합니다. 이러한 시간은 작업 항목에 자동으로 할당되지 않습니다. 보다 현실적인 발령 분배를 보장하기 위해서만 사용됩니다.
   * 계획 시작 일자 및 계획 완료 일자

* 다음을 포함한 사용자 정보:

   * 사용자 프로필에 1차 및 2차 역할 할당
   * 프로젝트 팀 정보

## 역할 제한 구성

역할 제한은 특정 역할을 사용하여 작업을 자동으로 할당할 수 있는 사용자 수를 제어합니다. 역할 제한 작업은 여러 사용자 간에 역할 기반 작업이 분산되지 않도록 프로젝트 별로 작동합니다.

다음 시나리오는 프로젝트에 역할 제한이 적용되는 방식을 설명합니다.

* **시나리오 1**: 프로젝트 팀에 할당된 사용자가 없는 경우 시스템은 역할 제한을 사용하여 작업을 할당합니다.\
   예를 들어 프로젝트 팀에 지정된 사용자가 없는 프로젝트가 있습니다. 이 프로젝트에는 할당해야 하는 프로젝트 관리 작업이 10개 있으며 프로젝트 관리자 역할에 대해 역할 제한을 1로 설정했습니다. 역할 제한이 1로 설정되어 있으므로 시스템은 10개의 작업을 1개의 프로젝트 관리자에 모두 할당합니다.

* **시나리오 2**: 역할 제한이 프로젝트 팀에 할당된 사용자 수보다 큰 경우 추가 사용자에게 작업이 할당됩니다.\
   예를 들어 프로젝트 팀에 작성기가 한 명 할당된 프로젝트가 있습니다. 이 프로젝트에는 할당해야 하는 12개의 작성기 작업이 있으며 작성기 역할에 대해 2개의 역할 제한이 설정되어 있습니다. 역할 제한이 2로 설정되어 있으므로 시스템은 프로젝트 팀 작성자와 추가 작성기 사이에 12개의 작업을 모두 할당합니다.

* **시나리오 3**: 역할 제한이 프로젝트 팀에 할당된 사용자 수보다 작은 경우 역할 제한이 무시됩니다.\
   예를 들어 프로젝트 팀에 디자이너 4명이 지정된 프로젝트가 있습니다. 이 프로젝트에는 8개의 디자이너 작업을 할당해야 하며 디자이너 역할에 대해 역할 제한을 2로 설정했습니다. 역할 제한은 2로 설정되지만 시스템은 4명의 프로젝트 팀 디자이너 각각에 8개의 작업을 할당합니다.

Job 역할 지정에 대한 제한을 설정하려면 다음을 수행합니다.

1. 여러 프로젝트 또는 개별 프로젝트의 예약 타임라인으로 이동합니다.

   * **여러 프로젝트의 경우**:  을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 **리소스 > 작업 로드 밸런서**&#x200B;를 선택하고 을 선택합니다. **예약** 를 클릭합니다.
   * **개별 프로젝트의 경우**: 프로젝트로 이동하여 **작업 로드 밸런서** 왼쪽 패널의 섹션에서 을(를) 선택한 다음 **예약** 왼쪽 위 드롭다운 메뉴에서 을 선택합니다.

1. 을(를) 클릭합니다. **설정** 아이콘.\
   ![Automode_settings.png](assets/automode-settings.png)

1. Automated Resource Scheduling 섹션에서 **제한** 인라인 열 및 **역할** 열을 입력하고 양수를 입력합니다.\
   Workfront에서 자동으로 변경 내용을 저장합니다.

   >[!NOTE]
   >
   >현재 프로젝트 팀 구성원은 역할 제한 집합에 관계없이 모든 권장 작업에 자동으로 참가할 수 있습니다.

   ![Set_Role_Limits.png](assets/set-role-limits-350x341.png)

1. (선택 사항) **표시** 제한 열 맨 위에 있는 메뉴를 선택하고 원하는 표시 옵션을 선택합니다.
1. 리소스 예약 영역으로 돌아가려면 를 클릭합니다. **예약으로 돌아가기**.

## 작업 및 문제 자동 할당

스케줄링 타임라인의 사용자에게 작업 및 문제를 지정할 수 있습니다. 스케줄링 탭에 있는지(여러 프로젝트에 대한 자원을 스케줄링할 때) 또는 스태핑 탭(개별 프로젝트에 대한 자원을 스케줄링할 때).

Workfront에서 지정되지 않음 영역의 작업 및 문제에 대한 할당을 자동으로 제안할 수 있도록 하려면

1. 여러 프로젝트 또는 개별 프로젝트의 예약 타임라인으로 이동합니다.

   * **여러 프로젝트의 경우**:  을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 **리소스 > 작업 로드 밸런서**&#x200B;를 선택하고 을 선택합니다. **예약** 를 클릭합니다.
   * **개별 프로젝트의 경우**: 프로젝트로 이동하여 **작업 로드 밸런서** 왼쪽 패널의 섹션에서 을(를) 선택한 다음 **예약** 왼쪽 위 드롭다운 메뉴에서 을 선택합니다.

1. (선택 사항) 필터를 만들어 예약 타임라인의 [지정되지 않음] 영역에 표시되는 콘텐츠를 사용자 지정합니다.\
   필터 만들기에 대한 자세한 내용은 [예약 영역에서 정보를 필터링합니다.](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md#creating-and-modifying-filters-on-the-scheduling-tab-for-projects) in [예약 영역에서 정보를 필터링합니다.](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md) [예약 영역에서 정보를 필터링합니다.](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md)

   >[!TIP]
   >
   >Workfront이 가장 적합한 사용자에게 작업을 할당하도록 하려면
   >
   >* Portfolio, 프로그램, 프로젝트 등 미지정 영역에 표시되는 작업에 영향을 주는 정보만 필터링합니다.
   >* 예약 타임라인에서 할당할 수 있는 사용자에게 영향을 주는 정보는 필터링하지 않는 것이 좋습니다. 이렇게 하면 Workfront에서 모든 잠재적 담당자를 볼 수 없게 되며, 이로 인해 배정이 덜 만족될 수 있습니다.


1. (선택 사항) 다음에 설명된 대로 예약 타임라인에 표시되는 날짜 범위를 수정합니다. [예약 영역의 날짜 범위 조정](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#adjusting-the-date-range-for-which-data-is-displayed) in [리소스 예약 시작](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md). Workfront은 예약 타임라인에서 볼 수 있는 날짜 범위 내의 작업 및 문제에 대해서만 할당을 수행합니다.

1. 을(를) 클릭합니다. **자동** 예약 타임라인의 오른쪽 위 모서리에 있는 단추.\
   ![scheduling_auto.png](assets/scheduling-auto-350x221.png)\
   Workfront에서는 각 작업 또는 문제에 대해 할당을 제안합니다 **지정되지 않음** 영역.

   >[!TIP]
   >
   >할당을 제안하려면 작업 및 문제가 이미 역할에 할당되어 있어야 합니다. 최상의 결과를 얻으려면 작업 및 문제에 [전제 조건](#prerequisites).

   제안된 할당은 다음과 같이 각 작업이나 문제에 점선 윤곽선으로 구분됩니다.\
   **제안된 작업 할당:**

   **기존 작업 할당:**

1. (선택 사항) 지정을 완료하기 전에 제안된 발령이나 기존 지정을 수정할 수 있습니다.

   >[!NOTE]
   >
   >기존 지정을 수정하는 경우 제안된 상태로 변경됩니다.

   * 다른 사용자에게 항목을 할당하려면

      * 제안된 사용자의 작업이나 문제를 할당하려는 다른 사용자의 행으로 드래그합니다.

         <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE: lists in this article need to be reformatted and maybe split - too many levels in)      
        </MadCap:conditionalText>      
        -->

         지정된 사용자에 대해 하루에 최대 10개의 작업이 표시됩니다. 목록을 확장하여 해당 사용자에게 현재 할당된 모든 작업을 볼 수 있습니다. 예약 타임라인에서 지정한 후에는 10개 이상의 작업이 일시적으로 표시될 수 있습니다.\
         항목을 드래그하면 작업이나 문제를 해제하고 할당을 완료하기 전에 다음 정보가 표시됩니다.

         * 사용자의 행에 드롭 표시기가 표시됩니다. 이를 통해 지정을 수행하기 전에 품목이 지정되는 위치를 확인할 수 있습니다.
         * 예약 타임라인에서 사용자 할당이 활성화되면 할당을 완료하면 사용자가 초과 할당될 때 빨간색 초과 할당 표시기가 표시됩니다.\
            초과 할당 지표에 대한 자세한 내용은 [할당 지표](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md#understanding-allocation-indicators).

         * 할당을 받을 수 없는 사용자는 흐리게 표시됩니다.
      * 지정할 작업 또는 문제를 확장하고 **지정** 필드에서 할당할 사용자의 이름을 입력하고 드롭다운 목록에서 사용자 이름을 클릭합니다.\
         ![schedule_task_expanded.png](assets/schedule-task-expanded-350x170.png)
   * 할당을 연기하려면 아직 다시 할당할 준비가 되지 않은 작업 또는 문제를 **지정되지 않음** 영역.



1. 을(를) 클릭합니다. **할당 만들기** 예약 타임라인의 맨 위에 있는 버튼을 눌러 제안된 지정을 완료합니다.\
   또는\
   클릭 **취소** 제안된 모든 과제들을 그들의 이전 직책에 되돌려주기 위해.
