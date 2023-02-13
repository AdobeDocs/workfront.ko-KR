---
content-type: reference
product-area: resource-management;user-management
navigation-topic: resource-planning
title: 사용자 뷰를 사용할 때 리소스 계획자에서 사용 가능한 시간, 계획 시간 또는 실제 시간 또는 FTE 보기
description: RP에서 User viewPlanning을 사용할 때 Resource Planner에서 사용 가능한 시간, 계획 시간 또는 실제 시간 또는 FTE를 봅니다. - "RP에서 예산 리소스" 또는 "RP에서 자원 관리" 기타.. - 또는 다른 POV에서 다시 생성해야 할 수 있습니다?!)"
author: Alina
feature: Resource Management
exl-id: 6b532aa2-435f-4fda-b7ce-abe0a785638f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1738'
ht-degree: 1%

---

# 사용자 뷰를 사용할 때 리소스 계획자에서 사용 가능한 시간, 계획 시간 또는 실제 시간 또는 FTE 보기

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Consider renaming this article (probably split already) to something other than "Planning" in the RP" - maybe "budgeting resources in the RP" or "Managing Resources in the RP." etc... - or might need to be repurposed from another POV?!)</p>
-->

프로젝트 및 역할 뷰에서 예산 책정 리소스 외에도 Adobe Workfront 리소스 계획자의 사용자 뷰를 사용하여 프로젝트 및 자원에 대한 계획, 사용 가능 및 실제 시간 또는 FTE 값에 대한 정보를 표시할 수 있습니다.

## 리소스 계획자의 사용자 뷰 개요

리소스 계획자에서 시간 또는 FTE 정보를 볼 때 다음 사항을 고려하십시오.

* Resource Planner의 모든 뷰에서 사용자, Job 역할 및 프로젝트에 대한 사용 가능 시간 및 계획 시간 또는 FTE 정보를 볼 수 있습니다.
* 사용자 보기에서만 다음 정보를 볼 수 있습니다.

   * 계획 시간 또는 FTE의 양과 사용 가능한 시간 또는 FTE의 양 간의 차이입니다. 그런 다음 프로젝트 및 역할 보기의 이 차이에 따라 사용자 할당 예산을 지정할 수 있습니다.
   * 실제 시간 또는 FTE입니다.

