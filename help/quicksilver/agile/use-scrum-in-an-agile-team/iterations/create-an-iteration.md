---
product-area: agile-and-teams
navigation-topic: iterations
title: 반복 만들기
description: 반복은 작업 용량을 계획하는 Screm Agile 팀의 주요 구성 요소입니다. [!DNL Adobe Workfront] 스크럼 애자일 팀이 팀 요구 사항에 맞게 여러 이터레이션을 작성하여 작업을 관리할 수 있도록 합니다.
author: Lisa
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '1049'
ht-degree: 0%

---

# 반복 만들기

반복은 작업 용량을 계획하는 Screm Agile 팀의 주요 구성 요소입니다. [!DNL Adobe Workfront] 스크럼 애자일 팀이 팀 요구 사항에 맞게 여러 이터레이션을 작성하여 작업을 관리할 수 있도록 합니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Review] 이상</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 확인하려면 [!DNL Workfront] 관리자

## 반복 추가

를 사용하십시오 [!UICONTROL 반복 추가] 반복을 신속하게 생성하고 나중에 작업 및 문제를 추가할 수 있는 기능입니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

1. 설정 **[!UICONTROL 반복]** 탭, **[!UICONTROL 반복 추가]**.\
   ![](assets/add-iteration-adobe-350x275.png)

1. 다음을 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Iteration Name]</strong></td> 
      <td>이터레이션의 이름을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 목표]</strong></td> 
      <td>반복에 대해 원하는 목표를 추가합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 시작 날짜]</strong></td> 
      <td>반복을 시작할 날짜를 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 종료 날짜]</strong></td> 
      <td><p>반복을 종료해야 하는 날짜를 입력합니다. [!DNL Workfront] 종료 날짜를 시작 날짜로부터 4주 이내로 설정할 것을 권장합니다.</p><p>팁: 작업 일을 종료 날짜로 선택해야 합니다. 번다운 차트는 계산에서 근무 일수만을 사용합니다.<br>기본적으로 번다운 차트는 기본 스케줄을 사용하여 작업 일수를 정의합니다(에 설명된 대로). <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">예약 만들기</a>). 또는, 팀별 비근무일을 통합하기 위해, 애자일 팀은 대체 스케줄을 사용하도록 선택할 수 있습니다. <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">애자일 팀 만들기</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Capacity]</strong></td> 
      <td> 이터레이션의 용량을 지정합니다. 반복에서 팀이 수행할 수 있는 지점 또는 시간 수입니다. 입력하는 숫자는 반복에 있는 모든 스토리의 합에서 포인트 또는 시간 수보다 크거나 같아야 합니다.<br>[!DNL Workfront] 기본적으로 이 필드는 50개의 용량으로 사전에 채웁니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>팀의 포커스 비율을 지정합니다. 팀의 모든 구성원이 이 반복에 완전히 집중하게 되면 포커스가 100%가 됩니다.<br>[!DNL Workfront] 기본적으로 이 필드는 100%로 미리 채웁니다. </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 제출]**. 반복을 만들었으므로 이제 스토리를 추가해야 합니다. 자세한 내용은 [기존 반복에 스토리 추가](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## 에서 반복 계획 [!UICONTROL 백로그] 탭

를 사용하십시오 [!UICONTROL 계획 반복] 백로그의 작업을 사용하여 반복을 만드는 기능입니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

1. 선택 **[!UICONTROL 백로그]** 왼쪽 패널에 표시됩니다. 그런 다음 **[!UICONTROL 계획 반복]**.

1. 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Iteration Name]</strong></td> 
      <td>이터레이션의 이름을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 시작 날짜]</strong></td> 
      <td> 이터레이션을 시작할 날짜를 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 종료 날짜]</strong> </td> 
      <td><p>반복을 종료해야 하는 날짜를 지정합니다. [!DNL Workfront] 종료 날짜를 시작 날짜로부터 4주 이내로 설정할 것을 권장합니다.</p><p>팁: 작업 일을 종료 날짜로 선택해야 합니다. 번다운 차트는 계산에서 근무 일수만을 사용합니다.<br>기본적으로 번다운 차트는 기본 스케줄을 사용하여 작업 일수를 정의합니다(에 설명된 대로). <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">예약 만들기</a>). 또는, 팀별 비근무 일수를 통합하기 위해, 애자일 팀이 대체 일정을 사용하도록 선택할 수 있습니다( 에 설명된 대로). <a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt--team-schedule-burndown-charts.md" class="MCXref xref">번다운 차트에 대체 팀 스케줄 사용</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>팀의 포커스 비율을 지정합니다. 팀의 모든 구성원이 이 반복에 완전히 집중하게 되면 포커스가 100%가 됩니다.<br>[!DNL Workfront] 이 필드를 팀의 이전 이터레이션의 평균 값으로 미리 채웁니다. 팀의 첫 번째 반복인 경우 이 필드 값은 기본적으로 0입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Capacity]</strong></td> 
      <td> 이터레이션의 용량을 지정합니다. 반복에서 팀이 수행할 수 있는 지점 또는 시간 수입니다. 입력하는 숫자는 반복에 있는 모든 스토리의 합에서 포인트 또는 시간 수보다 크거나 같아야 합니다.<br>[!DNL Workfront] 이 필드를 팀의 이전 이터레이션의 평균 값으로 미리 채웁니다. 팀의 첫 번째 반복인 경우 이 필드 값은 기본적으로 0입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL 목표]</strong></td> 
      <td> 반복에 대한 목표를 지정합니다. 이 필드는 필수가 아닙니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 지금 반복에 추가할 스토리를 선택하거나 이 단계를 건너뛰고 나중에 반복에 스토리를 추가할 수 있습니다. 백로그 맨 위에 있는 이야기들이 우선순위가 더 높습니다. 책에 들어맞는 얘기는 초록색으로 물든다. 그렇지 않으면 빨간색으로 강조 표시됩니다.\
   작업과 문제를 모두 단일 반복에 추가할 수 있습니다.

   * **반복에 작업을 추가하려면 다음을 수행합니다.** 설정 **[!UICONTROL 백로그]** 탭에서 다음을 확인합니다 **[!UICONTROL 스토리]** 탭이 선택되어 있습니다. 백로그를 볼 때 이 탭이 기본적으로 선택됩니다. 반복에 추가할 스토리를 선택합니다.\

      반복에 작업을 추가하면 작업 시작 날짜가 [[!UICONTROL 이해] 작업 시작 날짜를 반복 시 계산하는 방법](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration).

   * **반복에 문제를 추가하려면** 설정 **[!UICONTROL 백로그]** 탭에서 **[!UICONTROL 문제]** 탭. 반복에 추가할 문제를 선택합니다.

