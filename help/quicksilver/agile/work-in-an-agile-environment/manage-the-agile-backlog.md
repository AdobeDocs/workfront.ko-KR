---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: 애자일 백로그 관리
description: 작업 및 문제는 민첩한 팀에 할당하고 팀이 사용하는 민첩한 방법에 따라 해당 팀의 백로그에 스토리로서 추가할 수 있습니다.
author: Lisa
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: b855f032b24079ff27435fb833cd3ed8a382a77c
workflow-type: tm+mt
source-wordcount: '1376'
ht-degree: 0%

---

# 애자일 백로그 관리

다음 작업 항목은 애자일 팀에 할당하고 팀이 사용하는 애자일 방법에 따라 해당 팀의 백로그에 스토리로 추가할 수 있습니다.

* **[!UICONTROL 스크럼 애자일 팀]:** 작업 및 문제는 신속히 팀에 할당하고 백로그에 추가할 수 있습니다.
* **[!UICONTROL 간판 애자일 팀]:** 작업을 신속히 팀에 할당하고 백로그에 추가할 수 있습니다. 사용자는 의 설명에 따라 애자일 스토리 보드에서 직접 백로그를 볼 수 있습니다. [[!UICONTROL 백로그 추가] 간판 보드](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md). 팀은 이 백로그를 사용하여 작업 큐의 우선 순위를 지정하고 관리합니다.

작업 또는 문제는 의 모든 위치에서 팀에 지정(그런 다음 팀 백로그에 추가)할 수 있습니다 [!DNL Adobe Workfront]. 예를 들어, 단일 팀에 여러 프로젝트의 작업 할당이 할당될 수 있습니다.

>[!NOTE]
>
>백로그 항목에 여러 팀을 추가하는 경우 기본 팀의 백로그에 작업 또는 문제가 표시됩니다. 1차 팀은 첫 번째 팀입니다.

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
   <td> <p>[!UICONTROL Work] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>[!UICONTROL Worker] 이상</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>스토리가 있는 프로젝트에 대한 [!UICONTROL Manage] 액세스</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 백로그에 대한 스토리 생성 및 관리

