---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: 애자일 백로그 관리
description: 작업 및 문제는 팀이 사용 중인 애자일 방법론에 따라 애자일 팀에 할당되고 해당 팀의 백로그에 이야기로 추가될 수 있습니다.
author: Lisa
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '1371'
ht-degree: 0%

---

# 애자일 백로그 관리

다음 작업 항목은 팀이 사용 중인 애자일 방법론에 따라 애자일 팀에 할당되고 해당 팀의 백로그에 이야기로 추가될 수 있습니다.

* **[!UICONTROL 스크럼 애자일 팀]:** 작업 및 문제를 애자일 팀에 할당하고 백로그에 추가할 수 있습니다.
* **[!UICONTROL 칸반 애자일 팀]:** 작업은 애자일 팀에 할당하고 백로그에 추가할 수 있습니다. 에 설명된 대로 사용자는 애자일 스토리 보드에서 직접 백로그를 볼 수 있습니다. [[!UICONTROL 백로그 추가] 칸반 보드로](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md). 팀은 이 백로그를 사용하여 작업 대기열의 우선 순위를 지정하고 관리합니다.

작업 또는 문제는 의 어디에서든 팀에 할당(및 팀 백로그에 추가)될 수 있습니다. [!DNL Adobe Workfront]. 예를 들어 단일 팀에 여러 프로젝트의 작업 할당이 할당될 수 있습니다.

>[!NOTE]
>
>백로그 항목에 여러 팀을 추가하면 작업 또는 문제가 기본 팀의 백로그에만 표시됩니다. 기본 팀이 먼저 할당된 팀입니다.

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스</strong></td> 
   <td> <p>새로운 기능: [!UICONTROL Standard]</p><p>또는</p><p>현재: [!UICONTROL Work] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>새로운 기능: [!UICONTROL Standard]</p><p>또는</p><p>현재: [!UICONTROL Worker] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>스토리가 있는 프로젝트에 대한 [!UICONTROL 관리] 액세스 권한</p>  </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 백로그에 스토리 만들기 및 관리

