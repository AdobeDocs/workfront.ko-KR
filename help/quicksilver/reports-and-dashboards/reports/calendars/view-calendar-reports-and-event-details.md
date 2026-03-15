---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: 달력 보고서 및 이벤트 세부 사항 보기
description: Adobe Workfront에서 만들었거나 공유한 달력 보고서 및 이벤트 세부 사항을 볼 수 있습니다.
author: Courtney
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 3%

---

# 달력 보고서 및 이벤트 세부 사항 보기

Adobe Workfront에서 만들었거나 공유한 달력 보고서 및 이벤트 세부 사항을 볼 수 있습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스</td> 
   <td><p>기여자</p>
       <p>요청</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드 및 달력에 대한 보기 이상의 액세스 권한</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td>달력 보고서에 대한 권한 보기 이상</td> 
  </tr> 
 </tbody> 
</table>

이 표에 있는 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 달력 보고서 보기

<!--{{step1-to-calendars}}-->

1. Adobe Workfront 오른쪽 위 모서리에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)를 클릭하거나(사용 가능한 경우) 왼쪽 위 모서리에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)를 클릭한 다음 **[!UICONTROL 달력]**&#x200B;을 클릭합니다.

   액세스 수준에 따라 다음과 같은 달력이 나열될 수 있습니다.

   * 기본 [!DNL Adobe Workfront] 일정

     Workfront은 사용자에게 할당되거나 사용자가 할당된 팀, 그룹 또는 역할에 할당된 프로젝트, 작업 및 문제를 기반으로 달력을 만듭니다.

   * 만든 달력

     캘린더 만들기에 대한 자세한 내용은 [캘린더 보고서 개요](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md)를 참조하세요.

   * 다른 사용자가 사용자와 공유한 달력

     일정 공유에 대한 자세한 내용은 [[!UICONTROL 일정 공유] 보고서](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)를 참조하세요.

1. (조건부) **[!UICONTROL 보기]** 드롭다운을 클릭한 다음 보려는 달력 기간을 선택합니다.
   ![일정 기간](assets/view-menu-calendar-report-350x189.png)
다음 달력 보고서 보기 중에서 선택할 수 있습니다.

   * **[!UICONTROL 월]**: 일정 4주를 표시합니다.
   * **[!UICONTROL 주]**: 일정 1주를 표시합니다.
   * **[!UICONTROL Gantt]**: 달력의 연속 보기를 표시합니다.

     아래로 또는 옆으로 스크롤하여 **Gantt** 보기에서 더 많은 이벤트를 볼 수 있습니다. 뷰에 대해 데이터가 채워지면 로드 기호가 나타납니다.

   >[!NOTE]
   >
   >**월** 및 **주** 보기에서 현재 또는 미래의 이벤트(오늘이나 미래의 날을 포함하는 한 여러 날에 걸친 이벤트 포함)에는 프로젝트 또는 일정 그룹의 색상에 해당하는 음영이 있습니다. 이전 이벤트에는 더 이상 최신 상태가 아님을 나타내기 위해 더 밝은 음영이 있지만, 이러한 이벤트를 선택하여 볼 수는 있습니다.

1. (선택 사항) **월** 또는 **주** 보기에서 일정을 보고 있는 경우 다음 옵션으로 일정 보기를 변경할 수 있습니다.

   <!--   * To include or exclude weekends:
      1. On the **[!UICONTROL Calendar]** toolbar, click **[!UICONTROL Calendar Actions]**, then from the drop-down list select either **[!UICONTROL Show Weekend]** or **[!UICONTROL Hide Weekend]**.-->

   * 표시된 날짜를 빠르게 변경하려면:

      1. **[!UICONTROL 달력]** 도구 모음에서 날짜 표시기의 왼쪽 화살표를 클릭하여 달력에서 뒤로 이동하거나 오른쪽 화살표를 클릭하여 앞으로 이동합니다.

         ![날짜를 변경하려면 화살표를 클릭하십시오](assets/click-arrows-to-change-dates-calendar-report.png)

         표시된 날짜는 현재 달력 보기를 기준으로 간격에 따라 조정됩니다. 예를 들어 **주** 보기에서 달력을 보고 있는 경우 선택한 화살표에 따라 달력이 1주 앞으로 또는 1주 뒤로 표시됩니다.

      1. (선택 사항) 현재 날짜로 돌아가려면 [!UICONTROL **오늘**]&#x200B;을 클릭하세요.

1. (선택 사항) 달력에 연결된 프로젝트 또는 달력 그룹화에 대한 이벤트를 숨기려면 프로젝트 목록에서 프로젝트 또는 달력 그룹화를 지웁니다.
   ![이벤트 숨기기](assets/hide-events-for-project-or-cal-grouping.png)
프로젝트 목록에서 [!UICONTROL 프로젝트] 또는 일정 그룹을 선택하여 이벤트를 다시 표시할 수 있습니다.

## 달력 보고서 이벤트 세부 사항 보기

현재 이벤트와 과거 이벤트 모두에 대한 이벤트 세부 사항을 달력에서 볼 수 있습니다.

1. 세부 사항을 알고 싶은 이벤트로 이동한 다음 이벤트를 클릭합니다. 세부 사항은 오른쪽의 패널에서 열립니다.
1. (선택 사항) 연결된 프로젝트, 작업 또는 문제를 열려면 개체의 제목을 클릭합니다.
