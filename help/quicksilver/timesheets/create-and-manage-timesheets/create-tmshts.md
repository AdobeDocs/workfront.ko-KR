---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 일회용 타임시트 만들기
description: 반복되지 않는 타임시트를 원하는 경우 일회용 타임시트를 수동으로 만들 수 있습니다. 타임시트의 종료 날짜에 도달하여 더 많은 타임시트가 필요한 경우 새 타임시트를 만들어야 합니다.
author: Lisa
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1062'
ht-degree: 0%

---

# 일회용 타임시트 만들기

<!--Audited: 6/2025-->

반복되지 않는 타임시트를 원하는 경우 일회용 타임시트를 수동으로 만들 수 있습니다. 타임시트의 종료 날짜에 도달하여 더 많은 타임시트가 필요한 경우 새 타임시트를 만들어야 합니다.

사용자의 추가 개입 없이 사용자의 반복 타임시트를 생성하는 타임시트 프로필 만들기에 대한 자세한 내용은 [타임시트 프로필 만들기, 편집 및 할당](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)을 참조하십시오.

타임시트 프로필과 연결된 시스템의 모든 사용자에 대해 타임시트를 수동으로 생성하는 방법에 대한 자세한 내용은 [타임시트 수동으로 생성](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)을 참조하십시오.

>[!NOTE]
>
>* 그룹에 대해 일회용 타임시트를 만들 수 없습니다.
>* 일회용 타임시트를 만드는 경우 타임시트에 포함할 특정 일반 시간 유형을 선택할 수 없습니다. 시스템에서 활성화된 모든 일반 시간 유형이 수동으로 생성된 타임시트에 표시됩니다.
>
>타임시트에 표시할 특정 일반 시간 유형만 선택하려면 타임시트 프로필을 사용하십시오. 타임시트 프로필에 대한 자세한 내용은 [타임시트 프로필 만들기, 편집 및 할당](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)을 참조하세요.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td>
   <p>표준</p>
   <p>플랜</p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td><p>타임시트에 대한 관리 액세스</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 일회용 타임시트 만들기

{{step1-to-timesheets}}

기본적으로 **모두** 필터가 선택되어 있습니다. 보기 액세스 권한이 있는 모든 타임시트가 표시됩니다.