* [스토리 순서 바꾸기](#reorder-stories)
* [[!UICONTROL 분류] 스토리](#break-down-stories)
* [스토리 편집](#edit-stories)

### 스토리 순서 바꾸기 {#reorder-stories}

드래그 앤 드롭 방법을 사용하여 백로그 목록에서 스토리를 재정렬할 수 있습니다.

1. 스토리를 재정렬하려는 애자일 백로그로 이동합니다.
1. 다음에서 **[!UICONTROL 보기]** 드롭다운 메뉴에서 **[!UICONTROL 백로그]** 보기 또는 를 포함하는 사용자 지정 보기 **[!UICONTROL 주문]** 열.

   >[!NOTE]
   >
   >작업 또는 문제에 애자일 팀이 할당되어 있고 프로젝트가 현재 상태와 동등한 상태가 아닌 경우 백로그에 표시되지 않습니다. 하지만 주문 열의 백로그 카운트에는 여전히 영향을 줍니다.

1. 스토리를 하나 이상 선택한 다음 스토리를 백로그에 표시할 순서로 드래그합니다.\
   ![백로그 항목 드래그 앤 드롭](assets/agile-backlog-drag-and-drop.png)

### 스토리 분류 {#break-down-stories}

백로그에 있는 스토리의 크기가 다르기 때문에 사용자는 해당 스토리를 반복을 위해 작업 가능한 크기로 분류할 수 있습니다. 스토리를 분류하면 스토리가 나타내는 작업에 하위 작업이 만들어지고 백로그에 있는 원래 작업을 대체합니다. 상위 작업 또는 하위 작업을 애자일 팀에 할당할 수 있지만 두 작업을 동시에 팀에 할당할 수는 없습니다.

>[!NOTE]
>
>스토리를 분류할 때는 다음 제한 사항을 고려하십시오.
>
>* 작업을 나타내는 이야기만 분류할 수 있습니다. 문제를 나타내는 스토리는 분류할 수 없습니다.
>* 스토리는 프로젝트와 관련된 경우에만 분류할 수 있습니다.


스토리를 분류하려면:

1. 분류할 스토리가 포함된 백로그로 이동합니다.
1. 분류할 스토리를 선택한 다음 를 클릭합니다. **[!UICONTROL 분류 스토리]**.\
   다음 [!UICONTROL 분류 스토리] 대화 상자가 표시됩니다.\
   ![분류 스토리 대화 상자](assets/backlog-breakdown-dialog.png)

1. 스토리의 이름과 예상 값을 지정하고 스토리가 준비되었는지 여부를 선택합니다.
1. 클릭 **[!UICONTROL 스토리 추가]** 원래 스토리에서 다른 스토리를 만들 수 있습니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

### 스토리 편집 {#edit-stories}

다음에서 바로 스토리를 편집할 수 있습니다. [!UICONTROL 스토리] 또는 [!UICONTROL 문제] 에 설명된 대로 프로젝트 내의 모든 작업 또는 문제를 일괄적으로 편집할 수 있는 백로그 탭 [일괄 작업 편집](../../manage-work/tasks/manage-tasks/edit-tasks.md#edit-tasks-in-bulk) 위치: [작업 편집](../../manage-work/tasks/manage-tasks/edit-tasks.md), 및 [문제 편집](../../manage-work/issues/manage-issues/edit-issues.md).

## 백로그에 새 스토리 만들기 {#create-new-stories-on-the-backlog}

백로그에서 직접 스토리를 만들거나 기존 작업 또는 문제를 애자일 팀에 할당하여 백로그에 새 스토리를 만들 수 있습니다.

* [백로그에서 스토리 만들기](#create-a-story-from-the-backlog)
* [애자일 팀에 작업 또는 문제 할당](#assign-a-task-or-issue-to-an-agile-team)

### 백로그에서 스토리 만들기 {#create-a-story-from-the-backlog}

백로그에서 스토리를 만들면 스토리가 프로젝트 내의 작업 또는 문제로 생성됩니다. 백로그에서 스토리를 문제로 만들 수 없습니다.

백로그에서 스토리를 만들려면:

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리에서 을(를) 클릭하고 **[!UICONTROL 팀]**.

1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)그런 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 막대에서 팀을 검색하고 표시될 때 선택합니다.

1. 선택 **[!UICONTROL 백로그]** 왼쪽 패널에서 가져옵니다.
1. 작업 또는 문제 생성 여부에 따라 다음 중 하나를 수행합니다.

   * **작업을 생성하려면 다음을 수행합니다.** 클릭 **[!UICONTROL 스토리]**.

   * **문제를 만들려면 다음 작업을 수행하십시오.** 클릭 **[!UICONTROL 문제]**.

1. 클릭 **[!UICONTROL 새 스토리]** 또는 **[!UICONTROL 새 문제]**.

1. 다음 정보를 지정합니다.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td> 스토리의 이름을 입력합니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 설명]</strong></td>
      <td>(선택 사항) 스토리에 대한 설명을 입력합니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 준비]</strong></td>
      <td> 스토리를 반복에 추가할 준비가 되었는지 여부를 선택합니다. 이 설정은 정보 제공용입니다. 이 설정의 상태에 관계없이 반복에 스토리를 추가할 수 있습니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate]</strong></td>
      <td>스토리에 대한 포인트 또는 시간별 추정치를 지정합니다. 예상 값은 번다운 차트에 영향을 줍니다. 반복에 대한 번다운 차트는 각 스토리에 정확한 추정치가 포함된 경우에만 정확합니다. (포인트 예상치를 제공하는 경우 팀 설정에서 각 포인트가 나타내는 시간을 이미 지정했어야 합니다.)</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 상위 프로젝트]</strong></td>
      <td>이 스토리가 생성될 프로젝트의 이름을 입력한 다음 드롭다운 목록에 표시될 때 이름을 클릭합니다.<br>프로젝트의 상태를 [!UICONTROL Current]로 설정해야 합니다. 프로젝트의 상태가 [!UICONTROL Current]가 아니면 드롭다운 메뉴에 표시되지 않습니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 상위 작업]</strong></td>
      <td>(선택 사항) 이 스토리가 종속된 상위 작업의 이름을 입력한 다음 드롭다운 목록에 나타나면 해당 이름을 클릭합니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 사용자 지정 Forms]</strong></td>
      <td> (선택 사항) 이 스토리에 추가할 사용자 정의 양식을 선택합니다.</td>
     </tr>
    </tbody>
   </table>

