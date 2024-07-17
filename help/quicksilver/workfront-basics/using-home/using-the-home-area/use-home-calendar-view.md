---
product-area: calendars
navigation-topic: use-the-home-area
title: 홈 캘린더 보기 사용
description: '[!UICONTROL 홈] 영역의 [일정] 보기를 사용하여 근무일과 작업 할당을 관리할 수 있습니다. 귀하만 홈 캘린더를 보고 관리할 수 있습니다.'
author: Lisa
feature: Get Started with Workfront
exl-id: 07b33b56-ae57-4ae5-890e-c21feae1c4fd
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '1603'
ht-degree: 0%

---

# [!UICONTROL 홈 일정] 보기 사용

[!UICONTROL 홈] 영역의 [일정] 보기를 사용하여 근무일과 작업 할당을 관리할 수 있습니다. [!UICONTROL 홈 캘린더]를 보고 관리할 수 있습니다.

>[!NOTE]
>
>[!UICONTROL Home] 영역의 [!UICONTROL Calendar] 보기는 작업의 시각적 표현을 제공하는 동적 보고서인 [!DNL Adobe Workfront] [!UICONTROL Calendar] 보고서와 다릅니다. [!DNL Workfront] [!UICONTROL 캘린더] 보고서에 대한 자세한 내용은 [캘린더 보고서 개요](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md)를 참조하십시오.
>
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Due to a temporary problem, your Workfront Calendar data might not display as described in this article. This problem will be fixed in the near future. (NOTE: From Alina: Spoke with Lisa and Court and they agreed to draft or delete this. Court could not remember what this was referring to and Lisa did not add this note. Lisa might update this if she hears from the team that this is still accurate.)</li>>
>  -->


## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Work] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>작업 및 문제에 대한 [!UICONTROL 편집] 액세스</p> <p>참고: 여전히 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하십시오. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>캘린더에 추가할 작업 및 문제에 대한 [!UICONTROL Contribute] 권한 이상</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

## [!UICONTROL 홈 일정]에서 작업 항목 예약

[!UICONTROL 홈 일정]을 사용하여 주별 작업 항목을 예약할 수 있습니다.

>[!NOTE]
>
>[!UICONTROL 홈 일정]에 작업 항목을 추가해도 작업 항목과 연결된 기존 날짜는 변경되지 않습니다.

캘린더에 [!DNL Workfront] 작업 항목을 추가하려면:

