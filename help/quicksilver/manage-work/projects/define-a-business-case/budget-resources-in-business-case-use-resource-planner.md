---
navigation-topic: business-case-and-scorecards
title: 자원 계획자를 사용하여 업무 사례의 예산 자원
description: 자원 계획의 일부로 프로젝트 레벨 자원 계획자를 사용하여 업무 사례를 작성할 때 프로젝트에서 작업을 완료하는 데 필요한 작업 역할을 예산을 책정할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1249'
ht-degree: 0%

---

# 자원 계획자를 사용하여 업무 사례의 예산 자원

자원 계획의 일부로 프로젝트 레벨 자원 계획자를 사용하여 업무 사례를 작성할 때 프로젝트에서 작업을 완료하는 데 필요한 작업 역할을 예산을 책정할 수 있습니다.

비즈니스 사례 만들기에 대한 자세한 내용은 [프로젝트에 대한 비즈니스 사례 생성](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>프로젝트 레벨 자원 계획자에 입력하는 정보는 시스템 레벨 자원 계획자에도 표시됩니다. 그 반대도 사실이다. 리소스 계획자에 대한 자세한 내용은 [리소스 플래너 개요](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Adobe Workfront 시나리오 계획자를 사용하여 비즈니스 사례에서 리소스를 예측할 수도 있습니다. 자세한 내용은 [시나리오 계획자를 사용하여 비즈니스 사례의 예산 자원](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront 플랜</a>*</td> 
   <td> <p>Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront 라이선스 개요</a>*</td> 
   <td> <p>검토 이상</p> <p>중요 사항: 자원 예산 정보를 수정하려면 계획 라이센스가 있어야 합니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>다음에 대한 액세스 편집: </p> 
    <ul> 
     <li> <p>프로젝트</p> </li> 
     <li> <p>리소스 관리</p> </li> 
     <li> <p>재무 데이터</p> </li> 
    </ul> <p>예산 자원에 필요한 액세스에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Adobe Workfront의 예산 리소스에 대한 액세스 필요</a>.</p> <p>참고: 여전히 액세스 권한이 없는 경우 Adobe Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하기 전에 다음을 수행해야 합니다.

* Adobe Workfront에서 리소스 계획을 위한 모든 사전 요구 사항을 충족합니다. 자세한 내용은 [리소스 플래너 개요](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* 리소스 풀을 프로젝트와 연결합니다.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

   >[!NOTE]
   비즈니스 사례에서 문제에 지정된 자원을 예산을 책정할 수 없습니다. 시스템 레벨 자원 계획자에서 예산을 책정할 수 있습니다. 리소스 계획자에 대한 자세한 내용은 [리소스 플래너 개요](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* 필수 조건은 아니지만 프로젝트의 작업에 대해 계획 시간 을 표시하는 것이 좋습니다. 이를 통해 작업을 완료하는 데 필요한 작업의 양을 파악할 수 있으므로, 작업을 완료하기 위해 리소스를 예산을 책정해야 하는 많은 시간을 결정하는 데 도움이 됩니다. 작업과 계획 시간 연관에 대한 자세한 내용은 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## 비즈니스 사례에서 프로젝트 및 예산 자원에 자원 풀 적용

>[!IMPORTANT]
15년 동안 자원을 편성할 수 있습니다. 기간이 15년을 초과하는 프로젝트에 대한 자원을 예산을 책정하는 경우 예산 정보가 정확하지 않을 수 있습니다.

자원 풀이 없는 프로젝트에 대한 비즈니스 사례에서 자원 풀 및 예산 프로젝트 자원을 적용하려면

1. 자원을 예산을 편성할 프로젝트로 이동합니다.
1. 클릭 **비즈니스 사례** 왼쪽 패널에 표시됩니다.
1. (조건부) 회사에 Workfront 시나리오 플래너에 대한 라이센스가 없는 경우 **리소스 예산 책정 편집** 에서 **리소스 예산 책정** 섹션을 클릭한 다음 5단계를 계속 진행합니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. (선택 사항 및 조건부) 프로젝트 정보가 시나리오 플래너의 이니셔티브에서 게시된 경우 다음 중 하나를 수행합니다.

   * 에서 리소스 계획자 선택 **프로젝트의 예산책정된 노무비 계산에 사용할 시간을 선택합니다** 필드를 클릭한 다음 **> Edit Resource Budgeting 을 선택합니다.**.

      ![](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * 프로젝트에 대한 예산 책정 리소스를 위해 시나리오 계획자를 선택한 경우 **변경** > **리소스 예산 책정 편집**.

      ![](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)
   프로젝트의 예산책정된 시간(시간)을 사용하여 프로젝트의 예산책정된 노무비를 계산합니다.

   시나리오 플래너는 새 Adobe Workfront 경험에서만 사용할 수 있으며 추가 라이센스가 필요합니다. Workfront 시나리오 플래너에 대한 자세한 내용은 [시나리오 계획자 개요](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   프로젝트 작업을 시작할 때 리소스 계획자 또는 시나리오 계획자를 사용할지 여부를 결정하는 것이 좋습니다. 프로젝트 수명 중에 두 버전 간을 자주 전환하면 프로젝트에 대한 리소스를 할당하는 방식으로 일치하지 않을 수 있습니다.

1. 에서 **리소스 풀 선택** 필드, 하나 또는 여러 개 지정 **리소스 풀**.

   활성 사용자로 채워지는 리소스 풀만 지정해야 합니다.

   >[!TIP]
   프로젝트가 이미 자원 풀과 연관된 경우 기본적으로 자원 계획자가 표시됩니다. 프로젝트에 리소스 풀을 더 추가하려면 프로젝트를 편집합니다. 프로젝트 편집에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

1. 클릭 **적용**.

   선택한 프로젝트에 대한 리소스 계획자가 표시됩니다.

   기본적으로 이 프로젝트와 연관된 처음 20개의 작업 역할이 리소스 예산 책정 섹션에 알파벳 순서로 나열됩니다. 

   리소스 계획자에 대한 자세한 내용은 [리소스 플래너 개요](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![BC_resource_budgeting_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. (선택 사항 및 조건부) 작업 역할을 확장하여 연결된 사용자를 확인합니다.

   >[!NOTE]
   활성 사용자는 다음 기준을 충족하는 경우에만 연관된 작업 역할 아래에 표시됩니다.
   * 프로젝트의 리소스 풀 중 하나에 속합니다.
   * 그들에게 배정된 시간이 예산책정되어 있습니다.
   * 이 구성 요소는 프로젝트의 작업 역할 중 하나와 연결됩니다.


    

1. 클릭 **오늘** 을 입력하여 현재 시간 프레임으로 돌아갑니다.
1. (선택 사항) **주**, **월** 또는 **분기** 를 입력하여 프로젝트에 대한 정보를 다른 시간대에 표시할 수 있습니다.
1. (선택 사항) **시간** 드롭다운 메뉴에서 **시간**,**FTE**, 또는 **비용** 자원 계획자에 정보가 표시되는 방식을 변경하려면 기본적으로 시간은 표시됩니다.

1. (선택 사항) **내보내기** 리소스 계획자를 Excel 파일로 내보내기

   >[!NOTE]
   한 번에 최대 12개의 기간에 대한 데이터를 내보낼 수 있습니다.

1. (선택 사항) **전체 화면** 아이콘 ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png) 리소스 계획자를 전체 화면 모드로 표시하려면

1. 업데이트 **BDG** (예산책정된 시간) 다음 중 하나를 수행하여 사용자, 역할 또는 프로젝트에 대한 시간, FTE 또는 비용 값이 있는 필드:

   * 역할, 사용자 또는 프로젝트의 시간, FTE 또는 비용 값을 수동으로 예측합니다.

      또는

   * 을(를) 클릭합니다. **옵션** 프로젝트 또는 작업 역할의 아이콘과 역할, 사용자 또는 프로젝트에 대한 시간을 자동으로 편성하는 옵션을 선택합니다.
   리소스 계획자의 프로젝트 뷰에서 예산 편성에 대한 자세한 내용은 다음을 참조하십시오 [프로젝트 및 역할 보기를 사용하는 자원 계획자의 예산 자원](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   프로젝트의 타임라인에 관계없이 Resource Budgeting 영역에 표시되는 모든 기간 동안 자원에 대한 시간, FTE 또는 비용을 예측할 수 있습니다. 예를 들어, 프로젝트의 타임라인에서 자원을 사용할 수 없을 수도 있지만(계획 시간과 연관된 경우) 다른 시간 동안 사용할 수 있을 수도 있다는 것을 나타내려면 계획 시간이 0인 기간에 대해 예산을 책정하여 작업할 수 있습니다.

1. (선택 사항) 예산책정된 시간, FTE 또는 비용을 다른 시간대로 이동할 수 있는지 확인하려면 **옵션** 아이콘, **예산 책정 날짜 조정**.

   예산책정된 일자 조정에 대한 자세한 내용은 [자원 계획자에서 예산 책정 일자 조정](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. **저장**&#x200B;을 클릭합니다.

   Job 역할과 연관된 시간당 비용 비율이 있는 경우 Resource Budgeting 영역에서 자원 예산을 책정하는 것이 **예산책정된 인건비** 프로젝트 구성 예산책정된 노무비는 업무 사례의 자원 예산 영역 및 업무 사례 요약에 표시됩니다.

   >[!TIP]
   원가는 프로젝트 통화로 비즈니스 사례에 표시됩니다.

   업무 사례에 지정된 예산 정보는 자원 계획자에도 표시됩니다.
