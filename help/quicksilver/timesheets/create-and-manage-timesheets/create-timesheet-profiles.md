---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: 작업표 프로필 만들기, 편집 및 할당
description: 사용자의 추가 작업 없이 사용자의 반복 작업표를 생성하는 작업표 프로필을 만들고 편집하고 지정할 수 있습니다. 이렇게 하면 시간이 절약되고 사용자 간에 다음 사항이 일관되도록 할 수 있습니다. EDIT ME.
author: Alina
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 7e2a4b02277e8b82ac6ee92a7994250fcdebb0b0
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 1%

---

# 작업표 프로필 만들기, 편집 및 할당

사용자의 추가 작업 없이 사용자의 반복 작업표를 생성하는 작업표 프로필을 만들고 편집하고 지정할 수 있습니다. 이렇게 하면 시간이 절약되고 사용자 간에 다음 사항이 일관되도록 할 수 있습니다.

* 작업표 기간
* 승인자
* 일반 시간 유형

작업표 수동으로 만드는 방법에 대한 자세한 내용은 [단일 사용 작업표 만들기](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업표에 대한 관리자 액세스 권한이 있어야 합니다. </p> <p>자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p>  <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 작업표 프로필 만들기 또는 편집

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>현재 작업표에서 작업표 프로필 변경을 사용하려면 기존 작업표를 삭제한 다음 새 작업표를 생성해야 합니다. 자세한 내용은 [Adobe Workfront에서 작업표 삭제](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) 및 [작업표 수동으로 생성](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 시스템 전체에서 사용할 작업표 프로필을 만들거나 편집하는 경우 **작업표 및 시간**.

   또는

   그룹에 대한 작업표 프로필을 만들거나 편집하는 경우 **그룹**&#x200B;를 클릭한 다음 그룹 이름을 클릭합니다.

1. 클릭 **작업표 프로필**.
1. 새 작업표 프로필을 만들려면 **새 프로필**.

   또는

   기존 작업표 프로필을 편집하려면 편집할 작업표 프로필을 선택한 다음 **편집**.

   새 작업표 또는 기존 작업표 프로필이 표시됩니다.


1. 설정 **세부 정보 설정** 탭에서 다음을 입력합니다 **이름** 및 **설명** 작업표 프로필에 대해 다음 정보를 제공합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>관리 액세스를 가진 그룹</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>시스템 수준 작업표 프로필을 만드는 경우 이 필드를 비워 둡니다.</p> <p>사용자 계정을 편집할 수 있는 모든 사용자는 시스템 수준의 작업표를 다른 사용자에게 첨부할 수 있습니다.</p> <p>Workfront 관리자만 시스템 수준 작업표 프로필을 편집할 수 있습니다.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>관리하는 그룹에 대한 작업표 프로필을 만드는 경우 여기에서 그룹을 식별합니다.</p> <p>이렇게 해도 그룹의 사용자에게 작업표 프로필을 할당하지 않습니다. 작업표 프로필만 수정할 수 있습니다. 6단계에서 사용자에게 프로필을 할당합니다.</p> <p><b>메모</b>

   그룹 외부의 사용자가 작업표 프로필을 다른 사용자에게 첨부하면 이 작업표 프로필을 보거나 첨부할 수 없습니다.</p> </li>
   </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>타임시트 만들기</strong> </td> 
      <td> <p> <p>작업표 프로필에서 작업표를 생성할 시기를 지정합니다. 작업표는 주간, 격주, 반월별 또는 월별 기준으로 자동으로 생성되도록 설정할 수 있습니다. 작업표를 작성할 요일을 선택합니다.</p> <p><b>메모</b>

   금요일에 작업표를 만들도록 작업표 프로필을 구성하면 사용자는 금요일, 토요일, 일요일에 현재 주의 시간을 기록할 수 없습니다.</p> <p>Workfront은 항상 한 번에 두 개의 작업표를 만듭니다. 첫 번째 작업표는 항상 현재 날짜를 포함하며 첫 번째 작업표의 시간대가 종료되면 두 번째 작업표가 시작됩니다.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>승인자</strong></p> </td> 
      <td> <p> <p>승인자는 작업표와 연관된 사용자의 작업표를 승인하는 사용자입니다. 작업표에서 최대 7명의 사용자를 승인자로 식별할 수 있습니다. 여러 사용자를 식별하는 것은 누군가가 부재 중일 때 승인자를 사용할 수 있도록 하는 데 유용합니다. 사용자가 승인을 위해 작업표를 제출하면 모든 승인자에게 알림이 표시됩니다. 작업표를 승인하려면 한 명의 사용자만 작업표를 승인해야 합니다.</p> <p>작업표 관리 권한이 있는 사용자만 승인자로 설정할 수 있습니다. 작업표 관리 권한에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> <p>드롭다운 메뉴를 사용하여 작업표에 대한 승인자를 선택합니다(승인자가 필요한 경우). 다음 옵션 중에서 선택할 수 있습니다.</p> 
      <ul> 
      <li><strong>없음</strong>: 작업표를 승인할 필요가 없습니다.</li> 
      <li><strong>관리자</strong>: 시스템에서 설정한 기본 승인자입니다. 이 경우, 관리자로 지정된 사용자가 승인을 위해 제출되면 작업표를 승인합니다.</li> 
      <li><strong>특정 사용자:</strong> 특정 사용자를 이름별로 작업표 승인자로 지정할 수 있습니다. 작업표에 여러 승인자가 있을 수 있습니다. 이 경우 승인자 중 한 명이 작업표를 승인하면 작업표가 작업표로 표시됩니다 <strong>닫힘</strong> 나머지 모든 승인자의 작업표 승인 목록에서 사라집니다.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>시간을 편집할 수 있음 </strong> </td> 
      <td> <p> <p>승인자가 작업표에서 시간을 편집할 수 있도록 하려면 이 옵션을 선택합니다.

   이 옵션은 **소유자 및 관리자로 작업표 편집 제한** 설정 > 작업표 및 시간 > 기본 설정 영역에서 설정합니다. 자세한 내용은 <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">작업표 및 시간 환경 설정 구성</a>.

   다음 시나리오가 있습니다.

   <ul>
      <li>이 <b>소유자 및 관리자로 작업표 편집 제한</b> 옵션이 활성화됨:</li>
      <ul><li>승인자는 작업표를 승인하거나 거부할 수 있습니다. <b>시간 편집 가능</b> 이 활성화되어 있거나 활성화되어 있지 않습니다. </li>
      <li>작업표 소유자 관리자는 직접 보고서의 작업표만 볼 수 있습니다.</li></ul>
      <li>이 <b>소유자 및 관리자로 작업표 편집 제한</b> 옵션을 사용하지 않습니다.</li>
    <ul><li>이 <b>시간 편집 가능</b> 이 활성화되면 승인자가 작업표를 제출, 다시 열기 또는 닫고 시간을 편집할 수 있습니다.</li>
      <li>이 <b>시간 편집 가능</b> 이 비활성화되어 있으면 승인자가 작업표를 제출, 다시 열기 또는 닫을 수 없으며 시간을 편집할 수 없습니다. 승인자는 작업표를 승인하거나 거부할 수만 있습니다. </li>
      <li>작업표 소유자 관리자는 직접 보고서의 작업표를 제출, 회수, 다시 열고 편집할 수 있습니다.</li></ul>
      </ul>

   <p><b>메모</b>

   승인을 위한 작업표를 제출하면 더 이상 시간을 편집할 수 없습니다. 제출된 작업표를 편집 가능한 상태로 반환하려면 작업표를 회수하거나 승인자가 작업표를 거부하도록 하십시오. 자세한 내용은 <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">승인을 위한 작업표 제출</a> 및<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">작업표 승인</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>사용 가능한 시간 유형</strong> </td> 
      <td>기본적으로 사용자는 작업표에 대한 모든 일반 시간을 볼 수 있습니다. 그러나 특정 사용자 집합에 대해 특정 일반 시간만 표시하려는 경우에는 이 필드의 작업표 프로필에서 해당 시간을 선택하여 작업표에 표시해야 하는 일반 시간을 선택할 수 있습니다. 모든 일반 시간을 사용하지 않으려면 일반 시간 동안 섹션 없이 작업표를 생성하려면 모든 시간 유형을 선택 취소합니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">초과 작업</span> </td> 
      <td>작업표에서 초과 작업 시간 상자를 숨기도록 선택할 수 있습니다. 이 옵션은 기본적으로 비활성화됩니다.</td> 
     </tr> 
    </tbody> 
    </table>

1. 을(를) 클릭합니다. **사람 할당** 작업표 프로필을 특정 사용자, 그룹 또는 (Workfront 관리자인 경우) 팀과 연결하는 탭입니다. 사용자, 그룹 또는 팀의 이름을 입력하고 드롭다운 목록에 나타나면 클릭합니다.

   그룹 관리자인 경우, 작업표 프로필을 관리하는 그룹에 할당할 수 있지만 팀에 할당할 수는 없습니다. 자세한 내용은 [작업표 프로필을 할당하는 그룹 관리자의 제한 사항](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) 참조하십시오.

   >[!NOTE]
   >
   >* 사용자 프로필을 편집하여 사용자를 작업표 프로필에 연결할 수도 있습니다. 자세한 내용은 [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* 그룹을 추가하면 그룹 구성원 목록이 아니라 [사용자 지정] 탭에 그룹 이름만 나타납니다. 여기에 나열된 그룹 구성원을 보려면 변경 내용 저장을 클릭한 다음 방금 만든 작업표 프로필의 이름을 클릭합니다.
   >* 이 단계를 완료하면 작업표 프로파일에서 지정된 사용자 또는 그룹 구성원에 대해서만 작업표를 생성합니다. 지정된 사용자 또는 그룹 구성원에게 현재 기간에 대한 작업표가 없습니다.


1. 클릭 **변경 내용 저장**.

   작업표 프로필에서 작업표를 처음 생성하면 각 사용자에 대해 작업표가 2개 생성됩니다. 그런 다음 새 작업표를 생성할 때마다 작업표에서 사용자별로 작업표가 만들어집니다.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## 작업표 프로필을 할당하는 그룹 관리자의 제한 사항 {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

그룹 관리자이고 액세스 수준에서 작업표 및 시간 관리 액세스 옵션을 사용할 수 없는 경우 작업표 프로필을 만들 수 있지만 다음과 같은 경우에만 지정할 수 있습니다.

* 관리하는 그룹
* 관리하는 그룹에 있는 사용자를 편집할 수 있는 액세스 권한이 있는 개별 사용자

이러한 그룹 및 사용자의 경우 작업표 프로필에서 생성하는 작업표에 액세스할 수 없습니다.

또한 액세스 수준에서 사용자 관리자(그룹 사용자) 옵션이 비활성화되어 있으면, 관리하는 그룹에 작업표 프로필을 할당할 수 있지만, 편집할 수 있는 액세스 권한이 있는 그룹의 사용자만 영향을 받습니다. 그룹에 편집할 수 있는 액세스 권한이 없는 사용자가 포함되어 있으면 그룹의 나머지 사용자와 함께 작업표 프로필이 할당되지 않습니다.

액세스 수준의 작업표 및 시간 옵션에 대한 자세한 내용은 [특정 영역에 대한 관리자 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

액세스 수준의 사용자 관리자(사용자 그룹) 옵션에 대한 자세한 내용은 [사용자에게 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## 여러 반복 작업표 프로필

다음과 같은 경우 조직의 작업표 프로필을 두 개 이상 보유할 수 있습니다.

* 다양한 사용자 세트에 대한 고유한 지급 기간
* 여러 사용자 집합에 대한 고유한 승인자
* 다양한 사용자 세트에 대한 고유한 일반 시간 요구 사항

한 번에 두 명 이상의 작업표 프로필과 연결할 수 없습니다. 