1. [홈 캘린더 보기]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md)에 설명된 대로 [!UICONTROL 홈 캘린더] 보기로 이동합니다.[!UICONTROL 

   사용자 또는 사용자의 그룹, 팀 또는 작업 역할에 할당된 모든 작업 항목이 왼쪽 패널에 표시됩니다. 목록을 정렬하고 필터링하여 특정 항목만 표시할 수 있습니다.

   자세한 내용은 이 문서의 뒷부분에서 [작업 항목 필터링 및 정렬](#filter-and-sort-work-items)을 참조하세요.

1. 왼쪽 패널에서 작업 항목을 작업할 날짜와 시간으로 드래그합니다.

   계획된 완료 일자 후 또는 계획된 시간 수보다 많은 시간 동안 항목에 대한 작업을 수행하도록 스케줄을 지정하면 작업 항목이 빨간색으로 표시되고 경고가 나타납니다.

   작업 항목 기한과 이 기한이 [!UICONTROL 홈 일정]에 할당된 시간에 미치는 영향에 대해 알아보려면 [[!UICONTROL 홈 일정] 보기](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md)를 참조하세요.

1. 다음 중 하나를 수행합니다.

   * **작업 항목을 여러 날 동안 예약하려면:** 2단계를 반복하여 작업을 수행하려는 각 날짜와 시간에 항목을 추가합니다.
   * **일정 항목의 기간을 수정하려면:** 커서가 이중 화살표가 될 때까지 항목의 아래쪽 가장자리를 마우스로 가리킨 다음 아래쪽 가장자리를 원하는 종료 시간으로 끕니다.
   * **일정 항목을 삭제하려면:** 항목을 마우스로 가리킨 다음 표시되는 [!UICONTROL 휴지통] 아이콘을 클릭합니다.

## [!UICONTROL 홈 일정]에서 작업 항목 업데이트

[!UICONTROL 홈 일정] 보기에 표시되는 작업 항목을 업데이트할 수 있습니다. 실제 작업 항목의 [!UICONTROL 업데이트] 탭에도 업데이트가 표시됩니다.

1. [홈 캘린더 보기]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md)에 설명된 대로 [!UICONTROL 홈 캘린더] 보기로 이동합니다.[!UICONTROL 

1. 업데이트할 작업 항목의 [!UICONTROL 세부 정보] 패널을 엽니다.

   * 왼쪽 패널에서 작업 항목을 선택한 다음 **[!UICONTROL 세부 정보]**&#x200B;를 클릭합니다.
   * 달력에서: 예약된 달력 이벤트를 클릭합니다.

   작업 항목에 대한 세부 정보가 창 오른쪽에 나타나는 패널에 표시됩니다.

   ![](assets/click-cal-item-to-see-details-350x217.png)

1. 다음 중 하나를 수행하여 작업 항목을 업데이트합니다.

   * **[!UICONTROL 새 업데이트 시작]** 상자에서 업데이트를 입력하고 다음 정보를 지정한 다음 **[!UICONTROL 업데이트]**&#x200B;를 클릭합니다.

     <table style="table-layout:auto">
      <col>
      <col>
      <tbody>
       <tr>
        <td role="rowheader"><strong>[!UICONTROL Notify]</strong></td>
        <td><p> 업데이트에 대해 알릴 사용자를 태그합니다. 자세한 내용은 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">업데이트에 다른 사용자 태그 지정</a>을 참조하세요.</p><p> </p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><strong>[!UICONTROL 커밋 일자]</strong></td>
        <td>드롭다운 달력에서 작업 항목을 완료하기로 약속하는 날짜를 선택합니다. [!UICONTROL 커밋 일자] 설정에 대한 자세한 내용은 <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">[!UICONTROL 커밋 일자] 개요</a>를 참조하십시오.</td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><strong>[!UICONTROL 어떻게 되어가고 있습니까?]</strong></td>
        <td>작업 또는 문제에 대한 새 조건을 선택합니다. 작업 및 문제 조건에 대한 자세한 내용은 <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">작업 및 문제에 대한 상태 업데이트</a>를 참조하십시오.</td>
       </tr>
       <tr>
        <td role="rowheader"><strong>[!UICONTROL Private to] 내 회사</strong></td>
        <td>회사 외부의 사용자가 이 업데이트를 볼 수 없도록 하려면 비활성화하십시오.</td>
       </tr>
      </tbody>
     </table>

   * 항목에 대한 현재 **[!UICONTROL 상태]**&#x200B;를 클릭한 다음 표시되는 목록에서 새 상태를 클릭합니다. 자세한 내용은 [승인 프로세스 개요](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md)를 참조하십시오.

     >[!NOTE]
     >
     >할당된 작업 항목을 [!UICONTROL 완료 - 승인 보류 중](으)로 표시하면 캘린더에 더 이상 표시되지 않을 수 있습니다. 항목을 승인하도록 설정된 사용자가 항목을 [!UICONTROL 승인됨](으)로 표시할 때까지 추가 작업이 필요하지 않기 때문입니다. 이 경우 캘린더에 있는 항목을 [!UICONTROL 승인됨] 항목으로 볼 수 있습니다.

   * (선택 사항) 기존 댓글 또는 업데이트에 회신하려면 **[!UICONTROL 회신]**&#x200B;을 클릭하고 **[!UICONTROL 알림]** 상자에 수신자를 지정한 다음 회신을 입력한 다음 **[!UICONTROL 회신]**&#x200B;을 클릭합니다.\

     받는 사람 지정에 대한 정보가 필요한 경우 [업데이트에 다른 사람 태그 지정](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)을 참조하세요.

1. (선택 사항) **[!UICONTROL 세부 정보]** 패널을 닫으려면 패널 바깥쪽을 클릭합니다.

## 통합 달력에서 이벤트 업데이트

[!UICONTROL 홈 일정]에서 통합 일정 이벤트를 업데이트하려면:

1. [홈 캘린더 보기]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md)에 설명된 대로 [!UICONTROL 홈 캘린더] 보기로 이동합니다.[!UICONTROL 
1. [!UICONTROL 홈 캘린더]의 오른쪽 위 모서리에 있는 **[!UICONTROL 캘린더 새로 고침]**&#x200B;을 클릭합니다.

   ![](assets/refresh-qs-350x360.png)

   [!UICONTROL 홈 일정] 보기를 열거나 [!UICONTROL 홈 일정]을 새로 고치면 통합 일정 이벤트가 자동으로 업데이트됩니다.

## 작업 항목 필터링 및 정렬

1. [홈 캘린더 보기]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md)에 설명된 대로 [!UICONTROL 홈 캘린더] 보기로 이동합니다.[!UICONTROL 
1. **[!UICONTROL 필터]** 드롭다운 메뉴를 클릭합니다.

   >[!NOTE]
   >
   >일부 필터 옵션은 개체(작업, 요청, 문제, 승인, 증명 및 개인)를 기반으로 하고, 다른 옵션은 상태([!UICONTROL 작업 중], [!UICONTROL 시작할 준비가 됨], [!UICONTROL 준비되지 않음] 및 [!UICONTROL 완료됨])를 기반으로 합니다. 선택한 상태가 없으면 [!UICONTROL 홈 일정]에 선택한 모든 상태의 개체가 표시됩니다. 마찬가지로, 선택된 객체가 없으면 선택된 상태의 모든 객체가 표시됩니다.

1. 다음 필터 옵션 중에서 선택하여 표시할 항목 유형을 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL All]</strong></td> 
      <td><span>모든 항목을 표시하고 선택합니다. 여기에는 작업,</span> <span data-mc-edit-date="2022-02-16T13:45:46.9712518-05:00" data-mc-editor="alinaw" data-mc-comment="this might need indenting when it goes to Preview" data-mc-initials="AL" data-mc-creator="alinaw" data-mc-create-date="2022-02-16T13:45:23.7889689-05:00">문제</span><span>, 승인, 개인 작업 및 완료된 작업 및 문제가 포함됩니다.</span></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 작업 처리 중]</strong></td> 
      <td> <p><span>현재 진행 중인 작업만 표시합니다. [!UICONTROL Work On It] 단추를 클릭한 사용자에게 할당된 작업입니다.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 작업 시작할 준비 완료]</strong></td> 
      <td> 
       <div> 
        <p>시작할 준비가 된 작업만 표시합니다. 다음 문은 모두 true여야 합니다.</p> 
        <ul style="list-style-type: square;"> 
         <li> <p>과제와 그 부모에게는 작업을 할 수 없는 전임자나 과업 제한이 없다.</p> </li> 
         <li> <p>작업의 [!UICONTROL 계획된 시작 일자]가 과거 또는 최대 2주 후입니다.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 작업이 준비되지 않음]</strong></td> 
      <td> 
       <div> 
        <p>아직 시작할 준비가 되지 않은 작업만 표시합니다. 다음 문 중 하나가 true여야 합니다.</p> 
        <ul> 
         <li> <p>작업 및 상위 사용자에게 작업을 수행할 수 없는 선행 작업 또는 작업 제한이 있을 수 있습니다.</p> </li> 
         <li> <p>작업에 앞으로 2주 이상 소요되는 [!UICONTROL 계획된 시작 일자]가 있습니다.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 문제 처리 중]</strong></td> 
      <td> <p>현재 진행 중인 문제만 표시합니다. 이는 [!UICONTROL Work On It] 버튼을 클릭한 사용자에게 할당된 문제입니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 문제 요청됨]</strong></td> 
      <td><span>할당되었지만 [!UICONTROL Work On It] 단추를 클릭하지 않은 문제만 표시합니다.</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Personal]</strong></td> 
      <td>개인 작업만 표시합니다. 문서 <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">[!UICONTROL 홈] 영역에서 작업 항목 만들기</a>의 <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#creating-a-personal-task">[!UICONTROL 개인 작업 만들기]</a> 섹션에 설명된 대로 [!UICONTROL 할 일] 작업으로 만드는 작업입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Approvals]</strong></td> 
      <td> 
       <div> 
        <p>귀하에게 할당되거나 위임된 승인 및 귀하가 제출한 승인만 표시합니다. 승인에는 작업 항목(프로젝트, 작업 및 문제)에 대한 승인과 문서, 증명, 액세스 요청 및 타임시트에 대한 승인이 포함됩니다. 승인에 대한 자세한 내용은 다음 문서를 참조하십시오.</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">승인 보기 </a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">승인 관리</a> </p> </li> 
        </ul> 
        <p>참고: 제출한 승인과 승인자 중 하나인 승인은 두 번 계산됩니다. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 완료]</strong></td> 
      <td><span>완료된 작업, 문제 및 개인 작업만 표시합니다. 완료된 작업이 이전 2주 동안 표시되고 주별로 작업 목록에 그룹화됩니다. 승인이 포함되지 않았습니다.</span> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/calendar-filters-nwe-350x392.png)

