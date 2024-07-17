---
user-type: administrator
product-area: system-administration;user-management
keywords: 그룹,환경 설정,작업,그룹,문제,잠금 해제
navigation-topic: create-and-manage-groups
title: 그룹에 대한 타임시트 및 시간 환경 설정 구성
description: 시스템 수준에서 Adobe Workfront 관리자는 타임시트 및 시간 환경 설정 섹션의 잠금을 해제할 수 있습니다. 일반 환경 설정 및 타임시트 미리 채우기 이를 통해 그룹 관리자는 해당 섹션의 옵션을 자체 그룹에 대해 독립적으로 구성할 수 있습니다.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1379'
ht-degree: 1%

---

# 그룹에 대한 타임시트 및 시간 환경 설정 구성

Adobe Workfront 관리자는 시스템 수준에서 타임시트 및 시간 환경 설정의 다음 섹션을 잠금 해제하여 그룹 관리자가 고유한 그룹에 대해 독립적으로 구성할 수 있도록 할 수 있습니다.

* 일반 환경 설정
* 사용자가 시간을 기록할 수 있는 위치
* 타임시트 미리 채우기

관리하는 그룹 위에 그룹이 있는 경우 해당 관리자는 해당 그룹에 대해 이 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹)의 경우도 마찬가지입니다.

타임시트 및 시간 환경 설정 페이지의 다음 섹션은 시스템 수준에서만 구성할 수 있으며 그룹에 대해 잠금 해제할 수 없습니다.

* 삭제된 프로젝트, 작업 및 문제

Workfront 관리자가 타임시트 및 시간 환경 설정을 잠금 해제하는 방법에 대한 자세한 내용은 문서 [타임시트 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)의 [그룹에 대한 타임시트 및 시간 환경 설정 잠금 해제](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) 섹션을 참조하십시오.

