---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 사용자 프로필 일괄 편집
description: Adobe Workfront 관리자는 사용자 계정을 일괄적으로 편집할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: 5433008d93e99d69f8116e222bfce02411b77825
workflow-type: tm+mt
source-wordcount: '2194'
ht-degree: 0%

---

# 사용자 프로필 일괄 편집

<!--drafted for Work Time field: 
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

In the table below, under Resource Planning, add the "Work Time" field and update the "FTE" field:

<b><span class="preview">Work Time</span></b>: <span class="preview">Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.</span> 

<span class="preview">The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work.</span>  

<span class="preview">The system uses this number to calculate the availability of the user for actual, project-related work.</span> 

<span class="preview">For more information about creating schedules in Workfront, see Create a schedule.</span>

<span class="preview">Schedule exceptions and time off might also affect the user capacity. 

Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see Configure Resource Management preferences. (*****INSERT LINK****)


***UPDATED FTE FIELD***

FTE: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. The FTE indicates the amount of time that the user can spend at work. This includes overhead, and  time that is not spent on project work, but on other type of work. For example, time that is spent in meetings, or training is also included in the FTE. 

The FTE must be a decimal number up to 1, and it cannot be 0. 
The field's default is 1.

For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

Schedule exceptions, time off might, <span class="preview">and the value of Work Time</span> may affect the amount of available hours or the FTE. 

Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see Configure Resource Management preferences. (*****INSERT LINK****)

If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