1. **[!UICONTROL 저장]을 클릭합니다.**
이터레이션이 생성됩니다.

1. (선택 사항) 기존 반복에 스토리를 추가하려면 [기존 반복에 스토리 추가](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## 반복에 추가될 때 작업 시작 날짜를 계산하는 방법을 알아봅니다 {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

작업을 스토리로 반복에 추가하면 [!UICONTROL 작업 완료] 제한은 각 스토리에 사용됩니다. 대부분의 경우 작업의 계획 시작 날짜는 다음 공식을 기준으로 계산됩니다.

[!UICONTROL 반복 종료 날짜] 빼기(-) [!UICONTROL 작업 기간] equals (=) [!UICONTROL 작업 계획 시작 날짜]

다음 [!UICONTROL 프로젝트 종료 날짜] 프로젝트 시작 날짜가 반복 시작 날짜 이후이고 프로젝트 종료 날짜가 반복 종료 날짜 이후인 경우 대신 사용됩니다.

반복 날짜가 아닌 기본적으로 프로젝트 날짜를 사용하도록 개별 스크럼 팀을 구성할 수 있습니다. 자세한 내용은 섹션을 참조하십시오 [작업 항목을 이터레이션에 추가할 때 날짜가 적용되는 방식을 구성합니다](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) 기사 [스크럼 구성](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).
