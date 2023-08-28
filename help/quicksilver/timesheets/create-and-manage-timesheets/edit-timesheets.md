---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 타임시트 정보 편집
description: 타임시트에 대한 관리 액세스 권한이 있는 사용자는 Adobe Workfront에서 기존 타임시트에 대한 정보를 편집할 수 있습니다. 예를 들어 타임시트의 소유자, 승인자 또는 시간대를 편집할 수 있습니다.
author: Alina
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 3a2745437e00ac968f2a4590be2637dbc01594ad
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 2%

---

# 타임시트 정보 편집

타임시트에 대한 관리 액세스 권한이 있는 사용자는 Adobe Workfront에서 기존 타임시트에 대한 정보를 편집할 수 있습니다. 예를 들어 타임시트의 소유자, 승인자 또는 시간대를 편집할 수 있습니다.

단일 타임시트의 정보를 편집하거나 여러 타임시트를 일괄적으로 편집할 수 있습니다.

>[!IMPORTANT]
>
>사용자가 타임시트 프로필과 연결되어 있고 타임시트가 자동으로 생성되는 경우, 기존 타임시트에 대한 변경 사항은 이후 날짜에 대해 생성될 타임시트에 반영되지 않습니다. 자동으로 생성된 모든 타임시트에는 타임시트 프로필에 설정된 설정이 있습니다. 자세한 내용은 [타임시트 프로필 만들기](../create-and-manage-timesheets/create-timesheet-profiles.md)


## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

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
   <td> <p>타임시트에 대한 관리 액세스 권한이 있어야 합니다. </p> <p>자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">사용자에게 특정 영역에 대한 관리 액세스 권한 부여</a>.</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 타임시트 편집

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **타임시트**.

   다음 **모두** 보기 액세스 권한이 있는 모든 타임시트를 표시하는 필터가 기본적으로 선택됩니다.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (선택 사항) **검색** 아이콘 ![](assets/search-icon.png) 키워드를 입력하고 특정 타임시트를 검색합니다. 예를 들어 타임시트 시간대 또는 소유자 이름을 검색할 수 있습니다.

1. (선택 사항) 다음 중 하나를 수행하여 타임시트 목록의 필터를 업데이트합니다.

   * 선택 **내 타임시트 승인** 페이지 오른쪽 상단 모서리에서 승인한 타임시트만 볼 수 있습니다.

     또는

     선택 **내 타임시트** 내 타임시트만 봅니다.

     내 타임시트 승인 또는 내 타임시트 필터가 타임시트 목록에 적용됩니다.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 필터 아이콘 클릭 ![](assets/filter-nwepng.png) 다른 필터를 적용하거나 새 필터를 만듭니다. 필터 만들기 또는 업데이트에 대한 자세한 내용은 [Adobe Workfront에서 필터 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 설정 영역의 목록 컨트롤 또는 레이아웃 템플릿에서 내 타임시트 승인 및 내 타임시트 필터를 제거한 경우 내 타임시트 승인 및 내 타임시트 옵션이 타임시트 목록 맨 위나 필터 목록에 표시되지 않습니다. 자세한 내용은 다음 문서를 참조하십시오.
   >
   >   
   >   
   * [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 맞춤화](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (선택 사항)**보기** ![](assets/view-icon.png) 또는 **그룹화** ![](assets/grouping.png) 다른 보기 또는 그룹화를 적용하거나 새 보기를 만드는 아이콘입니다.

   필터, 보기 또는 그룹화 만들기에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront에서 필터 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfront에서 보기 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfront에서 그룹화 만들기](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 하나 이상의 타임시트를 선택한 다음 **편집** 아이콘 ![](assets/edit-icon.png) 을 클릭합니다.
1. 다음 정보를 보거나 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>소유자</strong> </td> 
      <td> <p>타임시트가 생성된 사용자의 이름입니다. 이 필드는 편집할 수 없습니다. </p> <p>여러 타임시트를 선택하면 필드가 표시되지 않습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>시작 일자</strong> </td> 
      <td>타임시트의 시작 날짜입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>종료 일자</strong> </td> 
      <td> 타임시트의 종료 날짜입니다.</td> 
     </tr>
<tr> 
      <td role="rowheader"><strong>상태</strong> </td> 
      <td> 타임시트의 상태입니다.
      다음은 가능한 타임시트 상태 옵션입니다. 
      <ul><li><b>열기</b>: 타임시트가 열려 있으며 시간 항목을 편집할 수 있습니다.</li>
      <li><b>제출됨</b>: 타임시트가 지정된 승인자에게 승인을 위해 제출됩니다.</li>
      <li><b>거부됨</b>: 타임시트가 승인자에 의해 승인되지 않았으므로 사용자가 시간 항목을 편집할 수 있습니다.</li>
      <li><b>종료됨</b>: 타임시트가 사용자에 의해 종료되거나 승인자에 의해 승인되어 현재 종료되었습니다. 종료된 타임시트에 시간을 추가할 수 없습니다.</li>
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>승인자</strong> </td> 
      <td> <p>승인자는 타임시트와 연계된 사용자에 대해 타임시트를 승인하는 사용자입니다. 타임시트에 대한 관리 액세스 권한이 있는 사용자만 승인자로 설정할 수 있습니다. </p> <p>타임시트 관리 권한에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">사용자에게 특정 영역에 대한 관리 액세스 권한 부여</a>.</p> <p>타임시트 승인자의 이름을 입력하기 시작하고 목록에 표시될 때 선택합니다.</p> <p>타임시트에 여러 승인자가 있을 수 있습니다. 이 경우 승인자 중 한 명이 타임시트를 승인하면 타임시트가 다음과 같이 표시됩니다. <strong>종료됨</strong> 그리고 나머지 모든 승인자의 타임시트 승인 목록에서 사라집니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>시간을 편집할 수 있음</strong> </td> 
      <td> <p>승인자가 타임시트의 시간을 편집할 수 있도록 하려면 이 옵션을 선택합니다.</p> <p>여러 타임시트를 선택하는 경우에는 이 옵션을 사용할 수 없습니다. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">초과 작업</span> </td> 
      <td> <p>타임시트에서 초과 작업 시간 상자를 숨기도록 선택할 수 있습니다.</p> <p>이 옵션은 기본적으로 비활성화되어 있습니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.
