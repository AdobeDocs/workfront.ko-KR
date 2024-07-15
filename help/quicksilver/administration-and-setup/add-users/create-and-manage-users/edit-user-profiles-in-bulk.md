---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 사용자 프로필 일괄 편집
description: Adobe Workfront 관리자는 사용자 계정을 대량으로 편집할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: bfaf566e556882078875649549c0dfadacd800b8
workflow-type: tm+mt
source-wordcount: '2245'
ht-degree: 0%

---

# 사용자 프로필 일괄 편집

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

사용자 계정을 일괄적으로 편집할 수 있습니다. 사용자를 일괄 편집할 때 특별히 선택한 필드만 선택한 모든 사용자에 대해 동일한 정보로 업데이트됩니다. 선택하지 않은 다른 모든 필드는 각 사용자에 대해 다르더라도 각 개별 사용자에 대해 동일하게 유지됩니다.

>[!NOTE]
>
>* 사용자 프로필의 개인 정보 섹션은 모든 사용자에 대해 고유해야 하므로 벌크 편집할 수 없습니다.
>* 데이터의 정확성과 최적의 성능을 보장하려면 일괄 편집을 위해 한 번에 2000명 이하의 사용자를 선택하는 것이 좋습니다.
>

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>다음 중 하나가 있어야 합니다.</p> 
    <ul> 
     <li> <p>시스템 관리자 액세스 수준입니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>를 참조하십시오. </p> </li> 
     <li> <p>액세스 수준의 <b>사용자</b> 설정이 <b>편집</b> 액세스로 구성되었으며, <b>만들기</b>와 <b>설정을 미세 조정</b> <img src="assets/gear-icon-in-access-levels.png">에서 두 개의 <b>사용자 관리</b> 옵션 중 하나 이상을 사용할 수 있습니다. </p> <p>이 두 옵션 중 사용자 <b>관리자(그룹 사용자)</b>이(가) 활성화된 경우 사용자가 멤버인 그룹의 그룹 관리자여야 합니다.</p> <p>액세스 수준의 <b>사용자</b> 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>를 참조하십시오.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자 계정 일괄 편집

1. Adobe Workfront의 오른쪽 상단에 있는 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **사용자** ![](assets/users-icon-in-main-menu.png)를 클릭합니다.

1. 사용자를 두 명 이상 선택한 다음 편집 아이콘 ![](assets/edit-icon.png)을(를) 클릭합니다.