1. 작업 목록을 그룹화하고 정렬하려면 **[!UICONTROL 그룹화 기준]** 드롭다운 메뉴를 클릭한 다음 사용할 기준을 선택하십시오.

   항목은 지정한 순서와 기준에 따라 달력의 왼쪽에 나열됩니다.

   ![](assets/home-calendar-sort-group-nwe-350x288.png)

   다음 옵션 중에서 선택합니다.

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL 계획된 완료]</strong></td>
        <td>작업 및 문제는 [!UICONTROL 계획된 완료 일자] 순서로 정렬됩니다. [!UICONTROL 계획된 완료 일자]에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-information/planned-hours.md">계획된 시간 개요</a>를 참조하십시오.</td>
        <td></td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 계획 시작]</strong></td>
        <td>작업 및 문제는 [!UICONTROL 계획된 시작 일자] 순서로 정렬됩니다. 작업 [!UICONTROL 계획된 시작 일자]에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-information/task-planned-start-date.md">작업 [!UICONTROL 계획된 시작 일자] 개요</a>를 참조하십시오.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 커밋 일자]</strong></td>
        <td>작업 및 문제는 [!UICONTROL 커밋 일자] 순서로 정렬됩니다. [!UICONTROL 커밋 일자]에 대한 자세한 내용은 <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md">[!UICONTROL 커밋 일자] 개요</a>를 참조하십시오.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 프로젝트]</strong></td>
        <td>프로젝트별로 작업 항목을 정렬합니다.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 내 우선 순위]</strong></td>
        <td>선택한 순서대로 항목이 표시됩니다. 자세한 내용은 <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md">[!UICONTROL Home] 영역에서 작업 우선 순위 지정</a>을 참조하십시오.</td>
    </tr>
   </table>

## 다른 주로 이동

1. [홈 캘린더 보기]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md)에 설명된 대로 [!UICONTROL 홈 캘린더] 보기로 이동합니다.[!UICONTROL 
1. **[!UICONTROL 달력 도구 모음]**&#x200B;에서 날짜 표시기의 왼쪽 화살표를 클릭하여 달력 보기를 1주일 뒤로 이동하거나 오른쪽 화살표를 클릭하여 1주일 앞으로 이동합니다.

   ![](assets/week-arrows-350x206.png)

   **[!UICONTROL 오늘]**&#x200B;을 클릭하여 현재 주로 돌아갈 수 있습니다.

## 표시할 캘린더 지정

[!UICONTROL 홈 캘린더]에서 볼 통합 캘린더(예: 유급휴가, 생일 또는 휴일 캘린더)를 지정할 수 있습니다. 지침은 [[!UICONTROL 홈 일정 구성] 보기 설정 구성](../../../workfront-basics/using-home/using-the-home-area/configure-home-calendar-view.md)을 참조하세요.
