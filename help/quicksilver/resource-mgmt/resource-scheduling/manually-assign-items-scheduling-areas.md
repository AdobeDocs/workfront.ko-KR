---
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: 예약 영역에서 지정되지 않은 작업 및 문제를 수동으로 지정
description: 예약 타임라인을 사용하면 각 사용자가 작업 항목에 대해 할당되는 시간을 지정하는 것 외에도 사용자 지정을 관리할 수 있습니다.
author: Alina
feature: Resource Management
exl-id: 627e4442-767a-41a2-9700-76f2ad2dc9cf
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# 예약 영역에서 지정되지 않은 작업 및 문제를 수동으로 지정

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
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.  </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

예약 타임라인을 사용하면 각 사용자가 작업 항목에 대해 할당되는 시간을 지정하는 것 외에도 사용자 지정을 관리할 수 있습니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

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
   <td> <p>프로젝트, 작업 및 문제에 대한 보기 이상의 액세스 권한</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트, 작업 및 문제에 대한 권한 기여</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 예약 타임라인에서 작업 및 문제를 지정하기 전에 사전 요구 사항

이 섹션에 설명된 대로 사용자 할당 관리를 시작하기 전에 의 설명에 따라 Workfront에서 리소스 예약이 작동하는 방식을 숙지하십시오 [리소스 예약 시작](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

이 섹션에 설명된 대로 사용자 지정을 성공적으로 관리하려면 먼저 사용자, 프로젝트, 작업 및 문제가 [Workfront에서 예약 도구를 사용하기 위한 사전 요구 사항](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#prerequisites) 문서의 섹션 [리소스 예약 시작](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

다음 섹션에서는 사용자 지정을 수동으로, 자동으로 또는 사용자 또는 역할별로 할당을 변경하여 수정하는 방법에 대해 설명합니다.

## 사용자에게 할당되지 않은 작업 또는 문제를 수동으로 할당

예약 타임라인은 사용자가 작업이나 문제를 완료할 수 있는 필요한 가시성을 제공합니다.\
예약 타임라인에 대한 자세한 내용은 [리소스 예약 시작](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Workfront의 다음 영역에서 예약 타임라인의 사용자에게 개별 작업 및 문제를 할당할 수 있습니다.

* 리소스(여러 프로젝트에 대한 리소스를 예약할 때)의 예약 섹션을 참조하십시오.
* 프로젝트 아래의 예약 섹션(단일 프로젝트에 대한 리소스를 예약할 때).
* 팀 아래의 예약 섹션(팀을 위한 리소스를 예약할 때).

예약 타임라인 위쪽에 있는 [지정되지 않음] 영역에 표시되는 정보는 리소스 예약을 사용하는 Workfront의 영역(여러 프로젝트에 대한 리소스를 예약할 때), [예약] 섹션(단일 프로젝트에 대한 리소스를 예약할 때) 또는 [예약] 섹션(팀에 대한 리소스를 예약할 때)에 따라 다릅니다. 자세한 내용은 섹션을 참조하십시오 [예약 영역에서 사용 가능한 기능](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md#functionality-available-in-the-scheduling-area) 기사 [예약 영역 개요](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md).

예약 타임라인을 보고 있는 Workfront의 영역에 따라 일부 사용자에게만 작업이 할당될 수 있습니다. 자세한 내용은 [예약 영역 개요](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md).

예약 타임라인에서 사용자에게 할당되지 않은 작업 또는 문제를 할당하려면 다음을 수행합니다.

1. 여러 프로젝트, 개별 프로젝트 또는 팀의 예약 타임라인으로 이동합니다.

   * **여러 프로젝트의 경우**:  을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 **리소스 > 작업 로드 밸런서**&#x200B;를 선택하고 을 선택합니다. **예약** 를 클릭합니다.
   * **개별 프로젝트의 경우**: 프로젝트로 이동하여 **작업 로드 밸런서** 왼쪽 패널의 섹션에서 을(를) 선택한 다음 **예약** 왼쪽 위 드롭다운 메뉴에서 을 선택합니다.
   * **팀**: 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **팀**&#x200B;를 클릭하고, 팀을 선택하고 **작업 로드 밸런서** 왼쪽 패널에서 를 선택하고 **예약** 왼쪽 위 드롭다운 메뉴에서 을 선택합니다.

   ![scheduling_contours.png](assets/scheduling-contours-350x139.png)

1. (선택 사항) 다음에 설명된 대로 예약 타임라인에 표시되는 컨텐츠를 사용자 지정하는 필터를 만듭니다. [예약 영역에서 정보를 필터링합니다.](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md) . [예약 영역에서 정보를 필터링합니다.](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md). 예를 들어 예약 타임라인에 문제를 표시하려면 필터를 만들어야 합니다.

1. (선택 사항) 다음에 설명된 대로 예약 타임라인에 표시되는 날짜 범위를 수정합니다. [예약 영역의 날짜 범위 조정](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#adjusting-the-date-range-for-which-data-is-displayed) in [리소스 예약 시작](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

1. 할당되지 않은 작업 또는 문제를 할당하려면 다음을 수행합니다.

   * 할당하려는 사용자 행으로 작업이나 문제를 드래그합니다.\
      지정된 사용자에 대해 하루에 최대 10개의 작업이 표시됩니다. 목록을 확장하여 해당 사용자에게 현재 할당된 모든 작업을 볼 수 있습니다. 예약 타임라인에서 지정한 후에는 10개 이상의 작업이 일시적으로 표시될 수 있습니다.\
      항목을 드래그하면 작업이나 문제를 해제하고 할당을 완료하기 전에 다음 정보가 표시됩니다.

   * 예약 타임라인에서 사용자 할당이 활성화되면 할당 결과를 완료하면 사용자가 초과 할당되는 경우 빨간색 초과 할당 표시기가 표시됩니다.\
      초과 할당 지표에 대한 자세한 내용은 섹션을 참조하십시오 [할당 지표](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md#understanding-allocation-indicators) 기사 [예약 영역에서 사용자 할당 관리](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).

      만약 **일치하는 역할을 가진 사용자에게 지정 제한** 설정 영역에서 옵션을 활성화하면 할당을 받을 수 없는 사용자는 흐리게 표시됩니다. 이 옵션을 비활성화하면 모든 사용자가 할당을 받을 수 있습니다. 이 옵션은 기본적으로 활성화되어 있습니다.\
      이 옵션에 대한 자세한 내용은 [](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md#allowing-assignmennts-to-users-regardless-of-role) in [예약 영역에서 역할 및 그룹 구성원에 관계없이 사용자 지정 허용](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md)

      사용자의 행에 드롭 표시기가 표시됩니다. 이를 통해 지정을 수행하기 전에 품목이 지정되는 위치를 확인할 수 있습니다.

      지정할 작업 또는 문제를 확장하고 **지정** 필드에서 할당할 사용자의 이름을 입력하고 드롭다운 목록에서 사용자 이름을 클릭합니다.\
      ![schedule_task_expanded.png](assets/schedule-task-expanded-350x170.png)

1. (조건부) 사용자에게 지정되지 않은 작업 또는 문제를 할당한 후 예약 타임라인에서 사용자 간의 작업 및 문제에 대한 기존 지정을 조정할 수 있습니다. 프로젝트에 대한 자원을 스케줄링할 때(스케줄링 탭 또는 스태핑 탭 중 하나) 동일한 작업 역할이 있는 사용자만 지정을 받을 수 있습니다.\
   다른 사용자에게 작업이나 문제를 다시 할당하려면 한 사용자 행에서 다른 사용자 행으로 작업을 드래그합니다.
1. (선택 사항)에 설명된 대로 지정된 각 사용자가 작업 또는 문제에 할당되는 시간을 구성합니다. [예약 영역에서 사용자 할당 관리](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md) .
