---
navigation-topic: business-case-and-scorecards
title: 리소스 플래너를 사용한 비즈니스 사례의 예산 리소스
description: 리소스 계획의 일부로, 프로젝트 수준 리소스 플래너를 사용하여 비즈니스 사례를 작성할 때 프로젝트에서 작업을 완료하는 데 필요한 작업 역할의 예산을 책정할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: 14b6b9c4a184131cfdc33b6156c578218ed9119a
workflow-type: tm+mt
source-wordcount: '1229'
ht-degree: 0%

---

# 리소스 플래너를 사용한 비즈니스 사례의 예산 리소스

<!--Audited: 06/2025-->

리소스 계획의 일부로, 프로젝트 수준 리소스 플래너를 사용하여 비즈니스 사례를 작성할 때 프로젝트에서 작업을 완료하는 데 필요한 작업 역할의 예산을 책정할 수 있습니다.

비즈니스 사례를 만드는 방법에 대한 자세한 내용은 [프로젝트에 대한 비즈니스 사례 만들기](../../../manage-work/projects/define-a-business-case/create-business-case.md)를 참조하세요.

>[!TIP]
>
>프로젝트 레벨 리소스 플래너에 입력한 정보는 시스템 레벨 리소스 플래너에도 표시됩니다. 그 반대도 마찬가지다. 리소스 플래너에 대한 자세한 내용은 [리소스 플래너 개요](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)를 참조하십시오.

Adobe Workfront 시나리오 플래너를 사용하여 비즈니스 사례에서 리소스의 예산을 책정할 수도 있습니다. 자세한 내용은 [시나리오 플래너를 사용하여 비즈니스 사례에서 리소스 예산](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md)을 참조하세요.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 플랜*</p></td> 
   <td> <p>현재: Prime 이상</p>
   <p>레거시: Pro 이상</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
   <td> <p>전류: 라이트 이상</p>
   <p>레거시: 검토 이상</p>

<p><b>중요 사항:</b></p> 
   <p>현재: 리소스 예산 정보를 수정하려면 Standard 라이센스가 있어야 합니다. </p> 
   <p>레거시: 리소스 예산 정보를 수정하려면 플랜 라이선스가 있어야 합니다. </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>다음에 대한 액세스 권한 편집: </p> 
    <ul> 
     <li> <p>프로젝트</p> </li> 
     <li> <p>리소스 관리</p> </li> 
     <li> <p>재무 데이터</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td> <p>프로젝트에 대한 권한 관리</p> </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

시작하기 전에 다음을 수행해야 합니다.

* Adobe Workfront에서 리소스 계획을 수립하기 위한 모든 사전 요구 사항을 충족합니다. 자세한 내용은 [리소스 플래너 개요](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)를 참조하십시오.

* 리소스 풀을 프로젝트와 연결합니다.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

  >[!NOTE]
  >
  >비즈니스 사례의 문제에 할당된 리소스의 예산을 책정할 수 없습니다. 시스템 수준 리소스 플래너에서 예산을 책정할 수 있습니다. 리소스 플래너에 대한 자세한 내용은 [리소스 플래너 개요](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)를 참조하십시오.

* 전제 조건은 아니지만 프로젝트의 작업에 대해 계획된 시간을 표시하는 것도 좋습니다. 이를 통해 작업을 완료하는 데 필요한 작업의 양을 파악할 수 있습니다. 이는 작업을 완료하기 위해 리소스 예산을 책정해야 하는 시간을 결정하는 데 도움이 됩니다. 작업을 계획된 시간과 연결하는 방법에 대한 자세한 내용은 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md)을 참조하십시오.

## 비즈니스 사례에서 프로젝트에 리소스 풀 적용 및 예산 리소스

>[!IMPORTANT]
>
>15년 동안 리소스의 예산을 책정할 수 있습니다. 15년을 초과하는 기간 동안 프로젝트에 대한 리소스의 예산을 책정하는 경우 예산 책정 정보가 정확하지 않을 수 있습니다.

리소스 풀이 없는 프로젝트에 대해 비즈니스 사례에 리소스 풀과 예산 프로젝트 리소스를 적용하려면 다음을 수행합니다.

1. 리소스 예산을 책정할 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **비즈니스 사례**&#x200B;를 클릭합니다.
1. (조건부) 회사에 Workfront 시나리오 플래너에 대한 라이선스가 없는 경우 **리소스 예산 책정** 섹션에서 **리소스 예산 편성 편집**&#x200B;을(를) 클릭한 다음 5단계를 계속하십시오.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. (선택 사항 및 조건부) 프로젝트 정보가 시나리오 플래너의 이니셔티브에서 게시된 경우 다음 중 하나를 수행합니다.

   * **프로젝트의 예산 인건비를 계산하는 데 사용할 시간을 선택하십시오** 필드에서 리소스 플래너를 선택한 다음 **선택 > 리소스 예산 편집**&#x200B;을 클릭합니다.

     <!--![Business case in Resource Planner](assets/business-case-rp-selected-with-choose-button-350x120.png)-->

   * 시나리오 플래너가 프로젝트의 리소스 예산 책정을 위해 선택된 경우 **변경** > **리소스 예산 편집**&#x200B;을 클릭합니다.

     <!--![Business case in Scenario Planner](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)-->

   프로젝트의 예산 시간을 사용하여 프로젝트의 예산 인건비를 계산합니다.

   시나리오 플래너는 새 Adobe Workfront 경험에서만 사용할 수 있으며 추가 라이선스가 필요합니다. Workfront 시나리오 플래너에 대한 자세한 내용은 [시나리오 플래너 개요](../../../scenario-planner/scenario-planner-overview.md)를 참조하십시오.

   >[!NOTE]
   >
   >프로젝트 작업을 시작할 때 리소스 플래너 또는 시나리오 플래너를 사용할지 여부를 결정하는 것이 좋습니다. 프로젝트 기간 동안 둘 사이를 자주 전환하면 프로젝트에 대한 리소스 예산 책정 방식에 일치하지 않을 수 있습니다.

