---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: 애자일 팀 만들기
description: Adobe Workfront을 사용하면 민첩한 팀이 점진적이고 체계적으로 작업을 완료할 수 있습니다.
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 0%

---

# 애자일 팀 만들기

[!DNL Adobe Workfront] 민첩한 팀이 점진적이고 체계적으로 작업을 완료할 수 있도록 합니다.

조직의 모든 사용자는 민첩한 팀을 볼 수 있고 백로그, 반복, 스토리 보드 및 개별 스토리를 포함하여 팀에 대한 모든 애자일 구성 요소를 볼 수 있습니다. 하지만, [!UICONTROL 편집] 작업에 액세스하면 팀에 할당된 작업을 변경할 수 있습니다.

[!DNL Workfront] 는 다음과 같은 민첩한 방법을 지원합니다.

* **[!UICONTROL 스크럼]**: 팀들은 해야 할 일이 많다. 팀이 특정 작업 청크에 대해 작업할 준비가 되면 작업이 백로그에서 반복으로 이동됩니다. 스크럼 팀 관리에 대한 자세한 내용은 [애자일 팀의 스크럼](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL 간판]:** 팀은 일정 상태에 걸쳐 간판 보기에서 작업을 이동합니다. 기본 상태는 다음과 같습니다. 백로그, 처리 중, 완료 간판 팀 관리에 대한 자세한 내용은 다음을 참조하십시오 [애자일 팀의 간판](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

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
   <td> <p>[!UICONTROL Plan] 새로운 애자일 팀 작성 [!UICONTROL Work] 이상 항목을 사용하여 팀을 민첩한 팀으로 변환합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 확인하려면 [!DNL Workfront] 관리자

## 민첩한 방법론 결정

민첩한 팀에 대해 스크럼 또는 간판 애자일 방법을 사용할 수 있습니다. 각 방법론은 다양한 이점을 제공합니다. 민첩한 팀이 작동하는 방식은 사용자가 사용하려는 민첩한 방법을 결정합니다.

Screm 및 간판 애자일 방법론 모두 [!DNL Workfront] 스토리 보드를 통해 스토리를 이동하여 스토리의 상태 변경 및 진행 상황을 표시할 수 있습니다.

Screm과 간판 애자일 방법론 [!DNL Workfront] 다음과 같은 방법으로 다릅니다.

### 간판 사용 이점 [!DNL Workfront]

다음 [!DNL Kanban] 애자일 방법론 [!DNL Workfront] 진행 중인 작업의 양을 제한하면서 민첩한 스토리 보드 간에 스토리를 보다 쉽게 이동할 수 있습니다. 를 사용할 때 시작 및 종료 날짜가 없습니다 [!DNL Kanban] 기민한 방법론.

다음은 이 방법을 지원하는 기능입니다.

* 백로그를 [!DNL Kanban] 애자일 스토리보드\
   자세한 내용은 [백로그를 [!UICONTROL 간판] 보드](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* 백로그에 자동으로 추가할 항목을 구성합니다 [!UICONTROL 간판] 다른 항목이 완성과 동일한 상태로 이동되면 애자일 스토리 보드.\
   자세한 내용은 섹션을 참조하십시오 [백로그에서 자동으로 추가할 스토리를 구성합니다](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) 기사 [간판 구성](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* WIP(Work In Progress) 제한을 구성하여에 [!UICONTROL 간판] 애자일 스토리보드\
   자세한 내용은 [간판 보드의 진행 중인 작업(WIP) 한도 관리](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Screm을 사용하여 얻을 수 있는 이점 [!DNL Workfront]

의 스크럼 애자일 방법론 [!DNL Workfront] 일련의 스토리를 애자일 반복에 추가하고 해당 반복을 위한 스토리 보드를 만들 수 있습니다. 이터레이션은 사용자가 정의한 시작 날짜와 종료 날짜를 기준으로 합니다.

다음은 이 방법을 지원하는 기능입니다.

* 에 문제 포함 [!UICONTROL 스크럼] 스토리 보드
* 애자일 팀의 백로그에 문제 포함
* 하위 작업은 [!UICONTROL 스크럼] 스토리 보드
* 반복 중 스토리에 대한 진행 상황을 보려면 번다운 차트를 봅니다.\
   자세한 내용은 [Agile Burndown 차트 개요](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## 새로운 애자일 팀 만들기

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.
1. 을(를) 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 **[!UICONTROL 새 팀 만들기]**.

   ![새 팀 만들기를 선택합니다.](assets/create-new-team-350x198.png)

1. 다음 정보를 [!UICONTROL 새 팀] 대화 상자:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Name]</strong> </td> 
      <td>새 애자일 팀의 이름을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Agile Team]입니다.</strong> </td> 
      <td>이 새 팀을 애자일 팀으로 구성하려면 이 옵션을 선택합니다.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Group]</strong> </td> 
      <td> <p>팀에 추가할 그룹의 이름을 입력하고 드롭다운 목록에 표시될 이름을 선택합니다.</p> <p>참고: 한 팀이 그룹이나 하위 그룹에 할당되면 해당 그룹 또는 하위 그룹의 모든 그룹 관리자가 구성원이 아니더라도 팀을 관리할 수 있습니다. 그룹 관리자는 [!UICONTROL 기본 메뉴]에서 [!UICONTROL Teams] 영역으로 이동하여 [!UICONTROL Switch Teams] 화살표를 클릭할 수 있습니다 <img src="assets/switch-team-icon.png" alt="팀 전환 아이콘"> 관리하는 그룹에 할당된 모든 팀을 나열하려면 다음을 수행하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Members]</strong> </td> 
      <td>팀에 있을 사용자의 이름을 입력하기 시작한 다음 드롭다운 목록에 표시될 이름을 선택합니다.<br>이 프로세스를 반복하여 팀에 여러 사용자를 추가합니다.<br>사용자는 두 개 이상의 팀에 있을 수 있으므로 민첩하고 민첩하지 않은 팀에 모두 포함될 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Description]</strong> </td> 
      <td><p>팀에 대한 설명을 입력합니다.</p> <p>팀을 선택하면 [!UICONTROL Teams] 영역의 오른쪽 상단에 설명이 표시됩니다.</p>
      <p>설명이 긴 경우 해당 설명을 클릭하여 팝업에 전체 설명을 표시할 수 있습니다. [!UICONTROL 팀 설정]을 편집할 수 있는 액세스 권한이 있는 경우에는 팝업에서 직접 설명을 편집할 수도 있습니다.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**.

   Agile 팀 구성에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [구성 [!UICONTROL 간판]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [구성 [!UICONTROL 스크럼]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## 기존 팀을 민첩한 팀으로 전환

기존 팀을 민첩한 팀으로 변환할 수 있습니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.
1. 을(를) 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

1. 민첩한 팀으로 변환할 팀을 선택합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 메뉴를 선택한 다음 **[!UICONTROL 편집]**.\
   팀 구성원만 [!UICONTROL 계획] 또는 [!UICONTROL 작업] 라이센스를 보려면 이 옵션을 참조하십시오.\
   ![](assets/edit-team-settings-350x205.png)

1. 에서 **[!UICONTROL 애자일]** 섹션, **[!UICONTROL 애자일 팀입니다]**.

1. 에서 **[!UICONTROL 방법론]** 섹션에서 팀이 **[!UICONTROL 스크럼]** 또는 **[!UICONTROL 간판]** 기민한 방법론.

1. 클릭 **변경 사항을 저장합니다.**

   Agile 팀 구성에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [구성 [!UICONTROL 간판]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [구성 [!UICONTROL 스크럼]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
