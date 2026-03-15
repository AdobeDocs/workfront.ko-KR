---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 보드 관리 보기 관리
description: 보드 관리 보기에는 시스템 관리자가 전체 보드 세부 사항에 대한 빠른 스냅샷을 얻는 데 사용할 수 있는 계정의 모든 보드 목록이 포함되어 있습니다.
author: Courtney
feature: Agile
exl-id: 4a7f2f68-14d2-4532-8c76-2ba78b45deac
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 2%

---

# 보드 관리 보기 관리

The Boards Admin View contains a list of every Board in your account that System Administrators can use to get a quick snapshot of the overall Boards details, including when they were last updated, how many cards each one has, and more.

From this area, you can perform the following actions:

* 보드 목록 필터링
* 보드 목록 열 구성
* 보드 목록 그룹화

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

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
   <td> <p>표준</p>
        <p> 플랜 </p></td> 
  </tr> 
    <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 관리자 </p>
        </td> 
  </tr> 
 </tbody> 
</table>

이 표에 있는 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

You must create a Board before you can view it from the Admin View.

For more information, see [Create or edit a board](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## 보드 목록 필터링

{{step1-to-boards}}

1. **게시판** 페이지에서 **관리자 보기** 탭을 선택합니다.

1. **필터**&#x200B;를 선택하십시오. **필터** 패널이 열립니다.

1. Follow the steps below to configure the filter:

   1. (Optional) Click the **Calendar** icon ![Calendar icon](assets/calendar-icon.png) and then select a date range to filter by Boards that were last modified within that timeframe.

   1. (선택 사항) **템플릿** 섹션에서 목록에서 필터링할 보드 템플릿 유형을 선택합니다. 템플릿 유형을 두 개 이상 선택할 수 있습니다.
게시판 템플릿 유형에 대한 자세한 내용은 [게시판 만들기 또는 편집](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md)을 참조하십시오.

   1. (선택 사항) **보관됨** 섹션에서 보관되거나 보관되지 않은 게시판이 표시되는지 여부를 선택합니다. 두 개 이상의 옵션을 선택할 수 있습니다.

      ![보관된 섹션임](assets/is-archived-section.png)

1. 닫으려면 **필터** 패널 바깥쪽을 클릭하십시오. 필터 선택은 기본 보기로 다시 변경될 때까지 보드 목록에 적용된 상태로 유지됩니다.

   >[!NOTE]
   >
   >To remove a filter, open the **Filters** panel and click **Back to default** in the upper-right corner.

## Configure the Boards list columns

{{step1-to-boards}}

1. **게시판** 페이지에서 **관리자 보기** 탭을 선택합니다.

1. **열**&#x200B;을(를) 선택하십시오. **필드 표시 및 순서** 패널이 열립니다.

1. 각 열과 함께 인라인으로 토글을 선택하거나 선택 취소하여 보드 목록에 표시할 열을 구성합니다.

   * **소유자**
   * **Last updated**
   * **Members**
   * **Archived**
   * **템플릿**
   * **카드 개수**

1. (Optional) To adjust the order the fields appear in, click and hold the **Drag** icon to the left of a field, then drag it to a new position.

   ![Click and drag](assets/click-and-drag.png)

1. Click outside the **Fields visibility and order** panel to close it. Your column configurations will remain applied to the Boards list until they&#39;re modified.

   >[!NOTE]
   >
   > When the Boards list columns display is modified, a blue dot appears above the **Columns** icon to indicate that the current view has been modified from the default.

## 특정 필드를 기준으로 게시판 목록 그룹화

{{step1-to-boards}}

1. On the **Boards** page, select the **Admin View** tab.

1. **그룹**&#x200B;을(를) 선택하십시오. The **Group by** panel opens.

1. 보드 목록을 그룹화할 필드를 선택합니다.

   * **보관됨**
   * **소유자**
   * **템플릿**

1. (Optional) To expand or collapse the grouping from the **Group by** panel, click **Collapse all** or **Expand all**.

   ![Collapse all](assets/collapse-all.png)

1. (Optional) To change the grouping&#39;s display order from A-Z to Z-A, select the field the list is currently grouped by, then select **Z-A** from the drop-down.

   ![Display by order](assets/display-by-order.png)

1. **그룹화 기준** 패널 바깥쪽을 클릭하여 닫습니다. 여기에서 그룹화 제목 옆에 있는 화살표를 선택하여 목록에서 적용된 그룹화를 축소하거나 확장할 수 있습니다.

   ![축소 또는 확장](assets/collapse-or-expand.png)

   >[!NOTE]
   >   
   >게시판 목록 그룹화 표시를 수정하면 **그룹** 아이콘 위에 파란색 점이 표시되어 현재 보기가 기본값과 다르다는 것을 나타냅니다. <br>
   >If you want to remove a grouping, open the **Group by** panel and select **Clear all** in the upper-right corner.
