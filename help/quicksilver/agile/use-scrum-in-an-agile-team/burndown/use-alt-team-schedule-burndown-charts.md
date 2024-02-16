---
product-area: agile-and-teams
navigation-topic: burndown
title: 번다운 차트에 대체 팀 일정 사용
description: 에 정의된 일정 [!DNL Adobe Workfront] 번다운 시 휴무(주말 및 공휴일)를 제외하여 번다운 차트에 영향을 줍니다.
author: Lisa
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# 번다운 차트에 대체 팀 일정 사용

에 정의된 일정 [!DNL Adobe Workfront] 번다운 시 휴무(주말 및 공휴일)를 제외하여 번다운 차트에 영향을 줍니다.

번다운 차트는 기본적으로 기본 일정을 사용합니다. 애자일 팀은 기본 일정 외에도 팀별 비근무일을 통합하기 위해 대체 일정을 사용하도록 선택할 수 있습니다. 이 대체 일정은 팀에 할당된 모든 반복의 번다운 차트에 반영됩니다. 대체 일정은 번다운 차트에만 영향을 줍니다. (기본 일정에 대한 자세한 정보와 [!DNL Workfront] 관리자가 팀별 일정을 만들 수 있습니다. 다음을 참조하십시오. [일정 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

번다운 차트는 일부 요일을 고려하지 않습니다. 예를 들어 팀이 매주 금요일에 4시간씩 근무하는 경우 번다운 차트에 하루로 표시됩니다.

번다운 차트 사용에 대한 자세한 내용은 [애자일 번다운 차트 개요](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜*</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Work] 이상</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜 또는 라이선스 유형을 확인하려면 다음으로 문의하십시오. [!DNL Workfront] 관리자.

## 번다운 차트에 대체 팀 일정 사용

1. 다음을 확인합니다. [!DNL Workfront] 관리자가에 설명된 대로 이미 대체 일정을 만들었습니다. [일정 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Adobe Workfront]을 클릭한 다음 을 클릭합니다 **[!UICONTROL 팀]**.

1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)그런 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 창에서 팀을 검색합니다.

1. 관리할 애자일 팀을 선택합니다.
1. 다음을 클릭합니다. **[!UICONTROL 자세히]** 메뉴, 선택 **[!UICONTROL 편집]**.

1. 다음에서 **[!UICONTROL 애자일]** 섹션, **[!UICONTROL 예약]** 영역에서 드롭다운 메뉴에서 새 일정을 선택합니다.

1. **[!UICONTROL 변경 내용 저장]**&#x200B;을 클릭합니다.