타임시트가 하나 선택된 ![타임시트 목록](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (선택 사항) 다음 중 하나를 수행하여 타임시트 목록의 필터를 업데이트합니다.

   * 승인한 타임시트만 보려면 페이지의 오른쪽 상단에서 **내 타임시트 승인**&#x200B;을 선택하십시오.

     또는

     내 타임시트만 보려면 **내 타임시트**&#x200B;를 선택하십시오.

     내 타임시트 승인 또는 내 타임시트 필터가 타임시트 목록에 적용됩니다.

     ![타임시트 목록 페이지의 내 타임시트 필터 단추](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * **필터** 아이콘 ![필터 아이콘](assets/filter-nwepng.png)을 클릭하여 다른 필터를 적용하거나 새 필터를 만드십시오. 필터 만들기 또는 업데이트에 대한 자세한 내용은 [Adobe Workfront에서 필터 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)을 참조하세요.

   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 설정 영역의 목록 컨트롤 또는 레이아웃 템플릿에서 내 타임시트 승인 및 내 타임시트 필터를 제거한 경우 내 타임시트 승인 및 내 타임시트 옵션이 타임시트 목록 맨 위나 필터 목록에 표시되지 않습니다. 자세한 내용은 다음 문서를 참조하십시오.
   > 
   >   * [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (선택 사항) **검색** 아이콘 ![검색 아이콘](assets/search-icon.png)을 클릭하여 키워드를 입력하고 특정 타임시트를 검색합니다. 예를 들어 소유자 이름의 타임시트 시간대를 검색할 수 있습니다.

1. (선택 사항) **보기** ![보기 아이콘](assets/view-icon.png) 또는 **그룹화** ![그룹화 아이콘](assets/grouping.png) 아이콘을 클릭하여 다른 보기 또는 그룹화를 적용하거나 새 보기를 만듭니다.

   필터, 보기 또는 그룹화 만들기에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront에서 필터 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfront에서 보기 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfront에서 그룹화 만들기](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 타임시트 목록 맨 위에 있는 **새 타임시트**&#x200B;를 클릭합니다.

   다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>다음에 대한 타임시트 만들기</strong> </td> 
      <td>타임시트를 만들 사용자, 작업 역할 또는 팀의 이름을 입력하고 목록에 표시될 때 클릭합니다.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>시작 날짜</strong> </td> 
      <td>타임시트의 시작 날짜입니다.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>종료 날짜</strong> </td> 
      <td> 타임시트의 종료 날짜입니다.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>승인자</strong> </td> 
      <td>승인자는 타임시트와 연계된 사용자에 대해 타임시트를 승인하는 사용자입니다. 타임시트 관리 권한이 있는 사용자만 승인자로 설정할 수 있습니다. 타임시트 관리 권한에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>를 참조하십시오.<br>타임시트 승인자의 이름을 입력하고 목록에 나타나면 클릭합니다.<br>타임시트에 여러 승인자가 있을 수 있습니다. 이 경우 승인자 중 한 명이 타임시트를 승인하면 타임시트가 <strong>마감됨</strong>(으)로 표시되고 나머지 모든 승인자의 타임시트 승인 목록에서 사라집니다.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>시간을 편집할 수 있음</strong> </td>

   <td> <p>승인자가 타임시트의 시간을 편집할 수 있도록 하려면 이 옵션을 선택합니다.</p>

   이 옵션은 설정 > 타임시트 및 시간 > 환경 설정 영역에서 **타임시트 편집을 소유자 및 관리자로 제한** 설정과 함께 작동합니다. 자세한 내용은 <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">타임시트 및 시간 환경 설정 구성</a>을 참조하십시오.

   다음과 같은 시나리오가 있습니다.

   <ul>
      <li><b>타임시트 편집을 소유자 및 관리자로 제한</b> 옵션이 활성화된 경우:</li>
   <ul><li>승인자는 <b>시간 편집 가능</b>의 사용 여부와 관계없이 타임시트만 승인하고 거부할 수 있습니다. </li>
   <li>타임시트 소유자의 관리자는 부하 직원의 타임시트만 볼 수 있습니다.</li></ul>
   <li><b>타임시트 편집을 소유자 및 관리자로 제한</b> 옵션이 비활성화된 경우:</li>
   <ul><li><b>시간을 편집할 수 있음</b>을 사용하도록 설정하면 승인자가 타임시트를 제출하거나 다시 열거나 닫을 수 있으며 시간을 편집할 수 있습니다.</li>
   <li><b>시간을 편집할 수 있음</b>을 사용하지 않도록 설정하면 승인자가 타임시트를 제출하거나 다시 열거나 닫을 수 없으며 시간을 편집할 수 없습니다. 승인자는 타임시트만 승인하거나 거부할 수 있습니다. </li>
   <li>타임시트 소유자의 관리자는 부하 직원의 타임시트를 제출, 회수, 다시 열고 편집할 수 있습니다.</li></ul>
   </ul>

   <p><b>메모</b>

   승인을 위해 타임시트를 제출하면 더 이상 시간을 편집할 수 없습니다. 제출된 타임시트를 편집 가능한 상태로 되돌리려면 타임시트를 불러오거나 승인자가 타임시트를 거부하도록 하십시오. 자세한 내용은 <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">승인을 위한 타임시트 제출</a> 및 <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">타임시트 승인</a>을 참조하세요.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">초과 작업 시간</span> </td> 
      <td>타임시트에서 초과 작업 시간 상자를 숨기도록 선택할 수 있습니다. 이 옵션은 기본적으로 비활성화되어 있습니다.</td> 
      </tr> 
      </tbody> 
   </table>

1. **타임시트 만들기**&#x200B;를 클릭합니다.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## 사용자의 타임시트에 작업 및 문제가 표시되는 경우

사용자에게 할당된 작업 또는 문제가 다음 기준을 충족하면 사용자의 타임시트에 자동으로 표시됩니다.

* 사용자가 작업 또는 문제에 시간을 기록했습니다.
* 작업 또는 문제의 계획된 일자가 타임시트의 일자 내에 있습니다.
* 작업 또는 문제의 실제 시작 일자(작업 또는 문제 상태가 진행 중)가 있습니다.
* 작업 또는 문제가 타임시트에 고정됨
* 계획된 완료 일자가 타임시트의 일자 범위에 속하며 상태는 진행 중입니다.

**타임시트를 ...** 환경 설정(타임시트 및 시간 환경 설정에 있음)을 선택 취소한 경우 타임시트에 진행 중 상태의 문제와 작업이 표시됩니다. 타임시트 및 시간 환경 설정에 대한 자세한 내용은 [타임시트 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)을 참조하십시오.