* 사용 가능한 사용자와 계획 시간 또는 FTE의 금액 차이를 사용자 뷰에서 숫자 또는 백분율 값으로 표시할 수 있습니다.
* 비용별로 사용자 보기에 정보를 표시할 수 없습니다.
* Adobe Workfront은 해당 스케줄의 사용자와 연관된 작업 시간에 따라 사용 가능한 시간 또는 FTE를 채웁니다.\
   예약과 연관되지 않은 사용자는 기본 스케줄에 따라 가용성을 표시합니다.\
   기본 스케줄에 대한 자세한 내용은 [예약 만들기](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Workfront은 프로젝트의 작업 및 문제에 대한 계획 시간 정보에서 계획 시간 또는 FTE를 채웁니다.
* Workfront은 실제 시간을 작업에 할당된 사용자에 의해 작업 및 문제에 로그된 실제 시간으로 채웁니다. 여기에는 프로젝트에서 로그온한 시간이 포함됩니다.
* 사용자 보기에서 다음을 수행할 수 있습니다.

   * 각 사용자를 확장하여 해당 사용자가 지정된 프로젝트 목록을 표시합니다.

      >[!NOTE]
      >
      >필터에 포함된 프로젝트와 연결된 사용자만 확장할 수 있습니다.

   * 모든 프로젝트를 확장하여 해당 프로젝트에서 사용자가 수행할 수 있는 작업 역할 목록을 표시합니다.
   * 각 역할을 확장하여 해당 역할의 사용자가 할당받은 작업 목록을 표시합니다.

   사용자에게 연관된 Job 역할이 없는 경우 사용 가능, 계획 및 실제 시간 또는 FTE는 **역할 없음** 섹션을 참조하십시오.\
   리소스 계획자에 사용자 보기를 적용할 때 표시되는 필드 및 항목에 대한 자세한 내용은 [리소스 플래너 탐색 개요](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## 리소스 계획자의 사용자 뷰에 표시되는 필드 개요

리소스 계획자의 사용자 뷰에 표시되는 정보를 이해하려면 다음 테이블을 참조하십시오. 정보는 시간 또는 FTE 값으로 표시됩니다.

* [AVL(사용 가능) 열](#the-avl-available-column)
* [PLN(계획됨) 열](#the-pln-planned-column)
* [ACT (실제) 열](#The%C2%A0ACT)
* [DIF(차이점) 열](#the-dif-difference-column)
* [%(계획 시간 할당 퍼센트) 열](#the-planned-hours-allocation-percentage-column)

### AVL(사용 가능) 열 {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>표시 기준</strong> </td> 
   <td> <p><strong>설명</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>사용자</td> 
   <td>예약에 따른 사용자의 총 가용 시간 또는 FTE </td> 
  </tr> 
  <tr> 
   <td>프로젝트</td> 
   <td>이 정보는 리소스 계획자에 사용자 뷰를 적용할 때 프로젝트에 사용할 수 없습니다. </td> 
  </tr> 
  <tr> 
   <td>역할</td> 
   <td> <p>사용자 일정 및 사용자 스케줄에 따라 역할에 대한 사용 가능한 시간 또는 FTE의 총 합계 <strong>FTE 가용성 비율</strong> 역할.</p> </td> 
  </tr> 
  <tr> 
   <td>작업 또는 문제</td> 
   <td>이 정보는 작업 또는 문제에 사용할 수 없습니다. </td> 
  </tr> 
 </tbody> 
</table>

사용자 일정 및 역할의 FTE 가용성 비율을 기반으로 사용자 및 역할 가용성을 계산하는 방법에 대한 자세한 내용은 [리소스 계획자에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

### PLN(계획됨) 열 {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>표시 기준</strong> </td> 
   <td> <p><strong>설명</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>사용자</td> 
   <td> 모든 프로젝트에서 사용자에게 할당된 모든 작업 또는 문제로부터 계획된 시간 또는 FTE의 총 수입니다.<br><p>여기에는 사용자에게 지정되지만 작업 역할 및 작업과 연관되지 않은 작업 및 문제가 포함되며, 이 작업은 사용자가 관리 액세스 권한이 있는 프로젝트에 없습니다.</p><p>작업 로드 밸런서를 사용하여 시간 동안의 사용자 할당이 수정된 경우 선택한 날짜에 작업이나 문제의 일부만 포함되어 있으면 리소스 플래너의 데이터에 영향을 줄 수 있습니다. 사용자의 할당 수정에 대한 자세한 내용은 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">작업 로드 밸런서에서 사용자 할당 관리</a> . </p></td> 
  </tr> 
  <tr> 
   <td>프로젝트</td> 
   <td> 프로젝트의 특정 사용자에게 할당된 모든 작업 및 문제로부터 계획된 시간 또는 FTE의 총 수입니다.<br><p>참고: 작업이나 사용자에게 할당되지 않은 문제에 대해 계획된 시간이나 FTE가 포함되지 않습니다. </p></td> 
  </tr> 
  <tr> 
   <td>역할</td> 
   <td> <p>프로젝트에서 이 역할에서 사용자에게 할당된 모든 작업 및 문제로부터 계획된 시간 또는 FTE의 총 수입니다.</p> <p> <p>참고: 이 역할에는 이 역할에 지정되지만 이 사용자에게는 할당되지 않은 작업 또는 문제에 계획된 시간이나 FTE가 포함되지 않습니다. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>작업 또는 문제</td> 
   <td>작업 또는 프로젝트 문제와 연관된 예정 시간 또는 FTE입니다.</td> 
  </tr> 
 </tbody> 
</table>

계획 시간을 볼 때 다음 사항을 고려하십시오.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view)</p>
-->

* 계획 시간은 지정된 각 리소스에 대해 작업 및 문제 기간 내의 각 날에 균등하게 분배됩니다. 태스크 또는 출고 기간은 계획 시작 및 완료 일자를 기반으로 하며 해당 기간 내의 모든 달력 일자를 포함합니다.\
   Workfront은 사용자 또는 프로젝트에 계획 시간을 배포할 때 사용자 또는 프로젝트의 일정을 고려합니다. 이 경우 계획 시간은 주말, 휴가 일수 및 스케줄 예외를 제외한 태스크 또는 문제의 기간 내에 각 날에 균등하게 분배됩니다.

   예를 들어, 주별 리소스 계획자를 표시하고 프로젝트에서 여러 주에 걸쳐 있는 작업이 있는 경우, 주 단위 계획 시간 수는 해당 주 내의 일 수가 태스크 지속 기간의 일부인 기간에 따라 달라집니다. 이 기능은 월 또는 분기별로 리소스 계획자를 표시할 때와 작업이 여러 달 또는 분기에 걸쳐 있을 때 비슷하게 작동합니다.\
   주말 일, 예약 예외 및 휴가 일은 이 배포에서 제외됩니다.

* 각 자원에 대한 계획 시간 계산에는 다음 태스크 범주가 포함됩니다.

   * 프로젝트의 리소스 풀, 작업 역할 또는 팀에서 사용자에게 할당된 작업입니다.

      >[!TIP]
      >
      >작업이 팀에 할당되면 해당 할당이 **역할 없음** 및 **사용자 없음** 섹션에 자세히 설명되어 있습니다. 팀과 연관된 계획 시간 을 볼 수 있지만 작업과 연관된 역할이나 사용자가 없으므로 시간을 계산할 수 없습니다.

* 자원 계획자의 계획 시간은 다음과 연관된 계획 시간을 포함하지 않습니다.

   * 상위 작업
   * 할당되지 않은 작업
   * 문제, **문제 발생 시간 포함** 설정이 비활성화되어 있습니다.

* 작업 또는 발행 기간이 0인 경우 계획 시간이 자원 계획자에 표시되지 않습니다.
* 비활성화된 사용자와 연결된 계획된 시간이 표시되지 않습니다.

리소스 계획자의 계획 시간 및 FTE에 대한 자세한 내용은 다음을 참조하십시오 [리소스 계획자의 프로젝트 및 역할 뷰의 시간, FTE 및 비용 정보 개요](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

### ACT (실제) 열

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>표시 기준</strong> </td> 
   <td> <p><strong>설명</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>사용자 </td> 
   <td> <p>사용자에게 할당된 모든 작업 또는 문제에 대해 사용자가 로그한 시간입니다.</p> <p>여기에는 다음 항목이 포함되어 있습니다.</p> 
    <ul> 
     <li>사용자에게 지정되지만 작업 역할과 연관되지 않은 작업 및 문제</li> 
     <li>관리 액세스 권한이 있는 프로젝트에 없는 작업 및 문제 </li> 
    </ul> <p>여기에는 사용자가 해당 프로젝트의 작업 또는 문제에 지정되는 경우에만 프로젝트에 로그온한 시간이 포함됩니다.  </p> </td> 
  </tr> 
  <tr> 
   <td>프로젝트 </td> 
   <td> <p>프로젝트에서 사용자에게 할당된 모든 작업 및 문제에 대해 사용자가 로그한 시간입니다.</p> <p>여기에는 프로젝트에 직접 로그인한 시간이 포함됩니다.</p> <p>여기에는 다음 내용이 포함되지 않습니다.</p> 
    <ul> 
     <li> <p>사용자에게 할당되지 않은 작업 및 문제에 로그온한 시간입니다. </p> </li> 
     <li> <p>상위 작업에 로그온한 시간입니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>역할</td> 
   <td> <p>이 역할에서 사용자에게 할당된 모든 작업 또는 문제에 대해 로그된 시간입니다. </p> <p>여기에는 다음 내용이 포함되지 않습니다.</p> 
    <ul> 
     <li>이 역할에 지정된 작업 및 문제에 로그온한 시간입니다. 이 사용자에게는 할당되지 않습니다.</li> 
     <li>프로젝트 또는 상위 작업에 직접 로그온한 시간입니다. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>작업 또는 문제 </td> 
   <td> <p>또한 사용자에게 할당된 사용자가 작업에 로그온한 시간 및 문제입니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>로그된 시간은 시간이 기록되는 작업, 문제 또는 프로젝트의 기간에 관계없이 시간 항목의 시작 날짜에 해당하는 시간대에 표시됩니다.

실제 시간에 대한 자세한 내용은 [실제 시간 보기](../../manage-work/tasks/task-information/actual-hours.md).

### DIF(차이점) 열 {#the-dif-difference-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>표시 기준</strong> </td> 
   <td> <p><strong>설명</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>사용자</td> 
   <td> <p>사용자의 사용 가능 시간 및 예정 시간 또는 FTE 간의 차이입니다. </p> <p>시간 또는 FTE 차이는 다음 공식을 사용하여 계산됩니다.</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <p>참고: 값이 음수 빨간색 수로 표시되면 사용자가 초과 할당됩니다. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>프로젝트</td> 
   <td>이 정보는 프로젝트에 사용할 수 없습니다. </td> 
  </tr> 
  <tr> 
   <td>역할</td> 
   <td> <p>Job 역할의 사용 가능 시간 및 예정 시간 또는 FTE 간의 차이입니다. </p> <p>시간 또는 FTE 차이는 다음 공식을 사용하여 계산됩니다.</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <p>참고: 값이 음수 빨간색 숫자로 표시되면 역할이 오버할당됩니다. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>작업 또는 문제</td> 
   <td>이 정보는 작업, 문제 또는 프로젝트에 사용할 수 없습니다. </td> 
  </tr> 
 </tbody> 
</table>

### %(계획 시간 할당 퍼센트) 열 {#the-planned-hours-allocation-percentage-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>표시 기준</strong> </td> 
   <td> <p><strong>설명</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>사용자</td> 
   <td> <p>사용 가능한 시간의 백분율로 계획된 시간 또는 FTE의 할당. 계획 시간 할당의 백분율은 다음 공식을 사용하여 계산됩니다.</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>FTE 값에도 동일한 계산이 사용됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td>프로젝트</td> 
   <td>이 정보는 프로젝트를 적용할 때 사용할 수 없습니다 <strong>사용자별 보기</strong> 리소스 계획자 보기</td> 
  </tr> 
  <tr> 
   <td>역할</td> 
   <td> 사용 가능한 시간의 백분율로 계획된 시간 또는 FTE의 할당. <p>계획 시간 할당의 백분율은 다음 공식을 사용하여 계산됩니다.</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>FTE 값에도 동일한 계산이 사용됩니다.</p></td> 
  </tr> 
  <tr> 
   <td>작업 또는 문제</td> 
   <td>이 정보는 작업, 문제 또는 프로젝트에 사용할 수 없습니다. </td> 
  </tr> 
 </tbody> 
</table>

계획 시간 또는 FTE의 값이 0인 경우 백분율 할당은 0%입니다. 사용 가능한 시간 또는 FTE 값이 0인 경우 백분율 할당을 계산할 수 없습니다.

계획 시간 및 FTE와 리소스 계획자에 표시되는 방법에 대한 자세한 내용은 [프로젝트 및 역할 보기를 사용하는 자원 계획자의 예산 자원](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this table is ideal but it does not render in Markdown) </p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours or FTE)</strong> </td>
<td><strong>Displayed By</strong> </td>
<td> <p><strong>Description</strong> </p> </td>
</tr>
<tr>
<td rowspan="5">AVL <br>(Available Hours or FTE)</td>
<td>User</td>
<td>The total of Available Hours or FTE for the user according to their schedule. </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the User view to the Resource Planner. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Available Hours or FTE for the role according to the schedule of the user and the <strong>Percentage of FTE Availability</strong> of the role.</p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project.</td>
</tr>
<tr>
<td colspan="2"> <p colspan="2">For more information about how user and role availability is calculated based on the schedule of the user and the Percentage of FTE Availability of the role, see <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">PLN <br>(Planned Hours or FTE)</td>
<td>User</td>
<td> The total of Planned Hours or FTE from all the tasks or issues assigned to the user on all the projects.<br><p>This includes tasks and issues that are assigned to the user but not associated with any job role and tasks or issues that are not on projects that you have access to Manage.</p><p>When the user allocation for hours has been modified using the Workload Balancer, the data in the Resource Planner can be affected if the dates selected contain only a portion of a task or issue. For information about modifying allocations for users, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a> . </p></td>
</tr>
<tr>
<td>Project</td>
<td> The total of Planned Hours or FTE from all the tasks and issues assigned to a specific user on the project.<br><note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are not assigned to any users.
</note></td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Planned Hours or FTE from all the tasks and issues assigned to the user in this role on the project.</p> <p> <note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are assigned to this role but not to this user in this role.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>The Planned Hours or FTE associated with the task or the issue on the project.</td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view))</p>
<ul>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks and issues , for each resource assigned to them. The task or issue Duration is based on their Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks or issues excluding weekends, time-off days, and schedule exceptions.</p> <p>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> <p>The following categories of tasks are included in calculating the Planned Hours for each resource: </p>
<ul>
<li> <p> tasks assigned to users in Resource Pools, job roles, or teams on the project.</p> <note type="tip">
If tasks are assigned to teams, their allocation will appear under
<strong>No Role</strong> and
<strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks.
</note> </li>
</ul> </li>
</ul>
<ul>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>unassigned tasks</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task or issue Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> <p>For more information about Planned Hours and FTE in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">ACT<br>(Actual Hours or FTE) </td>
<td>User </td>
<td> <p>The time logged by the user on all the tasks or issues assigned to them.</p> <p>This includes the following:</p>
<ul>
<li>Tasks and issues that are assigned to the user but not associated with any job role.</li>
<li>Tasks and issues that are not on projects for which you have access to Manage.. </li>
</ul> <p>This does not include time logged directly on the project or on parent tasks. </p> </td>
</tr>
<tr>
<td>Project </td>
<td> <p>The time logged by the user on all the tasks and issues assigned to them on the project.</p> <p>This includes any time that they logged directly on the project.</p> <p>This does not include the following:</p>
<ul>
<li> <p>Time logged on tasks and issues that are not assigned to any users. </p> </li>
<li> <p>Time logged on parent tasks. </p> </li>
</ul> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The time logged on all the tasks or issues assigned to the user in this role. </p> <p>This does not include the following:</p>
<ul>
<li>Time logged on tasks and issues assigned to this role but not to this user in this role.<em> </em></li>
<li>Time logged directly on the project or parent tasks. </li>
</ul> </td>
</tr>
<tr>
<td>Task or Issue </td>
<td> <p>The time logged on tasks and issues by the user who is also assigned to them. </p> </td>
</tr>
<tr>
<td colspan="2"> <p> <note type="important">
The time logged is displayed in the timeframe corresponding to the Entry Date of the hour entry, regardless of the timeframe of the task, issue, or project where the hours are logged.
</note> </p> <p>For more information about Actual Hours, see <a href="../../manage-work/tasks/task-information/actual-hours.md" class="MCXref xref">View Actual Hours</a></p> </td>
</tr>
<tr>
<td rowspan="4">DIF <br>(Hour or FTE Difference) <br><br></td>
<td>User</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the user. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <note type="note">
If the value displays in negative red numbers, the user is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the job role. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <note type="note">
If the value is displayed in negative red numbers, the role is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td rowspan="5">Planned Hours or FTE Allocation Percentage (%)</td>
<td>User</td>
<td> <p>The allocation of the Planned Hours or FTE as a percentage of the Available Hours. The percentage of the Planned Hours Allocation is calculated using the following formula:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>The same calculation is used for FTE values. </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the <strong>View by User</strong> view to the Resource Planner.</td>
</tr>
<tr>
<td>Role</td>
<td> The allocation of the Planned Hours or FTE as a percentage of the Available Hours. <p>The percentage of the Planned Hours Allocation is calculated using the following formula:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>The same calculation is used for FTE values.</p></td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td colspan="2"> <p> If the value of the Planned Hours or FTE is zero, the Percentage Allocation is 0%. If the value of the Available Hours or FTE is zero, the Percentage Allocation cannot be calculated. </p> <p>For more information about Planned Hours and FTE and how they are displayed in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> </td>
</tr>
</tbody>
</table>
-->
