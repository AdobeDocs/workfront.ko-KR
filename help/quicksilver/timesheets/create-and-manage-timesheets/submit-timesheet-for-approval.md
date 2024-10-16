---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 승인을 위해 타임시트 제출
description: 승인을 위해 타임시트를 제출하면 관리자가 작업 시간을 파악할 수 있습니다. 승인자는 기록된 모든 시간이 올바른 영역에 할당되었고 해당 기간에 충분한 시간이 기록되었는지 확인할 수 있습니다.
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 0%

---

# 승인을 위해 타임시트 제출

<!--Audited: 8/2024-->

승인을 위해 타임시트를 제출하면 관리자가 작업 시간을 파악할 수 있습니다. 승인자는 기록된 모든 시간이 올바른 영역에 할당되었고 해당 기간에 충분한 시간이 기록되었는지 확인할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>새로운 기능: 밝게 또는 높음 </p>
   <p>현재: 검토 이상 </p>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>작업 및 문제에 대한 보기 또는 상위 액세스 권한 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>타임시트에 대한 이상의 권한 보기</p> </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 승인을 위해 타임시트 제출

* [승인을 위해 타임시트 제출](#submit-a-timesheet-for-approval)
* [제출된 타임시트의 상태 보기](#view-the-status-of-a-submitted-timesheet)

### 승인을 위해 타임시트 제출

타임시트 승인자가 설정되면([타임시트 승인](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md) 문서의 [타임시트 승인자 지정](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) 섹션에 설명된 대로) 타임시트 하단의 **닫기** 단추가 **승인을 위해 제출** 단추로 변경됩니다.

승인을 위해 타임시트를 제출하려면 다음을 수행하십시오.

1. 승인자가 있도록 구성된 타임시트로 이동합니다.
1. [로그 시간](../../timesheets/create-and-manage-timesheets/log-time.md)에 설명된 대로 로그 시간입니다.
1. 타임시트 승인 프로세스를 시작하려면 **승인을 위해 제출**&#x200B;을 클릭하십시오.

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   **승인을 위해 제출** 단추가 **승인**, **거부** 및 **회수** 단추로 바뀝니다. 타임시트의 상태가 **제출됨**(으)로 변경됩니다.

   승인을 위해 타임시트가 제출되면 승인자는 **홈** 영역의 **내 승인** 위젯에 나열된 타임시트를 볼 수 있습니다. 다음과 같은 상황이 발생할 수 있습니다.

   * 승인하면 **다시 시작** 단추가 **다시 열기**(으)로 바뀌고 타임시트 상태가 **열기**(으)로 업데이트됩니다.
   * 거부하는 경우 **승인을 위해 제출** 단추가 **회수** 단추를 대체하며 타임시트 상태가 **거부됨**(으)로 업데이트됩니다.

1. (선택 사항) 타임시트를 다시 열고 시간을 업데이트하려면 **회수**&#x200B;를 클릭합니다. 자세한 내용은 이 문서의 [타임시트 회수](#recall-a-timesheet) 섹션을 참조하십시오.

### 제출된 타임시트의 상태 보기 {#view-the-status-of-a-submitted-timesheet}

타임시트를 제출한 후 타임시트의 상태를 볼 수 있습니다.

Workfront 관리자가 사용자에 대한 타임시트 승인 및 사용자 이벤트 핸들러에 대한 타임시트 거부를 활성화한 경우 타임시트가 승인 또는 거부되면 알림을 받게 됩니다. 이벤트 알림 활성화에 대한 자세한 내용은 [이벤트 알림 유형](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)을 참조하세요.

이러한 알림이 없으면 Workfront의 타임시트 영역에서 제출된 타임시트의 상태에 대해 알 수 있습니다.

타임시트의 상태를 보려면 다음 작업을 수행하십시오.

1. Adobe Workfront 오른쪽 상단의 **주 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭합니다.
1. **타임시트**&#x200B;를 클릭합니다. 기본적으로 **모두** 필터가 선택되어 있습니다.

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
   >Workfront 관리자 또는 그룹 관리자가 설정 영역의 목록 컨트롤 또는 레이아웃 템플릿에서 내 타임시트 승인 및 내 타임시트 필터를 제거한 경우 내 타임시트 승인 및 내 타임시트 옵션이 타임시트 목록 맨 위나 필터 목록에 표시되지 않습니다. 자세한 내용은 다음 문서를 참조하십시오.
   >
   >   
   >   
   >   * [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (조건부) **내 타임시트**&#x200B;를 선택한 경우 **표준** 보기가 적용되었는지 확인하고 **상태** 열을 확인합니다.

   타임시트의 상태는 다음과 같습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">열기</td> 
      <td> <p>타임시트가 현재 열려 있으며 시간을 기록할 수 있습니다. </p> <p>회수된 타임시트가 열림 상태로 표시됩니다. 자세한 내용은 이 문서의 <a href="#recall-a-timesheet" class="MCXref xref">타임시트 회수</a> 섹션을 참조하십시오. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">제출됨</td> 
      <td>승인을 위해 타임시트를 제출했지만 아직 승인되지 않았습니다. 제출된 타임시트를 회수하여 계속 편집할 수 있습니다. 자세한 내용은 이 문서의 <a href="#recall-a-timesheet" class="MCXref xref">타임시트 회수</a> 섹션을 참조하십시오. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">마감됨</td> 
      <td> <p>다음과 같은 시나리오가 있습니다.</p> 
       <ul> 
        <li> <p>타임시트에 승인자가 없는 경우 시간을 절약하고 닫았습니다.</p> </li> 
        <li> <p>타임시트에 승인자가 있는 경우 승인을 위해 제출한 후 승인되었습니다.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">거부됨</td> 
      <td>승인을 위해 타임시트를 제출했으며 승인자가 이를 거부했습니다.</td> 
     </tr> 
    </tbody> 
   </table>

## 타임시트 회수 {#recall-a-timesheet}

승인을 위해 이미 제출된 타임시트를 불러올 수 있습니다. 승인되지 않은 타임시트만 회수할 수 있습니다.

타임시트를 회수하려면:

1. Adobe Workfront 오른쪽 상단의 **주 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭합니다.

1. **타임시트**&#x200B;를 클릭합니다.
1. 화면 오른쪽 상단의 **내 타임시트**&#x200B;를 클릭하거나 **필터** ![](assets/filter-nwepng.png) 드롭다운 메뉴에서 **내 타임시트**&#x200B;을(를) 선택합니다.
1. 상태가 **제출됨**&#x200B;인 타임시트의 시간대를 클릭합니다.
1. **회수**&#x200B;를 클릭합니다.

   타임시트를 다시 편집할 수 있게 되고 상태가 **열기**(으)로 변경됩니다.
