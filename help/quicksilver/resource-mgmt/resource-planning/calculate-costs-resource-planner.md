---
product-area: resource-management
navigation-topic: resource-planning
title: 리소스 계획자에서 비용 계산
description: 시간 또는 FTE 값 대신 비용 값을 사용하여 Adobe Workfront Resource Planner에서 리소스를 예측할 수 있습니다. 원가 값은 리소스 플래너의 **사용자별 보기** 보기에 사용할 수 없습니다.
author: Lisa
feature: Resource Management
exl-id: 2f3ca8c2-51b3-4282-af8b-7f433365d386
source-git-commit: 61a107e1ee8a415fd94e73fc65fa5f59f7de02d1
workflow-type: tm+mt
source-wordcount: '1390'
ht-degree: 0%

---

# 리소스 계획자에서 비용 계산

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)</p>
-->

<!--'(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)'-->

시간 또는 FTE 값 대신 비용 값을 사용하여 Adobe Workfront Resource Planner에서 리소스를 예측할 수 있습니다. 비용 값은&#x200B;**사용자별 보기** 리소스 계획자에서 보기

>[!IMPORTANT]
>
>자원 계획자에 원가 정보를 표시하려면 사용자 및 작업 역할을 시간당 비용과 연관시켜야 합니다.\
>시간당 비용을 Job 역할과 연관시키는 방법에 대한 자세한 내용은 [작업 역할 만들기 및 관리](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
>시간당 비용과 사용자를 연관시키는 방법에 대한 자세한 내용은 [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

자원 예산을 책정하는 경우 먼저 어떤 작업을 수행해야 하는지(계획 시간, FTE 또는 비용) 및 사용자가 작업 시간(사용 가능한 시간, FTE 또는 비용)을 알 수 있습니다.\
시간 또는 FTE별로 예산을 책정할 때 리소스 계획자의 정보를 이해하는 방법에 대한 자세한 내용은 [리소스 계획자의 프로젝트 및 역할 뷰의 시간, FTE 및 비용 정보 개요](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

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
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>리소스 계획자의 우선순위 및 예산 시간 편집에 대한 액세스 권한을 포함하는 리소스 관리에 대한 액세스 편집</p> <p>재무 데이터, 프로젝트 및 사용자에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>재무 관리 기능을 사용하여 예산을 책정하려는 프로젝트에 대한 권한을 관리합니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 원가별 리소스 계획자에 정보 표시

기본적으로 가용성 및 할당 정보는 리소스 계획자의 시간 단위로 표시됩니다.

Resource Planner에서 비용별 가용 정보, 계획 정보 및 예산 정보를 표시하려면

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

1. 클릭 **리소스**.
1. 리소스 플래너로 이동합니다.
1. (조건부) 선택 **프로젝트별 보기** 또는 **역할별 보기**.\
   기본적으로 **프로젝트별 보기** 이 선택되어 있습니다.\
   할당 및 가용성 정보는 시간 단위로 표시됩니다.

1. 에서 **시간** 드롭다운 메뉴에서 **비용**.

   액세스 수준에서 재무 데이터에 액세스할 수 없는 경우 이 옵션을 사용할 수 없습니다.\
   프로젝트에 시스템 통화와 다른 통화가 있는 경우 이러한 프로젝트의 원가가 시스템의 통화로 변환된 리소스 계획자에 표시됩니다. 시스템 관리자가 시스템 통화를 정의합니다.\
   Workfront에서 시스템 통화 및 전환율 설정에 대한 자세한 내용은 다음을 참조하십시오 [환율 설정](../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).\
   ![cost_in_the_planner_with_no_budgeting.png](assets/costs-in-the-planner-with-no-budgeting-350x240.png)

## 리소스 계획자에서 사용 가능한 비용 계산

자원 계획자에 사용 가능한 원가 값을 표시하려면 다음 항목이 있어야 합니다.

* 사용자 및 역할에 대한 시간당 비용 비율
* 사용자 가용성에 대한 정보입니다.

   사용자 가용성에 대한 정보를 얻는 것은 Workfront 관리자가 리소스 관리 환경 설정을 구성하는 방법에 따라 다릅니다.\
   사용자 가용성 계산 및 자원 관리 환경설정 설정에 대한 자세한 내용은 [리소스 관리 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

다음 테이블은 리소스 계획자에서 사용 가능한 원가를 계산하는 방법을 보여줍니다.

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
   <td>사용 가능한 비용</td> 
   <td> <p>사용자당 사용 가능한 비용은 다음 공식을 사용하여 계산됩니다.</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p><b>메모</b>

사용자의 프로필에 시간당 비용이 없는 경우, 사용자가 나열된 작업 역할의 시간당 비용 비율이 계산에 사용됩니다. 사용자에게 연관된 역할이 없는 경우 사용 가능한 사용자 비용은 $0입니다. </p> </td>
</tr> 
  <tr> 
   <td>역할 사용 가능한 비용</td> 
   <td> <p>역할당 사용 가능한 비용은 다음 공식을 사용하여 계산됩니다.</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p><b>메모</b>

역할에 시간당 비용이 없는 경우 사용 가능한 역할 비용은 $0입니다.</p> </td>
</tr> 
  <tr> 
   <td>프로젝트 가용 비용</td> 
   <td> <p>프로젝트당 사용 가능한 비용은 다음 공식을 사용하여 계산됩니다.</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## 자원 계획자에서 계획 원가 계산

Resource Planner에서 작업 정보를 볼 수 없지만 다음 작업 정보를 고려하여 사용자, 역할 및 프로젝트에 대한 계획 비용을 계산합니다.

* 작업에 대한 할당 유형입니다.\
   작업을 할당되지 않은 상태로 두거나 다음 엔터티를 작업에 할당할 수 있습니다.

   * 사용자(작업 역할 포함 또는 없음)
   * 역할
   * 팀\
      Resource Planner의 관점에서 Team에 할당된 작업은 지정이 취소된 것으로 간주됩니다.

* 다음 **비용 유형** 프로젝트에 있는 작업의 수입니다.\
   작업의 비용 유형에 대한 자세한 내용은 [비용 추적](../../manage-work/projects/project-finances/track-costs.md).

>[!NOTE]
>
>사용자 계획 원가는 프로젝트 계획 원가에 영향을 주지 않습니다. 역할 계획 원가는 자원 계획자의 프로젝트 계획 원가에 영향을 줍니다.

사용자, 역할 및 프로젝트에 대한 계획 비용을 계산할 때 다음 시나리오가 존재합니다.

* 이 **비용 유형** **시간별 사용자 **이고 다음 항목이 있습니다 **할당 없음** 작업:

   * **역할 및 사용자 계획 비용**:

      역할 및 사용자 계획 비용은 0.00달러입니다.

   * **프로젝트 계획 원가**:

      프로젝트 계획 비용은 0.00달러입니다.

* 이 **비용 유형** is **시간별 사용자** 그리고 **사용자 지정** 작업:

   * **역할 및 사용자 계획 비용**:

      사용자 계획 원가는 다음 공식을 사용하여 계산됩니다.



      ```
      User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate
      ```

      사용자가 프로파일에 원가율이 있는 경우 그 비율을 사용하여 계획 원가를 계산합니다. 그렇지 않으면 기본 역할의 시스템 레벨 시간당 비용이 사용됩니다.

      >[!NOTE]
      >
      >사용자는 보조 작업 역할 중 하나를 사용하여 작업에 할당할 수 있지만 기본 작업 역할의 비율은 여기에서 대신 사용됩니다.

      역할 계획 원가는 다음 공식을 사용하여 계산됩니다.

      ```
      Role Planned Cost = SUM(User Planned Cost)
      ```

   * **프로젝트 계획 원가**:

      프로젝트 계획 비용은 0.00달러입니다.

* 이 **비용 유형** is **시간별 사용자** 그리고 **작업 역할 할당** 작업:

   * **역할 및 사용자 계획 비용**:

      사용자 계획 비용은 0.00달러입니다.

      역할 계획 원가는 다음 공식을 사용하여 계산됩니다.

      ```
      Role Planned Cost = Role Planned Hours * Role Cost per Hours
      ```

      작업에 지정된 작업 역할의 시스템 레벨 시간당 비용 비율은 계획 원가를 계산하는 데 사용됩니다.

   * **프로젝트 계획 원가**:

      프로젝트 계획 비용은 0.00달러입니다.

* 이 **비용 유형** is **시간별 역할** 그리고 **할당 없음** 작업:

   * **역할 및 사용자 계획 비용**:

      역할 및 사용자 계획 비용은 0.00달러입니다.

   * **프로젝트 계획 원가**:

      프로젝트 계획 비용은 0.00달러입니다.

* 이 **비용 유형** is **시간별 역할** 그리고 **사용자 지정** 작업:

   * **역할 및 사용자 계획 비용**:

      사용자 계획 비용은 0.00달러입니다.

      역할 계획 원가는 다음 공식으로 계산됩니다.

      ```
      Role Planned Cost = Role Planned Hours * Role Cost per Hours
      ```

      Workfront은 사용자가 작업에서 충족한 작업 역할을 보고 역할에 대한 계획 비용을 계산합니다.

      사용자가 작업의 역할과 연관되지 않은 경우 계획 비용은 $0.00입니다.

   * **프로젝트 계획 원가**:

      프로젝트 계획 원가는 다음 공식을 사용하여 계산됩니다.

      ```
      Project Planned Cost = SUM(Role Planned Costs)
      ```

* 이 **비용 유형** is **시간별 역할** 그리고 **작업 역할 할당** 작업:

   * **역할 및 사용자 계획 비용**:

      사용자 계획 비용은 0.00달러입니다.

      역할 계획 원가는 다음 공식으로 계산됩니다.

      ```
      Role Planned Cost = Role Planned Hours * Role Cost per Hours
      ```

      Workfront은 사용자가 작업에서 충족한 작업 역할을 보고 역할에 대한 계획 비용을 계산합니다.

   * **프로젝트 계획 원가**:

      프로젝트 계획 원가는 다음 공식을 사용하여 계산됩니다.

      ```
      Project Planned Cost = SUM(Role Planned Costs)
      ```

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

## 자원 계획자에서 예산 비용 계산

Resource Planner에 예산책정된 원가 값을 표시하려면 다음 항목이 있어야 합니다.

* 역할, 사용자 및 프로젝트에 대한 예산책정 시간
* 사용자 및 역할에 대한 시간당 비용

>[!NOTE]
>
>프로젝트에 대한 예산책정된 시간은 사용자가 아닌 역할에 대한 예산책정된 시간을 기준으로 계산됩니다.

다음 테이블은 Resource Planner에서 예산책정된 원가를 계산하는 방법을 보여줍니다.

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
   <td>사용자 예산책정된 비용</td> 
   <td> <p>사용자당 예산책정된 비용은 다음 공식을 사용하여 계산됩니다.</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p><b>메모</b>

사용자의 프로필에 시간당 비용이 없는 경우 예산책정된 사용자 비용은 $0.00입니다.</p> </p> </td>
</tr> 
  <tr> 
   <td>역할 예산 비용</td> 
   <td> <p>역할 예산 원가는 다음 공식을 사용하여 계산됩니다.</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p><b>메모</b>

롤에 시간당 비용이 없는 경우 예산책정된 역할 비용은 0.00달러입니다.</p> </p> </td>
</tr> 
  <tr> 
   <td>프로젝트 예산 비용</td> 
   <td> <p>프로젝트당 예산책정된 비용은 다음 공식을 사용하여 계산됩니다.</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