1. 표시되는 **사용자 편집** 상자에서 다음 옵션을 변경합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">환경 설정</td> 
      <td> 
       <ul> 
        <li><b>시간대:</b> 사용자의 시간대입니다.</li> 
        <li><b>로케일</b>: 사용자가 선호하는 로케일입니다. 이 오류는 Workfront에서 전송되는 이메일의 숫자 및 날짜 형식에 영향을 줍니다.</li> 
        <li><b>내가 자신에게 할당한 작업을 내 처리 중 탭으로 보내기</b>: 사용자가 자신에게 할당한 모든 작업을 [처리 중] 탭에 직접 표시하려면 이 옵션을 선택하십시오. 기본적으로 사용자에게 할당된 모든 항목이 작업 요청 탭에 나열됩니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">알림</td> 
      <td>새 사용자에 대해 활성화해야 하는 이메일 알림을 선택합니다.<p>인스턴트 및 일별 다이제스트 알림을 선택할 수 있습니다. 모든 일별 다이제스트 알림은 선택한 모든 사용자에 대해 같은 시간 이후에 전달됩니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">시스템의 모든 사용자를 위한 이벤트 알림 구성</a>을 참조하십시오.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">액세스</td> 
      <td> 
       <ul> 
        <li><b>활성 상태입니다.</b> 이 필드를 선택하여 사용자가 활성 상태인지 여부를 나타냅니다. 활성 사용자는 Workfront 라이선스를 사용합니다. 필드를 선택 해제하면 사용자가 비활성화됩니다.</li> 
        <li> 
        <p><b>액세스 수준:</b> 이 사용자에게 할당할 액세스 수준을 선택합니다. 선택한 모든 사용자의 액세스 수준은 동일합니다.
        </p> 
        <p>사용자에게 액세스 수준을 할당할 때 자신의 액세스 수준과 같거나 낮은 수준을 할당할 수 있습니다. (예를 들어 액세스 수준이 플래너인 경우 관리자 액세스 수준을 할당할 수 없습니다.) </p>
        <p>하지만 Workfront 관리자가 직접 활성화되지 않은 액세스 수준에 대한 권한을 활성화한 경우(<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>에 설명된 대로 미세 조정 설정을 통해) 자신보다 낮은 액세스 수준을 할당할 수 없습니다.</p> 
        <p>액세스 수준에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Adobe Workfront 액세스 구성</a>을 참조하십시오.</p> 
         </li> 
        <li> 
        <p><b>레이아웃 템플릿</b>: 사용자에 대한 레이아웃 템플릿을 선택하십시오. 사용자에게 할당된 레이아웃 템플릿은 홈 그룹, 홈 팀 또는 기본 작업 역할에 할당된 모든 레이아웃 템플릿보다 우선합니다. 레이아웃 템플릿의 할당 우선 순위에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">레이아웃 템플릿 만들기 및 관리</a>를 참조하십시오.</p> 
        <p><b>참고</b>: 이 필드에서 사용할 수 있는 레이아웃 템플릿 목록은 액세스 권한에 따라 다릅니다.
          <ul>
           <li>Workfront 관리자는 모든 시스템 수준 및 그룹 수준 레이아웃 템플릿을 볼 수 있습니다.</li>
           <li>그룹 관리자는 시스템 수준 레이아웃 템플릿과 관리하는 그룹과 관련된 템플릿을 볼 수 있습니다.</li>
           <li><p>플래너 라이선스를 가지고 있고 사용자 편집 액세스 권한을 가진 사용자는 시스템 수준 레이아웃 템플릿만 볼 수 있습니다. </p>
           <p>그룹 수준 레이아웃 템플릿에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">레이아웃 템플릿 만들기 및 관리</a>를 참조하십시오.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">조직</td> 
      <td> 
       <ul> 
        <li><b>회사</b>: 사용자의 회사입니다. 사용자는 한 회사에만 연결할 수 있습니다. 회사를 사용자와 연결하려면 먼저 회사를 만들어야 합니다. 활성 회사만 목록에 표시됩니다. 회사 만들기에 대한 내용은 회사 이해 및 관리를 참조하십시오.</li> 
        <li><b>홈 팀</b>: 사용자의 홈 팀을 지정합니다. 사용자는 홈 팀을 하나만 보유할 수 있습니다. </li> 
        <li><b>다른 팀</b>: 사용자가 여러 팀에 속할 수 있습니다. </li> 
        <li> <p><b>홈 그룹:</b> 사용자를 홈 그룹으로 할당할 적절한 그룹을 선택하십시오. 이를 통해 사용자는 그룹과 공유되는 객체에 액세스할 수 있습니다.</p> <p><b>참고</b>: 필수 필드입니다. 홈 그룹에 연결되지 않은 사용자를 가질 수 없습니다.</p> <p>다음 상황에서만 사용자에게 그룹을 할당할 수 있습니다.</p> 
         <ul> 
          <li>Workfront 관리자입니다.</li> 
          <li>해당 그룹의 관리자입니다.</li> 
          <li>이 그룹은 공개적입니다.</li> 
         </ul> </li> 
        <li> <p><b>기타 그룹</b>: 사용자가 여러 그룹에 속할 수 있습니다. 다음과 같은 경우에만 사용자에게 그룹을 할당할 수 있습니다.</p> 
         <ul> 
          <li>Workfront 관리자입니다.</li> 
          <li>해당 그룹의 관리자입니다.</li> 
          <li> <p>이 그룹은 공개적입니다. </p> 
          <p>공용 그룹에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">그룹 만들기</a>를 참조하십시오.</p> 
          <p>그룹에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">그룹 개요</a>를 참조하세요.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">리소스 계획 수립</td> 
      <td> 
       <ul>

   <li>
       <b>작업 시간</b>: 사용자가 오버헤드를 포함하지 않고 실제 작업에 사용할 수 있는 FTE(Full Time Equivalent) 시간의 백분율을 나타냅니다. 작업 시간은 최대 1의 10진수여야 하며 0일 수 없습니다. 예를 들어, 실제 작업에 대한 20% 가용성은 0.2입니다.

   필드의 기본값은 1이며, 사용자가 전체 FTE를 실제 프로젝트 관련 작업에 사용함을 나타냅니다.

   시스템은 이 숫자를 사용하여 실제 프로젝트 관련 작업에 대한 사용자의 가용성을 계산합니다.

   Workfront에서 일정을 만드는 방법에 대한 자세한 내용은 <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">일정 만들기</a>를 참조하십시오.

   일정 예외 및 휴무는 사용자 용량에도 영향을 줄 수 있습니다.

   Workfront은 설정 영역의 리소스 관리 기본 설정에 따라 사용자의 가용성을 계산합니다. 자세한 내용은 <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">리소스 관리 환경 설정 구성</a>을 참조하십시오.

   <b>팁</b>

   작업 시간 값을 1로 설정하면 사용자가 프로젝트 관련 작업에 전체 시간에 해당하는 전체 시간을 사용할 수 있음을 나타냅니다.
   </li>

   <li><b>비활성화 예약</b>: 일정 시간이 지난 후에 사용자를 비활성화하도록 예약하려면 이 확인란을 선택하십시오.</li> 
       <li><b>예약된 비활성화 날짜</b>: 사용자가 비활성화되는 날짜입니다. 비활성화 일정을 예약하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">사용자 비활성화 또는 다시 활성화</a>의 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">비활성화 일정</a> 섹션을 참조하십시오.</li> 
       <li> <p><b>기본 역할</b>: 사용자가 Workfront에서 보유하는 기본 작업 역할입니다. 사용자가 할당된 모든 작업 및 문제도 기본적으로 이 작업 역할에 할당됩니다. 작업 역할은 리소스 관리에서 필수적입니다. 작업 역할에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">작업 역할 만들기 및 관리</a>를 참조하세요.</p> <p>관리 사용자 액세스 권한이 있는 플랜 라이선스가 있거나 Workfront 관리자인 경우에만 이 필드를 업데이트할 수 있습니다. 관리자 액세스 권한을 가진 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>를 참조하십시오.</p> </li> 
       <li>(조건부) <b>기본 역할</b>을(를) 선택한 경우 <b>FTE 가용성의 백분율</b> 필드가 표시됩니다. 사용자의 일정 중 이 작업 역할에 할당되는 시간의 백분율을 지정합니다. 기본 역할에 대한 FTE 가용성 백분율의 기본값은 100%입니다.</li> 
       <li> <p><b>다른 역할</b>: 사용자는 Workfront에서 여러 작업 역할을 가질 수 있습니다. 작업 역할은 리소스 관리에서 필수적입니다. 사용자가 이행할 수 있는 작업 역할 수에는 제한이 없습니다. 그러나 너무 많은 수의 작업 역할에 한 명의 사용자를 할당하지 않는 것이 좋습니다. 리소스 관리가 너무 복잡해질 수 있기 때문입니다.</p> <p>작업 역할에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">작업 역할 만들기 및 관리</a>를 참조하십시오.</p> <p>관리 사용자 액세스 권한이 있는 플랜 라이선스가 있거나 Workfront 관리자인 경우에만 이 필드를 업데이트할 수 있습니다. 관리자 액세스 권한을 가진 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>를 참조하십시오.</p> </li> 
       <li> <p>(조건부) 하나 이상의 <b>다른 역할</b>을(를) 선택한 경우 각 역할에 대해 <b>FTE 가용성의 백분율</b> 필드가 표시됩니다. 사용자의 일정 중 각 작업 역할에 할당되는 시간의 백분율을 지정합니다. 다른 역할에 대한 FTE 가용성 백분율의 기본값은 0%입니다.</p> <p><b>참고</b>:  
       <ul> 
       <li>다른 역할에 0% FTE 가용성이 있는 경우 사용자가 이러한 역할의 작업에 할당되지 않는 한 리소스 플래너에 표시되지 않습니다.</li> 
       <li> <p>모든 역할에 대한 모든 FTE 가용성 백분율의 합은 100%여야 합니다. FTE 가용성의 각 비율은 리소스 플래너의 사용자당 각 역할에 대한 가용 시간을 계산합니다. 사용자당 각 역할에 대한 사용 가능한 시간은 사용자의 사용 가능한 시간에 따라 다릅니다.</p> <p>Workfront 관리자가 리소스 관리 환경 설정에서 FTE를 계산하기 위해 선택한 방법에 따라 사용자의 사용 가능한 시간이 Workfront에서 계산됩니다.</p> <p>사용자 가용성의 계산에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">리소스 플래너에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요</a>를 참조하십시오.</p> <p>리소스 관리 환경 설정 구성에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">리소스 관리 환경 설정 구성</a>을 참조하십시오.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>일정</b>: 일정을 사용자와 연결합니다. 사용자 일정은 사용자가 할당된 작업의 타임라인을 계산합니다.</p> <p>Workfront 관리자 또는 그룹 관리자는 일정을 만든 후에 사용자와 연결해야 합니다.</p> <p>시스템 수준 또는 그룹 일정을 선택하여 선택한 사용자에게 할당합니다.</p> <p>시스템 수준 및 그룹 일정에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">일정 만들기</a>를 참조하십시오.</p> <p><b>중요</b>: Workfront에서는 리소스 가용성 계산 설정이 사용자의 일정으로 설정된 경우에만 사용자의 일정을 사용합니다. 리소스 관리에 사용되는 일정에 영향을 주는 리소스 가용성 계산 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">리소스 관리 환경 설정 구성</a>을 참조하십시오.</p> </li> 
       <li> <p><b>타임시트 프로필</b>: 타임시트 프로필을 사용자와 연결합니다. 이렇게 하면 타임시트가 사용자를 위해 자동으로 생성됩니다.</p> 
       <p><b>참고</b>:  
       <ul> 
       <li>이 필드에서 사용할 수 있는 타임시트 프로필 목록은 액세스 권한에 따라 다릅니다.
       <ul>
       <li>Workfront 관리자는 모든 시스템 수준 및 그룹 수준 타임시트 프로필을 볼 수 있습니다.</li>
       <li><p>그룹 관리자는 시스템 수준 타임시트 프로필과 관리하는 그룹과 관련된 프로필을 볼 수 있습니다.</p></li>
       <li><p>플래너 라이선스가 있고 사용자 편집 액세스 권한이 있는 사용자는 시스템 수준 타임시트 프로필만 볼 수 있습니다.</p></li>
       </ul></li> 
       <li>그룹 관리자인 경우 편집 중인 모든 사용자는 관리하는 그룹의 구성원이어야 합니다.</li> 
       </ul> </p> </li> 
       <li><b>기본 시간 유형</b>: 사용자의 기본 시간 유형을 선택합니다. 사용자가 시간을 기록할 때 기본적으로 사용되는 시간 유형입니다.</li> 
       <li> <p><b>사용 가능한 시간 유형</b>: 사용자가 사용할 수 있는 시간 유형을 선택합니다. 이러한 시간 유형은 사용자가 시간을 기록할 수 있는 Workfront의 모든 곳에서 볼 수 있습니다. 사용자는 프로젝트 수준과 사용자 수준에서 활성화된 시간 유형만 볼 수 있습니다.</p> 
       <p>사용자가 사용할 수 있는 시간 유형에 대한 자세한 내용은 <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">시간 유형 및 가용성 정의</a>를 참조하십시오.</p> 
       </li> 
       <li> <b>FTE</b>: 사용자의 FULL TIME입니다. Workfront은 시스템 수준의 리소스 관리 기본 설정이 기본 일정으로 설정된 경우에만 이 숫자를 사용하여 기본 일정을 기준으로 사용자의 가용성을 계산합니다.

   <p>FTE는 사용자가 직장에서 보낼 수 있는 시간을 나타냅니다. 여기에는 간접비와 프로젝트 작업에 소비된 시간이 포함됩니다. 예를 들어, 회의나 교육에서 보내는 시간도 FTE에 포함됩니다.</p>

   FTE는 최대 1까지의 십진수여야 하며 0일 수 없습니다. 예를 들어 FTE 값이 0.5이고 Workfront의 기본 일정이 40시간인 경우 사용자는 일주일에 20시간 동안 사용할 수 있습니다.

   필드의 기본값은 1입니다.

   일정 예외, 휴무가 있을 수 있으며 작업 시간 값이 사용자의 가용성에 영향을 줄 수 있습니다.

   Workfront은 설정 영역의 리소스 관리 기본 설정에 따라 사용자의 가용성을 계산합니다.

   시스템 수준의 리소스 관리 기본 설정이 사용자 일정으로 설정된 경우 여기에서 지정한 값이 무시되며 사용자는 일정에 지정된 내용에 따라 사용할 수 있는 것으로 간주됩니다.

   자세한 내용은 <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">리소스 관리 환경 설정 구성</a>을 참조하십시오.

   Workfront에서 일정을 만드는 방법에 대한 자세한 내용은 <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">일정 만들기</a>를 참조하십시오.
   </li> 
       <li> <p><b>리소스 풀</b>: 사용자를 리소스 풀과 연결합니다.</p> <p><b>참고</b>: 선택한 모든 사용자에게 공통되는 리소스 풀만 이 필드에 나타납니다. 선택한 사용자에게 공유 리소스 풀이 없는 경우 이 필드는 비어 있습니다. 이 필드가 비어 있으면 여기에서 지정한 리소스 풀이 해당 개별 리소스 풀을 덮어씁니다.</p> 
       <p>리소스 풀에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> 리소스 풀 개요 </a>을(를) 참조하십시오.</p> </li> 
       <li><b>시간당 비용</b>: 사용자의 시간당 비용입니다. </li> 
       <li><b>시간당 청구</b>: 사용자의 시간당 청구 금액입니다.</li> 
       <li><b>사용자 지정 Forms</b>: 기존 사용자 정의 양식을 사용자와 연결합니다. 사용자 정의 양식을 사용자와 연결하려면 먼저 사용자 정의 양식을 만들어야 합니다. 활성 사용자 정의 양식만 목록에 표시됩니다. 사용자 정의 양식 만들기에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">사용자 정의 양식 만들기 또는 편집</a>을 참조하십시오.</li> 
       <li><b>댓글</b>: 제공된 필드에 댓글을 입력하십시오. 선택한 모든 사용자는 인앱 알림과 함께 귀하의 의견이 포함된 이메일 알림을 받게 됩니다. 주석은 사용자 프로필의 업데이트 탭에 표시됩니다.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) **사용자 지정 Forms** 섹션에서 **사용자 지정 표현식 다시 계산** 옵션을 선택하여 선택한 사용자에게 첨부된 사용자 지정 양식의 모든 계산된 사용자 지정 필드가 최신 상태인지 확인합니다.

1. **변경 내용 저장**&#x200B;을 클릭합니다.