1. **리소스 풀 선택** 필드에서 하나 또는 여러 개의 **리소스 풀**&#x200B;을(를) 지정합니다.

   활성 사용자로 채워진 리소스 풀만 지정해야 합니다.

   >[!TIP]
   >
   >프로젝트가 이미 리소스 풀과 연결된 경우 리소스 플래너가 기본적으로 표시됩니다. 프로젝트에 리소스 풀을 더 추가하려면 프로젝트를 편집하십시오. 프로젝트 편집에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md)을 참조하세요.

1. **적용**&#x200B;을 클릭합니다.

   선택한 프로젝트에 대한 리소스 플래너가 표시됩니다.

   기본적으로 이 프로젝트와 연관된 처음 20개의 작업 역할은 리소스 예산 섹션에서 알파벳순으로 나열됩니다. 

   리소스 플래너에 대한 자세한 내용은 [리소스 플래너 개요](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)를 참조하십시오.

   <!--![BC_resource_budgeting_area.png](assets/bc-resource-budgeting-area-350x276.png)-->

1. (선택 사항 및 조건부) 작업 역할을 확장하여 연결된 사용자를 확인합니다.

   >[!NOTE]
   >
   >활성 사용자는 다음 기준을 충족하는 경우에만 연결된 작업 역할 아래에 표시됩니다.
   >
   >   
   >   
   >   * 이는 프로젝트의 리소스 풀 중 하나에 속합니다.
   >   * 그들에게 할당된 예산 시간이 있습니다.
   >   * 프로젝트의 작업 역할 중 하나와 연결됩니다.
   >   
   >

    

1. 오늘의 시간대로 돌아가려면 **오늘**&#x200B;을 클릭하세요.
1. (선택 사항) **주**, **월** 또는 **분기**&#x200B;를 클릭하여 다른 시간대에 프로젝트에 대한 정보를 표시합니다.
1. (선택 사항) **시간** 드롭다운 메뉴를 클릭하고 **시간**,**FTE** 또는 **비용**&#x200B;을 선택하여 리소스 플래너에 정보가 표시되는 방식을 변경합니다. 시간은 기본적으로 표시됩니다.

1. (선택 사항) 리소스 플래너를 Excel 파일로 내보내려면 **내보내기**&#x200B;를 클릭합니다.

   >[!NOTE]
   >
   >한 번에 최대 12개의 기간 동안 데이터를 내보낼 수 있습니다.

1. (선택 사항) **전체 화면** 아이콘 ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png)을 클릭하여 리소스 플래너를 전체 화면 모드로 표시합니다.

1. 다음 중 하나를 수행하여 사용자, 역할 또는 프로젝트에 대한 시간, FTE 또는 비용 값으로 **BDG**(예산 시간) 필드를 업데이트합니다.

   * 역할, 사용자 또는 프로젝트에 대한 시간, FTE 또는 비용 값을 수동으로 예측합니다.

     또는

   * 프로젝트 또는 작업 역할에 대한 **옵션** 아이콘을 클릭하고 역할, 사용자 또는 프로젝트에 대한 시간을 자동으로 예산책정하는 옵션을 선택하십시오.

   리소스 플래너의 프로젝트 보기에서 예산을 책정하는 방법에 대한 자세한 내용은 [프로젝트 및 역할 보기를 사용하여 리소스 플래너의 리소스 예산](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)을 참조하십시오.

   >[!NOTE]
   >
   >프로젝트의 타임라인에 관계없이 리소스 예산 영역에 표시되는 모든 시간대에 리소스에 대한 시간, FTE 또는 비용을 예산할 수 있습니다. 예를 들어, 프로젝트의 타임라인(계획된 시간과 연관된 시간) 중에는 리소스를 사용할 수 없지만 다른 시간에는 사용할 수 있음을 나타내려면 계획된 시간이 0인 시간대(작업을 할 수 있는 시간대인 경우)에 예산을 편성하여 리소스를 사용할 수 있습니다.

1. (선택 사항) 예산 시간, FTE 또는 비용을 다른 시간대로 이동할 수 있는지 확인하려면 **옵션** 아이콘을 클릭한 다음 **예산 책정 날짜 조정**&#x200B;을 클릭합니다.

   예산 일자 조정에 대한 자세한 내용은 [리소스 플래너에서 예산 일자 조정](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md)을 참조하십시오.

1. **저장**&#x200B;을 클릭합니다.

   작업 역할과 연계된 시간당 비용 비율이 있는 경우 리소스 예산 책정에서 리소스 예산을 책정하면 프로젝트의 **예산 인건비**&#x200B;가 계산됩니다. 예산 인건비는 업무 사례의 자원 예산 책정 영역 및 업무 사례 요약에 표시됩니다.

   >[!TIP]
   >
   >비용은 프로젝트 통화로 비즈니스 사례에 표시됩니다.

   비즈니스 사례에 지정된 예산 편성 정보는 리소스 플래너에도 표시됩니다.

   프로젝트를 복사할 때 예산 시간을 새 프로젝트에도 복사할 수 있습니다. 리소스 플래너에 예산 책정된 시간만 복사됩니다. 자세한 내용은 [프로젝트 복사](../manage-projects/copy-project.md)를 참조하십시오.
