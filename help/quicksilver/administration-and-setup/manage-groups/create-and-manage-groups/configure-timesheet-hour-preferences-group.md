---
user-type: administrator
product-area: system-administration;user-management
keywords: 그룹,환경 설정,작업,그룹,문제,잠금 해제
navigation-topic: create-and-manage-groups
title: 그룹에 대한 작업표 및 시간 환경 설정 구성
description: 시스템 수준에서 Adobe Workfront 관리자는 작업표 및 시간 기본 설정 섹션의 잠금을 해제하고 작업표를 미리 채울 수 있습니다. 이렇게 하면 그룹 관리자가 해당 섹션의 옵션을 해당 그룹에 대해 독립적으로 구성할 수 있습니다.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: df55d6659fac7588610bc05ea0380a766b4277a2
workflow-type: tm+mt
source-wordcount: '1368'
ht-degree: 6%

---

# 그룹에 대한 작업표 및 시간 환경 설정 구성

Adobe Workfront 관리자는 시스템 수준에서 작업표 및 시간 환경 설정의 다음 섹션을 잠금 해제할 수 있으므로 그룹 관리자가 자신의 그룹에 대해 독립적으로 구성할 수 있습니다.

* 일반 환경 설정
* 사용자가 시간을 기록할 수 있는 위치
* 작업표 미리 채우기

관리하는 그룹 위에 그룹이 있으면 해당 관리자가 사용자 그룹을 위해 이 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹의 경우)도 마찬가지입니다.

작업표 및 시간 기본 설정 페이지의 다음 섹션은 시스템 수준에서만 구성할 수 있으며 그룹의 잠금을 해제할 수 없습니다.

* 삭제된 프로젝트, 작업 및 문제

