---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 승인을 위해 타임시트 제출
description: 승인을 위해 타임시트를 제출하면 관리자가 작업 시간을 파악할 수 있습니다. 승인자는 기록된 모든 시간이 올바른 영역에 할당되었고 해당 기간에 충분한 시간이 기록되었는지 확인할 수 있습니다.
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 0%

---

# 승인을 위해 타임시트 제출

승인을 위해 타임시트를 제출하면 관리자가 작업 시간을 파악할 수 있습니다. 승인자는 기록된 모든 시간이 올바른 영역에 할당되었고 해당 기간에 충분한 시간이 기록되었는지 확인할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업 및 문제에 대한 액세스 이상 보기</p> <p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 및 문제에 대한 이상의 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 승인을 위해 타임시트 제출

* [승인을 위해 타임시트 제출](#submit-a-timesheet-for-approval)
* [제출된 타임시트의 상태 보기](#view-the-status-of-a-submitted-timesheet)

### 승인을 위해 타임시트 제출

타임시트 승인자가 설정된 후( 섹션에 설명된 대로) [타임시트 승인자 지정](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) 이 문서에서 [타임시트 승인](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)), **닫기** 타임시트 하단의 단추가 **승인을 위해 제출** 단추를 클릭합니다.

승인을 위해 타임시트를 제출하려면 다음을 수행하십시오.

1. 승인자가 있도록 구성된 타임시트로 이동합니다.
1. 에 설명된 대로 시간을 기록합니다. [로그 시간](../../timesheets/create-and-manage-timesheets/log-time.md).
1. 클릭 **승인을 위해 제출** 타임시트 승인 프로세스를 시작합니다.

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   다음 **승인을 위해 제출** 단추가 **승인**, **거부**, 및 **회수** 단추. 타임시트의 상태가 (으)로 변경됨 **제출됨**.

   승인을 위해 타임시트가 제출되면 승인자에게 다음에 나열된 타임시트가 표시됩니다. **승인** 의 영역 **홈** 페이지를 가리키도록 업데이트하는 중입니다. 다음과 같은 상황이 발생할 수 있습니다.

   * 만약 그들이 승인한다면 **회수** 단추 변경 **다시 열기** 및 타임시트 상태가 다음으로 업데이트됨: **열기**.
   * 거부하면 **승인을 위해 제출** 단추를 클릭하면 **회수** 버튼 및 타임시트 상태 업데이트 대상 **거부됨**.

1. (선택 사항) **회수** 타임시트를 다시 열고 시간을 업데이트해야 하는 경우. 자세한 내용은 [타임시트 회수](#recall-a-timesheet) 이 문서의 섹션.

### 제출된 타임시트의 상태 보기 {#view-the-status-of-a-submitted-timesheet}

타임시트를 제출한 후 타임시트의 상태를 볼 수 있습니다.

Workfront 관리자가 사용자에 대한 타임시트 승인 및 사용자 이벤트 핸들러에 대한 타임시트 거부를 활성화한 경우 타임시트가 승인 또는 거부되면 알림을 받게 됩니다. 이벤트 알림 활성화에 대한 자세한 내용은 [이벤트 알림 유형](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

이러한 알림이 없으면 Workfront의 타임시트 영역에서 제출된 타임시트의 상태에 대해 알 수 있습니다.

타임시트의 상태를 보려면 다음 작업을 수행하십시오.

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront 오른쪽 상단에 있습니다.
1. 클릭 **타임시트**. 다음 **모두** 기본적으로 필터가 선택되어 있습니다.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (선택 사항) 다음 중 하나를 수행하여 타임시트 목록의 필터를 업데이트합니다.

   * 선택 **내 타임시트 승인** 페이지 오른쪽 상단 모서리에서 승인한 타임시트만 볼 수 있습니다.

     또는

     선택 **내 타임시트** 내 타임시트만 봅니다.

     내 타임시트 승인 또는 내 타임시트 필터가 타임시트 목록에 적용됩니다.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 필터 아이콘 클릭 ![](assets/filter-nwepng.png) 다른 필터를 적용하거나 새 필터를 만듭니다. 필터 만들기 또는 업데이트에 대한 자세한 내용은 [Adobe Workfront에서 필터 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 설정 영역의 목록 컨트롤 또는 레이아웃 템플릿에서 내 타임시트 승인 및 내 타임시트 필터를 제거한 경우 내 타임시트 승인 및 내 타임시트 옵션이 타임시트 목록 맨 위나 필터 목록에 표시되지 않습니다. 자세한 내용은 다음 문서를 참조하십시오.
   >
   >   
   >   
   >   * [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 맞춤화](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (조건부) (선택한 경우) **내 타임시트**, 다음을 확인합니다. **표준** 보기가 적용되고 **상태** 열.

   타임시트의 상태는 다음과 같습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">진행 중</td> 
      <td> <p>타임시트가 현재 열려 있으며 시간을 기록할 수 있습니다. </p> <p>회수된 타임시트가 열림 상태로 표시됩니다. 자세한 내용은 <a href="#recall-a-timesheet" class="MCXref xref">타임시트 회수</a> 이 문서의 섹션. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">제출됨</td> 
      <td>승인을 위해 타임시트를 제출했지만 아직 승인되지 않았습니다. 제출된 타임시트를 회수하여 계속 편집할 수 있습니다. 자세한 내용은 <a href="#recall-a-timesheet" class="MCXref xref">타임시트 회수</a> 이 문서의 섹션. </td> 
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

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront 오른쪽 상단에 있습니다.

1. 클릭 **타임시트**.
1. 클릭 **내 타임시트** 화면의 오른쪽 상단에서 또는 를 선택합니다. **내 타임시트** 다음에서 **필터** ![](assets/filter-nwepng.png) 드롭다운 메뉴.
1. 상태가 인 타임시트의 시간대를 클릭합니다. **제출됨**.
1. 클릭 **회수**.

   타임시트를 다시 편집할 수 있게 되고 상태가 (으)로 변경됩니다. **열기**.
