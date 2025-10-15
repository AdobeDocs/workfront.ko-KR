---
product-area: resource-management
navigation-topic: resource-planning
title: 프로젝트 및 역할 보기를 사용하여 리소스 플래너의 예산 리소스
description: 프로젝트 및 역할 보기를 사용하여 Adobe Workfront 리소스 플래너에서 리소스의 예산을 책정할 수 있습니다. 리소스 플래너의 사용자 보기를 사용하여 리소스 예산을 책정할 수 없습니다.
author: Lisa
feature: Resource Management
exl-id: b1b48529-68e7-4aee-aaa1-d78e91fbb39c
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '2098'
ht-degree: 0%

---

# 프로젝트 및 역할 보기를 사용하여 리소스 플래너의 예산 리소스

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: broken off of another larger article (Planning in the RP); reformat, restructure, relink)</p>
-->

리소스 플래너의 주요 기능은 프로젝트에서 완료해야 하는 작업에 대한 리소스 예산을 책정하는 것입니다.

>[!IMPORTANT]
>
>리소스 플래너에 **프로젝트별 보기** 또는 **역할별 보기** 보기를 적용하는 경우에만 리소스 예산을 책정할 수 있습니다.

리소스 플래너에서 예산 정보를 시작하기 전에 다음 문서를 참조하십시오.

