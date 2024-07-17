---
product-area: resource-management
navigation-topic: resource-planning
title: 리소스 플래너에서 비용 계산
description: 시간 또는 FTE 값 대신 비용 값을 사용하여 Adobe Workfront 리소스 플래너에서 리소스의 예산을 책정할 수 있습니다. 리소스 플래너의 **사용자별 조회** 조회에는 원가 값을 사용할 수 없습니다.
author: Lisa
feature: Resource Management
exl-id: 2f3ca8c2-51b3-4282-af8b-7f433365d386
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '1458'
ht-degree: 0%

---

# 리소스 플래너에서 비용 계산

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)</p>
-->

<!--'(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)'-->

시간 또는 FTE 값 대신 비용 값을 사용하여 Adobe Workfront 리소스 플래너에서 리소스의 예산을 책정할 수 있습니다. 리소스 플래너의 **사용자별 보기** 보기에 대해 비용 값을 사용할 수 없습니다.

>[!IMPORTANT]
>
>리소스 플래너에 비용 정보를 표시하려면 사용자 및 작업 역할을 시간당 비용에 연결해야 합니다.\
>시간당 비용을 작업 역할과 연결하는 방법에 대한 자세한 내용은 [작업 역할 만들기 및 관리](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)를 참조하십시오.\
>시간당 비용을 사용자와 연결하는 방법에 대한 자세한 내용은 [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하십시오.

리소스 예산을 책정하기 전에 수행해야 할 작업(계획된 시간, FTE 또는 비용)과 사용자가 작업할 수 있는 시간(가용 시간, FTE 또는 비용)을 잘 이해해야 합니다.\
시간 또는 FTE별로 예산을 책정할 때 리소스 플래너의 정보를 이해하는 방법에 대한 자세한 내용은 리소스 플래너의 프로젝트 및 역할 보기에서 [시간, FTE 및 비용 정보 개요](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)를 참조하십시오.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>리소스 플래너에서 우선순위 및 예산 시간 편집에 대한 액세스 권한이 포함된 리소스 관리에 대한 액세스 편집</p> <p>재무 데이터, 프로젝트 및 사용자에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>재무 관리 기능으로 예산을 책정하려는 프로젝트에 대한 권한을 관리합니다.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 원가별 리소스 플래너에 정보 표시

기본적으로 리소스 플래너에는 가용성 및 할당 정보가 시간으로 표시됩니다.

리소스 플래너에 비용별 가용, 계획 및 예산 정보를 표시하려면

1. Adobe Workfront 오른쪽 상단의 **주 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭합니다.

1. **리소스 조달**&#x200B;을 클릭합니다.
1. 리소스 플래너로 이동합니다.
1. (조건부) **프로젝트별 보기** 또는 **역할별 보기**&#x200B;를 선택합니다.\
   기본적으로 **프로젝트별 보기**&#x200B;가 선택되어 있습니다.\
   할당 및 가용성 정보는 시간 단위로 표시됩니다.

1. **시간** 드롭다운 메뉴에서 **비용**&#x200B;을(를) 선택합니다.

   액세스 수준에 재무 데이터에 대한 액세스 권한이 없는 경우 이 옵션을 사용할 수 없습니다.\
   프로젝트가 시스템 통화와 다른 통화를 사용하는 경우 해당 프로젝트의 원가는 시스템 통화로 변환된 리소스 플래너에 표시됩니다. 시스템 관리자가 시스템 통화를 정의합니다.\
   Workfront 및 전환율로 시스템 통화를 설정하는 방법에 대한 자세한 내용은 [환율 설정](../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)을 참조하십시오.\
   ![costs_in_the_planner_with_no_budgeting.png](assets/costs-in-the-planner-with-no-budgeting-350x240.png)

## 리소스 플래너에서 사용 가능한 비용 계산

리소스 플래너에 사용 가능한 원가 값을 표시하려면 다음 항목이 있어야 합니다.

* 사용자 및 역할에 대한 시간당 비용 요금
* 사용자 가용성에 대한 정보.

  사용자 가용성에 대한 정보를 얻는 방법은 Workfront 관리자가 리소스 관리 기본 설정을 구성하는 방법에 따라 다릅니다.\
  사용자 가용성 계산 및 리소스 관리 환경 설정 지정에 대한 자세한 내용은 [리소스 관리 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)을 참조하십시오.

다음 테이블은 리소스 플래너에서 가용 비용이 계산되는 방법을 보여 줍니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>사용 가능한 비용</strong> </th> 
   <th><strong>계산</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>사용자 가용 비용</td> 
   <td> <p>사용자당 가용 비용은 다음 공식을 사용하여 계산됩니다.</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p><b>메모</b>

사용자가 프로필에 시간당 비용 비율이 없는 경우 나열된 작업 역할의 시간당 비용 비율이 계산에 사용됩니다. 사용자에게 연결된 역할이 없는 경우 사용 가능한 사용자 비용은 $0입니다. </p> </td>
</tr> 
  <tr> 
   <td>역할 사용 가능 비용</td> 
   <td> <p>역할당 가용 비용은 다음 공식을 사용하여 계산됩니다.</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p><b>메모</b>

역할에 시간당 비용이 없는 경우 사용 가능한 역할 비용은 $0입니다.</p> </td>
</tr> 
  <tr> 
   <td>프로젝트 가용 비용</td> 
   <td> <p>프로젝트당 가용 비용은 다음 공식을 사용하여 계산됩니다.</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## 리소스 플래너에서 계획된 비용 계산

리소스 플래너에서 작업 정보를 볼 수는 없지만 사용자, 역할 및 프로젝트에 대한 계획된 비용은 다음 작업 정보를 고려하여 계산됩니다.

* 작업에 대한 할당 유형입니다.\
  작업을 할당 해제한 상태로 두거나 작업에 다음 엔티티를 할당할 수 있습니다.

   * 사용자(작업 역할 포함 또는 제외)
   * 역할
   * 팀\
     리소스 플래너의 관점에서 팀에 할당된 작업은 할당 해제된 것으로 간주됩니다.

* 프로젝트에 있는 작업의 **비용 유형**.\
  작업의 비용 유형에 대한 자세한 내용은 [비용 추적](../../manage-work/projects/project-finances/track-costs.md)을 참조하십시오.

* 작업 역할 및 사용자에 대한 비용 요율의 유효 일자.

  예를 들어 역할 또는 사용자가 2월에 계획된 시간이 10시간이고 3월에 계획된 시간이 10시간이지만 원가율이 3월에 $12에서 $20로 변경된 경우 2월의 계획된 비용 값은 $120이고 3월의 계획된 비용 값은 $200입니다.

>[!NOTE]
>
>사용자 계획 원가는 프로젝트 계획 원가에 영향을 주지 않습니다. 역할 계획 비용만 리소스 플래너의 프로젝트 계획 비용에 영향을 줍니다.

사용자, 역할 및 프로젝트에 대한 계획된 비용을 계산할 때 다음과 같은 시나리오가 있습니다.

* **비용 유형**&#x200B;이(가) **사용자 시간별**이고 작업에 **할당이 없음**&#x200B;인 경우:

   * **역할 및 사용자 계획 비용**:

     역할 및 사용자 계획 비용은 $0.00입니다.

   * **프로젝트 계획 비용**:

     프로젝트 계획 비용은 $0.00입니다.

* **비용 유형**&#x200B;이(가) **시간별 사용자**&#x200B;이고 작업에 **사용자 할당**&#x200B;이 있는 경우:

   * **역할 및 사용자 계획 비용**:

     사용자 계획 원가는 다음 공식을 사용하여 계산됩니다.

     `User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate`

     사용자가 프로필에 원가율이 있는 경우 해당 원가율은 계획된 원가를 계산하는 데 사용됩니다. 그렇지 않으면 기본 역할의 시스템 수준 시간당 비용 비율이 사용됩니다.

     >[!NOTE]
     >
     >사용자는 보조 작업 역할 중 하나가 있는 작업에 할당할 수 있지만 여기서는 대신 기본 작업 역할의 비율이 사용됩니다.

     역할 계획 비용은 다음 공식을 사용하여 계산됩니다.

     `Role Planned Cost = SUM(User Planned Cost)`

   * **프로젝트 계획 비용**:

     프로젝트 계획 비용은 $0.00입니다.

* **비용 유형**&#x200B;이(가) **시간별 사용자**&#x200B;이고 작업에 **작업 역할 할당**&#x200B;이 있는 경우:

   * **역할 및 사용자 계획 비용**:

     사용자 계획 비용은 $0.00입니다.

     역할 계획 비용은 다음 공식을 사용하여 계산됩니다.

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     작업에 할당된 작업 역할의 시스템 수준 시간당 비용 비율을 사용하여 계획된 비용을 계산합니다.

   * **프로젝트 계획 비용**:

     프로젝트 계획 비용은 $0.00입니다.

* **비용 유형**&#x200B;이(가) **시간별 역할**&#x200B;이고 작업에 **할당이 없음**&#x200B;인 경우:

   * **역할 및 사용자 계획 비용**:

     역할 및 사용자 계획 비용은 $0.00입니다.

   * **프로젝트 계획 비용**:

     프로젝트 계획 비용은 $0.00입니다.

* **비용 유형**&#x200B;이(가) **시간별 역할**&#x200B;이고 작업에 **사용자 할당**&#x200B;이 있는 경우:

   * **역할 및 사용자 계획 비용**:

     사용자 계획 비용은 $0.00입니다.

     역할 계획 원가는 다음 공식에 의해 계산됩니다.

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Workfront은 사용자가 작업을 수행하는 작업 역할을 확인하여 역할에 대한 계획된 비용을 계산합니다.

     사용자가 작업에 대한 어떤 역할과도 연결되어 있지 않으면 계획된 비용은 $0.00입니다.

   * **프로젝트 계획 비용**:

     프로젝트 계획 원가는 다음 공식을 사용하여 계산됩니다.

     `Project Planned Cost = SUM(Role Planned Costs)`

* **비용 유형**&#x200B;이(가) **시간별 역할**&#x200B;이고 작업에 **작업 역할 할당**&#x200B;이 있는 경우:

   * **역할 및 사용자 계획 비용**:

     사용자 계획 비용은 $0.00입니다.

     역할 계획 원가는 다음 공식에 의해 계산됩니다.

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Workfront은 사용자가 작업을 수행하는 작업 역할을 확인하여 역할에 대한 계획된 비용을 계산합니다.

   * **프로젝트 계획 비용**:

     프로젝트 계획 원가는 다음 공식을 사용하여 계산됩니다.

     `Project Planned Cost = SUM(Role Planned Costs)`

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(table below ideal but drafted because it does not display correctly in Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<col>
<col>
<tbody>
<tr>
<td rowspan="2">&nbsp;</td>
<td colspan="3"> <p><strong>Cost Type = User Hourly</strong> </p><strong>User Planned Cost</strong> </td>
<td colspan="3"> <p><strong>Cost Type = Role Hourly</strong> </p><strong>Role Planned Cost</strong> </td>
</tr>
<tr>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>User and Role Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is calculated using the following formula: </p> <p><code> User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate </code> </p> <p> If a user has a cost rate in their profile, then that rate is used to calculate Planned Cost. Otherwise, the system-level Cost per Hour rate of their Primary Role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code>Role Planned Cost = SUM(User Planned Cost)</code> </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code> Role Planned Cost = Role Planned Hours * Role Cost per Hours </code> </p> <p> The system-level Cost per Hour rate of the job role assigned to the task is used to calculate Planned Cost. </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> If the user is not associated with any role on the task, the Planned Cost is $0.00. </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td rowspan="2"> <p><strong>Project Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td colspan="2"> <p> The Project Planned Cost is calculated using the following formula: </p> <p><code> Project Planned Cost = SUM(Role Planned Costs) </code> </p> <p> </p> </td>
</tr>
<tr>
<td colspan="6"> <note type="note">
User Planned Costs do not influence the Project Planned Cost. Only the Role Planned costs affect the Project Planned Costs, in the Resource Planner.
</note> </td>
</tr>
</tbody>
</table>
-->

## 리소스 플래너에서 예산 비용 계산

리소스 플래너에 예산 원가 값을 표시하려면 다음을 충족해야 합니다.

* 역할, 사용자 및 프로젝트에 대한 예산 시간.
* 사용자 및 역할에 대한 시간당 비용 요금.

>[!NOTE]
>
>프로젝트의 예산 시간은 사용자가 아닌 역할의 예산 시간을 기반으로 계산됩니다.

다음 테이블은 리소스 플래너에서 예산 비용이 계산되는 방법을 보여줍니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>예산 비용</strong> </th> 
   <th><strong>계산</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>사용자 예산 비용</td> 
   <td> <p>사용자당 예산 비용은 다음 공식을 사용하여 계산됩니다.</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p><b>메모</b>

프로필에 시간당 비용 비율이 없는 경우 예산 사용자 비용은 $0.00입니다.</p> </p> </td>
</tr> 
  <tr> 
   <td>역할 예산 비용</td> 
   <td> <p>역할 예산 원가는 다음 공식을 사용하여 계산됩니다.</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p><b>메모</b>

역할에 시간당 비용이 없는 경우 예산 역할 비용은 $0.00입니다.</p> </p> </td>
</tr> 
  <tr> 
   <td>프로젝트 예산 비용</td> 
   <td> <p>프로젝트당 예산 비용은 다음 공식을 사용하여 계산됩니다.</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