1. 클릭 **[!UICONTROL 스토리 저장]**.

### 애자일 팀에 작업 또는 문제 할당 {#assign-a-task-or-issue-to-an-agile-team}

애자일 팀에 작업 또는 문제를 할당할 수 있습니다. 작업 또는 문제가 할당되면 팀 백로그에 새 스토리로 표시됩니다.

애자일 팀에 작업 또는 문제를 할당하려면 다음을 수행합니다.

1. 할당할 작업이 포함된 프로젝트로 이동합니다.
1. 목록에서 작업 또는 문제를 선택합니다.
1. 클릭 **[!UICONTROL 편집]**.
1. 클릭 **[!UICONTROL 할당]**.
1. (선택 사항) 기존 피할당자를 삭제합니다.
1. 클릭 **[!UICONTROL 피할당자 추가]**.
1. 작업 또는 문제에 할당할 애자일 팀의 이름을 입력한 다음 드롭다운 목록에 나타나면 팀 이름을 클릭합니다.
1. **[!UICONTROL 변경 내용 저장]**&#x200B;을 클릭합니다.\
   이제 작업 또는 문제를 팀 백로그에서 사용할 수 있습니다.

## 백로그 내부 또는 외부로 스토리 이동

{#move-stories-from-the-backlog-to-an-iteration-or-kanban-board}

* [백로그에서 반복 또는 + 보드로 스토리 이동](#move-stories-from-the-backlog-to-an-iteration-or--board)
* [기존 스토리를 백로그로 이동](#move-existing-stories-to-the-backlog)
* [백로그에서 스토리 내보내기](#export-stories-from-the-backlog)

### 백로그에서 반복 또는 + 보드로 스토리 이동

1. 애자일 팀의 백로그로 이동합니다.
1. 반복 또는 Kanban 보드로 이동할 스토리를 선택한 다음 을 클릭합니다. **[!UICONTROL 자세히]** > **[!UICONTROL 이동 위치:]**.\
   스토리를 로 이동하면 [!UICONTROL 칸반] 보드, [!UICONTROL 칸반으로 스토리 이동] 게시판이 표시됩니다.\
   스토리를 반복으로 이동하면 [!UICONTROL 스토리를 반복으로 이동] 대화 상자가 표시됩니다.\
   ![스토리 이동 대화 상자](assets/agile-backlog-addtoiteration.png)

1. 다음 중 하나를 수행합니다.

   * **스크럼 팀의 경우:** 다음에서 **[!UICONTROL 반복 선택]** 필드에서 스토리를 이동할 반복을 선택합니다.

   * **칸반 팀의 경우:** 다음에서 **[!UICONTROL 칸반 보드 선택]** 필드, 팀 선택 [!UICONTROL 칸반] 게시판. (Kanban 팀에는 하나만 있을 수 있음 [!UICONTROL 칸반] board.)

1. 클릭 **[!UICONTROL 스토리 이동]**.

### 기존 스토리를 백로그로 이동 {#move-existing-stories-to-the-backlog}

팀에서 아직 스토리를 작업할 준비가 되지 않은 경우 스토리를 백로그로 이동할 수 있습니다.

자세한 내용은 [애자일 스토리 이동](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### 백로그에서 스토리 내보내기 {#export-stories-from-the-backlog}

백로그에서 직접 하나 이상의 스토리(작업 및 문제 포함)를 내보낼 수 있습니다.

다른 데이터를에서 내보내는 것과 동일한 방식으로 백로그에서 스토리를 내보냅니다 [!DNL Workfront]에 설명된 대로 [데이터 내보내기](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).
