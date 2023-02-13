---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 작업표 정보 편집
description: 작업표에 대한 관리자 액세스 권한이 있는 사용자는 Adobe Workfront에서 기존 작업표에 대한 정보를 편집할 수 있습니다. 예를 들어 작업표의 소유자, 승인자 또는 기간을 편집할 수 있습니다.
author: Alina
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 2%

---

# 작업표 정보 편집

작업표에 대한 관리자 액세스 권한이 있는 사용자는 Adobe Workfront에서 기존 작업표에 대한 정보를 편집할 수 있습니다. 예를 들어 작업표의 소유자, 승인자 또는 기간을 편집할 수 있습니다.

단일 작업표에 대한 정보를 편집하거나 여러 작업표를 일괄로 편집할 수 있습니다.

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
   <td> <p>작업표에 대한 관리자 액세스 권한이 있어야 합니다. </p> <p>자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 작업표 편집

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **작업표**.

   다음 **모두** 기본적으로 필터를 선택하면 뷰할 수 있는 모든 작업표가 표시됩니다.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (선택 사항) **검색** 아이콘 ![](assets/search-icon.png) 키워드를 입력하고 특정 작업표를 검색합니다. 예를 들어 작업표 시간대나 소유자 이름을 검색할 수 있습니다.

1. (선택 사항) 작업표 목록에서 필터를 업데이트하려면 다음 중 하나를 수행하십시오.

   * 선택 **내 작업표 승인** 페이지의 오른쪽 위 모서리에서 사용자가 승인한 작업표만 볼 수 있습니다.

      또는

      선택 **내 작업표** 작업표만 표시합니다.

      작업표 목록에 내 작업표 승인 또는 내 작업표 필터가 적용됩니다.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 필터 아이콘을 클릭합니다 ![](assets/filter-nwepng.png) 다른 필터를 적용하거나 새 필터를 만듭니다. 필터 만들기 또는 업데이트에 대한 자세한 내용은 [Adobe Workfront에서 필터 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 설정 영역의 목록 컨트롤 또는 레이아웃 서식 파일에서 내 작업표 승인 및 내 작업표 필터를 제거한 경우 작업표 목록 맨 위나 필터 목록에 내 작업표 승인 및 내 작업표 옵션이 표시되지 않습니다. 자세한 내용은 다음 문서를 참조하십시오.
   * [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (선택 사항)**보기** ![](assets/view-icon.png) 또는 **그룹화** ![](assets/grouping.png) 아이콘을 사용하여 다른 보기나 그룹을 적용하거나 새 보기를 만들 수 있습니다.

   필터, 보기 또는 그룹화를 만드는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront에서 필터 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfront에서 보기 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfront에서 그룹화 만들기](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 작업표를 하나 또는 여러 개 선택한 다음 **편집** 아이콘 ![](assets/edit-icon.png) 작업표 목록의 맨 위에 있습니다.
1. 다음 정보를 보거나 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>소유자</strong> </td> 
      <td> <p>작업표를 만든 사용자의 이름입니다. 이 필드는 편집할 수 없습니다. </p> <p>여러 작업표를 선택하면 필드가 표시되지 않습니다. </p> </td> 
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
      <td> <p>승인자는 작업표와 연관된 사용자의 작업표를 승인하는 사용자입니다. 작업표에 대한 관리자 액세스 권한이 있는 사용자만 승인자로 설정할 수 있습니다. </p> <p>작업표 관리 권한에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> <p>작업표 승인자의 이름을 입력하고 목록에 표시될 때 선택합니다.</p> <p>작업표에 여러 승인자가 있을 수 있습니다. 이 경우 승인자 중 한 명이 작업표를 승인하면 작업표가 작업표로 표시됩니다 <strong>닫힘</strong> 나머지 모든 승인자의 작업표 승인 목록에서 사라집니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>시간을 편집할 수 있음</strong> </td> 
      <td> <p>승인자가 작업표에서 시간을 편집할 수 있도록 하려면 이 옵션을 선택합니다.</p> <p>여러 작업표를 선택하면 이 옵션을 사용할 수 없습니다. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">초과 작업</span> </td> 
      <td> <p>작업표에서 초과 작업 시간 상자를 숨기도록 선택할 수 있습니다.</p> <p>이 옵션은 기본적으로 비활성화됩니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 저장을 클릭합니다.
