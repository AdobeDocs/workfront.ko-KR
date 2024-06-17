---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: 애자일 팀 만들기
description: Adobe Workfront을 사용하면 애자일 팀이 점진적이고 조직적인 방식으로 작업을 완료할 수 있습니다.
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '1012'
ht-degree: 1%

---

# 애자일 팀 만들기

<!--Audited: 01/2024-->

[!DNL Adobe Workfront] 애자일 팀이 점진적이고 조직적인 방식으로 작업을 완료할 수 있도록 합니다.

조직의 모든 사용자는 애자일 팀을 보고 백로그, 반복, 스토리 보드 및 개별 스토리를 포함하여 팀에 대한 모든 애자일 구성 요소를 볼 수 있습니다. 단, 이 있는 팀의 멤버만 [!UICONTROL 편집] 작업 액세스는 팀에 할당된 작업을 변경할 수 있습니다.

[!DNL Workfront] 는 다음과 같은 애자일 방법론을 지원합니다.

* **[!UICONTROL 스크럼]**: 팀에는 수행해야 하는 작업이 백로그를 가지고 있습니다. 팀이 특정 작업 청크에서 작업할 준비가 되면 작업이 백로그에서 반복으로 이동됩니다. 스크럼 팀 관리에 대한 자세한 내용은 [애자일 팀의 스크럼](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL 칸반]:** 팀은 사전 결정된 상태에서 Kanban 보기에서 작업을 이동합니다. 기본 상태는 백로그, 처리 중 및 완료입니다. Kanban 팀 관리에 대한 자세한 내용은 [애자일 팀의 칸반](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
   <td> <p>새로운 기능: 표준</p>
   현재: 
   <ul><li><p>새 애자일 팀을 만들려면 [!UICONTROL Plan]</p></li> 
   <li><p>팀을 애자일 팀으로 전환하려면 [!UICONTROL Work] 이상</p></li></ul> </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜 또는 라이선스 유형을 확인하려면 다음으로 문의하십시오. [!DNL Workfront] 관리자.

+++

## 애자일 방법론 결정

애자일 팀에 대해 스크럼 또는 칸반 애자일 방법론을 사용할 수 있습니다. 각 방법론은 다양한 이점을 제공합니다. 애자일 팀이 작동하는 방식에 따라 사용하기 위해 선택하는 애자일 방법론이 결정됩니다.

의 스크럼 및 칸반 애자일 방법론 모두 [!DNL Workfront] 스토리 보드에서 스토리를 이동하여 스토리의 상태 변경 및 진행 상황을 나타낼 수 있습니다.

의 스크럼 및 칸반 애자일 방법론 [!DNL Workfront] 다음과 같은 점에서 차이가 있습니다.

### 에서 Kanban 사용의 이점 [!DNL Workfront]

다음 [!DNL Kanban] 의 애자일 방법론 [!DNL Workfront] 애자일 스토리 보드에서 스토리를 보다 쉽게 이동할 수 있도록 하면서 진행 중인 작업의 양을 제한할 수 있습니다. 를 사용할 때 시작 및 종료 날짜가 없습니다. [!DNL Kanban] 애자일 방법론.

다음 기능은 이 방법을 지원합니다.

* 의 백로그를 표시합니다. [!DNL Kanban] 애자일 스토리 보드.\
   자세한 내용은 [백로그를 다음에 추가합니다. [!UICONTROL 칸반] 보드](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* 백로그에 항목을 자동으로 추가하도록 구성 [!UICONTROL 칸반] 다른 항목이 완료와 동일한 상태로 이동될 때 애자일 스토리 보드.\
   자세한 내용은 섹션을 참조하십시오 [백로그에서 자동으로 추가될 스토리를 구성합니다.](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) 이 문서에서 [칸반 구성](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* 에 표시할 WIP(Work In Progress) 한도 구성 [!UICONTROL 칸반] 애자일 스토리 보드.\
   자세한 내용은 [Kanban 보드에서 WIP(Work In Progress) 한도 관리](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### 에서 스크럼 사용의 이점 [!DNL Workfront]

의 스크럼 애자일 방법론 [!DNL Workfront] 에서는 애자일 반복에 스토리 세트를 추가하고 해당 반복에 대한 스토리 보드를 만들 수 있습니다. 반복은 사용자가 정의하는 시작 및 종료 날짜를 기반으로 합니다.

다음 기능은 이 방법을 지원합니다.

* 에 문제 포함 [!UICONTROL 스크럼] 스토리보드
* 애자일 팀의 백로그에 문제 포함
* 하위 작업은 [!UICONTROL 스크럼] 스토리보드
* 번다운 차트를 보고 반복 중 스토리에 대한 진행률을 확인합니다.\
   자세한 내용은 [애자일 번다운 차트 개요](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## 애자일 팀 만들기

{{step1-to-team}}

1. 다음을 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)을 클릭한 다음 을 클릭합니다 **[!UICONTROL 새 팀 만들기]**.

   ![새 팀 만들기를 선택합니다.](assets/create-new-team-350x198.png)

   새 팀 상자가 표시됩니다.

1. 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 팀 이름]</strong> </td> 
      <td>새 애자일 팀의 이름을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 애자일 팀입니다]</strong> </td> 
      <td>이 새 팀을 애자일 팀으로 구성하려면 이 옵션을 선택하십시오.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>[!UICONTROL이 활성화됨]</strong> </td> 
      <td>이 팀을 활성화하려면 이 옵션을 선택하십시오. 비활성 팀은 작업에 할당할 다른 사용자에게 표시되지 않습니다. </td> 
     </tr>


   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Group]</strong> </td> 
      <td> <p>팀에 추가할 그룹 이름을 입력한 다음 드롭다운 목록에 표시될 때 이름을 선택합니다.</p> <p><b>메모</b></p> <p> 팀이 그룹 또는 하위 그룹에 할당되면 해당 그룹 또는 하위 그룹의 모든 그룹 관리자는 팀의 구성원이 되지 않고도 팀을 관리할 수 있습니다. 그룹 관리자는 [!UICONTROL Main Menu]에서 [!UICONTROL Teams] 영역으로 이동하여 [!UICONTROL Switch Teams] 화살표를 클릭합니다 <img src="assets/switch-team-icon.png" alt="팀 전환 아이콘"> 자신이 관리하는 그룹에 할당된 모든 팀을 나열합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 팀 구성원]</strong> </td> 
      <td>팀에 속한 사용자의 이름을 입력한 다음 드롭다운 목록에 표시될 때 이름을 선택합니다.<br>이 프로세스를 반복하여 팀에 여러 사용자를 추가합니다.<br>사용자는 두 개 이상의 팀에 있을 수 있으므로 애자일 팀과 애자일이 아닌 팀에 모두 있을 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 설명]</strong> </td> 
      <td><p>팀에 대한 설명을 입력합니다.</p> <p>팀을 선택하면 [!UICONTROL Teams] 영역의 오른쪽 상단에 설명이 표시됩니다.</p>
      <p>설명이 긴 경우 클릭하여 팝업에 전체 설명을 표시할 수 있습니다. [!UICONTROL 팀 설정] 편집 액세스 권한이 있는 경우 팝업에서 직접 설명을 편집할 수도 있습니다.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**.

   애자일 팀 구성에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [구성 [!UICONTROL 칸반]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [구성 [!UICONTROL 스크럼]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## 기존 팀을 애자일 팀으로 전환

기존 팀을 애자일 팀으로 변환할 수 있습니다.

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Adobe Workfront]을 클릭한 다음 을 클릭합니다 **[!UICONTROL 팀]**.
1. 다음을 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)을 클릭한 후 드롭다운 메뉴에서 새 팀을 선택하거나 검색 창에서 팀을 검색합니다.

1. 애자일 팀으로 변환할 팀을 선택합니다.
1. 다음을 클릭합니다. **[!UICONTROL 자세히]** 메뉴, 선택 **[!UICONTROL 편집]**.\
   다음 중 하나를 가진 팀원만 [!UICONTROL 플랜] 또는 [!UICONTROL 작업] 라이센스 이 옵션을 참조하십시오.\
   ![](assets/edit-team-settings-350x205.png)

1. 다음에서 **[!UICONTROL 애자일]** 섹션, 선택 **[!UICONTROL 애자일 팀입니다]**.

1. 다음에서 **[!UICONTROL 방법론]** 섹션에서 팀이 **[!UICONTROL 스크럼]** 또는 **[!UICONTROL 칸반]** 애자일 방법론.

1. 클릭 **변경 사항을 저장합니다.**

   팀은 애자일 팀으로 저장됩니다. 팀을 편집할 때 새 팀을 스크럼 또는 칸반 팀으로 구성할 수 있습니다.

   자세한 내용은 다음 문서를 참조하십시오.

   * [구성 [!UICONTROL 칸반]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [구성 [!UICONTROL 스크럼]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
