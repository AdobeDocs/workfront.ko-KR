---
product-area: resource-management
navigation-topic: resource-planning
title: Adobe Workfront Resource Planner를 사용하여 리소스 가용성 및 할당 검토
description: 자원 계획자에서 자원의 가용성과 프로젝트에 대한 계획 또는 예산책정된 작업 금액을 조회할 수 있습니다. 이러한 값은 시간, FTE(Full Time Equivalent) 또는 원가 금액으로 표시되며 열로 구성됩니다.
author: Alina
feature: Resource Management
exl-id: 5b3e52a6-af9b-4e68-8d6e-43a5151a2a2c
source-git-commit: 24cc3ece515fd778a9bc9e8afbcd534f48b24230
workflow-type: tm+mt
source-wordcount: '1270'
ht-degree: 4%

---

# Adobe Workfront Resource Planner를 사용하여 리소스 가용성 및 할당 검토

자원 계획자에서 자원의 가용성과 프로젝트에 대한 계획 또는 예산책정된 작업 금액을 조회할 수 있습니다. 이러한 값은 시간, FTE(Full Time Equivalent) 또는 원가 금액으로 표시되며 열로 구성됩니다.

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
   <td> <p>검토 이상 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>다음 항목에 대한 액세스 권한 보기 이상:</p> 
    <ul> 
     <li> <p>리소스 관리</p> </li> 
     <li> <p>재무 데이터</p> </li> 
     <li> <p>사용자</p> </li> 
     <li> <p>프로젝트</p> </li> 
    </ul> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>리소스 계획자에서 보려는 프로젝트에 대한 보기 또는 더 높은 권한</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

<!--note from the table about the license: Review or higher: 
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (waiting on Vazgen to confirm - working differenly in classic)
      </MadCap:conditionalText>
     -->

## 전제 조건