For more information about creating schedules in Workfront, see Create a schedule. (*****INSERT LINK*****)
-->

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 Admin Console에 아직 온보딩되지 않은 조직에만 적용됩니다. 조직이 Adobe Admin Console에 온보딩된 경우 Adobe Admin Console을 통해 이 작업을 수행해야 합니다.
>
>Adobe Admin Console에서 사용자 프로필 편집에 대한 지침은 문서에서 &quot;사용자 세부 사항 편집&quot; 섹션을 참조하십시오 [사용자 일괄 업로드](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) 또는 Adobe Admin Console 관리자에게 문의하십시오.
>
>조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 다른 절차 목록은 [플랫폼 기반의 관리 차이점(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

사용자 계정을 일괄적으로 편집할 수 있습니다. 사용자를 벌크 편집할 때 특별히 선택하는 필드만 선택한 모든 사용자에 대해 동일한 정보로 업데이트됩니다. 선택하지 않은 다른 모든 필드는 각 사용자에 대해 다르더라도 각 개별 사용자에 대해 동일하게 유지됩니다.

>[!NOTE]
>
>* 사용자 프로필의 개인 정보 섹션은 모든 사용자에 대해 고유해야 하므로 벌크로 편집할 수 없습니다.
>* 데이터의 정확성과 최적의 성능을 보장하기 위해 벌크 편집을 위해 한 번에 2000명 이하의 사용자를 선택하는 것이 좋습니다.
>


## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>다음 중 하나가 있어야 합니다.</p> 
    <ul> 
     <li> <p>시스템 관리자 액세스 수준입니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>. </p> </li> 
     <li> <p><b>사용자</b> 액세스 수준에서 설정 <b>편집</b> 액세스, 사용 <b>만들기</b> 둘 중 적어도 하나 <b>사용자 관리자</b> 옵션 사용 <b>설정 세부 조정</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>이 두 옵션 중 사용자가 <b>관리자(그룹 사용자)</b> 이 활성화되어 있으면 사용자가 구성원인 그룹의 그룹 관리자여야 합니다.</p> <p>에 대한 자세한 정보 <b>사용자</b> 액세스 수준에서 설정하는 방법은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자 계정 일괄 편집

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **사용자** ![](assets/users-icon-in-main-menu.png).

1. 두 명 이상의 사용자를 선택한 다음 편집 아이콘을 클릭합니다 ![](assets/edit-icon.png).

1. 에서 **사용자 편집** 표시되는 상자에서 다음 옵션 중 하나를 변경합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">환경 설정</td> 
      <td> 
       <ul> 
        <li><b>시간대:</b> 사용자의 시간대입니다.</li> 
        <li><b>로케일</b>: 사용자의 기본 로케일입니다. Workfront에서 오는 이메일의 숫자 및 날짜 형식에 영향을 줍니다.</li> 
        <li><b>업데이트 상태에 완료 비율 표시</b>: 모든 사용자에 대한 작업 업데이트 스트림 내에 전체 백분율 표시줄을 표시하려면 이 옵션을 선택합니다.</li> 
        <li><b>내 작업 중 탭에 할당하는 작업 보내기</b>: 사용자가 자신에게 할당한 모든 것을 작업 중 탭에 직접 표시하려면 이 옵션을 선택합니다. 기본값은 작업 요청 탭에서 사용자에게 할당된 모든 항목을 나열하는 것입니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">알림</td> 
      <td>새 사용자에 대해 활성화해야 하는 이메일 알림을 선택합니다.<p>일별 다이제스트 알림뿐만 아니라 인스턴트 항목을 선택할 수 있습니다. 모든 일별 다이제스트 알림은 선택한 모든 사용자에 대해 동일한 시간 후 전달됩니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">시스템의 모든 사용자에 대한 이벤트 알림을 구성합니다</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">액세스</td> 
      <td> 
       <ul> 
        <li><b>활성 상태:</b> 사용자가 활성 상태인지 여부를 표시하려면 이 필드를 선택합니다. 활성 사용자는 Workfront 라이센스를 사용합니다. 필드를 선택 해제하면 사용자가 비활성화됩니다.</li> 
        <li> 
        <p><b>액세스 수준:</b> 이러한 사용자에게 할당할 액세스 수준을 선택합니다. 선택한 모든 사용자의 액세스 수준이 동일합니다.
        </p> 
        <p>사용자에게 액세스 수준을 할당할 때, 사용자 자신의 액세스 수준 이하로 수준을 지정할 수 있습니다. 예를 들어, 액세스 레벨이 계획자이면 관리자 액세스 레벨을 지정할 수 없습니다. </p>
        <p>그러나 Workfront 관리자가 사용자 자신에서도 활성화되지 않은 액세스 수준에서(에 설명된 대로 세부 조정 설정을 통해) 권한을 활성화한 경우 사용자 것보다 낮은 액세스 수준을 할당할 수 없습니다 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>).</p> 
        <p>액세스 수준에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Adobe Workfront에 대한 액세스 구성</a>.</p> 
         </li> 
        <li> 
        <p><b>레이아웃 템플릿</b>: 사용자의 레이아웃 템플릿을 선택합니다. 사용자에게 할당된 레이아웃 템플릿이 홈 그룹, 홈 팀 또는 기본 작업 역할에 할당된 레이아웃 템플릿보다 우선합니다. 레이아웃 템플릿의 할당 우선 순위에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">레이아웃 템플릿 만들기 및 관리</a>.</p> 
        <p><b>참고</b>: 이 필드에서 사용할 수 있는 레이아웃 템플릿 목록은 액세스 권한에 따라 다릅니다.
          <ul>
           <li>Workfront 관리자는 모든 시스템 수준 및 그룹 수준 레이아웃 템플릿을 볼 수 있습니다.</li>
           <li>그룹 관리자는 시스템 수준 레이아웃 템플릿과 관리하는 그룹과 연관된 템플릿을 볼 수 있습니다.</li>
           <li><p>계획자 라이센스와 사용자 편집에 대한 액세스 권한이 있는 사용자는 시스템 수준 레이아웃 템플릿만 볼 수 있습니다. </p>
           <p>그룹 수준 레이아웃 템플릿에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">레이아웃 템플릿 만들기 및 관리</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">조직</td> 
      <td> 
       <ul> 
        <li><b>회사</b>: 사용자의 회사입니다. 사용자는 한 회사에만 연결할 수 있습니다. 회사와 사용자를 연결하려면 먼저 회사를 만들어야 합니다. 활성 회사만 목록에 표시됩니다. 회사 생성에 대한 자세한 내용은 회사 이해 및 관리를 참조하십시오.</li> 
        <li><b>홈 팀</b>: 사용자의 홈 팀을 지정합니다. 사용자는 하나의 홈 팀만 가질 수 있습니다. </li> 
        <li><b>기타 팀</b>: 사용자는 여러 팀에 속할 수 있습니다. </li> 
        <li> <p><b>홈 그룹:</b> 사용자를 홈 그룹으로 지정하려면 적절한 그룹을 선택합니다. 따라서 사용자는 그룹과 공유되는 객체에 액세스할 수 있습니다.</p> <p><b>참고</b>: 필수 필드입니다. 홈 그룹과 연결되지 않은 사용자는 가질 수 없습니다.</p> <p>그룹을 다음과 같은 경우에만 사용자에게 할당할 수 있습니다.</p> 
         <ul> 
          <li>Workfront 관리자입니다.</li> 
          <li>해당 그룹의 관리자입니다.</li> 
          <li>이 그룹은 공개적입니다.</li> 
         </ul> </li> 
        <li> <p><b>기타 그룹</b>: 사용자는 여러 그룹에 속할 수 있습니다. 다음과 같은 경우에만 그룹에 사용자를 할당할 수 있습니다.</p> 
         <ul> 
          <li>Workfront 관리자입니다.</li> 
          <li>해당 그룹의 관리자입니다.</li> 
          <li> <p>이 그룹은 공개적입니다. </p> 
          <p>공용 그룹에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">그룹 만들기</a>.</p> 
          <p>그룹에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">그룹 개요</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">리소스 계획 수립</td> 
      <td> 
       <ul> 
        <li><b>비활성화 예약</b>: 일정 기간 후에 사용자를 비활성화하도록 예약하려면 이 확인란을 선택합니다.</li> 
        <li><b>예약된 비활성화 날짜</b>: 사용자가 비활성화된 날짜입니다. 사용자 비활성화 예약에 대한 자세한 내용은 섹션을 참조하십시오 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">사용자 비활성화 예약</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">사용자 비활성화 또는 다시 활성화</a>.</li> 
        <li> <p><b>기본 역할</b>: Workfront에서 사용자가 가지는 기본 작업 역할입니다. 기본적으로 사용자가 할당되는 모든 작업 및 문제도 이 작업 역할에 할당됩니다. 자원 관리에는 직무 역할이 필수적입니다. 작업 역할에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">작업 역할 만들기 및 관리</a></p> <p>관리자 액세스 권한이 있는 Plan 라이센스가 있거나 Workfront 관리자인 경우에만 이 필드를 업데이트할 수 있습니다. 관리자 액세스 권한이 있는 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</p> </li> 
        <li>(조건부) <b>기본 역할</b>, <b>FTE 가용성 비율</b> 필드가 표시됩니다. 이 작업 역할에 할당된 사용자의 일정 비율을 지정합니다. 기본 역할에 대한 FTE 가용성 백분율에 대한 기본값은 100%입니다.</li> 
        <li> <p><b>기타 역할</b>: Workfront에서는 사용자에게 여러 작업 역할이 있을 수 있습니다. 자원 관리에는 직무 역할이 필수적입니다. 사용자가 수행할 수 있는 Job 역할 수에는 제한이 없습니다. 그러나 리소스 관리가 이러한 사용자에게 너무 복잡해질 수 있으므로 한 명의 사용자를 너무 많은 작업 역할에 할당하지 않는 것이 좋습니다.</p> <p>작업 역할에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">작업 역할 만들기 및 관리</a>.</p> <p>관리자 액세스 권한이 있는 Plan 라이센스가 있거나 Workfront 관리자인 경우에만 이 필드를 업데이트할 수 있습니다. 관리자 액세스 권한이 있는 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</p> </li> 
        <li> <p>(조건부) 하나 또는 여러 개를 선택한 경우 <b>기타 역할</b>, <b>FTE 가용성 비율</b> 각 역할에 대해 필드가 표시됩니다. 각 작업 역할에 할당된 사용자의 일정 비율을 지정합니다. 기타 역할에 대한 FTE 가용성 백분율에 대한 기본값은 0%입니다.</p> <p><b>메모</b>:  
          <ul> 
           <li>다른 역할에 0%의 FTE 가용성이 있는 경우, 사용자가 이러한 역할의 작업에 할당되지 않는 한 리소스 계획자에 표시되지 않습니다.</li> 
           <li> <p>모든 역할에 대한 모든 FTE 가용성의 합계는 100%여야 합니다. 각 FTE 가용성의 백분율은 Resource Planner에서 사용자당 각 역할에 대해 사용 가능한 시간을 계산합니다. 사용자당 각 역할에 대한 사용 가능한 시간은 사용자가 사용할 수 있는 시간에 따라 다릅니다.</p> <p>사용자가 사용할 수 있는 시간은 Workfront 관리자가 리소스 관리 기본 설정에서 FTE를 계산하도록 선택한 방법에 따라 Workfront에서 계산됩니다.</p> <p>사용자의 가용성 계산에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">리소스 계획자에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요</a>.</p> <p>리소스 관리 환경 설정 구성에 대한 자세한 내용은 다음을 참조하십시오 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">리소스 관리 환경 설정 구성</a>.</p> </li> 
          </ul> </p> </li> 
        <li> <p><b>예약</b>: 일정을 사용자와 연결합니다. 사용자의 예약은 사용자가 할당된 작업의 타임라인을 계산합니다.</p> <p>Workfront 관리자 또는 그룹 관리자는 일정을 만든 후에 사용자와 연결할 수 있습니다.</p> <p>시스템 레벨 또는 그룹 스케줄을 선택하여 선택된 사용자에게 할당합니다.</p> <p>시스템 수준 및 그룹 스케줄에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">예약 만들기</a>.</p> <p><b>중요 사항</b>: Workfront에서는 [리소스 가용성 계산]이 [사용자 일정]으로 설정된 경우에만 사용자 일정을 사용합니다. 자원 관리에 사용되는 스케줄에 영향을 주는 자원 가용성 계산 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">리소스 관리 환경 설정 구성</a>.</p> </li> 
        <li> <p><b>작업표 프로필</b>: 작업표 프로필을 사용자와 연결합니다. 이렇게 하면 작업표가 사용자에 대해 자동으로 생성됩니다.</p> 
        <p><b>메모</b>:  
          <ul> 
           <li>이 필드에서 사용할 수 있는 작업표 프로필 목록은 사용자의 액세스 권한에 따라 다릅니다.
            <ul>
             <li>Workfront 관리자는 모든 시스템 수준 및 그룹 수준 작업표 프로필을 볼 수 있습니다.</li>
             <li><p>그룹 관리자에게는 시스템 수준 작업표 프로필과 관리하는 그룹과 연관된 작업표 프로필이 표시됩니다.</p></li>
             <li><p>계획자 라이센스와 사용자 편집에 대한 액세스 권한이 있는 사용자는 시스템 수준의 작업표 프로필만 볼 수 있습니다.</p></li>
            </ul></li> 
           <li>그룹 관리자라면 편집하는 모든 사용자가 관리하는 그룹의 구성원이어야 합니다.</li> 
          </ul> </p> </li> 
        <li><b>기본 시간 유형</b>: 사용자의 기본 시간 유형을 선택합니다. 사용자가 시간을 기록할 때 기본적으로 사용되는 시간 유형입니다.</li> 
        <li> <p><b>사용 가능한 시간 유형</b>: 사용자가 사용할 수 있어야 하는 시간 유형을 선택합니다. 이러한 시간 유형은 사용자가 로그인할 수 있는 Workfront의 모든 위치에 표시됩니다. 사용자는 프로젝트 수준에서 활성화된 시간 유형과 사용자 레벨만 볼 수 있습니다.</p> 
        <p>사용자가 사용할 수 있는 시간 유형에 대한 자세한 내용은 <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">작업표의 시간 유형 및 가용성을 정의합니다.</a>.</p> 
        </li> 
        <li> <p><b>FTE</b>: 여기서 지정하는 숫자는 시스템 레벨의 자원 관리 환경설정이 로 설정된 경우에만 기본 스케줄을 기준으로 사용자의 가용성을 계산하기 위해 고려됩니다 <b>기본 예약</b>.</p> 
        <p>예를 들어 FTE 값이 0.5이고 기본 일정이 40시간인 경우 사용자는 일주일에 20시간 동안 작업할 수 있습니다. 기본 일정을 선택한 경우 예약 예외 또는 휴가가 사용자 가용성에 영향을 미치는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">리소스 관리 환경 설정 구성</a>. </p> 
        <p>시스템 레벨의 자원 관리 환경설정이 <b>사용자 일정</b>로 지정하는 값은 무시되고 사용자는 일정에 지정된 대로 사용할 수 있는 것으로 간주됩니다. 이 경우 리소스 계획자에 대한 사용자의 FTE는 다음 공식으로 계산됩니다.</p>
        <p><code style="font-style: normal;">User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code> </p> <p>사용자 FTE 계산에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">리소스 계획자에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요</a>.</p> <p>Workfront에서 예약 만들기에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">예약 만들기</a>.</p> <p>리소스 관리 기본 설정 구성에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">리소스 관리 환경 설정 구성</a>.</p> 
        </li> 
        <li> <p><b>리소스 풀</b>: 사용자를 리소스 풀과 연결합니다.</p> <p><b>참고</b>: 선택한 모든 사용자에게 공통인 리소스 풀만 이 필드에 나타납니다. 선택한 사용자에게 공유 리소스 풀이 없는 경우 이 필드는 비어 있습니다. 이 필드가 비어 있으면 여기에서 지정하는 리소스 풀이 개별 리소스 풀을 덮어씁니다.</p> 
        <p>리소스 풀에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> 리소스 풀 개요 </a>.</p> </li> 
        <li><b>시간당 비용</b>: 사용자의 시간당 비용 금액입니다. </li> 
        <li><b>시간당 청구</b>: 사용자에 대한 시간당 청구 금액입니다.</li> 
        <li><b>사용자 지정 Forms</b>: 기존 사용자 지정 양식을 사용자와 연결합니다. 사용자 지정 양식을 사용자와 연결하려면 먼저 사용자 지정 양식을 만들어야 합니다. 활성 사용자 지정 양식만 목록에 표시됩니다. 사용자 지정 양식 만들기에 대한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">사용자 지정 양식 만들기 또는 편집</a>.</li> 
        <li><b>댓글</b>: 제공된 필드에 설명을 입력합니다. 선택한 모든 사용자는 인앱 알림 및 댓글이 포함된 이메일 알림을 받게 됩니다. 사용자 프로필의 업데이트 탭에 주석이 표시됩니다.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항)에서 **사용자 지정 Forms** 섹션에서 **사용자 지정 표현식 다시 계산** 선택한 사용자에게 첨부된 사용자 지정 양식의 계산된 모든 사용자 지정 필드가 최신 상태인지 확인하는 옵션입니다.

1. 클릭 **변경 내용 저장**.
