---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Adobe Workfront에서 타임시트 삭제
description: 타임시트 프로필에 적용한 변경 사항은 타임시트 프로필 만들기, 편집 및 할당에 설명된 대로 현재 기존 타임시트에 바로 적용되지 않습니다. 변경 사항을 기존 타임시트에 표시하려면 생성된 타임시트를 삭제하고 새 타임시트를 생성해야 합니다. 이는 타임시트 프로필을 사용자와 연결하여 생성된 타임시트에만 적용됩니다.
author: Alina
feature: Timesheets
exl-id: c6a86c1b-8580-4896-8933-d4e2818e98ed
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Adobe Workfront에서 타임시트 삭제

타임시트 프로필에 적용한 변경 내용은 [타임시트 프로필 만들기, 편집 및 할당](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)에 설명된 대로 현재 기존 타임시트에 바로 적용되지 않습니다. 변경 사항을 기존 타임시트에 표시하려면 생성된 타임시트를 삭제하고 새 타임시트를 생성해야 합니다. 이는 타임시트 프로필을 사용자와 연결하여 생성된 타임시트에만 적용됩니다.

>[!NOTE]
>
>타임시트가 수동으로 생성된 이후 사용자가 타임시트 프로필과 연결되어 있지 않으면 수동으로 생성된 타임시트를 다시 생성하여 다시 만들 수 없습니다. 수동으로 만든 타임시트를 삭제하면 데이터가 손실될 수 있습니다. 단일 타임시트를 만드는 방법에 대한 자세한 내용은 [일회용 타임시트 만들기](../../timesheets/create-and-manage-timesheets/create-tmshts.md)를 참조하십시오.

Adobe Workfront 관리자 또는 그룹 관리자는 시스템의 모든 사용자에 대해 타임시트를 생성할 수 있습니다. 수동으로 타임시트를 생성하는 방법에 대한 자세한 내용은 다음을 참조하십시오.

* [수동으로 타임시트 생성](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
* [그룹의 타임시트 프로필 만들기 및 관리](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

>[!IMPORTANT]
>
>* 삭제된 타임시트는 복구할 수 없습니다.
>* 지난 타임시트는 타임시트 프로필을 기반으로 자동으로 생성되지 않으므로 삭제하지 않는 것이 좋습니다. 타임시트 프로필에 대한 변경 사항을 새 타임시트에 즉시 표시하려면 현재 및 미래 타임시트를 삭제하고 수동으로 생성할 수 있습니다.
>* 타임시트를 삭제할 때 작업, 문제 및 프로젝트에 대해 기록된 시간은 삭제되지 않습니다. 타임시트와 함께 일반 시간만 삭제됩니다. 별도의 텍스트 편집기에서 타임시트와 관련된 일반 시간을 기록합니다. 타임시트가 삭제된 후 새 타임시트에 기록할 수 있습니다.
>

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>타임시트에 대한 관리 액세스 권한이 있어야 합니다. </p> <p>자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>를 참조하십시오.</p> <p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 목록에서 타임시트 삭제

1. Adobe Workfront 오른쪽 상단의 **주 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭합니다.

1. **타임시트**&#x200B;를 클릭합니다. **모두** 필터는 기본적으로 선택되어 있으며 보기 액세스 권한이 있는 모든 타임시트를 표시합니다.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (선택 사항) 다음 중 하나를 수행하여 타임시트 목록의 필터를 업데이트합니다.

   * 승인한 타임시트만 보려면 페이지의 오른쪽 상단에서 **내 타임시트 승인**&#x200B;을 선택하십시오.

     또는

     내 타임시트만 보려면 **내 타임시트**&#x200B;를 선택하십시오.

     내 타임시트 승인 또는 내 타임시트 필터가 타임시트 목록에 적용됩니다.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 필터 아이콘 ![](assets/filter-nwepng.png)을(를) 클릭하여 다른 필터를 적용하거나 새 필터를 만듭니다. 필터 만들기 또는 업데이트에 대한 자세한 내용은 [Adobe Workfront에서 필터 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)을 참조하세요.

   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 설정 영역의 목록 컨트롤 또는 레이아웃 템플릿에서 내 타임시트 승인 및 내 타임시트 필터를 제거한 경우 내 타임시트 승인 및 내 타임시트 옵션이 타임시트 목록 맨 위나 필터 목록에 표시되지 않습니다. 자세한 내용은 다음 문서를 참조하십시오.
   >
   >   
   >   
   >   * [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (선택 사항) **보기** ![](assets/view-icon.png) 또는 **그룹화** ![](assets/grouping.png) 아이콘을 클릭하여 다른 보기 또는 그룹화를 적용하거나 새 보기 또는 그룹화를 만듭니다.

   필터, 보기 또는 그룹화 만들기에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront에서 필터 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfront에서 보기 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfront에서 그룹화 만들기](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 삭제할 타임시트를 하나 이상 선택하고 타임시트 목록 맨 위에 있는 **삭제** ![](assets/delete.png) 아이콘을 클릭합니다.

1. **삭제**&#x200B;를 클릭합니다.

   선택한 타임시트가 삭제되며 복구할 수 없습니다.

   새 타임시트를 생성하려면 사용자가 타임시트 프로필과 연결되어 있는지 확인하고 Workfront 관리자 또는 그룹 관리자에게 새 타임시트를 생성하도록 요청하십시오.

   자세한 내용은 다음을 참조하십시오.

   * [타임시트 프로필 만들기, 편집 및 할당](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)
   * [수동으로 타임시트 생성](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
   * [그룹의 타임시트 프로필 만들기 및 관리](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

## 타임시트 페이지에서 타임시트 삭제

1. Adobe Workfront 오른쪽 상단의 [!UICONTROL **주 메뉴**] 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭합니다.
1. 삭제할 타임시트를 클릭하여 엽니다.
1. 타임시트 이름 오른쪽에 있는 [!UICONTROL **자세히**] 아이콘 ![](assets/more-icon.png)을(를) 클릭한 다음 **삭제**&#x200B;를 클릭합니다.

   ![타임시트 페이지에서 타임시트 삭제](assets/delete-timesheet-from-timesheet-page.png)
1. 확인하려면 [!UICONTROL **삭제**]&#x200B;를 클릭하세요.

   타임시트가 삭제되어 복구할 수 없습니다.
