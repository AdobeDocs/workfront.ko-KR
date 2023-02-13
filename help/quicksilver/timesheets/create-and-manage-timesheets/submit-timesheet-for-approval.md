---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 승인을 위한 작업표 제출
description: 승인을 위해 작업표를 제출하면 관리자에게 작업 시간을 표시할 수 있습니다. 승인자는 기록된 모든 시간이 올바른 영역에 할당되었고 해당 기간 동안 충분한 시간이 기록되었는지 확인할 수 있습니다.
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# 승인을 위한 작업표 제출

승인을 위해 작업표를 제출하면 관리자에게 작업 시간을 표시할 수 있습니다. 승인자는 기록된 모든 시간이 올바른 영역에 할당되었고 해당 기간 동안 충분한 시간이 기록되었는지 확인할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업 및 문제에 대한 액세스 이상 보기</p> <p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 및 문제에 대한 권한 보기 이상</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 승인을 위한 작업표 제출

* [승인을 위한 작업표 제출](#submit-a-timesheet-for-approval)
* [제출된 작업표의 상태 보기](#view-the-status-of-a-submitted-timesheet)

### 승인을 위한 작업표 제출

작업표 승인자가 설정되면(섹션에 설명된 대로) [작업표 승인자 지정](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) 기사 [작업표 승인](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)), **닫기** 작업표 하단의 단추가 **승인을 위한 제출** 버튼을 클릭합니다.

승인을 위한 작업표를 제출하려면

1. 승인자가 있도록 구성된 작업표로 이동합니다.
1. 에 설명된 대로 로그 시간 [로그 시간](../../timesheets/create-and-manage-timesheets/log-time.md).
1. 클릭 **승인을 위한 제출** 작업표 승인 프로세스를 시작하려면

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   다음 **승인을 위한 제출** 단추가 **승인**, **거부**, 및 **회수** 단추. 작업표의 상태가 **제출됨**.

   승인을 위해 작업표를 제출하면 승인자는 해당 작업표에 나열된 작업표를 봅니다 **승인** 영역 **홈** 페이지. 다음 상황이 발생할 수 있습니다.

   * 그들이 승인하면 **회수** 단추 변경 **다시 열기** 작업표 상태가 **열기**.
   * 거절하면 **승인을 위한 제출** 버튼이 를 대체합니다 **회수** 단추와 작업표 상태가 **거부됨**.

1. (선택 사항) **회수** 작업표를 다시 열고 시간을 업데이트해야 하는 경우 자세한 내용은 [작업표 회수](#recall-a-timesheet) 섹션에 자세히 설명되어 있습니다.

### 제출된 작업표의 상태 보기 {#view-the-status-of-a-submitted-timesheet}

작업표를 제출한 후 작업표의 상태를 볼 수 있습니다.

Workfront 관리자가 사용자에게 작업표 승인 및 사용자 이벤트 처리기에 대한 작업표 거부 기능을 활성화한 경우 작업표가 승인되거나 거부되면 사용자에게 통지됩니다. 이벤트 알림 활성화에 대한 자세한 내용은 [Adobe Workfront에서 사용할 수 있는 이벤트 알림](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

이러한 알림이 없으면 Workfront의 작업표 영역에서 제출된 작업표의 상태에 대해 알 수 있습니다.

작업표의 상태를 보려면 다음을 수행합니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서
1. 클릭 **작업표**. 다음 **모두** 기본적으로 필터가 선택되어 있습니다.

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
   >   
   >   
   >   * [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (조건부) 선택한 경우 **내 작업표**, **표준** 보기가 적용되어 알림 **상태** 열.

   작업표의 상태는 다음과 같습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">열기</td> 
      <td> <p>작업표가 현재 열려 있으며 로그 시간을 지정할 수 있습니다. </p> <p>회수된 작업표가 열림 상태로 표시됩니다. 자세한 내용은 <a href="#recall-a-timesheet" class="MCXref xref">작업표 회수</a> 섹션에 자세히 설명되어 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">제출됨</td> 
      <td>승인을 위해 작업표를 제출했지만 아직 승인되지 않았습니다. 제출된 작업표를 회수하여 편집을 계속할 수 있습니다. 자세한 내용은 <a href="#recall-a-timesheet" class="MCXref xref">작업표 회수</a> 섹션에 자세히 설명되어 있습니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">마감됨</td> 
      <td> <p>다음 시나리오가 있습니다.</p> 
       <ul> 
        <li> <p>작업표에 승인자가 없는 경우 시간을 절약하고 마감했습니다.</p> </li> 
        <li> <p>작업표에 승인자가 있는 경우 승인을 위해 제출했으며 승인되었습니다.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">거부됨</td> 
      <td>승인을 위해 작업표를 제출했고 승인자가 이를 거부했습니다.</td> 
     </tr> 
    </tbody> 
   </table>

## 작업표 회수 {#recall-a-timesheet}

승인을 위해 이미 제출된 작업표를 회수할 수 있습니다. 승인되지 않은 작업표만 회수할 수 있습니다.

작업표를 회수하려면

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

1. 클릭 **작업표**.
1. 클릭 **내 작업표** 화면의 오른쪽 상단 모서리에서 을(를) 선택하거나 을(를) 선택합니다 **내 작업표** 에서 **필터** ![](assets/filter-nwepng.png) 드롭다운 메뉴
1. 상태가 인 작업표의 기간을 클릭합니다. **제출됨**.
1. 클릭 **회수**.

   작업표를 다시 편집할 수 있게 되고 상태가 **열기**.
