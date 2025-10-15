---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: 애자일 팀 만들기
description: Adobe Workfront을 사용하면 애자일 팀이 점진적이고 조직적인 방식으로 작업을 완료할 수 있습니다.
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 1%

---

# 애자일 팀 만들기

<!--Audited: 01/2024-->

[!DNL Adobe Workfront]을(를) 사용하면 애자일 팀이 점진적이고 조직화된 방식으로 작업을 완료할 수 있습니다.

조직의 모든 사용자는 애자일 팀을 보고 백로그, 반복, 스토리 보드 및 개별 스토리를 포함하여 팀에 대한 모든 애자일 구성 요소를 볼 수 있습니다. 그러나 작업에 대한 [!UICONTROL 편집] 액세스 권한이 있는 팀원만 팀에 할당된 작업을 변경할 수 있습니다.

[!DNL Workfront]은(는) 다음 애자일 방법론을 지원합니다.

* **[!UICONTROL 스크럼]**: 팀에 수행해야 하는 작업이 백로그되어 있습니다. 팀이 특정 작업 청크에서 작업할 준비가 되면 작업이 백로그에서 반복으로 이동됩니다. 스크럼 팀 관리에 대한 자세한 내용은 [애자일 팀의 스크럼](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md)을 참조하십시오.

* **[!UICONTROL Kanban]:** 팀은 사전 결정된 상태에서 Kanban 보기에서 작업을 이동합니다. 기본 상태는 백로그, 처리 중 및 완료입니다. 칸반 팀 관리에 대한 자세한 내용은 [애자일 팀의 칸반](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>표준</p>
   <p>새 애자일 팀 만들기 계획</p>
  <p>팀 또는 그 이상을 작업하여 팀을 애자일 팀으로 전환</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 애자일 방법론 결정

애자일 팀에 대해 스크럼 또는 칸반 애자일 방법론을 사용할 수 있습니다. 각 방법론은 다양한 이점을 제공합니다. 애자일 팀이 작동하는 방식에 따라 사용하기 위해 선택하는 애자일 방법론이 결정됩니다.

[!DNL Workfront]의 스크럼과 칸반 애자일 방법론을 사용하면 스토리 보드에서 스토리를 이동하여 스토리의 상태 변경 및 진행 상황을 나타낼 수 있습니다.

[!DNL Workfront]의 스크럼 및 Kanban 애자일 방법론은 다음과 같은 점에서 다릅니다.

### [!DNL Workfront]에서 Kanban을 사용할 때의 이점

[!DNL Kanban]의 [!DNL Workfront] 애자일 방법론을 사용하면 진행 중인 작업의 양을 제한하면서 애자일 스토리 보드에서 스토리를 보다 쉽게 이동할 수 있습니다. [!DNL Kanban] 애자일 방법론을 사용할 때 시작 및 종료 날짜가 없습니다.

다음 기능은 이 방법을 지원합니다.

* [!DNL Kanban] 애자일 스토리 보드에 백로그를 표시합니다.
자세한 내용은 [백로그를 [!UICONTROL Kanban] 보드에 추가](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)를 참조하십시오.

* 다른 항목이 완료와 동일한 상태로 이동될 때 백로그에 있는 항목이 [!UICONTROL Kanban] 애자일 스토리 보드에 자동으로 추가되도록 구성하십시오.
자세한 내용은 문서 [Kanban 구성](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5)의 [백로그에서 자동으로 추가할 스토리 구성](../../agile/get-started-with-agile-in-workfront/configure-kanban.md) 섹션을 참조하십시오.

* [!UICONTROL Kanban] 애자일 스토리 보드에 표시할 WIP(Work In Progress) 한도를 구성합니다.
자세한 내용은 [Kanban 보드에서 WIP(작업 진행 중) 제한 관리](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)를 참조하십시오.

### [!DNL Workfront]에서 스크럼 사용의 이점

[!DNL Workfront]의 스크럼 애자일 방법론을 사용하면 애자일 반복에 스토리 집합을 추가하고 해당 반복에 대한 스토리 보드를 만들 수 있습니다. 반복은 사용자가 정의하는 시작 및 종료 날짜를 기반으로 합니다.

다음 기능은 이 방법을 지원합니다.

* [!UICONTROL 스크럼] 스토리 보드에 문제 포함
* 애자일 팀의 백로그에 문제 포함
* 하위 작업은 [!UICONTROL 스크럼] 스토리 보드에 표시될 수 있습니다.
* 번다운 차트를 보고 반복 중 스토리에 대한 진행률을 확인합니다.
자세한 내용은 [애자일 번다운 차트 개요](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md)를 참조하세요.

## 애자일 팀 만들기

{{step1-to-team}}

1. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)을 클릭한 다음 **[!UICONTROL 새 팀 만들기]**&#x200B;를 클릭합니다.

   ![새 팀 만들기 선택](assets/create-new-team.png)

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
      <td role="rowheader"><strong>[!UICONTROL 애자일 팀입니다.]</strong> </td> 
      <td>이 새 팀을 애자일 팀으로 구성하려면 이 옵션을 선택하십시오.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>[!UICONTROL 이 활성 상태입니다]</strong> </td> 
      <td>이 팀을 활성화하려면 이 옵션을 선택하십시오. 비활성 팀은 작업에 할당할 다른 사용자에게 표시되지 않습니다. </td> 
     </tr>


   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL 그룹]</strong> </td> 
      <td> <p>팀에 추가할 그룹 이름을 입력한 다음 드롭다운 목록에 표시될 때 이름을 선택합니다.</p> <p><b>메모</b></p> <p> 팀이 그룹 또는 하위 그룹에 할당되면 해당 그룹 또는 하위 그룹의 모든 그룹 관리자는 팀의 구성원이 되지 않고도 팀을 관리할 수 있습니다. 그룹 관리자는 [!UICONTROL Main Menu]에서 [!UICONTROL Teams] 영역으로 이동하여 [!UICONTROL Switch Teams] 화살표 <img src="assets/switch-team-icon.png" alt="팀 전환 아이콘">을(를) 클릭하여 자신이 관리하는 그룹에 할당된 모든 팀을 나열할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 팀 구성원]</strong> </td> 
      <td>팀에 속한 사용자의 이름을 입력한 다음 드롭다운 목록에 표시될 때 이름을 선택합니다.<br>이 프로세스를 반복하여 팀에 여러 사용자를 추가합니다.<br>사용자는 둘 이상의 팀에 속할 수 있으므로 애자일 팀과 애자일 팀이 아닌 팀 모두에 속할 수 있습니다.</td> 
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

   * [[!UICONTROL Kanban] 구성](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [[!UICONTROL 스크럼] 구성](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## 기존 팀을 애자일 팀으로 전환

기존 팀을 애자일 팀으로 변환할 수 있습니다.

{{step1-to-team}}

1. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)을 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

1. 애자일 팀으로 변환할 팀을 선택합니다.
1. **[!UICONTROL 자세히]** 메뉴를 클릭한 다음 **[!UICONTROL 편집]**&#x200B;을 선택합니다.

   [!UICONTROL 표준], [!UICONTROL 플랜] 또는 [!UICONTROL 작업] 라이선스가 있는 팀원만 이 옵션을 참조하세요.
   ![편집 선택](assets/edit-team-settings.png)

1. **[!UICONTROL 애자일]** 섹션에서 **[!UICONTROL 애자일 팀입니다]**&#x200B;를 선택합니다.

1. **[!UICONTROL 방법론]** 섹션에서 팀이 **[!UICONTROL 스크럼]** 또는 **[!UICONTROL Kanban]** 애자일 방법론을 사용할지 여부를 선택합니다.

1. **변경 내용 저장**&#x200B;을 클릭합니다.

   팀은 애자일 팀으로 저장됩니다. 팀을 편집할 때 새 팀을 스크럼 또는 칸반 팀으로 구성할 수 있습니다.

   자세한 내용은 다음 문서를 참조하십시오.

   * [[!UICONTROL Kanban] 구성](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [[!UICONTROL 스크럼] 구성](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
