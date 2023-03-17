---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: 카드에 표시되는 필드를 사용자 정의합니다
description: 필드를 비활성화하여 전체 카드 또는 압축된 보기에 표시되지 않도록 하거나 압축된 카드 보기에서 필드를 숨기면 카드에 표시되는 필드를 사용자 지정할 수 있습니다.
author: Lisa
feature: Agile
source-git-commit: 88d0ce017401e7767ceeff9abc7a65986a07f0b9
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---


# 카드에 표시되는 필드를 사용자 정의합니다

{{highlighted-preview}}

>[!NOTE]
>
>이 기능은 의 초기 기능 옵트인을 통해서만 사용할 수 있습니다. [!DNL Workfront] [!UICONTROL 보드]. 자세한 내용은 [Adobe Workfront 보드에 대한 초기 기능 옵트인](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

기본적으로 사용 가능한 모든 필드는 카드가 열려 있을 때 전체 보기에서, 보드의 압축된 카드 보기에서 카드에 표시됩니다. 표시할 필드를 다음과 같이 사용자 지정할 수 있습니다.

* 두 보기에 표시되지 않도록 필드를 비활성화합니다
* 압축된 카드 보기에서 필드 숨기기

필드에 값이 들어 있고 필드를 비활성화하는 경우, 나중에 필드를 다시 활성화하면 값이 유지됩니다.

이전에 만든 사용자 지정 필드를 표시할 수도 있습니다. 보드 내에서 새 사용자 지정 필드를 디자인하고 만들 수 없습니다.

>[!NOTE]
>
>사용자가 수행하는 모든 필드 사용자 지정은 작업 중인 보드에만 적용됩니다.

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
   <td> <p>[!UICONTROL Request] 이상</p> </td> 
  </tr>
   </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 카드 구성 {#configure-cards}

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 보드]**.
1. 보드 액세스. 자세한 내용은 [보드 만들기 또는 편집](../../agile/get-started-with-boards/create-edit-board.md).
1. 클릭 [!UICONTROL **구성**] 보드 오른쪽의 구성 패널을 엽니다.
1. 확장 [!UICONTROL **카드**].

   대부분의 필드는 기본적으로 활성화되어 있습니다.

1. 두 카드 보기에서 필드를 비활성화하려면 필드를 끄십시오.
1. 숨기기 아이콘을 클릭합니다 ![아이콘 숨기기](assets/eye-hide-icon.png) 축소 보기에서 숨길 필드 옆에 있습니다.
1. 두 보기의 모든 필드를 표시하려면 [!UICONTROL **모든 필드를 기본값으로 복원**].
1. 클릭 [!UICONTROL **구성 숨기기**] 를 클릭하여 구성 패널을 닫습니다.

<div class="preview">

## 카드에 사용자 지정 필드 추가

>[!NOTE]
>
>사용자 지정 필드를 카드에 추가하면 카드의 데이터는 읽기 전용입니다. 또한 사용자 정의 필드는 연결된 카드에서만 사용할 수 있습니다.

1. 보드 액세스 및 클릭 [!UICONTROL **구성**] 구성 패널을 열려면 다음을 수행하십시오.
1. 확장 [!UICONTROL **카드**].
1. 아래 [!UICONTROL 카드 필드]를 클릭합니다. [!UICONTROL **사용자 지정 필드 추가**].
1. 선택 [!UICONTROL **작업**] 또는 [!UICONTROL **문제**].

   작업 또는 문제에 사용할 수 있는 필드 범주가 표시됩니다. 카테고리를 확장하여 모든 필드를 봅니다. 필드를 검색할 수도 있습니다.

   ![사용자 지정 필드 검색](assets/boards-search-for-custom-field.png)

1. 필드 이름을 선택합니다.

   사용자 지정 필드가 사용 가능한 필드 목록에 추가되며 기본적으로 활성화되어 있습니다. 의 단계에 따라 사용자 지정 필드를 비활성화하거나 숨길 수 있습니다 [카드 구성](customize-fields-on-card.md#configure-cards) 위의 섹션을 삭제하거나 보드에서 삭제합니다.

</div>
