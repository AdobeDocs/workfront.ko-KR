---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 단일 사용 작업표 만들기
description: 반복되지 않는 작업표를 원하는 경우 단일 사용 작업표를 수동으로 만들 수 있습니다. 작업표의 종료 날짜에 도달하여 작업표가 더 필요한 경우에는 새 작업표를 만들어야 합니다.
author: Alina
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 1%

---

# 단일 사용 작업표 만들기

반복되지 않는 작업표를 원하는 경우 단일 사용 작업표를 수동으로 만들 수 있습니다. 작업표의 종료 날짜에 도달하여 작업표가 더 필요한 경우에는 새 작업표를 만들어야 합니다.

사용자의 추가 작업 없이 사용자의 반복 작업표를 생성하는 작업표 프로필을 만드는 방법에 대한 자세한 내용은(권장) [작업표 프로필 만들기, 편집 및 할당](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

>[!NOTE]
>
>* 그룹에 대해 단일 사용 작업표를 만들 수 없습니다.

>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* 단일 사용 작업표를 만들 때는 작업표에 포함할 특정 일반 시간 형식을 선택할 수 없습니다. 시스템에서 활성화된 모든 일반 시간 유형은 수동으로 만든 작업표에 표시됩니다.
>
>  작업표에 표시할 특정 일반 시간 유형만 선택하려면 작업표 프로필을 사용하십시오. 작업표 프로필에 대한 자세한 내용은 [작업표 프로필 만들기, 편집 및 할당](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

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
   <td> <p>작업표에 대한 관리자 액세스 권한이 있어야 합니다. </p> <p>자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> <p><b> 메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 단일 사용 작업표 만들기

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

1. 클릭 **작업표**. 다음 **모두** 기본적으로 필터가 선택되어 있습니다. 뷰에 액세스할 수 있는 모든 작업표가 표시됩니다.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (선택 사항) 작업표 목록에서 필터를 업데이트하려면 다음 중 하나를 수행하십시오.

   * 선택 **내 작업표 승인** 페이지의 오른쪽 위 모서리에서 사용자가 승인한 작업표만 볼 수 있습니다.

      또는

      선택 **내 작업표** 작업표만 표시합니다.

      작업표 목록에 내 작업표 승인 또는 내 작업표 필터가 적용됩니다.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 필터 아이콘을 클릭합니다 ![](assets/filter-nwepng.png) 다른 필터를 적용하거나 새 필터를 만듭니다. 필터 만들기 또는 업데이트에 대한 자세한 내용은 [Adobe Workfront에서 필터 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 설정 영역의 목록 컨트롤 또는 레이아웃 서식 파일에서 내 작업표 승인 및 내 작업표 필터를 제거한 경우 작업표 목록 맨 위나 필터 목록에 내 작업표 승인 및 내 작업표 옵션이 표시되지 않습니다. 자세한 내용은 다음 문서를 참조하십시오.
   > 
   >   * [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)



1. (선택 사항) **검색** 아이콘 ![](assets/search-icon.png) 키워드를 입력하고 특정 작업표를 검색하려면 예를 들어 소유자 이름의 작업표 기간을 검색할 수 있습니다.

1. (선택 사항) **보기** ![](assets/view-icon.png) 또는 **그룹화** ![](assets/grouping.png) 아이콘을 사용하여 다른 보기나 그룹을 적용하거나 새 보기를 만들 수 있습니다.

   필터, 보기 또는 그룹화를 만드는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront에서 필터 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfront에서 보기 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfront에서 그룹화 만들기](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 클릭 **새 작업표** 작업표 목록 맨 위에 있습니다.

   다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>다음에 대한 타임시트 만들기:</strong> </td> 
      <td>작업표를 만들 사용자 이름, 작업 역할 또는 팀의 이름을 입력하고 목록에 표시할 때 클릭합니다.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>시작일</strong> </td> 
      <td>작업표의 시작 날짜입니다.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>종료 일자</strong> </td> 
      <td> 작업표의 종료 날짜입니다.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>승인자</strong> </td> 
      <td>승인자는 작업표와 연관된 사용자의 작업표를 승인하는 사용자입니다. 작업표 관리 권한이 있는 사용자만 승인자로 설정할 수 있습니다. 작업표 관리 권한에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.<br>작업표 승인자의 이름을 입력하고 목록에 나타나면 클릭합니다.<br>작업표에 여러 승인자가 있을 수 있습니다. 이 경우 승인자 중 한 명이 작업표를 승인하면 작업표가 작업표로 표시됩니다 <strong>닫힘</strong> 나머지 모든 승인자의 작업표 승인 목록에서 사라집니다.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>시간을 편집할 수 있음</strong> </td>

   <td> <p>승인자가 작업표에서 시간을 편집할 수 있도록 하려면 이 옵션을 선택합니다.</p>

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

   승인을 위한 작업표를 제출하면 더 이상 시간을 편집할 수 없습니다. 제출된 작업표를 편집 가능한 상태로 반환하려면 작업표를 회수하거나 승인자가 작업표를 거부하도록 하십시오. 자세한 내용은 <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">승인을 위한 작업표 제출</a> 및 <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">작업표 승인</a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">초과 작업</span> </td> 
      <td>작업표에서 초과 작업 시간 상자를 숨기도록 선택할 수 있습니다. 이 옵션은 기본적으로 비활성화됩니다.</td> 
      </tr> 
      </tbody> 
   </table>

1. 클릭 **작업표 만들기**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## 작업 및 문제가 사용자의 작업표에 나타나는 경우

작업이나 문제가 다음 기준을 충족하면 사용자에게 할당된 작업이나 문제가 사용자의 작업표에 자동으로 나타납니다.

* 사용자가 작업 또는 문제에 대해 로그온한 시간
* 작업이나 문제의 계획된 날짜가 작업표 날짜 내에 포함됩니다
* 작업 또는 문제에 실제 시작 날짜가 있습니다(작업 또는 문제 상태가 진행 중).
* 작업표 또는 문제가 작업표에 고정되어 있습니다
* 계획된 완료 날짜가 작업표의 날짜 범위 내에 있고 상태는 진행 중입니다.

만약 **작업표를 ... 로 미리 채웁니다.** 작업표 및 시간 기본 설정에 있는 기본 설정이 선택 취소되어 작업표에 진행 중 상태가 있는 문제와 작업이 표시됩니다. 작업표 및 시간 기본 설정에 대한 자세한 내용은 [작업표 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
