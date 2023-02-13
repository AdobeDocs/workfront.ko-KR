---
product-area: resource-management
navigation-topic: resource-planning
title: 프로젝트 및 역할 보기를 사용하는 자원 계획자의 예산 자원
description: 프로젝트 및 역할 보기를 사용하여 Adobe Workfront 리소스 플래너에서 리소스를 예측할 수 있습니다. 자원 계획자의 사용자 뷰를 사용하여 자원을 예약할 수 없습니다.
author: Alina
feature: Resource Management
exl-id: b1b48529-68e7-4aee-aaa1-d78e91fbb39c
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '2146'
ht-degree: 0%

---

# 프로젝트 및 역할 보기를 사용하는 자원 계획자의 예산 자원

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: broken off of another larger article (Planning in the RP); reformat, restructure, relink)</p>
-->

자원 계획자의 주요 기능은 프로젝트에서 완료해야 하는 작업에 대한 자원의 예산을 책정하는 것입니다.

>[!IMPORTANT]
>
>을(를) 적용하는 경우에만 리소스를 예약할 수 있습니다 **프로젝트별 보기** 또는 **역할별 보기** 리소스 계획자에 대한 보기.

자원 계획자에서 예산 정보를 시작하기 전에 다음 문서를 참조하십시오.

* [리소스 플래너 개요](../../resource-mgmt/resource-planning/get-started-resource-planner.md)
* [Adobe Workfront의 예산 리소스에 대한 액세스 필요](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)
* [리소스 계획자의 프로젝트 및 역할 뷰의 시간, FTE 및 비용 정보 개요](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>리소스 계획자의 우선순위 및 예산 시간 편집에 대한 액세스 권한을 포함하는 리소스 관리에 대한 액세스 편집</p> <p>비용별 예산 자원에 대한 재무 데이터 액세스 편집</p> <p>프로젝트 및 사용자에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>예산을 편성할 프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 자원 계획자의 예산 자원

* [프로젝트 보기의 예산 리소스](#budget-resources-in-the-project-view)
* [역할 보기의 예산 리소스](#budget-resources-in-the-role-view)
* [예산 자원 일괄 처리](#budget-resources-in-bulk)

### 프로젝트 보기의 예산 리소스 {#budget-resources-in-the-project-view}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section is linked to the Budgeting Project Resources in the Business Case article)</p>
-->

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

1. 클릭 **리소스**.
1. 다음 **계획자** 기본적으로 표시됩니다.
1. (조건부) **프로젝트별 보기** 보기.
1. 프로젝트 및 작업 역할을 확장하여 프로젝트, 작업 역할 또는 사용자의 할당을 관리합니다.
1. 사용자에 대한 예산 할당은 다음 중 하나를 수행합니다.

   * 에서 **BDG** 열, 사용자의 예산책정된 시간, FTE 또는 비용을 수동으로 지정합니다.

   * 을(를) 클릭합니다. **자세히** 사용자의 작업 역할에 대한 메뉴를 클릭한 다음 **사용자의 계획 시간을 예산책정으로 설정**.\
      각 사용자의 예산책정된 시간은 다음 공식을 사용하여 계산됩니다.

      ```
      User Budgeted Hours = User Planned Hours
      ```

1. Job 역할에 대한 할당 예산을 책정하려면 다음 중 하나를 수행합니다.

   * 에서 **BDG** 열, 작업 역할에 대해 예산책정된 시간, FTE 또는 비용을 수동으로 지정합니다.

      >[!NOTE]
      >
      >역할 예산책정된 시간은 프로젝트 예산책정된 시간에 추가됩니다.

   * (조건부) 사용자를 위해 시간 예산을 책정한 경우 **자세히** 작업 역할에 대한 메뉴를 클릭한 다음 **역할에 대한 총 사용자 예산책정 시간**.\
      각 역할에 대한 예산책정된 시간은 다음 공식을 사용하여 계산됩니다.

      ```
      Role Budgeted Hours = SUM(User Budgeted Hours)
      ```

   * 을(를) 클릭합니다. **자세히** 프로젝트에 대한 메뉴를 클릭한 다음 **역할 계획 시간을 예산책정으로 설정**.\
      각 역할에 대한 예산책정된 시간은 다음 공식을 사용하여 계산됩니다.\
      *

      ```
      Role Budgeted Hours = Role Planned Hours
      ```

      >[!NOTE]
      >   
      >* 역할 예산책정된 시간은 프로젝트 예산책정된 시간에 추가됩니다.
      >* 사용자는 기본 및 기타(또는 보조) 역할에 대해 예산 책정될 수 있습니다.
      >* 다음 **FTE 가용성 비율** 사용자 역할의 경우 [사용 가능한 시간]에서 작업 역할에 대한 리소스 계획자에 값을 표시하려면 사용자의 역할이 0%와 다른 숫자여야 합니다. 사용자가 0%의 역할과 연관된 경우 **FTE 가용성 비율**&#x200B;을 지정하는 경우 해당 작업 역할에 대해 사용 가능한 시간 값이 0입니다. 이 경우 이 역할은 부정적인 것으로 표시될 수 있습니다 **순 값**.\
         >에 대한 자세한 정보 **FTE 가용성 비율** 작업 역할에 대해서는 문서를 참조하십시오 [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).


   * 에서 **BDG** 열, 프로젝트에 대한 예산책정 시간, FTE 또는 비용을 수동으로 지정합니다. 프로젝트 예산책정된 시간 수를 프로젝트의 각 역할에 분배합니다. 다음 시나리오가 있습니다.

      * 지정한 프로젝트 예산책정된 시간 수가 프로젝트 계획시간과 같은 경우, 역할 예산책정된 시간은 역할 계획 시간과 일치합니다.
      * 지정한 프로젝트 예산책정된 시간 수가 프로젝트 계획시간과 같지 않으면 각 역할에 필요한 계획 시간 백분율에 따라 역할 예산책정된 시간이 분배됩니다.\
         예를 들어, 프로젝트에 20시간의 계획 시간이 있고 두 Job 역할 사이에 배포되는 경우(컨설턴트는 12시간의 계획 시간을 필요로 하며 엔지니어는 8시간의 계획 시간을 필요로 함), 프로젝트에 30시간을 편성하면 다음과 같이 시간이 배포됩니다. 컨설턴트 역할은 18시간의 예산책정된 시간을 수신하고 엔지니어 역할은 12시간의 예산책정된 시간을 수신한다.

1. 프로젝트에 대한 할당 예산을 책정하려면 다음 중 하나를 수행합니다.

   * 7단계에서 설명한 대로 프로젝트에서 역할에 예산을 책정하십시오.\
      프로젝트 예산책정된 시간은 다음 공식으로 계산됩니다.

      ```
      Project Budgeted Hours = SUM(Role Budgeted Hours)
      ```

   * 에서 **BDG** 열, 프로젝트에 대한 예산책정 시간, FTE 또는 비용을 수동으로 지정합니다.\
      단계 7에 설명된 대로 Role 예산 책정된 시간을 갱신합니다.\
      ![budget_for_project.png](assets/budget-for-project-350x182.png)

1. **저장**&#x200B;을 클릭합니다.\
   Resource Planner에서 자원을 예산을 지정한 후 자원에 대한 예산책정된 시간 및 이와 연관된 비용은 모든 프로젝트의 업무 사례에 나열됩니다.\
   Business Case의 Resource Budgeting 영역 이해에 대한 자세한 내용은 문서의 &quot;Resource Budgeting&quot; 섹션을 참조하십시오 [비즈니스 사례 영역 개요](../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (선택 사항) 사용자 뷰를 선택하여 각 사용자에 대한 가용 시간과 계획 시간 사이의 초과 할당 또는 저가동률을 확인합니다. 예산책정된 시간은 사용자 뷰에 표시되지 않습니다.

### 역할 보기의 예산 리소스 {#budget-resources-in-the-role-view}

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: THIS IS WRONG - I LOGGED A BUG TO FIX THIS LINK - IT SHOULD GO TO"ACCESS NEEDED TO BUDGET IN THE RP":</p>
<p>Planning in the resource planner has links to the UI - ensure Flare notes are there for this: https://workfront.zendesk.com/hc/en-us/articles/115006356928 - the "Budgeting resources in the role view" is linked to this tooltip: ***This is linked to the product in the RP when the user does not have Manage rights on one of the projects under the role. This tool tip is linked here: "You don't have Manage permissions for all projects. Budget hours by individual project instead. Learn more...")</p>
</div>
-->

자원 계획자에서 자원을 예산하기 위해서는 프로젝트에 대한 자원 관리 및 재무 데이터에 대한 편집 액세스 및 재무 관리 권한이 있어야 합니다. 작업 역할 아래에 나열된 하나 이상의 프로젝트에 대한 보기 액세스 권한만 있는 경우 역할 보기에서 역할에 대한 할당을 예산을 할당할 수 없습니다. 관리 권한이 있는 프로젝트에 대한 할당 예산을 계속 책정할 수 있습니다.

예산 책정 리소스에 필요한 액세스에 대한 자세한 내용은 문서를 참조하십시오 [Adobe Workfront의 예산 리소스에 대한 액세스 필요](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

**** 역할 뷰의 리소스 계획자에서 예산 배부를 수행하려면

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

1. 클릭 **리소스**.
1. 다음 **계획자** 기본적으로 표시됩니다.
1. (조건부) **역할별 보기** 보기.
1. 작업 역할 및 프로젝트를 확장하여 프로젝트, 작업 역할 또는 사용자에 대한 할당을 관리합니다.
1. 사용자에 대한 할당 예산을 책정하려면 다음 중 하나를 수행합니다.

   * 에서 **BDG** 열, 사용자의 예산책정된 시간, FTE 또는 비용을 수동으로 지정합니다.
   * 을(를) 클릭합니다. **자세히** 프로젝트에 대한 메뉴를 클릭한 다음 **사용자의 계획 시간을 예산책정으로 설정**.\
      각 사용자의 예산책정된 시간은 다음 공식을 사용하여 계산됩니다.

      ```
      User Budgeted Hours = User Planned Hours
      ```

1. Job 역할에 대한 할당 예산을 책정하려면 다음 중 하나를 수행합니다.

   * 에서 **BDG** 열, 작업 역할에 대해 예산책정된 시간, FTE 또는 비용을 수동으로 지정합니다.\
      관리할 수 있는 프로젝트에 대한 프로젝트 예산책정된 시간에 역할 예산책정시간을 분배합니다.

   * 을(를) 클릭합니다. **자세히** 작업 역할에 대한 메뉴를 클릭한 다음 **프로젝트의 계획 시간을 예산책정으로 설정합니다.**다음 공식을 사용하여 역할 예산책정 시간을 계산합니다.\
      *

      ```
      Role Budgeted Hours = SUM(Project Budgeted Hours)
      ```

      *프로젝트 예산책정된 시간은 다음 공식을 사용하여 계산됩니다.

      ```
      Project Budgeted Hours = Project Planned Hours
      ```

   * 에서 **BDG** 열, 작업 역할 아래에 나열된 프로젝트에 대한 예산책정된 시간, FTE 또는 비용을 수동으로 지정합니다.\
      그러면 역할에 프로젝트 예산책정된 시간 수가 추가됩니다.
   >[!NOTE]
   >
   >사용자는 기본 및 기타(또는 보조) 역할에 대해 예산 책정될 수 있습니다. 다음 **FTE 가용성 비율** 사용자 역할의 경우 [사용 가능한 시간]에서 작업 역할에 대한 리소스 계획자에 값을 표시하려면 사용자의 역할이 0%와 다른 숫자여야 합니다. 사용자가 0%의 역할과 연관된 경우 **FTE 가용성 비율**&#x200B;을 지정하는 경우 해당 작업 역할에 대해 사용 가능한 시간 값이 0입니다. 이 경우 이 역할은 부정적인 것으로 표시될 수 있습니다 **순 값**.\
   >에 대한 자세한 정보 **FTE 가용성 비율** 작업 역할에 대해서는 문서를 참조하십시오 [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. 프로젝트에 대한 할당 예산을 책정하려면 다음 중 하나를 수행합니다.

   * 에서 **BDG** 열, 프로젝트에 대한 예산책정 시간, FTE 또는 비용을 수동으로 지정합니다.\
      또한 프로젝트가 나열된 역할에 대한 예산책정된 시간도 갱신합니다.

   * 을(를) 클릭합니다. **자세히** 작업 역할에 대한 메뉴를 클릭한 다음 **프로젝트 계획 시간을 예산책정으로 설정**.\
      프로젝트 예산책정된 시간은 다음 공식으로 계산됩니다.

      ```
      Project Budgeted Hours = Project Planned Hours
      ```

      프로젝트 예산책정된 시간이 역할 예산책정된 시간에 추가됩니다.

   * (조건부) 사용자를 위해 시간 예산을 책정한 경우 **자세히** 프로젝트에 대한 메뉴를 클릭한 다음 **프로젝트에 대한 총 사용자 예산책정 시간**.\
      프로젝트 예산책정된 시간은 다음 공식을 사용하여 계산됩니다.

      ```
      Project Budgeted Hours = SUM(User Budgeted Hours)
      ```

      ![budget_by_role.png](assets/budget-by-role-350x181.png)

1. **저장**&#x200B;을 클릭합니다.\
   Resource Planner에서 자원을 예산을 지정한 후 자원에 대한 예산책정된 시간 및 이와 연관된 비용은 모든 프로젝트의 업무 사례에 나열됩니다.\
   Business Case의 Resource Budgeting 영역 이해에 대한 자세한 내용은 문서를 참조하십시오 [비즈니스 사례의 예산 자원](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

1. (선택 사항) **사용자별 보기** 각 사용자에 대해 사용 가능 시간과 계획 시간 사이의 사용자 초과 할당 또는 저가동률을 확인합니다. 예산책정된 시간은 사용자별 보기에 표시되지 않습니다.

### 예산 자원 일괄 처리 {#budget-resources-in-bulk}

빠른 링크를 사용할 때 리소스에 대한 예산 할당을 일괄 처리할 수 있습니다. 빠른 링크는 프로젝트 및 역할 보기에만 사용할 수 있습니다.

![](assets/rp-project-view-with-automatic-budgeting-options-on-project-350x173.png)

>[!NOTE]
>
>자원에 대한 예산 배부에 대한 빠른 링크를 사용하는 경우 화면에 표시된 기간에만 예산 편성이 자동으로 적용됩니다. 프로젝트의 타임라인이 화면에 표시된 시간보다 긴 시간 동안 지속되는 경우 왼쪽에서 오른쪽으로 스크롤한 다음 빠른 링크를 사용하여 리소스를 자동으로 예산을 책정해야 합니다.

자원을 일괄 편성하려면

1. 로 이동합니다.\
   리소스 계획자 액세스에 대한 자세한 내용은 문서의 &quot;리소스 계획자 액세스&quot; 섹션을 참조하십시오 [리소스 플래너 개요](../../resource-mgmt/resource-planning/get-started-resource-planner.md).\
   관리할 수 있는 프로젝트 목록이 목록에 표시됩니다.

1. (선택 사항) 각 프로젝트를 확장하여 연결된 작업 역할 목록을 봅니다.\
   또는
1. (선택 사항) 선택 **역할별 보기**&#x200B;그런 다음 각 역할을 확장하여 연결된 프로젝트 목록을 봅니다.
1. 프로젝트 이름 또는 작업 역할 위로 마우스를 가져갑니다.
1. 을(를) 클릭합니다. **자세히** 아이콘 ![options_icon_resource_planner.png](assets/options-icon-resource-planner.png)프로젝트 또는 역할 이름의 맨 오른쪽에 표시됩니다.

1. 사용 가능한 옵션 중 하나를 눌러 다른 객체에 대한 BDG(예산책정된 시간) 양을 자동으로 지정합니다.

   프로젝트에서 자세히 아이콘을 클릭했는지 또는 역할에 대해 자세히 아이콘을 클릭했는지 여부에 따라 일괄 예산 책정 옵션이 다릅니다. 아래 표에는 프로젝트 및 역할에 사용할 수 있는 옵션이 나와 있습니다.

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
        <li><strong>역할 계획 시간을 예산책정으로 설정</strong>: 역할의 예산 책정된 시간이 계획 시간과 동일하도록 하려면 이 옵션을 선택합니다. 역할에 대한 총 예산책정된 시간이 프로젝트 예산책정된 시간에 대해 표시됩니다. </li> 
        <li><strong>예산 책정 날짜 조정</strong> : 예산책정된 시간을 다른 기간으로 이동하려면 이 옵션을 선택합니다.<br>예산 책정 날짜 조정에 대한 자세한 내용은 <a href="../../resource-mgmt/resource-planning/adjust-budgeting-dates.md" class="MCXref xref">자원 계획자에서 예산 책정 일자 조정</a>.</li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>사용자의 계획 시간을 예산책정으로 설정</strong>: 사용자의 예산책정된 시간을 계획 시간과 동일하게 만들려면 이 옵션을 선택합니다. </li> 
        <li><strong>프로젝트에 대한 총 사용자 예산책정 시간</strong>: 모든 사용자 예산책정된 시간을 함께 추가하고 프로젝트 및 역할에 대한 총 예산책정된 시간으로 표시하려면 이 옵션을 선택합니다. 사용자의 예산을 수동으로 설정하거나 이전 옵션을 먼저 사용한 후에 이 옵션을 사용하는 것이 좋습니다. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>역할 옵션</td> 
      <td> 
       <ul> 
        <li><strong>사용자의 계획 시간을 예산책정으로 설정</strong>: 사용자의 예산책정된 시간을 계획 시간과 동일하게 만들려면 이 옵션을 선택합니다. </li> 
        <li><strong>역할에 대한 총 사용자 예산책정 시간</strong>: 사용자의 모든 예산책정된 시간을 함께 추가하고 롤과 프로젝트에 대한 총 예산책정된 시간으로 표시하려면 이 옵션을 선택합니다. 사용자의 예산을 수동으로 설정하거나 이전 옵션을 먼저 사용한 후에 이 옵션을 사용하는 것이 좋습니다. </li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>프로젝트 계획 시간을 예산책정으로 설정</strong>: 프로젝트 예산책정된 시간과 프로젝트 계획된 시간을 동일하게 하려면 이 옵션을 선택합니다. </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >리소스 플래너에서 작업하기 위한 필수 구성 요소 중 일부가 누락된 경우 일부 옵션이 표시되지 않을 수 있습니다.
   >
   >
   >Resource Planner에서 정확한 예산 편성을 위해 충족해야 하는 사전 요구 사항에 대한 자세한 내용은 의 &quot;Resource Planner 작업 사전 요구 사항&quot; 섹션을 참조하십시오 [리소스 플래너 개요](../../resource-mgmt/resource-planning/get-started-resource-planner.md) 문서.\
   >예를 들어 다음 시나리오에서는 일부 옵션이 표시되지 않을 수 있습니다.
   >
   >   
   >   
   >   * 프로젝트가 리소스 풀과 연결되어 있지 않은 경우
   >   * 프로젝트와 연결된 리소스 풀에 사용자가 없는 경우
   >   * 프로젝트와 연결된 리소스 풀에 연관된 작업 역할이 없는 사용자가 포함된 경우