Workfront 관리자가 작업표 및 시간 기본 설정을 잠금 해제하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [그룹에 대한 작업표 및 시간 환경 설정 잠금 해제](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) 기사 [작업표 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

>[!TIP]
>
>프로젝트 환경 설정, 작업 및 문제 환경 설정에 대해 그룹 수준의 구성이 가능합니다. 자세한 내용은 [그룹에 대한 프로젝트 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 및 [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront 플랜*</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> <p>그룹의 그룹 관리자 또는 Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a> 및 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 찾아야 하는 경우 Workfront 관리자에게 문의하십시오.

## 작업표 및 시간 환경 설정 그룹화

잠긴 작업표 또는 그룹에 대한 시간 기본 설정을 구성하는 방법에 대한 다음 정보를 고려하십시오.

* 그룹 관리자이고 그룹에 대한 작업표 또는 시간 기본 설정을 구성하는 경우 해당 그룹을 홈 그룹으로 사용하는 사용자에게 영향을 줍니다.
* 일반적으로 잠금 해제된 환경 설정은 무한정 잠금 해제된 상태로 유지됩니다. Workfront 관리자가 다시 잠근 경우 시스템 설정이 다시 적용되며 그룹 관리자가 만든 기본 설정에 대한 설정이 손실됩니다.
* 작업표는 작업표 소유자의 홈 그룹에 대해 구성된 작업표와 시간 기본 설정을 상속합니다.

   <!--
  Add example here?
  -->

* Workfront 관리자가 시스템 수준에서 환경 설정을 잠금 해제하고 그룹에 대해 구성한 후 해당 그룹을 잠그면 사용자 그룹 아래의 그룹이 동일한 구성을 사용하고 있는지 확인할 수 있습니다. 이는 Workfront 관리자가 시스템의 모든 사용자에 대한 환경 설정을 구성하고 잠그던 기능과 병렬입니다. 자세한 내용은 [그룹 작업표 및 시간 기본 설정 잠금 또는 잠금 해제](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## 그룹에 대해 잠금 해제된 작업표 또는 시간 기본 설정을 구성합니다

>[!TIP]
>
>Workfront 관리자인 경우 설정 > 작업표 및 시간 > 환경 설정으로 이동한 다음 페이지 맨 위의 상자에서 그룹 이름을 검색하여 1-4단계를 무시하면 됩니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png).

1. 작업표 또는 시간 기본 설정을 구성할 그룹의 이름을 클릭합니다.
1. 왼쪽 패널에서 **작업표 및 시간**.

1. 표시되는 페이지에서 **일반 환경 설정** 섹션에서 다음 옵션 중 하나를 구성합니다.

   >[!TIP]
   >
   >마우스로 기본 설정을 가리키면 도구 설명이 표시되어 잠긴 상태임을 알 수 있는 경우 Workfront 관리자에게 조직의 모든 그룹에 대해 잠금을 해제하도록 요청할 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">앞으로의 일자에 대한 시간을 기록하십시오</td> 
      <td> <p>다음 위치에서 시스템 전체에서 향후 날짜에 대한 시간을 기록할 수 있습니다.</p> 
       <ul> 
       <li>프로젝트 그룹에 상관없이 로그 시간에 액세스할 수 있는 모든 프로젝트, 작업 및 문제</li> 
       <li>일반 시간으로 작업표</li>
       </ul> 
       <p>이 기능은 사용자가 사무실을 비울 계획이며 해당 시간을 미리 기록하려는 경우 유용합니다.</p> 
       <p><b>참고</b>: 사용자가 닫혀 있거나 취소된 작업이나 문제에 대해 시간을 기록하는 것을 방지할 수 없습니다. 사용자가 전체 또는 데드 프로젝트에 대한 시간을 기록하지 못하도록 할 수만 있습니다. 작업 및 문제 목록에서 필터를 사용하여 완료되었거나 취소된 작업이 사용자에게 표시되지 않도록 하는 것이 좋습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">타임시트의 경비를 추가하십시오</td> 
      <td> <p>작업표에 시간과 비용을 모두 기록할 수 있습니다.</p> 
      <p>그룹에 대해 이 기본 설정이 활성화되고 특정 사용자의 홈 그룹으로 설정된 경우 해당 사용자의 작업표에 있는 프로젝트 및 작업 옆에 비용 아이콘이 표시됩니다. 사용자는 이 아이콘을 클릭하여 프로젝트 또는 작업에 대한 비용을 추가하거나 편집할 수 있습니다.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업 역할을 시간 항목에 수동으로 할당하십시오</td> 
      <td> <p>사용자가 사용자 프로필에 할당되거나 객체에 할당된 작업 역할을 수동으로 선택할 수 있도록 허용합니다.</p> <p><b>중요 사항</b>:  
        <ul> 
         <li>작업 역할을 시간 항목에 할당한 후 이 설정을 비활성화하면 프로젝트, 작업 또는 문제의 시간 탭에 있는 다양한 역할에 기록된 시간을 조정해야 합니다.</li> 
         <li>사용자에게 프로파일에 할당된 작업 역할이 없고 [고급 할당] 대화 상자에 [작업 소유자]로 지정된 작업이 있는 경우 사용자가 작업 시간을 기록하면 해당 작업 역할이 나타납니다.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">타임시트 편집을 소유자 및 관리자로 제한합니다</td> 
      <td> <p>프로젝트 그룹 및 Workfront 관리자에 관계없이 작업표 소유자로 편집을 제한합니다. 이 옵션을 비활성화하면 작업표를 다음 방법으로 편집할 수도 있습니다.</p> 
       <ul> 
        <li> <p>작업표와 액세스 수준의 시간에 대한 관리자 액세스 권한이 있는 사용자</p> </li> 
        <li> <p>작업표에서 "시간 편집 가능"을 사용하는 경우 작업표 승인자</p> </li> 
        <li> <p>작업표 소유자의 관리자</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">시간 편집을 소유자 및 관리자로 제한합니다</td> 
      <td>시간을 입력한 사용자 및 Workfront 관리자로 편집을 제한합니다. 이 설정은 프로젝트 또는 시간 보고서의 시간 탭에 적용됩니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 에서 **사용자가 로그할 수 있는 위치** 섹션에서 다음 옵션 중 하나를 구성합니다.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">프로젝트에 직접 시간을 기록합니다</td> 
      <td>사용자가 프로젝트에서 로그할 수 있습니다( 업데이트 탭과 작업표 모두). 사용자가 프로젝트 수준에서 시간을 기록하지 못하도록 제한하려면 이 옵션을 선택 취소합니다.</td>
     </tr>
     <tr>
      <td role="rowheader">완료된 프로젝트에 시간을 기록하십시오</td>
      <td>사용자가 완료된 것으로 표시된 프로젝트에 시간을 기록할 수 있습니다. 이 옵션을 비활성화하면 사용자가 완료 상태의 프로젝트에서 완료한 작업에 대한 시간을 기록할 수 없습니다.</td>
     </tr>
     <tr>
      <td role="rowheader">중단된 프로젝트에 시간을 기록합니다</td> 
      <td>이 옵션이 활성화되면 사용자가 중단 상태로 프로젝트에 대한 시간을 기록할 수 있습니다.</td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >이 기본 설정은 사용자의 홈 그룹 기본 설정 구성에 따라 적용됩니다. 이러한 설정을 사용자의 홈 그룹 환경 설정에서 활성화하면 프로젝트의 그룹 환경 설정이 허용하는지 여부에 관계없이 완료되었거나 중단된 프로젝트를 포함하여 프로젝트에 직접 시간을 기록할 수 있습니다.

1. 에서 **작업표 미리 채우기** 섹션에서 다음 옵션 중 하나를 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">내에 있는 작업 &lt;number of="" weeks=""&gt; 작업표의 작업 범위</td> 
      <td> <p>사용자에게 할당된 작업 및 문제의 날짜가 포함된 작업표의 날짜 범위 전후의 주 수를 정의합니다. 기본 설정은 1주이며 이 범위를 4주로 확장할 수 있습니다. 즉, 작업표에 작업표의 날짜 범위 이전 4주 사이의 날짜가 있는 작업 및 문제로 미리 채워져 있습니다. 작업표의 날짜 범위 이후 최대 4주(해당 범위에 대해 4주를 선택하면) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">완료된 작업 및 문제</td> 
      <td>일반적으로 여러 리소스가 단일 작업에 할당되는 경우 이 설정을 사용하는 것이 좋습니다. 즉, 한 리소스가 작업에 대해 시간을 기록하고 완료된 것으로 표시하면 작업에 할당된 다른 리소스가 작업 또는 문제를 작업표에서 찾아 해당 시간을 기록할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">타임시트의 일자 범위 내에 계획된 일자가 있는 작업 및 문제입니다</td> 
      <td> <p>선택한 경우 작업표에 작업표의 날짜 범위 내에 있는 계획 시작 날짜나 완료 날짜가 있는 작업 및 문제가 포함됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> 타임시트의 일자 범위 내에 예상 일자가 있는 작업</td> 
      <td> <p>선택한 경우, 작업표에 예상 시작 날짜 또는 완료 날짜가 프로젝트의 시간 기간 내에 있는 작업이 포함되며, 해당 문제 또는 작업의 계획된 날짜가 작업표 날짜 범위를 벗어나는 경우에도 작업표에 포함된 작업이 포함됩니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.
