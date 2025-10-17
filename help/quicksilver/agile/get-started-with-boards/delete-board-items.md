---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 보드에서 카드 삭제 또는 보관
description: 보드에서 카드를 삭제하면 영구적으로 삭제되며 복원할 수 없습니다. 카드를 보관하면 아카이브로 전송되고 나중에 보드에 복원할 수 있습니다.
author: Jenny
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 1%

---

# 보드에서 카드 삭제 또는 보관

보드에서 임시 카드를 삭제하면 영구적으로 삭제되며 복원할 수 없습니다. 연결된 카드는 삭제한 후 보드에 수동으로 다시 추가할 수 있습니다.

연결된 카드를 동적 보드에서 삭제하면 보드를 새로 고칠 때 이 보드 유형이 특정 프로젝트에서 모든 작업과 문제를 가져오기 때문에 다시 나타납니다. 카드를 삭제하려면 Workfront 프로젝트에서 연결된 작업 또는 문제를 삭제해야 합니다.

접수 열이 있는 다른 보드 유형에서 연결된 카드를 삭제하면 연결된 작업 또는 문제가 아직 완료로 표시되지 않은 경우 보드를 새로 고칠 때 카드가 접수 열에 다시 나타납니다. 접수 열에 대한 자세한 내용은 [보드에 접수 열 추가](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)를 참조하십시오.

카드를 보관하면 아카이브로 전송되고 나중에 보드에 복원할 수 있습니다.

보관된 카드가 Workfront 작업 및 문제와 동기화되지 않습니다. 카드를 복원하면 다시 동기화됩니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>기여자 이상</p> 
   <p>요청 이상</p>
   </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 보드에서 카드 삭제

{{step1-to-boards}}

1. 보드에 액세스합니다. 자세한 내용은 [게시판 만들기 또는 편집](../../agile/get-started-with-boards/create-edit-board.md)을 참조하세요.
1. 카드에서 **[!UICONTROL 기타]** 메뉴 ![기타 메뉴](assets/more-icon-spectrum.png)를 클릭하고 **[!UICONTROL 삭제]**&#x200B;를 선택합니다.
1. 확인 메시지에서 **[!UICONTROL 삭제]**&#x200B;를 클릭합니다.

## 보드에서 카드 보관

1. 보드에 액세스합니다.
1. 카드에서 **[!UICONTROL 기타]** 메뉴 ![기타 메뉴](assets/more-icon-spectrum.png)를 클릭하고 **[!UICONTROL 보관]**&#x200B;을 선택합니다.

   보관된 카드는 필터를 적용하여 표시하지 않는 한 보드에서 숨겨집니다. 자세한 내용은 이 문서에서 [보드로 보관된 카드를 표시하도록 보드 필터링](#filter-a-board-to-show-archived-cards)을 참조하십시오.

   보관된 카드에 [!UICONTROL 보관] 아이콘 ![보관](assets/archive-icon-spectrum-25x20.png)이 표시됩니다. 보관된 카드는 편집할 수 없지만 삭제하거나 다른 열로 이동할 수 있습니다.

1. 보관된 카드를 복원하려면 카드에서 **[!UICONTROL 추가]** 메뉴 ![추가 메뉴](assets/more-icon-spectrum.png)를 클릭하고 **[!UICONTROL 복원]**&#x200B;을 선택하십시오.

## 보드를 필터링하여 보관된 카드 표시

기본적으로 활성 카드만 보드에 표시됩니다. 보드를 필터링하여 보관된 카드도 표시할 수 있습니다.

1. 보드에 액세스합니다.
1. 보드 오른쪽의 [!UICONTROL **구성**]&#x200B;을 클릭하여 구성 패널을 엽니다.
1. [!UICONTROL **카드**]&#x200B;를 확장합니다.
1. [!UICONTROL **보드에 보관된 카드 표시**]&#x200B;를 켭니다.
1. [!UICONTROL **필터**]&#x200B;를 클릭하고 [!UICONTROL 보관된 카드] 섹션을 확장한 다음 **[!UICONTROL 보관된 카드]**&#x200B;를 선택하여 보관된 카드를 표시합니다.

   필터에는 보관된 카드 수가 표시됩니다.

   ![보관된 카드 필터링](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >보관된 카드를 표시하도록 구성 설정을 켜지 않은 경우 [!UICONTROL 보관된 카드] 섹션을 필터에서 사용할 수 없습니다. 자세한 내용은 [카드에 표시할 필드 사용자 지정](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md)을 참조하십시오.

1. **[!UICONTROL 보관된 카드]**&#x200B;를 다시 선택하여 옵션을 지우고 활성 카드만 표시합니다.
