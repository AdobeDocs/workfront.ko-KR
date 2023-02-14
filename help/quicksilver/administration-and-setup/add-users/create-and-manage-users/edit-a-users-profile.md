---
title: 사용자 프로필 편집
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Adobe Workfront 관리자는 새 사용자를 만들고 기존 사용자의 프로필을 관리할 수 있습니다.
author: Courtney, Alina
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 5433008d93e99d69f8116e222bfce02411b77825
workflow-type: tm+mt
source-wordcount: '2557'
ht-degree: 0%

---

# 사용자 프로필 편집

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
>Adobe Admin Console에서 사용자 프로필 편집에 대한 지침은 문서에서 &quot;사용자 세부 사항 편집&quot; 섹션을 참조하십시오 [개별 사용자 관리](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 또는 Adobe Admin Console 관리자에게 문의하십시오.
>
>조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 다른 절차 목록은 [플랫폼 기반의 관리 차이점(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe Workfront 관리자는 새 사용자를 만들고 기존 사용자의 프로필을 관리할 수 있습니다. 사용자 만들기에 대한 내용은 [사용자 추가](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

계획 라이센스가 있는 사용자는 사용자를 만들고 관리할 수도 있습니다. 사용자 편집에 필요한 액세스에 대한 자세한 내용은 [사용자에게 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

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

## 사용자 프로필 편집

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **사용자** ![](assets/users-icon-in-main-menu.png).
1. 사용자를 선택한 다음 편집 아이콘을 클릭합니다 ![](assets/edit-icon.png).

1. 에서 **사용자 편집** 표시되는 상자에서 다음 정보를 변경한 다음 **변경 내용 저장**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">개인적인 정보 </td> 
      <td> 
       <ul> 
        <li><b>이름</b>, <b>성</b></li> 
        <li> <p><b>이메일 주소:</b> 사용자의 이메일 주소 또한 Workfront의 사용자 이름입니다. 이 필드는 대/소문자를 구분하며 고유해야 합니다. 사용자가 10분 창 내에서 3번 고유하지 않은 이메일 주소를 추가하려고 하면 reCAPTCHA 응답이 나타납니다.</p> <p>이메일을 사용하고 목록에 허용 목록에 추가하다 없는 이메일 도메인을 입력하면 사용자는 이메일 알림을 받지 않습니다. 에 대한 자세한 허용 목록에 추가하다 내용은 <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">이메일 허용 목록에 추가하다 구성</a>.</p> </li> 
        <li> <p><b>암호 재설정</b>: 사용자 암호를 재설정하려면 이 링크를 클릭하십시오. 사용자 암호를 재설정하기 전에 사용자 암호를 입력해야 합니다.</p> <p>다른 사용자의 암호를 재설정하려면 Workfront 관리자나 그룹 관리자여야 합니다.</p> <p><b>메모</b>:  
          <ul> 
           <li> <p>그룹 관리자라면 암호를 재설정할 수 있습니다. 또한 액세스 수준에서 사용자 관리자(그룹 사용자) 권한을 활성화해야 합니다.</p> <p> <img src="assets/group-admin-user.png" > </p> <p>이 설정은 기본적으로 비활성화됩니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </li> 
           <li> <p>Workfront 관리자의 암호를 재설정할 수 없습니다.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;sso configuration=""&gt; 사용자 이름</b>: Workfront 관리자가 Workfront과의 SSO 통합을 활성화한 경우 이 필드에 SSO 사용자 이름이 표시됩니다. Workfront 인스턴스에 대해 활성화된 SSO 구성 유형이 이 필드에 표시됩니다. </li> 
        <li> <p><b>OnlyAllow &lt;sso configuration=""&gt; 인증</b>: Workfront 관리자가 Workfront과의 SSO 통합을 활성화하고 모든 SSO 사용자를 업데이트한 경우 이 필드가 기본적으로 선택됩니다. Workfront 인스턴스에 대해 활성화된 SSO 구성 유형이 이 필드에 표시됩니다.</p> <p>이 필드를 선택한 경우 사용자는 SSO 자격 증명으로 Workfront에 로그인해야 합니다. 이 옵션을 선택 해제하면 Workfront 자격 증명으로 Workfront에 로그인할 수 있습니다.</p> <p>SSO 솔루션과 Workfront 구성에 대한 자세한 내용은 을 참조하십시오 <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Adobe Workfront의 단일 사인온 개요</a></p> <p>SSO용 사용자 업데이트에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">단일 사인온용 사용자 업데이트</a>.</p> <p><b>참고</b>: 그룹 관리자인 경우 &lt;sso configuration=""&gt; 사용자로 지정된 그룹의 사용자에 대해서만 필드를 표시합니다. 또한 액세스 수준에서 사용자 관리자(그룹 사용자) 권한을 활성화해야 합니다.
        <p>그룹 관리자이고 액세스 수준에서 사용자 관리자(모든 사용자) 권한이 활성화되어 있는 경우, &lt;sso configuration=""&gt; 모든 사용자의 필드.</p> </li> 
        <li><b>작업 정보:</b> 직책, 사용자에게 책임이 있는 전문 분야 등 Job에 대한 정보입니다.</li> 
        <li><p><b>연락처 정보</b>: 사용자의 전화 번호와 주소입니다.</p>
        <p>사용자가 UUM(Unified User Management) 또는 IMS(Analysis Workspace System)에 대해 활성화되어 있으면 <b>국가</b> 연락처 정보 섹션의 필드는 국가 코드 값(예: 미국, GB, IN)만 허용합니다.</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">환경 설정 </td> 
      <td> 
       <ul> 
        <li> <p><b>시간대:</b> 사용자의 시간대입니다.</p> <p>시간대에 걸쳐 Workfront에서 사용자가 공동 작업하는 데 도움이 되는 방법에 대한 자세한 내용은 <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">시간대 작업</a>.</p> </li> 
        <li><b>전자 메일 로케일</b>: 사용자의 기본 전자 메일 로케일입니다. Workfront에서 오는 이메일의 숫자 및 날짜 형식에 영향을 줍니다.</li> 
        <li><b>업데이트 상태에 완료 비율 표시</b>: 이 사용자 작업의 업데이트 영역 내에 백분율 전체 막대를 표시하려면 이 옵션을 선택합니다.</li> 
        <li><b>내 작업 중 탭에 할당하는 작업 보내기</b>: 사용자가 자신에게 할당한 모든 것을 작업 중 탭에 직접 표시하려면 이 옵션을 선택합니다. 기본값은 작업 요청 탭에서 사용자에게 할당된 모든 항목을 나열하는 것입니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">알림</td> 
      <td> <p>새 사용자에 대해 활성화해야 하는 이메일 알림을 선택합니다.</p> <p>일별 다이제스트 알림뿐만 아니라 인스턴트 항목을 선택할 수 있습니다.</p> <p>자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">시스템의 모든 사용자에 대한 이벤트 알림을 구성합니다</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">액세스</td> 
      <td> 
       <ul> 
        <li><b>활성 상태:</b> 사용자가 활성 상태임을 나타내려면 이 상자를 선택합니다. 활성 사용자는 Workfront 라이센스를 사용합니다. 상자를 지우면 사용자가 비활성화됩니다.</li> 
        <li> <p><b>액세스 수준:</b> 이 사용자에게 할당할 액세스 수준을 선택합니다.</p> 
        <p>사용자에게 액세스 수준을 할당할 때, 사용자 자신의 액세스 수준 이하로 수준을 지정할 수 있습니다. 예를 들어, 액세스 레벨이 계획자이면 관리자 액세스 레벨을 지정할 수 없습니다. 그러나 Workfront 관리자가 액세스 수준(에 설명된 대로 세부 조정 설정을 통해)에서도 활성화되지 않은 액세스 수준에서 기본적으로 고유한 액세스 수준보다 낮은 액세스 수준을 할당할 수 없습니다 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>). </p> 
        <p>액세스 수준에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Adobe Workfront에 대한 액세스 구성</a>.</p> </li> 
        <li> <p><b>레이아웃 템플릿</b>: 사용자의 레이아웃 템플릿을 선택합니다. 이 레이아웃 템플릿은 사용자의 홈 그룹, 홈 팀 또는 기본 작업 역할에 할당된 모든 레이아웃 템플릿보다 우선합니다. 레이아웃 템플릿의 할당 우선 순위에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">레이아웃 템플릿 만들기 및 관리</a>.</p> <p><b>메모</b>:  <p>이 필드에서 사용할 수 있는 템플릿 목록은 액세스 권한에 따라 다릅니다.</p> 
          <ul> 
           <li>Workfront 관리자는 모든 시스템 수준 및 그룹 수준 레이아웃 템플릿을 볼 수 있습니다.</li> 
           <li>그룹 관리자는 시스템 수준 레이아웃 템플릿과 관리하는 그룹과 연관된 템플릿을 볼 수 있습니다.</li> 
           <li>플랜 라이센스가 있고 사용자 편집에 액세스할 수 있는 사용자는 시스템 수준 레이아웃 템플릿만 볼 수 있습니다.</li> 
          </ul> <p>그룹 수준 레이아웃 템플릿에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">레이아웃 템플릿 만들기 및 관리</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">조직 </td> 
      <td> 
       <ul> 
      <li><b>회사</b>: 사용자의 회사입니다. 사용자는 한 회사에만 연결할 수 있습니다. 회사와 사용자를 연결하려면 먼저 회사를 만들어야 합니다. 활성 회사만 목록에 표시됩니다. 회사 만들기에 대한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">회사 만들기 및 편집</a>.</li> 
      <li><b>보고서 대상:</b> 사용자에 대해 회사를 지정한 경우 이 필드에 사용자의 직접 관리자를 지정할 수도 있습니다. 사용자는 한 명의 관리자만 가질 수 있습니다.</li> 
      <li><b>직접 보고서:</b> 사용자를 위해 회사를 지정한 경우 사용자의 직접 보고서를 지정할 수도 있습니다. 사용자는 여러 개의 직접 보고서를 가질 수 있습니다.</li> 
      <li><b>홈 팀</b>: 사용자의 홈 팀을 지정합니다. 사용자는 하나의 홈 팀만 가질 수 있습니다.</li> 
      <li><b>기타 팀</b>: 사용자는 여러 팀에 속할 수 있습니다.</li> 
      <li> <p><b>홈 그룹:</b> 사용자를 할당할 적절한 그룹을 선택합니다. 따라서 사용자는 그룹과 공유되는 객체에 액세스할 수 있습니다.</p> <p>필수 필드입니다. 모든 사용자는 홈 그룹과 연결되어 있어야 합니다. 선택하지 않으면 그룹이 새 사용자의 홈 그룹으로 할당됩니다.</p> <p><b>참고</b>: Workfront 관리자이거나, 그룹의 관리자이거나, 그룹이 공개인 경우에만 그룹을 사용자에게 할당할 수 있습니다.</p> </li> 
      <li> <p><b>기타 그룹</b>: 사용자는 여러 그룹에 속할 수 있습니다. Workfront 관리자이거나, 그룹의 관리자이거나, 그룹이 공개인 경우에만 그룹을 사용자에게 할당할 수 있습니다.</p> <p><b>중요 사항</b>: 100개 이상의 그룹에 사용자를 추가하면 그룹 목록을 로드하는 Workfront의 모든 영역에서 성능 문제가 발생할 수 있습니다.</p> <p>공용 그룹에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">그룹 만들기</a>.</p> <p>그룹에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">그룹 개요</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">리소스 계획 수립 </td> 
      <td> 
       <ul>
       <li><b>비활성화 예약</b>: 일정 기간 후에 이 사용자를 비활성화하도록 예약하려면 이 상자를 선택합니다. </li> 
       <li><b>예약된 비활성화 날짜</b>: 사용자가 비활성화된 날짜입니다. 사용자 비활성화 예약에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">사용자 비활성화 예약</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">사용자 비활성화 또는 다시 활성화</a>.</li> 
       <li> <p><b>기본 역할</b>: 사용자가 Workfront에서 수행할 수 있는 기본 작업 역할입니다. 사용자가 할당되는 모든 작업 및 문제도 이 작업 역할에 할당됩니다. 자원 관리에는 직무 역할이 필수적입니다. 관리자 액세스 권한이 있는 Plan 라이센스가 있거나 Workfront 관리자인 경우에만 이 필드를 업데이트할 수 있습니다. 관리자 액세스 권한이 있는 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</p> <p>활성 작업 역할만 목록에 표시됩니다. </p> </li> 
       <li>선택한 경우 <b>기본 역할</b>, <b>FTE 가용성 비율</b> 필드가 표시됩니다. 이 작업 역할에 할당된 사용자의 일정 시간의 백분율을 지정합니다. 기본 역할에 대한 FTE 가용성 백분율에 대한 기본값은 100%입니다. </li> 
       <li> <p><b>기타 역할</b>: 사용자는 Workfront에서 여러 작업 역할을 가질 수 있습니다. 자원 관리에는 직무 역할이 필수적입니다. 사용자가 수행할 수 있는 Job 역할 수에는 제한이 없습니다. 그러나 리소스 관리가 이러한 사용자에게 너무 복잡해질 수 있으므로 한 명의 사용자를 너무 많은 작업 역할에 할당하지 않는 것이 좋습니다.<p>활성 작업 역할만 목록에 표시됩니다. 작업 역할에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">작업 역할 만들기 및 관리</a>.</p> <p>관리자 액세스 권한이 있는 Plan 라이센스가 있거나 Workfront 관리자인 경우에만 이 필드를 업데이트할 수 있습니다. <br>관리자 액세스 권한이 있는 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</p> </li> 
       <li> <p>(조건부) 하나 또는 여러 개를 선택한 경우 <b>기타 역할</b>, <b>FTE 가용성 비율</b> 각 역할에 대해 필드가 표시됩니다. 각 작업 역할에 할당된 사용자의 일정 시간의 백분율을 지정합니다. 기타 역할에 대한 FTE 가용성 백분율에 대한 기본값은 0%입니다.</p> <p><b>참고</b>: 다른 역할에 0%의 FTE 가용성이 있는 경우, 사용자가 이러한 역할의 작업에 할당되지 않는 한 리소스 계획자에 표시되지 않습니다.</p> <p> <img alt="user_settings_roles_and_dte_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>메모</b>: <p>모두 <b>FTE 가용성 백분율</b> 모든 역할에 대해 100%가 같아야 합니다. 각 FTE 가용성의 백분율은 Resource Planner에서 사용자당 각 역할에 대해 사용 가능한 시간을 계산합니다. 사용자당 각 역할에 대한 사용 가능한 시간은 사용자가 사용할 수 있는 시간에 따라 다릅니다.</p> <p>사용자가 사용할 수 있는 시간은 Workfront 관리자가 리소스 관리 기본 설정에서 FTE를 계산하도록 선택한 방법에 따라 Workfront에서 계산됩니다.</p> <p>사용자의 가용성 계산에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">리소스 계획자에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요</a>.</p> <p>리소스 관리 기본 설정 구성에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">리소스 관리 환경 설정 구성</a>.</p> </p> </li> 
       <li> <p><b>예약</b>: 일정을 사용자와 연결합니다. 사용자의 예약은 사용자가 할당된 작업의 타임라인을 계산합니다.</p> <p>일정을 만들어야 사용자와 일정을 연결할 수 있습니다. 예약 작성에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">예약 만들기</a>.</p> <p><b>참고</b>: 사용자와 연결하는 예약은 사용자의 시간대와 일치하는 것이 좋습니다.</p> </li> 
       <li> <p><b>작업표 프로필</b>: 작업표 프로필을 사용자와 연결하여 작업표가 사용자에 대해 자동으로 생성되도록 합니다.</p> <p><b>참고</b>: 이 필드에서 사용할 수 있는 프로필 목록은 액세스 권한에 따라 다릅니다.
       <ul>
       <li>Workfront 관리자는 모든 시스템 수준 및 모든 그룹 수준 작업표 프로필을 볼 수 있습니다.</li>
       <li>그룹 관리자에게는 시스템 수준의 작업표 프로필과 관리하는 그룹과 연관된 작업표를 볼 수 있습니다.</li>
       <li>계획 라이선스와 사용자 편집 액세스 권한이 있는 사용자는 시스템 수준의 작업표 프로필만 볼 수 있습니다. 그룹 수준 작업표 프로필에 대한 자세한 내용은 <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">작업표 프로필 만들기, 편집 및 할당</a>.</li>
      </ul></p> </li> 
       <li><b>기본 시간 유형</b>: 사용자의 기본 시간 유형을 선택합니다. 사용자가 시간을 기록할 때 기본적으로 사용되는 시간 유형입니다.</li> 
       <li><b>사용 가능한 시간 유형</b>: 사용자가 사용할 수 있어야 하는 시간 유형을 선택합니다. 이러한 시간 유형은 사용자가 로그인할 수 있는 Workfront의 모든 위치에 표시됩니다. 사용자는 프로젝트 수준에서 활성화된 시간 유형과 사용자 레벨만 볼 수 있습니다. 사용자가 사용할 수 있는 시간 유형에 대한 자세한 내용은 <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">작업표의 시간 유형 및 가용성을 정의합니다.</a>.</li> 
       <li><b>로그인 시간:</b> 사용자가 작업 항목에 대한 시간을 시간 또는 일 단위로 기록할지 여부를 선택합니다. 자세한 내용은 <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">시간 또는 일 단위로 로그인 여부 구성</a>.</li> 
       <li> <p><b>FTE</b>: 시스템 레벨의 자원 관리 환경설정이 <b>기본 예약</b>. 값은 <i>0</i> 또는 다음 사이 <i>.1</i> 및 <i>1</i>.</p> <p>예를 들어 FTE 값이 0.5이고 기본 일정이 40시간인 경우 사용자는 일주일에 20시간 동안 작업할 수 있습니다.</p> <p>시스템 레벨의 자원 관리 환경설정이 <b>사용자 일정</b>로 지정하는 값은 무시되고 사용자는 일정에 지정된 대로 사용할 수 있는 것으로 간주됩니다. 이 경우 리소스 계획자에 대한 사용자의 FTE는 다음 공식으로 계산됩니다.</p> <p ><code>User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code><em><br></em> </p> <p>사용자 FTE 계산에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">리소스 계획자에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요</a>.<br>Workfront에서 예약 만들기에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">예약 만들기</a>.</p> <p>스케줄 예외 및 타임오프는 계획 시간 또는 FTE의 양에 영향을 줄 수 있습니다. 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">리소스 관리 환경 설정 구성</a>. </p> </li> 
        <li><b>리소스 풀</b>: 사용자를 리소스 풀에 연결합니다. 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">사용자와 리소스 풀 연결 </a>.</li> 
        <li><b>시간당 비용</b>: 사용자의 시간당 비용 금액입니다. </li> 
        <li><b>시간당 청구</b>: 사용자에 대한 시간당 청구 금액입니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 정의 양식</td> 
      <td>기존 사용자 지정 양식을 이 사용자와 연결합니다. 사용자 지정 양식을 사용자와 연결하려면 먼저 사용자 지정 양식을 만들어야 합니다. 활성 사용자 지정 양식만 목록에 표시됩니다. 사용자 지정 양식 만들기에 대한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">사용자 지정 양식 만들기 또는 편집</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">댓글</td> 
      <td> <p>사용자에게 보낼 댓글과 사용자 프로필의 업데이트 영역을 입력합니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>
