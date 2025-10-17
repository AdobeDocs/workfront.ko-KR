---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: 카드에 표시되는 필드 사용자 지정
description: 전체 카드나 압축된 보기로 표시되지 않도록 필드를 비활성화하거나 압축된 카드 보기에서 필드를 숨겨서 카드에 표시되는 필드를 사용자 정의할 수 있습니다.
author: Jenny
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# 카드에 표시할 필드 사용자 지정

기본적으로 사용할 수 있는 모든 필드는 카드에 표시되며, 카드가 열릴 때 전체 보기와 보드의 압축된 카드 보기 모두에 표시됩니다. 표시되는 필드를 사용자 지정할 수 있습니다.

* 어느 보기에도 표시되지 않도록 필드 비활성화
* 압축된 카드 보기에서 필드 숨기기

필드에 값이 들어 있는 경우 필드를 비활성화하면 나중에 필드를 다시 활성화해도 값이 유지됩니다.

섹션(카드 세부 정보에서 왼쪽 탐색 옵션으로 표시됨)을 표시하거나 숨길 수도 있습니다.

이전에 만든 사용자 지정 필드를 표시할 수도 있습니다. 보드 내에서 새 사용자 정의 필드를 디자인하고 만들 수 없습니다.

>[!NOTE]
>
>필드 사용자 지정은 작업 중인 보드에만 적용됩니다.

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

## 카드 구성 {#configure-cards}

{{step1-to-boards}}

1. 보드에 액세스합니다. 자세한 내용은 [게시판 만들기 또는 편집](../../agile/get-started-with-boards/create-edit-board.md)을 참조하세요.
1. 보드 오른쪽의 [!UICONTROL **구성**]&#x200B;을 클릭하여 구성 패널을 엽니다.
1. [!UICONTROL **카드**]&#x200B;를 확장합니다.

   대부분의 필드와 섹션은 기본적으로 활성화되어 있습니다.

1. 필드 또는 섹션을 해제하여 두 카드 보기에서 모두 비활성화합니다.
1. 필드 또는 섹션 옆에 있는 숨기기 아이콘 ![숨기기 아이콘](assets/eye-hide-icon.png)을 클릭하여 압축된 보기에서 숨깁니다.
1. 두 보기의 모든 필드와 섹션을 표시하려면 [!UICONTROL **모든 필드를 기본값으로 복원**]&#x200B;을 클릭합니다.
1. 구성 패널을 닫으려면 [!UICONTROL **구성 숨기기**]&#x200B;를 클릭하십시오.

## 카드에 사용자 정의 필드 추가

사용자 정의 필드는 연결된 카드에서 사용할 수 있습니다. 보드에 있는 요약 보기가 아닌 전체 카드 보기에서만 볼 수 있습니다.

사용자 정의 필드의 데이터는 카드에서 편집할 수 있지만 특정 사용자 정의 요소는 카드가 아닌 원래 필드에서만 편집할 수 있습니다.

1. 보드에 액세스하고 [!UICONTROL **구성**]&#x200B;을 클릭하여 구성 패널을 엽니다.
1. [!UICONTROL **카드**]&#x200B;를 확장합니다.
1. [!UICONTROL 카드 필드]에서 [!UICONTROL **사용자 지정 필드 추가**]&#x200B;를 클릭합니다.
1. [!UICONTROL **작업**] 또는 [!UICONTROL **문제**]&#x200B;를 선택하십시오.

   작업 또는 문제에 사용 가능한 필드의 범주가 나타납니다. 카테고리를 확장하여 모든 필드를 표시합니다. 필드를 검색할 수도 있습니다.

   ![사용자 지정 필드 검색](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >Adobe XD, 이미지, PDF, 비디오 필드 유형을 카드에 추가할 수 없습니다.

1. 필드 이름을 선택합니다.
1. (선택 사항) **[!UICONTROL 필드 값]** 필드를 클릭하여 이 사용자 지정 필드를 다른 값으로 변경합니다.
1. (선택 사항) **[!UICONTROL 필드 레이블]**&#x200B;을 카드에 표시할 필드 이름으로 변경합니다.
1. 변경을 마치면 [!UICONTROL **필드 저장**]&#x200B;을 클릭합니다.

   ![사용자 지정 필드 값 및 레이블](assets/save-custom-field-value-label.png)

   사용자 지정 필드는 사용 가능한 필드 목록에 추가되며 기본적으로 활성화됩니다. 위의 [카드 구성](customize-fields-on-card.md#configure-cards) 섹션의 단계에 따라 사용자 지정 필드를 비활성화하거나 필드를 편집하거나 모든 카드에서 삭제할 수 있습니다.

>[!NOTE]
>
>나중에 Workfront에서 사용자 정의 필드의 이름을 바꾸는 경우 일치시키려면 구성 패널에서 필드 레이블을 편집해야 합니다. 그렇지 않으면 필드가 카드에 표시되지 않습니다.

## 보관된 카드 표시 또는 숨기기

보드에 보관된 카드를 표시하려면 구성 설정을 켜야 합니다.

1. 보드에 액세스하고 [!UICONTROL **구성**]&#x200B;을 클릭하여 구성 패널을 엽니다.
1. [!UICONTROL **카드**]&#x200B;를 확장합니다.
1. [!UICONTROL **보드에 보관된 카드 표시**]&#x200B;를 켭니다.

   이제 보드를 필터링하여 보관된 카드를 표시할 수 있습니다. 자세한 내용은 [게시판에서 필터링 및 검색](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md)을 참조하세요.

1. 구성 패널을 닫으려면 [!UICONTROL **구성 숨기기**]&#x200B;를 클릭하십시오.

## 카드 폴오프 구성

일정 시간이 지난 후 보드에서 카드를 자동으로 제거하려면 [카드 폴오프 구성](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md)을 참조하십시오.