리소스 계획자와 함께 작업하는 데 필요한 모든 전제 조건을 충족해야 합니다. 자세한 내용은 [리소스 플래너 개요](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

>[!IMPORTANT]
>
>Resource Planner의 올바른 기능에 필요한 사전 요구 사항이 누락된 경우, 숫자 중 일부가 0이거나 예산책정 시간이 흐리게 표시될 수 있습니다.

## 자원 가용성 및 할당

자원의 가용성 및 할당을 표시하는 열은 리소스 계획자에 적용하는 뷰에 따라 변경됩니다. 프로젝트, 역할 또는 사용자별로 리소스 계획자에 정보를 표시하는 방법에 대한 자세한 내용은 [리소스 플래너 탐색 개요](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

뷰를 자원 계획자로 변경할 때 다음 사항을 고려하십시오.

* 을 적용할 때 **프로젝트별 보기** 또는&#x200B;**역할별 보기** 보기를 보면 다음 열이 표시됩니다.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: Alina: (some of the information in this area is also covered in Calculating Costs in the RP - https://workfront.zendesk.com/hc/en-us/articles/115004186433 - update this article also, when changes here occur)
  </MadCap:conditionalText>
  -->



   * 사용 가능한 시간, FTE 또는 비용
   * 계획 시간, FTE 또는 비용
   * 예산 책정된 시간, FTE 또는 비용
   * 시간, FTE 또는 원가 차이
   * 순시간, FTE 또는 비용

* 을 적용할 때 **사용자별 보기** 보기, 다음 열이 표시됩니다.

   * 사용 가능한 시간 또는 FTE
   * 계획된 시간 또는 FTE
   * 시간 또는 FTE 차이
   * 계획 시간 할당 퍼센트

>[!TIP]
>
>이 정보는 **사용자별 보기** 리소스 계획자 보기
>
>각 열에 표시되는 내용에 대한 자세한 내용을 보려면 숫자가 표시되는 열의 이름 위로 마우스를 가져갑니다.\
>![Net_hours_res_planner_mouse_over.png](assets/net-hours-res-planner-mouse-over-350x95.png)
>
>각 열에 표시되는 데이터에 대한 자세한 내용은 다음 문서를 참조하십시오.
>
>* [리소스 계획자의 프로젝트 및 역할 뷰의 시간, FTE 및 비용 정보 개요](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)
>* [사용자 뷰를 사용할 때 리소스 계획자에서 사용 가능한 시간, 계획 시간 또는 실제 시간 또는 FTE 보기](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)
>


## 시간, FTE 또는 원가별로 정보 보기

1. 리소스 플래너로 이동합니다.

   기본적으로 Resource Planner에 Hours로 정보가 표시됩니다.

1. 드롭다운 메뉴를 확장합니다.\
   ![Hours_fte_or_cost_dropdown.png](assets/hours-fte-or-cost-dropdown.png)

1. 다음 옵션 중에서 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">시간</td> 
      <td>가용성 및 할당 정보를 시간 단위로 표시합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">FTE</td> 
      <td> <p>FTE로 가용성 및 할당 정보를 표시합니다.</p> <p>Resource Planner에서 FTE를 계산하는 방법에 대한 자세한 내용은 <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">리소스 계획자에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">비용</td> 
      <td> <p>프로젝트 또는 역할 뷰에서 리소스 계획자를 보고 있는 경우 원가별로 가용성 및 할당 정보를 표시합니다. 정보는 시스템 통화로 값을 표시합니다. Workfront 관리자가 시스템 통화를 정의합니다. Workfront에서 시스템 통화 설정에 대한 자세한 내용은 <a href="../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">환율 설정</a>.</p> <p><b>메모</b>

   자원 계획자에 원가 정보를 표시하려면 사용자 및 작업 역할을 시간당 비용과 연관시켜야 합니다.<br style="font-style: italic;">시간당 비용을 Job 역할과 연관시키는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">작업 역할 만들기 및 관리</a>.<br style="font-style: italic;">시간당 비용과 사용자를 연관시키는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">사용자 프로필 편집</a>.<br style="font-style: italic;">Resource Planner에서 비용을 계산하는 방법에 대한 자세한 내용은 다음을 참조하십시오 <a href="../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md" class="MCXref xref">리소스 계획자에서 비용 계산 </a>.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">맞춤화</td> 
      <td>리소스 계획자에 표시되는 열의 사용자 정의 뷰를 생성합니다. 아래 단계에 설명된 대로 리소스 계획자에 표시할 옵션을 선택합니다. </td> 
     </tr> 
    </tbody> 
   </table>

1. (조건부) 선택한 경우 **사용자 지정**&#x200B;에서 옵션을 지정합니다. **표시된 지표 사용자 지정** 상자를 사용하여 사용자 지정 보기를 설정합니다.

   ![](assets/planner-customize-view-box-350x114.png)

1. 에서 **보기 유형** 왼쪽의 열에서 다음 보기 중 하나를 선택합니다.

   * 프로젝트
   * 역할
   * 사용자

1. 에서 **선택한 항목 표시** 섹션에서 선택한 뷰의 열에 표시할 정보 유형을 선택합니다. 다음 표는 각 보기에서 사용할 수 있는 옵션을 보여줍니다.

   | **옵션** | 사용자 조회 | 프로젝트 보기 | 역할 보기 |
   |---|---|---|---|
   | 사용 가능 | ✔ | ✔ | ✔ |
   | 계획됨 | ✔ | ✔ | ✔ |
   | 예산 |   | ✔ | ✔ |
   | 변량 |   | ✔ | ✔ |
   | 순 |   | ✔ | ✔ |
   | 실제 | ✔ |   |   |
   | 차이 | ✔ |   |   |
   | 백분율 | ✔ |   |   |

1. 선택 **NET 계산에서 계획(PLN) 값 사용** 프로젝트 및 역할 뷰에서 순 값을 계산할 때 예산책정 정보 대신 계획됨 을 사용할 수 있습니다.

   이 옵션을 선택하면 Workfront은 다음 공식을 사용하여 네트 값을 계산합니다.

   ```
   Net = Available - Planned
   ```

   >[!TIP]
   >
   >**이 옵션은 선택한 항목 표시 섹션에서 보기를 사용자 지정하는 하나 이상의 옵션을 선택한 경우에만 적용됩니다.**

1. **저장**&#x200B;을 클릭합니다.

   선택한 열을 포함하는 사용자 지정된 보기가 표시됩니다.

   리소스 계획자는 시간 드롭다운 메뉴에서 사용자 정의 뷰를 사용자 지정으로 나열합니다.

   >[!NOTE]
   >
   >사용자 지정된 보기는 하나만 사용할 수 있습니다.

   ![](assets/planner-hours-drop-down-with-custom-and-customize-option-183x281.png)

## 사용자 할당 차트 보기

사용자 가용성에 대한 사용자 계획 할당을 차트에 표시할 수 있습니다.

차트에 사용자 할당을 표시하려면 다음을 수행합니다.

1. 리소스 플래너로 이동합니다.

   리소스 계획자 액세스에 대한 자세한 내용은 [리소스 계획자 찾기](../../resource-mgmt/resource-planning/get-started-resource-planner.md#accessing-the-resource-planner) 문서의 섹션 [리소스 플래너 개요](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

1. 선택 **사용자별 보기**.

   >[!TIP]
   >
   >사용자 보기에서만 사용자 할당 차트를 볼 수 있습니다.

1. 을(를) 클릭합니다. **사용자 할당 차트** 아이콘 ![RP_user_allocation_chart.png](assets/rp-user-allocation-chart.png) 다음 정보를 표시하려면 다음을 수행하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">모든 사용자에 대해 초과 할당이 없는 가용성 %</td> 
      <td>이 시간은 사용 가능한 총 시간의 백분율로 표시되는 기간 동안 모든 사용자가 작업할 수 있는 시간입니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">모든 사용자의 초과 할당(%) </td> 
      <td> <p>사용자가 한 기간에 과다 할당되는 시간으로, 총 가용 시간의 백분율로 표시됩니다.</p> <p><b>메모</b>

   초과 할당은 계획 시간이 가용 시간보다 높을 때 발생합니다. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">모든 사용자의 과소 활용(%)</td> 
      <td> <p>이는 총 사용 가능한 시간의 백분율로 표시되는 기간 동안 사용자가 제대로 활용되지 않는 시간입니다.</p> <p><b>메모</b>

   가용 시간보다 계획 시간이 낮으면 활용률이 낮아집니다. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">이 기간 동안 최소 한 명의 사용자에게 초과 할당이 있습니다.</td> 
      <td>이는 해당 기간 동안 모든 사용자의 총 시간이 초과되지 않더라도 일정 기간 동안 하나 이상의 사용자에 대해 오버할당이 있음을 나타냅니다.<br>사용자 목록을 스크롤해야 하며, 초과 할당된 사용자의 시간은 빨간색으로 강조 표시됩니다.</td> 
     </tr> 
    </tbody> 
   </table>

   ![RP__user_allocation_chart_Dec._7__2017.png](assets/rp--user-allocation-chart-dec.-7--2017-350x148.png)

1. (선택 사항) **모든 사용자에 대한 초과 할당 %** 영역 내에 있습니다.\
   초과 할당된 모든 사용자는 빨간색으로 강조 표시됩니다.
1. (선택 사항) **모든 사용자에 대한 활용률 % 미만** 영역 내에 있습니다.\
   활용도가 낮은 모든 사용자는 파란색으로 강조 표시됩니다.

1. (선택 사항) 표시기 아이콘을 클릭합니다 ![one_user_overallocation_marker.png](assets/one-user-overallocation-marker.png) 사용자가 적어도 한 명 이상 과다 할당된 위치를 보여줍니다.\
   초과 할당된 사용자는 빨간색으로 강조 표시됩니다.

1. (선택 사항) 페이지를 새로 고쳐 차트를 축소합니다.
