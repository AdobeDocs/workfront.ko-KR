---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: 카드에 표시할 필드 사용자 정의
description: 전체 카드 또는 압축된 보기에 표시되지 않도록 필드를 비활성화하거나 압축된 카드 보기에서 필드를 숨겨 카드에 표시되는 필드를 사용자 정의할 수 있습니다.
author: Courtney
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 2%

---

# 카드에 표시할 필드 사용자 정의

기본적으로 사용 가능한 모든 필드는 카드가 열려 있을 때의 전체 보기와 보드의 압축된 카드 보기 모두에서 카드에 표시됩니다. 다음 방법으로 표시할 필드를 사용자 정의할 수 있습니다.

* 어느 쪽 보기에서도 표시되지 않도록 필드를 비활성화합니다.
* 압축된 카드 보기에서 필드 숨기기

필드에 값이 포함되어 있는 경우 필드를 비활성화하면 나중에 필드를 다시 활성화해도 값이 유지됩니다.

섹션(카드 세부 정보에서 왼쪽 탐색 옵션으로 표시됨)을 표시하거나 숨길 수도 있습니다.

이전에 만든 사용자 지정 필드를 표시할 수도 있습니다. 게시판 내에서 새 사용자 정의 필드를 디자인하고 만들 수 없습니다.

>[!NOTE]
>
>Any field customizations you make only apply to the board you are working in.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>Any</p> </td> 
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

## Configure cards {#configure-cards}

{{step1-to-boards}}

1. 보드에 액세스합니다. 자세한 내용은 [게시판 만들기 또는 편집](../../agile/get-started-with-boards/create-edit-board.md)을 참조하세요.
1. 보드 오른쪽의 [!UICONTROL **구성**]&#x200B;을 클릭하여 구성 패널을 엽니다.
1. [!UICONTROL **카드**]&#x200B;를 확장합니다.

   대부분의 필드와 섹션은 기본적으로 활성화되어 있습니다.

1. Turn off a field or section to disable it in both card views.
1. Click the Hide icon ![Hide icon](assets/eye-hide-icon.png) next to a field or section to hide it on the condensed view.
1. 두 보기 모두에서 모든 필드와 섹션을 표시하려면 [!UICONTROL **모든 필드를 기본값으로 복원**]&#x200B;을 클릭하십시오.
1. [!UICONTROL **구성 숨기기**]&#x200B;를 클릭하여 구성 패널을 닫습니다.

## 카드에 사용자 정의 필드 추가

사용자 정의 필드는 연결된 카드에서 사용할 수 있습니다. 이 옵션은 보드의 압축된 보기가 아닌 전체 카드 보기에서만 표시됩니다.

사용자 정의 필드의 데이터는 카드에서 편집할 수 있지만 특정 사용자 정의 요소는 카드가 아닌 원래 필드에서만 편집할 수 있습니다.

1. Access a board and click [!UICONTROL **Configure**] to open the Configure panel.
1. [!UICONTROL **카드**]&#x200B;를 확장합니다.
1. [!UICONTROL 카드 필드]에서 [!UICONTROL **사용자 지정 필드 추가**]&#x200B;를 클릭합니다.
1. [!UICONTROL **작업**] 또는 [!UICONTROL **문제**]&#x200B;를 선택하십시오.

   작업 또는 문제에 사용 가능한 필드의 범주가 나타납니다. 카테고리를 확장하여 모든 필드를 표시합니다. 필드를 검색할 수도 있습니다.

   ![Search for custom field](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >The following field types are not available to add to cards: Adobe XD, Image, PDF, Video.

1. Select the field name.
1. (Optional) Click in the **[!UICONTROL Field value]** field to change this custom field to a different one.
1. (Optional) Change the **[!UICONTROL Field label]** to the field name you want to appear on cards.
1. 변경을 마치면 [!UICONTROL **필드 저장**]&#x200B;을 클릭하세요.

   ![사용자 지정 필드 값 및 레이블](assets/save-custom-field-value-label.png)

   사용자 정의 필드는 사용 가능한 필드 목록에 추가되며 기본적으로 활성화됩니다. 위의 [카드 구성](customize-fields-on-card.md#configure-cards) 섹션에 있는 단계에 따라 사용자 지정 필드를 비활성화하거나, 필드를 편집하거나, 모든 카드에서 삭제할 수 있습니다.

>[!NOTE]
>
>If you later rename the custom field in Workfront, you must edit the field label on the Configure panel to match, or the field will not display on the cards.

## Display or hide archived cards

보드에 보관된 카드를 표시하려면 구성 설정을 켜야 합니다.

1. Access a board and click [!UICONTROL **Configure**] to open the Configure panel.
1. [!UICONTROL **카드**]&#x200B;를 확장합니다.
1. [!UICONTROL **보드에 보관된 카드 표시**]&#x200B;를 켭니다.

   이제 보드를 필터링하여 보관된 카드를 표시할 수 있습니다. For details, see [Filter and search in a board](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

1. Click [!UICONTROL **Hide configure**] to close the Configure panel.

## 카드 폴오프 구성

To automatically remove cards from the board after a period of time, see [Configure card falloff](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).
