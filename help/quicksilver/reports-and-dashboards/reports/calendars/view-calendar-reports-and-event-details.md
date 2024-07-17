---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: 달력 보고서 및 이벤트 세부 정보 보기
description: Adobe Workfront에서 생성했거나 공유한 캘린더 보고서 및 이벤트 세부 사항을 볼 수 있습니다.
author: Lisa
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

# 달력 보고서 및 이벤트 세부 정보 보기

Adobe Workfront에서 생성했거나 공유한 캘린더 보고서 및 이벤트 세부 사항을 볼 수 있습니다.

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
   <td> <p>[!UICONTROL Request] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>[!UICONTROL 보고서], [!UICONTROL 대시보드] 및 [!UICONTROL 달력]에 대한 [!UICONTROL 보기] 이상 액세스</p> <p>참고: 여전히 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하십시오. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>달력 보고서에 대한 [!UICONTROL 보기] 이상의 권한</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

## 캘린더 보고서 보기

1. [!DNL Adobe Workfront]의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 달력]**&#x200B;을 클릭합니다.

   액세스 수준에 따라 다음 캘린더가 표시될 수 있습니다.

   * 기본 [!DNL Adobe Workfront] 캘린더\

     Workfront은 사용자에게 할당되거나 할당된 팀, 그룹 또는 역할에 할당된 프로젝트, 작업 및 문제를 기반으로 달력을 만듭니다.
   * 만든 캘린더\

     일정 만들기에 대한 자세한 내용은 [일정 보고서 개요](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md)를 참조하세요.

   * 다른 사용자가 귀하와 공유한 캘린더

     일정 공유에 대한 자세한 내용은 [[!UICONTROL 일정 공유] 보고서](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)를 참조하세요.

1. (조건부) **[!UICONTROL 보기]** 드롭다운을 클릭한 다음 보려는 일정 기간을 선택합니다.\
   ![일정 기간](assets/view-menu-calendar-report-350x189.png)\
   다음 달력 보고서 보기 중에서 선택할 수 있습니다.

   * **[!UICONTROL 월]**: 달력의 4주를 표시합니다.
   * **[!UICONTROL 주]**: 달력의 1주일을 표시합니다.
   * **[!UICONTROL 간트]**: 캘린더의 연속 보기를 표시합니다\

     ![[!UICONTROL 간트] 일정 보고서](assets/gantt-calendar-report.png)
아래로 스크롤하거나 옆으로 스크롤하여 [!UICONTROL 간트] 보기에서 더 많은 이벤트를 볼 수 있습니다. 보기의 데이터가 채워질 때 로딩 기호가 나타납니다.
   >[!NOTE]
   >
   >[!UICONTROL 월] 및 [!UICONTROL 주] 보기에서 현재 또는 미래 이벤트(오늘 또는 미래 날짜가 포함된 경우 여러 날에 걸친 이벤트 포함)에는 프로젝트 또는 일정 그룹화의 색상에 해당하는 음영이 있습니다. 이전 이벤트에는 더 이상 최신 상태가 아님을 나타내는 더 밝은 음영이 표시되지만, 이러한 이벤트를 선택하여 볼 수 있습니다.

1. (선택 사항) [!UICONTROL 월] 또는 [!UICONTROL 주] 보기에서 캘린더를 보는 경우 다음 옵션을 사용하여 캘린더 보기를 변경할 수 있습니다.

   * 주말을 포함하거나 제외하려면 다음을 수행합니다.

      1. **[!UICONTROL 일정]** 도구 모음에서 **[!UICONTROL 일정 작업]**&#x200B;을 클릭한 다음 드롭다운 목록에서 **[!UICONTROL 주말 표시]** 또는 **[!UICONTROL 주말 숨기기]**&#x200B;를 선택합니다.
   * 표시된 일자를 빠르게 변경하려면

      1. **[!UICONTROL 달력]** 도구 모음에서 날짜 표시기의 왼쪽 화살표를 클릭하여 달력에서 뒤로 이동하거나 오른쪽 화살표를 클릭하여 앞으로 이동합니다.\

         날짜를 변경하려면 ![화살표를 클릭하세요](assets/click-arrows-to-change-dates-calendar-report.png)\
         표시되는 날짜는 현재 달력 보기에 따라 간격에 따라 조정됩니다. 예를 들어, [!UICONTROL 주] 보기에서 달력을 보는 경우 선택한 화살표에 따라 달력은 1주일 앞으로 또는 1주일 뒤로 표시됩니다.

      1. (선택 사항) 현재 날짜로 돌아가려면 **Today**&#x200B;를 클릭합니다.


1. (선택 사항) 전체 화면으로 달력을 보려면 **[!UICONTROL 달력]** 도구 모음의 오른쪽에 있는 전체 화면 화살표를 클릭합니다.
   날짜를 변경하려면 ![화살표를 클릭하세요](assets/click-arrows-to-change-dates-calendar-report.png)\
   캘린더의 일반 보기로 돌아가려면 Esc 키를 누릅니다.

1. (선택 사항) 달력에 연결된 프로젝트 또는 달력 그룹화에 대한 이벤트를 숨기려면 프로젝트 목록에서 프로젝트 또는 달력 그룹화를 지웁니다.
   ![이벤트 숨기기](assets/hide-events-for-project-or-cal-grouping.png)\
   프로젝트 목록에서 [!UICONTROL 프로젝트] 또는 일정 그룹화를 선택하여 이벤트를 다시 표시할 수 있습니다.

## 달력 보고서 이벤트 세부 정보 보기

현재 이벤트와 과거 이벤트 모두에 대한 이벤트의 세부 정보를 달력에서 볼 수 있습니다.

1. 세부 정보를 알 이벤트로 이동한 다음 이벤트를 클릭합니다.\
   이벤트에 대한 세부 정보 페이지가 열립니다.\
   ![calendar_report_EventDetails.png](assets/calendar-report-eventdetails-350x145.png)

1. (선택 사항) 객체에 대한 추가 세부 정보를 보려면 다음과 같이 하십시오.

   1. 프로젝트, 작업 또는 문제 이름 위로 마우스를 가져갑니다.

      객체에 대한 세부 정보 페이지가 열립니다.\
      ![additional_object_details_-_calendar_report.png](assets/additional-object-details---calendar-report-350x131.png)

   1. (선택 사항) 연결된 프로젝트, 작업 또는 문제를 열려면 개체의 제목을 클릭합니다.
   1. (선택 사항) 열려 있는 모든 세부 정보 페이지를 닫으려면 이벤트 세부 정보 페이지의 바깥쪽을 클릭합니다.