* [리소스 플래너 개요](../../resource-mgmt/resource-planning/get-started-resource-planner.md)
* [Adobe Workfront에서 리소스 예산을 책정하는 데 필요한 액세스](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)
* [리소스 플래너의 프로젝트 및 역할 보기에서 시간, FTE 및 비용 정보 개요](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>임의</p></td>
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
       <p>플랜</p></td> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>리소스 플래너에서 우선순위 및 예산 시간 편집에 대한 액세스 권한이 포함된 리소스 관리에 대한 액세스 편집</p> <p>재무 데이터에 대한 액세스 권한을 편집하여 원가별 예산 리소스</p> <p>프로젝트 및 사용자에 대한 액세스 편집</p></td> 
  </tr> 
  <tr> 
   <td>개체 권한</td> 
   <td> <p>정보의 예산을 책정할 프로젝트에 대한 권한 관리</p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 리소스 플래너의 예산 리소스

* [프로젝트 보기의 리소스 예산](#budget-resources-in-the-project-view)
* [역할 보기의 예산 리소스](#budget-resources-in-the-role-view)
* [예산 리소스 일괄](#budget-resources-in-bulk)

### 프로젝트 보기의 예산 리소스 {#budget-resources-in-the-project-view}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section is linked to the Budgeting Project Resources in the Business Case article)</p>
-->

{{step1-to-resourcing}}

1. **Planner**&#x200B;이(가) 기본적으로 표시됩니다.
1. (조건부) **프로젝트별 보기** 보기를 선택합니다.
1. 프로젝트 및 작업 역할을 확장하여 프로젝트, 작업 역할 또는 사용자에 대한 할당을 관리합니다.
1. 사용자에 대한 할당 예산을 책정하려면 다음 중 하나를 수행합니다.

   * **BDG** 열에서 사용자에 대한 예산 시간, FTE 또는 비용을 수동으로 지정하십시오.

   * 사용자의 작업 역할에 대한 **자세히** 메뉴를 클릭한 다음 **사용자 계획 시간을 예산에 맞게 설정**&#x200B;을 클릭합니다.\
     각 사용자의 예산 시간은 다음 공식을 사용하여 계산됩니다.

     `User Budgeted Hours = User Planned Hours`

1. 작업 역할에 대한 할당 예산을 책정하려면 다음 중 하나를 수행합니다.

   * **BDG** 열에서 작업 역할에 대한 예산 시간, FTE 또는 비용을 수동으로 지정하십시오.

     >[!NOTE]
     >
     >역할 예산 시간이 프로젝트 예산 시간에 추가됩니다.

   * (조건부) 사용자에 대한 예산 시간이 있는 경우 작업 역할에 대해 **자세히** 메뉴를 클릭한 다음 **역할에 대한 총 사용자 예산 시간**&#x200B;을 클릭합니다.\
     각 역할에 대한 예산 시간은 다음 공식을 사용하여 계산됩니다.

     `Role Budgeted Hours = SUM(User Budgeted Hours)`

   * 프로젝트에 대한 **자세히** 메뉴를 클릭한 다음 **예산에 따라 역할 계획된 시간 설정**&#x200B;을 클릭합니다.\
     각 역할에 대한 예산 시간은 다음 공식을 사용하여 계산됩니다.\
     &#x200B;*

     `Role Budgeted Hours = Role Planned Hours`

     >[!NOTE]
     >   
     >* 역할 예산 시간이 프로젝트 예산 시간에 추가됩니다.
     >* 사용자는 기본 및 기타(또는 보조) 역할 모두에 대한 예산을 책정할 수 있습니다.
     >* 작업 역할에 대한 리소스 플래너에 값을 표시하려면 사용자 역할에 대한 **FTE 가용성의 백분율**&#x200B;이(가) 사용 가능한 시간에 대해 0%와 다른 숫자여야 합니다. 사용자가 FTE 가용성의 0% **백분율**&#x200B;을(를) 가진 역할과 연결된 경우 해당 작업 역할에 대해 사용 가능한 시간 값이 0입니다. 이 경우 역할에 음수 **순 값**&#x200B;이 표시될 수 있습니다.\
     >작업 역할의 **FTE 가용성 비율**&#x200B;에 대한 자세한 내용은 문서 [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하십시오.

   * **BDG** 열에서 프로젝트에 대한 예산 시간, FTE 또는 비용을 수동으로 지정하십시오. 이렇게 하면 프로젝트 예산 시간 수가 프로젝트의 각 역할에 분배됩니다. 다음과 같은 시나리오가 있습니다.

      * 지정한 프로젝트 예산 시간이 프로젝트 계획 시간과 같은 경우 역할 예산 시간은 역할 계획 시간과 일치합니다.
      * 지정한 프로젝트 예산 시간 수가 프로젝트 계획 시간과 같지 않으면 역할 예산 시간은 각 역할에 필요한 계획 시간의 백분율에 따라 분배됩니다.\
        예를 들어 프로젝트에 20개의 계획된 시간이 있고 두 작업 역할 사이에 분배되어 있고(컨설턴트는 12개의 계획된 시간이 필요하고 엔지니어는 8개의 계획된 시간이 필요함) 프로젝트에 30시간을 예산책정하는 경우, 시간은 다음과 같이 분배됩니다. 컨설턴트 역할에는 18개의 예산 시간이 필요하고 엔지니어 역할에는 12개의 예산 시간이 제공됩니다.

1. 프로젝트에 대한 할당 예산을 책정하려면 다음 중 하나를 수행합니다.

   * 7단계에 설명된 대로 프로젝트 아래 역할의 예산을 책정합니다.\
     프로젝트 예산 시간은 다음 공식에 의해 계산됩니다.

     `Project Budgeted Hours = SUM(Role Budgeted Hours)`

   * **BDG** 열에서 프로젝트에 대한 예산 시간, FTE 또는 비용을 수동으로 지정하십시오.\
     이렇게 하면 7단계에 설명된 대로 역할 예산 시간이 업데이트됩니다.\
     ![budget_for_project.png](assets/budget-for-project-350x182.png)

1. **저장**&#x200B;을 클릭합니다.\
   리소스 플래너에서 리소스의 예산을 책정한 후 리소스 및 이와 연관된 비용에 대한 예산 시간이 모든 프로젝트의 비즈니스 사례에 나열됩니다.\
   비즈니스 사례의 리소스 예산 책정 영역을 이해하는 방법에 대한 자세한 내용은 [비즈니스 사례 영역 개요](../../manage-work/projects/define-a-business-case/areas-of-business-case.md) 문서의 &quot;리소스 예산 책정&quot; 섹션을 참조하십시오.

1. (선택 사항) 각 사용자의 가용 시간과 계획된 시간 사이에 초과 할당 또는 미달 활용을 통지하려면 사용자 보기를 선택합니다. 예산 시간은 사용자 보기에 표시되지 않습니다.

   Workfront에서 사용자 가용성을 계산하는 방법에 대한 자세한 내용은 [리소스 관리 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)을 참조하십시오.

### 역할 보기의 예산 리소스 {#budget-resources-in-the-role-view}

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: THIS IS WRONG - I LOGGED A BUG TO FIX THIS LINK - IT SHOULD GO TO"ACCESS NEEDED TO BUDGET IN THE RP":</p>
<p>Planning in the resource planner has links to the UI - ensure Flare notes are there for this: https://workfront.zendesk.com/hc/en-us/articles/115006356928 - the "Budgeting resources in the role view" is linked to this tooltip: ***This is linked to the product in the RP when the user does not have Manage rights on one of the projects under the role. This tool tip is linked here: "You don't have Manage permissions for all projects. Budget hours by individual project instead. Learn more...")</p>
</div>
-->

리소스 플래너에서 리소스 예산을 책정하려면 프로젝트에 대한 리소스 관리 및 재무 데이터에 대한 편집 액세스 권한과 재무 관리 권한이 있어야 합니다. 작업 역할 아래에 나열된 하나 이상의 프로젝트에 대한 보기 액세스 권한만 있는 경우 역할 보기에서 역할 할당의 예산을 책정할 수 없습니다. 관리 권한이 있는 프로젝트에 대한 할당 예산을 책정할 수 있습니다.

리소스 예산 책정에 필요한 액세스에 대한 자세한 내용은 문서 [Adobe Workfront의 리소스 예산 책정에 필요한 액세스](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)를 참조하십시오.

역할 보기의 리소스 플래너에서 할당 예산&#x200B;**&#x200B;** 책정하려면

1. Adobe Workfront 오른쪽 위 모서리에 있는 **주 메뉴** 아이콘 ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭합니다.

1. **리소스 조달**&#x200B;을 클릭합니다.
1. **Planner**&#x200B;이(가) 기본적으로 표시됩니다.
1. (조건부) **역할별 보기** 보기를 선택합니다.
1. 작업 역할 및 프로젝트를 확장하여 프로젝트, 작업 역할 또는 사용자에 대한 할당을 관리합니다.
1. 사용자에 대한 할당 예산을 책정하려면 다음 중 하나를 수행합니다.

   * **BDG** 열에서 사용자에 대한 예산 시간, FTE 또는 비용을 수동으로 지정하십시오.
   * 프로젝트에 대한 **자세히** 메뉴를 클릭한 다음 **사용자 계획 시간을 예산에 맞게 설정**&#x200B;을 클릭합니다.\
     각 사용자의 예산 시간은 다음 공식을 사용하여 계산됩니다.

     `User Budgeted Hours = User Planned Hours`

1. 작업 역할에 대한 할당 예산을 책정하려면 다음 중 하나를 수행합니다.

   * **BDG** 열에서 작업 역할에 대한 예산 시간, FTE 또는 비용을 수동으로 지정하십시오.\
     이렇게 하면 관리 액세스 권한이 있는 프로젝트에 대한 역할 예산 시간이 프로젝트 예산 시간으로 분산됩니다.

   * 작업 역할에 대한 **자세히** 메뉴를 클릭한 다음 **예산에 따른 프로젝트 계획 시간 설정&rbrack;을 클릭합니다.**&#x200B;역할 예산 시간은 다음 공식을 사용하여 계산됩니다.\
     &#x200B;*

     `Role Budgeted Hours = SUM(Project Budgeted Hours)`

     *프로젝트 예산 시간은 다음 공식을 사용하여 계산됩니다.

     `Project Budgeted Hours = Project Planned Hours`

   * **BDG** 열에서 작업 역할에 나열된 프로젝트의 예산 시간, FTE 또는 비용을 수동으로 지정하십시오.\
     이렇게 하면 역할에 프로젝트 예산 시간 수가 추가됩니다.

   >[!NOTE]
   >
   >사용자는 기본 및 기타(또는 보조) 역할 모두에 대한 예산을 책정할 수 있습니다. 작업 역할에 대한 리소스 플래너에 값을 표시하려면 사용자 역할에 대한 **FTE 가용성의 백분율**&#x200B;이(가) 사용 가능한 시간에 대해 0%와 다른 숫자여야 합니다. 사용자가 FTE 가용성의 0% **백분율**&#x200B;을(를) 가진 역할과 연결된 경우 해당 작업 역할에 대해 사용 가능한 시간 값이 0입니다. 이 경우 역할에 음수 **순 값**&#x200B;이 표시될 수 있습니다.\
   >작업 역할의 **FTE 가용성 비율**&#x200B;에 대한 자세한 내용은 문서 [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하십시오.

1. 프로젝트에 대한 할당 예산을 책정하려면 다음 중 하나를 수행합니다.

   * **BDG** 열에서 프로젝트에 대한 예산 시간, FTE 또는 비용을 수동으로 지정하십시오.\
     프로젝트가 나열된 역할의 예산 시간도 업데이트됩니다.

   * 작업 역할에 대한 **자세히** 메뉴를 클릭한 다음 **예산에 따라 프로젝트 계획된 시간 설정**&#x200B;을 클릭합니다.\
     프로젝트 예산 시간은 다음 공식에 의해 계산됩니다.

     `Project Budgeted Hours = Project Planned Hours`

     프로젝트 예산 시간이 역할 예산 시간에 추가됩니다.

   * (조건부) 사용자의 예산 시간을 책정했다면 프로젝트에 대해 **기타** 메뉴를 클릭한 다음 **프로젝트의 총 사용자 예산 시간**&#x200B;을 클릭합니다.\
     프로젝트 예산 시간은 다음 공식을 사용하여 계산됩니다.

     `Project Budgeted Hours = SUM(User Budgeted Hours)`

     ![budget_by_role.png](assets/budget-by-role-350x181.png)

1. **저장**&#x200B;을 클릭합니다.\
   리소스 플래너에서 리소스의 예산을 책정한 후 리소스 및 이와 연관된 비용에 대한 예산 시간이 모든 프로젝트의 비즈니스 사례에 나열됩니다.
비즈니스 사례의 리소스 예산 책정 영역을 이해하는 방법에 대한 자세한 내용은 문서 [비즈니스 사례의 리소스 예산](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)을 참조하세요.

1. (선택 사항) **사용자별 보기** 보기를 선택하여 각 사용자의 사용 가능 시간과 계획된 시간 사이에 초과 할당 또는 미달 활용률을 확인합니다. 예산 시간은 사용자별 조회 보기에 표시되지 않습니다.

### 예산 리소스 일괄 {#budget-resources-in-bulk}

빠른 링크를 사용할 때 리소스에 대한 할당의 예산을 일괄 책정할 수 있습니다. 빠른 링크는 프로젝트 및 역할 보기에만 사용할 수 있습니다.

![자동 예산 옵션](assets/rp-project-view-with-automatic-budgeting-options-on-project-350x173.png)

>[!NOTE]
>
>리소스에 대한 예산 배부에 대한 빠른 링크를 사용할 경우 화면에 표시되는 기간에만 예산이 자동으로 적용됩니다. 프로젝트의 타임라인이 화면에 표시되는 시간보다 긴 기간에 걸쳐 있는 경우 왼쪽에서 오른쪽으로 스크롤한 다음 빠른 링크를 사용하여 리소스의 예산을 자동으로 책정해야 합니다.

자원의 예산을 일괄 책정하려면

1. 로 이동합니다.\
   리소스 플래너에 액세스하는 방법에 대한 자세한 내용은 문서 [리소스 플래너 개요](../../resource-mgmt/resource-planning/get-started-resource-planner.md)의 &quot;리소스 플래너에 액세스&quot; 섹션을 참조하십시오.\
   관리할 수 있는 프로젝트 목록이 목록에 표시됩니다.

1. (선택 사항) 각 프로젝트를 확장하여 연결된 작업 역할 목록을 확인합니다.\
   또는
1. (선택 사항) **역할별 보기**&#x200B;를 선택한 다음 각 역할을 확장하여 연결된 프로젝트 목록을 확인합니다.
1. 프로젝트 또는 작업 역할의 이름 위로 마우스를 가져갑니다.
1. 프로젝트 또는 역할 이름의 맨 오른쪽에 표시되는 **자세히** 아이콘 ![options_icon_resource_planner.png](assets/options-icon-resource-planner.png)을 클릭합니다.

1. 사용 가능한 옵션 중 하나를 눌러 다른 객체에 대한 예산 시간(BDG)을 자동으로 지정합니다.

   프로젝트에서 자세히 아이콘을 클릭했는지 또는 역할을 클릭했는지에 따라 예산 책정 옵션이 달라집니다. 아래 표는 프로젝트 및 역할에 사용할 수 있는 옵션을 보여 줍니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td> </td> 
      <td><strong>프로젝트 보기</strong> </td> 
      <td><strong>역할 보기</strong> </td> 
     </tr> 
     <tr> 
      <td>프로젝트 옵션</td> 
      <td> 
       <ul> 
        <li><strong>역할의 계획된 시간을 예산 시간으로 설정</strong>: 역할의 예산 시간을 계획된 시간과 동일하게 하려면 이 옵션을 선택하십시오. 역할에 대한 총 예산 시간이 프로젝트 예산 시간에 대해 표시됩니다. </li> 
        <li><strong>예산 책정 날짜 조정</strong> : 예산 시간을 다른 일정으로 이동하려면 이 옵션을 선택합니다.<br>예산 책정 날짜 조정에 대한 자세한 내용은 <a href="../../resource-mgmt/resource-planning/adjust-budgeting-dates.md" class="MCXref xref">리소스 플래너에서 예산 책정 날짜 조정</a>을 참조하세요.</li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>사용자의 계획된 시간을 예산 시간으로 설정</strong>: 사용자의 예산 시간을 계획된 시간과 동일하게 하려면 이 옵션을 선택하십시오. </li> 
        <li><strong>프로젝트에 대한 총 사용자 예산 시간</strong>: 모든 사용자 예산 시간을 함께 추가하고 합계를 프로젝트 및 역할의 예산 시간으로 표시하려면 이 옵션을 선택하십시오. 수동으로 사용자 예산을 책정했거나 이전 옵션을 먼저 사용한 후에 이 옵션을 사용하는 것이 좋습니다. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>역할 옵션</td> 
      <td> 
       <ul> 
        <li><strong>사용자의 계획된 시간을 예산 시간으로 설정</strong>: 사용자의 예산 시간을 계획된 시간과 동일하게 하려면 이 옵션을 선택하십시오. </li> 
        <li><strong>역할에 대한 총 사용자 예산 시간</strong>: 사용자의 모든 예산 시간을 함께 추가하고 역할 및 프로젝트의 예산 시간으로 합계를 표시하려면 이 옵션을 선택하십시오. 수동으로 사용자 예산을 책정했거나 이전 옵션을 먼저 사용한 후에 이 옵션을 사용하는 것이 좋습니다. </li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>프로젝트의 계획된 시간을 예산 시간으로 설정</strong>: 프로젝트 예산 시간을 프로젝트 계획된 시간과 동일하게 하려면 이 옵션을 선택하십시오. </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >리소스 플래너에서 작업하는 전제 조건 중 일부가 누락된 경우 일부 옵션이 표시되지 않을 수 있습니다.
   >
   >
   >리소스 플래너의 정확한 예산 책정을 위해 충족해야 하는 필수 구성 요소에 대한 자세한 내용은 [리소스 플래너 개요](../../resource-mgmt/resource-planning/get-started-resource-planner.md) 문서의 &quot;리소스 플래너에서 작업하기 위한 필수 구성 요소&quot; 섹션을 참조하십시오.\
   >예를 들어, 일부 옵션은 다음 시나리오에 표시되지 않을 수 있습니다.
   >
   >   
   >   
   >   * 프로젝트가 리소스 풀과 연결되지 않은 경우
   >   * 프로젝트와 연결된 리소스 풀에 사용자가 없는 경우
   >   * 프로젝트와 연결된 리소스 풀에 연결된 작업 역할이 없는 사용자가 포함된 경우.
   >   
   >
