---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 보드에서 구성원 추가 또는 제거
description: 보드를 보고 카드에 할당하려면 먼저 사람을 구성원으로 보드에 추가해야 합니다.
author: Lisa
feature: Agile
exl-id: 8a46846c-f9b8-45cb-9923-e7596854557b
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# 보드에서 구성원 추가 또는 제거

사용자와 팀이 보드를 보려면 먼저 보드에 구성원으로 추가되어야 합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td> 
   <p>새로운 기능: [!UICONTROL Contributor] 이상</p> 
   <p>또는</p>
   <p>현재: [!UICONTROL Request] 이상</p>
   </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 보드에 구성원 추가

{{step1-to-boards}}

1. 새 게시판을 만들거나 기존 게시판을 편집합니다. 자세한 내용은 [게시판 만들기 또는 편집](../../agile/get-started-with-boards/create-edit-board.md)을 참조하세요.
1. **[!UICONTROL 구성원 추가]** 아이콘 ![구성원 추가](assets/boards-addmember-spectrum-25x25.png)를 클릭합니다.
1. **[!UICONTROL 구성원 추가]** 상자에서 이름을 입력한 다음 목록에 표시될 때 선택합니다.

   개별 구성원 또는 팀을 선택할 수 있습니다. 팀을 선택하면 팀 자체가 보드에 추가됩니다.

   >[!NOTE]
   >
   >개별 사용자는 팀의 액세스 수준에 **[!UICONTROL 보기]** 또는 **[!UICONTROL 편집]** 옵션이 설정되어 있어야 합니다. 그렇지 않으면 보드를 볼 수 없습니다.


   ![보드에 구성원 추가](assets/boards-add-members.png)

## 보드에서 구성원 제거

{{step1-to-boards}}

1. 새 게시판을 만들거나 기존 게시판을 편집합니다. 자세한 내용은 [게시판 만들기 또는 편집](../../agile/get-started-with-boards/create-edit-board.md)을 참조하세요.
1. **[!UICONTROL 구성원 추가]** 아이콘 ![구성원 추가](assets/boards-addmember-spectrum-25x25.png)를 클릭합니다.
1. **[!UICONTROL 구성원 추가]** 상자에서 개인 또는 팀 이름 옆에 있는 X를 클릭하여 보드에서 제거합니다.

   ![보드에서 구성원 제거](assets/boards-remove-member-from-board-350x367.png)

   보드에서 멤버를 제거하면 할당된 카드에서 해당 멤버가 제거되지 않습니다. 연결된 카드의 경우 [!DNL Workfront] 작업 또는 문제에 대해서도 할당이 업데이트됩니다.

   구성원은 이 게시판에서만 제거됩니다. 해당 세그먼트는 속한 다른 보드에서 제거되지 않습니다.

   >[!NOTE]
   >
   >게시판 소유자를 제거할 수 없습니다.