>[!TIP]
>
>프로젝트 환경 설정, 작업 및 문제 환경 설정에 대해서도 그룹 수준 구성이 가능합니다. 자세한 내용은 [그룹에 대한 프로젝트 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 및 [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront 플랜*</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> <p>그룹의 그룹 관리자 또는 Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a> 및 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>를 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜 또는 라이선스 유형을 확인해야 하는 경우 Workfront 관리자에게 문의하십시오.

+++

## 그룹 타임시트 및 시간 환경 설정

그룹에 대해 잠금 해제된 타임시트 또는 시간 환경 설정 구성에 대한 다음 정보를 고려하십시오.

* 그룹 관리자이고 그룹에 대한 타임시트 또는 시간 환경 설정을 구성하는 경우 그룹을 홈 그룹으로 사용하는 사람에게 영향을 줍니다.
* 일반적으로 잠금 해제된 환경 설정은 무기한 잠금 해제된 상태로 유지됩니다. Workfront 관리자가 다시 잠근 경우 시스템 설정이 다시 적용되며 그룹 관리자가 설정한 기본 설정이 손실됩니다.
* 타임시트는 타임시트 소유자의 홈 그룹에 대해 구성된 타임시트 및 시간 환경 설정을 상속합니다.

  <!--
  Add example here?
  -->

* Workfront 관리자가 시스템 수준에서 환경 설정을 잠금 해제하고 그룹에 대해 구성한 후에는 그룹의 모든 사용자가 동일한 구성을 사용하도록 잠글 수 있습니다. 이는 Workfront 관리자가 시스템 내의 모든 사용자에 대한 환경 설정을 구성하고 잠그는 기능과 병행됩니다. 자세한 내용은 [그룹 타임시트 및 시간 환경 설정 잠금 또는 잠금 해제](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md)를 참조하십시오.

## 그룹에 대해 잠금 해제된 타임시트 또는 시간 환경 설정 구성

>[!TIP]
>
>Workfront 관리자인 경우 설정 > 타임시트 및 시간 > 환경 설정으로 이동한 다음 페이지 상단에 있는 상자에서 그룹 이름을 검색하여 1-4단계를 건너뛸 수 있습니다.

1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png)을(를) 클릭합니다.

1. 타임시트 또는 시간 환경 설정을 구성할 그룹의 이름을 클릭합니다.
1. 왼쪽 패널에서 **타임시트 및 시간**&#x200B;을 클릭합니다.

1. 표시되는 페이지에서 **일반 환경 설정** 섹션에서 다음 옵션을 구성합니다.

   >[!TIP]
   >
   >환경 설정 위로 마우스를 가져가면 도구 설명이 표시되어 잠겨 있음을 알려주는 경우, Workfront 관리자에게 조직의 모든 그룹에 대해 잠금을 해제하도록 요청할 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">미래 날짜에 대한 시간 기록</td> 
      <td> <p>사용자가 시스템 전체에서 미래 날짜에 대한 시간을 기록할 수 있도록 해줍니다.</p> 
       <ul> 
       <li>프로젝트의 그룹에 관계없이 로그 시간에 액세스할 수 있는 모든 프로젝트, 작업 및 문제</li> 
       <li>일반 시간으로서의 타임시트</li>
       </ul> 
       <p>이 기능은 사용자가 사무실을 비울 예정이고 해당 시간을 미리 기록하려는 경우 유용합니다.</p> 
       <p><b>참고</b>: 사용자가 닫히거나 취소한 작업 또는 문제에 시간을 기록하지 못하도록 할 수 없습니다. 사용자가 완료 또는 중단된 프로젝트에 시간을 기록하지 못하도록 할 수만 있습니다. 작업 및 문제 목록에서 필터를 사용하여 완료되거나 취소된 작업을 사용자가 볼 수 없도록 제외하는 것이 좋습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">타임시트의 경비 추가</td> 
      <td> <p>사용자가 타임시트에 시간과 비용을 모두 기록할 수 있습니다.</p> 
      <p>그룹에 대해 이 환경 설정을 활성화하고 그룹을 특정 사용자의 홈 그룹으로 설정하면 해당 사용자의 타임시트의 프로젝트 및 작업 옆에 경비 아이콘이 표시됩니다. 사용자는 이 아이콘을 클릭하여 프로젝트 또는 작업에 대한 비용을 추가하거나 편집할 수 있습니다.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">시간 항목에 수동으로 작업 역할 할당</td> 
      <td> <p>사용자가 사용자 프로필에 할당되거나 객체에 할당된 작업 역할을 수동으로 선택할 수 있습니다.</p> <p><b>중요</b>:  
        <ul> 
         <li>작업 역할을 시간 항목에 할당한 후 이 설정을 사용하지 않으면 사용자는 프로젝트, 작업 또는 문제의 시간 탭에서 다양한 역할에 기록된 시간을 조정해야 합니다.</li> 
         <li>사용자의 프로필에 작업 역할이 할당되어 있지 않고 고급 할당 대화 상자에 작업 소유자로 할당된 작업이 있는 경우 사용자가 작업에 시간을 기록할 때 해당 작업 역할이 표시됩니다.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">타임시트 편집을 소유자 및 관리자로 제한</td> 
      <td> <p>프로젝트 그룹 및 Workfront 관리자에 관계없이 타임시트 소유자로 편집을 제한합니다. 이 옵션이 비활성화되면 타임시트는 다음 작업으로도 편집할 수 있습니다.</p> 
       <ul> 
        <li> <p>타임시트에 대한 관리 액세스 권한과 액세스 수준의 시간이 있는 사용자</p> </li> 
        <li> <p>타임시트에서 "시간 편집 가능"이 활성화된 경우 타임시트 승인자</p> </li> 
        <li> <p>타임시트 소유자의 관리자</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">시간 편집을 소유자 및 관리자로 제한</td> 
      <td>시간을 입력한 사용자 및 Workfront 관리자로 편집을 제한합니다. 이 설정은 프로젝트 또는 시간 보고서의 시간 탭에 적용됩니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. **사용자가 시간을 기록할 수 있는 위치** 섹션에서 다음 옵션을 구성합니다.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">프로젝트에 직접 시간 기록</td> 
      <td>사용자가 프로젝트의 시간을 기록할 수 있습니다( 업데이트 탭과 타임시트 모두). 프로젝트 수준에서 사용자의 기록 시간을 제한하려면 이 옵션을 선택하지 않은 상태로 두십시오.</td>
     </tr>
     <tr>
      <td role="rowheader">완료된 프로젝트에 시간 기록</td>
      <td>사용자가 완료로 표시된 프로젝트의 시간을 기록할 수 있습니다. 이 옵션이 비활성화되면 사용자는 완료 상태의 프로젝트에서 완료한 작업의 시간을 기록할 수 없습니다.</td>
     </tr>
     <tr>
      <td role="rowheader">중단된 프로젝트에 시간 기록</td> 
      <td>이 옵션이 활성화되면 사용자는 중단 상태인 프로젝트에 시간을 기록할 수 있습니다.</td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >이 환경 설정은 사용자의 홈 그룹 환경 설정 구성을 기반으로 적용됩니다. 이러한 설정을 사용자의 홈 그룹 환경 설정에서 활성화하면 프로젝트의 그룹 환경 설정에서 허용하는지 여부에 관계없이 완료된 프로젝트나 중단된 프로젝트를 포함하여 프로젝트에 직접 시간을 기록할 수 있습니다.

1. **타임시트 미리 채우기** 섹션에서 다음 옵션을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">타임시트의 작업 범위 &lt;주 수&gt; 내에 있는 작업</td> 
      <td> <p>사용자에게 할당된 작업 및 문제의 날짜가 포함된 타임시트의 날짜 범위 전후 주 수를 정의합니다. 기본 설정은 1주이며 이 범위를 4주로 확장할 수 있습니다. 즉, 범위에 대해 4주를 선택하는 경우, 타임시트의 일자 범위 전 4주부터 타임시트의 일자 범위 후 4주까지의 일자 범위가 있는 작업 및 문제로 타임시트가 미리 채워집니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">완료된 작업 및 문제</td> 
      <td>일반적으로 여러 리소스가 단일 작업에 할당되는 경우 이 설정을 사용하는 것이 좋습니다. 즉, 한 리소스가 작업에 시간을 기록하고 완료로 표시하면 작업에 할당된 다른 리소스가 여전히 타임시트에서 작업 또는 문제를 찾아 시간을 기록할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">타임시트의 일자 범위에 계획된 일자가 있는 작업 및 문제</td> 
      <td> <p>선택한 경우 타임시트에는 타임시트의 날짜 범위에 계획된 시작 일자 또는 완료 일자가 있는 작업 및 문제가 포함됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> 타임시트의 일자 범위 내에 예상 일자가 있는 작업</td> 
      <td> <p>이 옵션을 선택하면 문제나 작업의 계획된 일자가 타임시트 일자 범위를 벗어나는 경우에도 프로젝트의 기간 내에 예상 시작 일자 또는 완료 일자가 있는 작업이 타임시트에 포함됩니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.