* [스토리 순서 조정](#reorder-stories)
* [[!UICONTROL 브레이크] 다운 이야기](#break-down-stories)
* [스토리 편집](#edit-stories)
* [백로그에 새 스토리 만들기](#create-new-stories-on-the-backlog)
* [백로그에서 이터레이션 또는 간판 보드로 스토리 이동](#move-stories-from-the-backlog-to-an-iteration-or-kanban-board)

### 스토리 순서 조정 {#reorder-stories}

드래그 앤 드롭 방법을 사용하여 백로그 목록에서 스토리 순서를 변경할 수 있습니다.

1. 스토리를 다시 정렬하려는 민첩한 백로그로 이동합니다.
1. 에서 **[!UICONTROL 보기]** 드롭다운 메뉴에서 **[!UICONTROL 백로그]** 를 포함하는 사용자 지정 보기 또는 보기 **[!UICONTROL 주문]** 열.

   >[!NOTE]
   >
   >작업 또는 문제에 민첩한 팀이 할당되어 있고 프로젝트가 현재 팀과 같은 상태가 아닌 경우 백로그에 표시되지 않습니다. 하지만 주문 열의 백로그 수에는 여전히 영향을 줍니다.

1. 하나 이상의 스토리를 선택하고 스토리를 백로그에 표시할 순서로 드래그합니다.\
   ![백로그 항목을 드래그 앤 드롭](assets/agile-backlog-drag-and-drop.png)

### 스토리 분류 {#break-down-stories}

백로그의 스토리는 크기가 다르기 때문에 사용자가 반복을 위해 실행 가능한 크기로 분류할 수 있습니다. 스토리를 분류하면 스토리가 나타내는 작업에 하위 작업이 생성되고 백로그의 원래 작업을 대체합니다. 상위 작업 또는 하위 작업이 애자일 팀에 할당될 수 있지만 두 작업을 동시에 팀에 할당할 수는 없습니다.

>[!NOTE]
>
>스토리를 분류할 때 다음 제한 사항을 고려하십시오.
>
>* 작업을 나타내는 스토리만 분류할 수 있습니다. 문제를 나타내는 이야기는 분류할 수 없습니다.
>* 스토리는 프로젝트와 연결된 경우에만 분류할 수 있습니다.



스토리를 분류하려면:

1. 분류할 스토리가 포함된 백로그로 이동합니다.
1. 분류할 스토리를 선택한 다음 **[!UICONTROL 분류 스토리]**.\
   다음 [!UICONTROL 분류 스토리] 대화 상자가 표시됩니다.\
   ![분류 스토리 대화 상자](assets/backlog-breakdown-dialog.png)

1. 스토리의 이름과 예상치를 지정하고 스토리가 준비되었는지 여부를 선택합니다.
1. 클릭 **[!UICONTROL 스토리 추가]** 원작에서 다른 이야기를 만들어내기 위해서.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

### 스토리 편집 {#edit-stories}

에서 직접 스토리를 편집할 수 있습니다 [!UICONTROL 스토리] 또는 [!UICONTROL 문제] 다음에 설명된 대로 프로젝트 내의 모든 작업이나 문제를 일괄적으로 편집하는 것처럼 백로그의 탭을 확인합니다. [일괄 작업 편집](../../manage-work/tasks/manage-tasks/edit-tasks.md#editing-tasks-in-bulk) in [작업 편집](../../manage-work/tasks/manage-tasks/edit-tasks.md) 및 [문제 편집](../../manage-work/issues/manage-issues/edit-issues.md#bulk-editing-issues) in [문제 편집](../../manage-work/issues/manage-issues/edit-issues.md).

## 백로그에 새 스토리 만들기 {#create-new-stories-on-the-backlog}

백로그에서 직접 스토리를 만들거나 기존 작업이나 문제를 신속히 팀에 할당하여 백로그에 새 스토리를 만들 수 있습니다.

* [백로그에서 스토리 만들기](#create-a-story-from-the-backlog)
* [민첩한 팀에 작업 또는 문제 할당](#assign-a-task-or-issue-to-an-agile-team)

### 백로그에서 스토리 만들기 {#create-a-story-from-the-backlog}

백로그에서 스토리를 만들면 프로젝트 내에서 작업 또는 문제로 스토리가 만들어집니다. 백로그에서 문제로 스토리를 만들 수 없습니다.

백로그에서 스토리를 생성하려면

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

1. 선택 **[!UICONTROL 백로그]** 왼쪽 패널에서 생성합니다.
1. 작업을 작성할지 아니면 문제를 생성할지를 따라 다음 중 하나를 수행합니다.

   * **작업을 만들려면 다음을 수행하십시오.** 클릭 **[!UICONTROL 스토리]**.

   * **문제를 만들려면:** 클릭 **[!UICONTROL 문제]**.

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
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>(선택 사항) 스토리에 대한 설명을 입력합니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td> 반복에 스토리를 추가할 준비가 되었는지 여부를 선택합니다. 이 설정은 정보 제공용입니다. 이 설정의 상태에 관계없이 반복에 스토리를 추가할 수 있습니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate]</strong></td>
      <td>스토리의 포인트 또는 시간별 예상 값을 지정합니다. 추정은 번다운 차트에 영향을 줍니다. 각 스토리에 정확한 추적이 포함되어 있는 경우에만 반복에 대한 번다운 차트가 정확합니다. (포인트 추정을 제공하는 경우 각 점이 나타내는 시간을 팀 설정에 이미 지정했어야 합니다.)</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 상위 프로젝트]</strong></td>
      <td>이 스토리를 만들 프로젝트의 이름을 입력하고 드롭다운 목록에 표시될 이름을 클릭합니다.<br>프로젝트의 상태를 [!UICONTROL Current]로 설정해야 합니다. 프로젝트의 상태가 [!UICONTROL Current]를 제외한 경우에는 드롭다운 메뉴에 표시되지 않습니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 상위 작업]</strong></td>
      <td>(선택 사항) 이 스토리가 종속되는 상위 작업의 이름을 입력하고 드롭다운 목록에 나타나면 이름을 클릭합니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td> (선택 사항) 이 스토리에 추가할 사용자 지정 양식을 선택합니다.</td>
     </tr>
    </tbody>
   </table>

1. 클릭 **[!UICONTROL 스토리 저장]**.

### 민첩한 팀에 작업 또는 문제 할당 {#assign-a-task-or-issue-to-an-agile-team}

민첩한 팀에 작업이나 문제를 할당할 수 있습니다. 작업이 할당되면 작업이나 문제가 팀 백로그에 새 스토리로 나타납니다.

민첩한 팀에 작업 또는 문제를 할당하려면

1. 재할당할 작업이 포함된 프로젝트로 이동합니다.
1. 목록에서 작업이나 문제를 선택합니다.
1. 클릭 **[!UICONTROL 편집]**.
1. 클릭 **[!UICONTROL 지정]**.
1. (선택 사항) 기존 담당자를 삭제합니다.
1. 클릭 **[!UICONTROL 할당자 추가]**.
1. 작업이나 문제에 지정할 애자일 팀의 이름을 입력한 다음 드롭다운 목록에 나타나는 팀 이름을 클릭합니다.
1. 클릭 **[!UICONTROL 변경 내용 저장]**.\
   이제 팀 백로그에서 작업이나 문제를 사용할 수 있습니다.

## 백로그에서 반복 또는 + 보드로 스토리를 이동합니다. {#move-stories-from-the-backlog-to-an-iteration-or-kanban-board}

* [기존 스토리를 백로그로 이동](#move-existing-stories-to-the-backlog)
* [백로그에서 스토리 내보내기](#export-stories-from-the-backlog)

1. 애자일 팀의 백로그로 이동합니다.
1. 반복 또는 간판 보드로 이동하려는 스토리를 선택한 다음 **[!UICONTROL 자세히]** > **[!UICONTROL 이동 위치]**.\
   스토리를 [!UICONTROL 간판] 보드, [!UICONTROL 간판으로 스토리 이동] 보드가 표시됩니다.\
   스토리를 반복으로 이동하면 [!UICONTROL 반복으로 스토리 이동] 대화 상자가 표시됩니다.\
   ![스토리 이동 대화 상자](assets/agile-backlog-addtoiteration.png)

1. 다음 중 하나를 수행합니다.

   * **스크럼 팀의 경우:** 에서 **[!UICONTROL 반복 선택]** 필드에서 스토리를 이동할 이터레이션을 선택합니다.

   * **간판 팀의 경우:** 에서 **[!UICONTROL 간판 보드 선택]** 필드에서 팀을 선택합니다. [!UICONTROL 간판] 보드. (간판 팀은 하나만 가질 수 있음 [!UICONTROL 간판] 보드)

1. 클릭 **[!UICONTROL 스토리 이동]**.

### 기존 스토리를 백로그로 이동 {#move-existing-stories-to-the-backlog}

팀이 아직 이야기를 작업할 준비가 되지 않았다고 판단하면 스토리를 백로그로 옮길 수 있습니다.

자세한 내용은 [민첩한 스토리 이동](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### 백로그에서 스토리 내보내기 {#export-stories-from-the-backlog}

백로그에서 하나 이상의 스토리(작업 및 문제 포함)를 직접 내보낼 수 있습니다.

백로그에서 다른 데이터를 내보내는 것과 동일한 방식으로 스토리를 내보냅니다 [!DNL Workfront]에 설명된 대로 [데이터 내보내기](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).
