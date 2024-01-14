---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 보드 대시보드 사용
description: 다음 [!UICONTROL 게시판] 대시보드에는 사용자가 만든 보드와 추가한 보드를 포함하여 사용자가 액세스할 수 있는 보드 목록이 표시됩니다.
author: Lisa
feature: Agile
exl-id: bb275f4f-efaf-4dcc-b184-40e015f089b6
source-git-commit: 9c4aa8d1f812299ba6cdcb664b990c1119e3cb31
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# 보드 대시보드 사용

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>작업 스트림은 특정 고객 그룹만 사용할 수 있습니다.

보드 대시보드에는 사용자가 생성한 보드와 사용자가 추가한 보드를 포함하여 사용자가 액세스할 수 있는 보드 및 작업 스트림 목록이 표시됩니다. 워크스트림의 일부가 아닌 액세스 권한이 있는 개별 보드가 먼저 표시됩니다.

대시보드에서 보드 및 워크스트림에 대해 다음을 수행할 수 있습니다.

* 보드 또는 워크스트림 보관
* 보드 및 작업 스트림 필터링
* 게시판 이름 또는 수정한 날짜별로 게시판 목록 정렬
* 보드 또는 작업 스트림 검색
* 보드 또는 작업 스트림 삭제

새 보드를 만들거나 기존 보드를 편집하는 방법에 대한 자세한 내용은 [보드 만들기 또는 편집](../../agile/get-started-with-boards/create-edit-board.md). 새 작업 스트림 만들기에 대한 내용은 [작업 스트림 관리](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜*</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> 
   <p>새로운 기능: [!UICONTROL Contributor] 이상</p> 
   <p>또는</p>
   <p>현재: [!UICONTROL Request] 이상</p>
   </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## 보드 및 작업 스트림 필터링 {#filter-boards}

보드 대시보드를 필터링하여 활성, 보관된 보드 또는 모든 보드 또는 워크스트림을 표시할 수 있습니다.

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리에서 을(를) 클릭하고 **[!UICONTROL 게시판]**.
1. 클릭 [!UICONTROL **필터**] 보드(Boards) 영역 또는 작업 스트림(Workstreams) 영역에서 을 선택합니다. **[!UICONTROL 모두]**, **[!UICONTROL 활성]**, 또는 **[!UICONTROL 보관됨]**.

   대시보드에 기본값 이외의 필터가 적용되면 필터 아이콘에 표시기가 표시됩니다 ![대시보드에 적용된 필터](assets/boards-filterapplied-30x30.png).

## 보드 정렬

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리에서 을(를) 클릭하고 **[!UICONTROL 게시판]**.
1. 보드 목록을 정렬하려면 [!UICONTROL **정렬**]. 페이지의 기본 정렬 옵션은 기준입니다. **[!UICONTROL 수정한 날짜]**. 게시판별로 페이지를 정렬할 수도 있습니다 **[!UICONTROL 이름]**.

   선택 **[!UICONTROL 순서 바꾸기]** 보드를 수정한 날짜 또는 이름의 역순으로 정렬합니다. 정렬 아이콘의 화살표가 위를 가리키면 역순서가 적용됩니다. 화살표가 아래를 가리키면 표준 순서가 적용됩니다.

   기본 이외의 정렬을 대시보드에 적용하면 정렬 아이콘에 표시기가 표시됩니다 ![정렬 적용됨](assets/sort-applied-boards.png).

## 보드 또는 작업 스트림 검색

보드 영역에서 특정 보드를 검색하거나 작업 스트림 영역에서 특정 작업 스트림을 검색할 수 있습니다.

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리에서 을(를) 클릭하고 **[!UICONTROL 게시판]**.
1. 클릭 [!UICONTROL **검색**] 검색어를 입력합니다. 그런 다음 Enter 키를 누릅니다.

   제목에 검색어가 포함된 모든 보드 또는 작업 스트림이 표시됩니다.

   X를 클릭하여 검색을 지웁니다.

   ![대시보드에서 보드 검색](assets/boards-searchbox.png)

## 보드 또는 작업 스트림 보관

보드 또는 워크스트림을 보관하면 아카이브로 전송되고 나중에 복원할 수 있습니다.

>[!NOTE]
>
>보드를 보관하면 모든 보드 멤버에 대해 보관됩니다.
>
>워크스트림을 보관할 때 해당 워크스트림의 모든 보드가 보관됩니다.

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리에서 을(를) 클릭하고 **[!UICONTROL 게시판]**.
1. 다음을 클릭합니다. **[!UICONTROL 자세히]** 메뉴 ![기타 메뉴](assets/more-icon-spectrum.png) 게시판 또는 워크스트림에서 **[!UICONTROL 보관]**.

   작업 스트림에서 메뉴는 오른쪽, 다음 옆에 있습니다. [!UICONTROL **작업 스트림 보기**] 단추를 클릭합니다.

   An [!UICONTROL 보관] 아이콘 ![보관](assets/archive-icon-spectrum-25x20.png) 는 보드 또는 워크스트림에 나타납니다. 보관된 보드 또는 워크스트림을 편집할 수 없습니다.

   보관된 항목은 필터를 적용하여 표시하지 않는 한 보드 대시보드에서 숨겨집니다. 자세한 내용은 [[!UICONTROL 보드 필터링]](#filter-boards) 이 문서의 섹션.

1. 보관된 보드 또는 워크스트림을 복원하려면 **[!UICONTROL 자세히]** 메뉴 ![기타 메뉴 아이콘](assets/more-icon-spectrum.png) 게시판 또는 워크스트림에서 **[!UICONTROL 복원]**.

## 보드 또는 작업 스트림 삭제

보드를 삭제하면 보드에서 영구적으로 제거됩니다 [!DNL Workfront] 및 을(를) 복원할 수 없습니다. 보드에 있는 모든 카드도 보드와 함께 삭제됩니다.

작업 스트림을 삭제하면 작업 스트림의 모든 보드도 삭제됩니다.

>[!NOTE]
>
>추가한 보드와 작업 스트림은 삭제되지 않고 생성한 보드와 작업 스트림만 삭제할 수 있습니다.

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리에서 을(를) 클릭하고 **[!UICONTROL 게시판]**.
1. 다음을 클릭합니다. **[!UICONTROL 자세히]** 메뉴 ![[!UICONTROL 기타 메뉴]](assets/more-icon-spectrum.png) 게시판 또는 워크스트림에서 **[!UICONTROL 삭제]**.

   작업 스트림에서 메뉴는 오른쪽, 다음 옆에 있습니다. [!UICONTROL **작업 스트림 보기**] 단추를 클릭합니다.

1. 클릭 **[!UICONTROL 보드 삭제]** 또는 [!UICONTROL **작업 스트림 삭제**] 확인 메시지 표시.

<!-- ## Move a board to a workstream

You can move a standalone board into a workstream, or move a board from one workstream to another workstream.

>[!NOTE]
>
>You can only move boards that you created, not boards that you were added to.

1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of [!DNL Adobe Workfront], then click **[!UICONTROL Boards]**.
1. Click the **[!UICONTROL More]** menu ![[!UICONTROL More menu]](assets/more-icon-spectrum.png) on the board, and select [!UICONTROL **Move to workstream**].
1. Select which workstream to add the board to, and click [!UICONTROL **Move**].

   The board is moved into the workstream and no longer appears in the [!UICONTROL Boards] area.
   If you have not created a workstream yet, you are prompted to create one to move the board into.
-->
