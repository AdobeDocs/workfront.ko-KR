---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 보드에서 카드 삭제 또는 보관
description: 보드에서 카드를 삭제하면 영구적으로 삭제되며 복원할 수 없습니다. 카드를 보관하면 아카이브로 전송되고 나중에 보드에 복원할 수 있습니다.
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: 46099e6ceba4310453743c023823e8952f5ce553
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---

# 보드에서 카드 삭제 또는 보관

보드에서 임시 카드를 삭제하면 영구적으로 삭제되며 복원할 수 없습니다. 연결된 카드는 삭제한 후 보드에 수동으로 다시 추가할 수 있습니다.

연결된 카드를 동적 보드에서 삭제하면 보드를 새로 고칠 때 이 보드 유형이 특정 프로젝트에서 모든 작업과 문제를 가져오기 때문에 다시 나타납니다. 카드를 삭제하려면 Workfront 프로젝트에서 연결된 작업 또는 문제를 삭제해야 합니다.

접수 열이 있는 다른 보드 유형에서 연결된 카드를 삭제하면 연결된 작업 또는 문제가 아직 완료로 표시되지 않은 경우 보드를 새로 고칠 때 카드가 접수 열에 다시 나타납니다. 접수 열에 대한 자세한 내용은 [보드에 접수 열 추가](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

카드를 보관하면 아카이브로 전송되고 나중에 보드에 복원할 수 있습니다.

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
   <td> <p>[!UICONTROL Request] 이상</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

## 보드에서 카드 삭제

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Adobe Workfront]을 클릭한 다음 을 클릭합니다 **[!UICONTROL 게시판]**.
1. 보드에 액세스합니다. 자세한 내용은 [보드 만들기 또는 편집](../../agile/get-started-with-boards/create-edit-board.md).
1. 다음을 클릭합니다. **[!UICONTROL 자세히]** 메뉴 ![기타 메뉴](assets/more-icon-spectrum.png) 카드에서 을(를) 선택하고 **[!UICONTROL 삭제]**.
1. 클릭 **[!UICONTROL 삭제]** 확인 메시지 표시.

## 보드에서 카드 보관

1. 보드에 액세스합니다.
1. 다음을 클릭합니다. **[!UICONTROL 자세히]** 메뉴 ![기타 메뉴](assets/more-icon-spectrum.png) 카드에서 을(를) 선택하고 **[!UICONTROL 보관]**.

   보관된 카드는 필터를 적용하여 표시하지 않는 한 보드에서 숨겨집니다. 자세한 내용은 [보드를 필터링하여 보관된 카드 표시](#filter-a-board-to-show-archived-cards) 이 문서에서.

   An [!UICONTROL 보관] 아이콘 ![보관](assets/archive-icon-spectrum-25x20.png) 은 보관된 카드에 나타납니다. 보관된 카드는 편집할 수 없지만 삭제하거나 다른 열로 이동할 수 있습니다.

1. 보관된 카드를 복원하려면 **[!UICONTROL 자세히]** 메뉴 ![기타 메뉴](assets/more-icon-spectrum.png) 카드에서 다음을 선택합니다. **[!UICONTROL 복원]**.

## 보드를 필터링하여 보관된 카드 표시 {#filter-a-board-to-show-archived-cards}

기본적으로 활성 카드만 보드에 표시됩니다. 보드를 필터링하여 보관된 카드도 표시할 수 있습니다.

1. 보드에 액세스합니다.
1. 클릭 [!UICONTROL **구성**] 보드 오른쪽에서 Configure 패널을 엽니다.
1. 확장 [!UICONTROL **카드**].
1. 켜기 [!UICONTROL **보드에 보관된 카드 표시**].
1. 클릭 [!UICONTROL **필터**]&#x200B;를 확장합니다. [!UICONTROL 보관된 카드] 섹션, 선택 **[!UICONTROL 보관된 카드]** 보관된 카드를 표시합니다.

   필터에는 보관된 카드 수가 표시됩니다.

   ![보관된 카드 필터링](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >다음 [!UICONTROL 보관된 카드] 보관된 카드를 표시하도록 구성 설정을 켜지 않은 경우 필터에서 섹션을 사용할 수 없습니다. 자세한 내용은 [카드에 표시할 필드 사용자 지정](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. 선택 **[!UICONTROL 보관된 카드]** 다시 클릭하여 옵션을 지우고 활성 카드만 표시합니다.
