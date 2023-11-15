---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: 카드에 표시할 필드 사용자 지정
description: 전체 카드나 압축된 보기로 표시되지 않도록 필드를 비활성화하거나 압축된 카드 보기에서 필드를 숨겨서 카드에 표시되는 필드를 사용자 정의할 수 있습니다.
author: Lisa
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: 63d043a85c2e5300d8b5872b2ec7983de4ba1f50
workflow-type: tm+mt
source-wordcount: '572'
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

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

## 카드 구성 {#configure-cards}

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Adobe Workfront]을 클릭한 다음 을 클릭합니다 **[!UICONTROL 게시판]**.
1. 보드에 액세스합니다. 자세한 내용은 [보드 만들기 또는 편집](../../agile/get-started-with-boards/create-edit-board.md).
1. 클릭 [!UICONTROL **구성**] 보드 오른쪽에서 Configure 패널을 엽니다.
1. 확장 [!UICONTROL **카드**].

   대부분의 필드와 섹션은 기본적으로 활성화되어 있습니다.

1. 필드 또는 섹션을 해제하여 두 카드 보기에서 모두 비활성화합니다.
1. Hide 아이콘을 클릭합니다. ![아이콘 숨기기](assets/eye-hide-icon.png) 필드 또는 섹션 옆에 있는 경우 요약된 보기에서 숨길 수 있습니다.
1. 두 보기의 모든 필드와 섹션을 표시하려면 [!UICONTROL **모든 필드를 기본값으로 복원**].
1. 클릭 [!UICONTROL **구성 숨기기**] 을 클릭하여 구성 패널을 닫습니다.

## 카드에 사용자 정의 필드 추가

사용자 정의 필드는 연결된 카드에서 사용할 수 있습니다. 보드에 있는 요약 보기가 아닌 전체 카드 보기에서만 볼 수 있습니다.

사용자 정의 필드의 데이터는 카드에서 편집할 수 있지만 특정 사용자 정의 요소는 카드가 아닌 원래 필드에서만 편집할 수 있습니다.

1. 보드에 액세스하여 클릭 [!UICONTROL **구성**] 구성 패널을 엽니다.
1. 확장 [!UICONTROL **카드**].
1. 아래 [!UICONTROL 카드 필드], 클릭 [!UICONTROL **사용자 정의 필드 추가**].
1. 선택 [!UICONTROL **작업**] 또는 [!UICONTROL **문제**].

   작업 또는 문제에 사용 가능한 필드의 범주가 나타납니다. 카테고리를 확장하여 모든 필드를 표시합니다. 필드를 검색할 수도 있습니다.

   ![사용자 정의 필드 검색](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >Adobe XD, 이미지, PDF, 비디오 필드 유형을 카드에 추가할 수 없습니다.

1. 필드 이름을 선택합니다.
1. (선택 사항) **[!UICONTROL 필드 값]** 필드 : 이 사용자 정의 필드를 다른 사용자 정의 필드로 변경합니다.
1. (선택 사항) **[!UICONTROL 필드 레이블]** 카드에 표시할 필드 이름을 입력합니다.
1. 변경을 마쳤으면 [!UICONTROL **필드 저장**].

   ![사용자 정의 필드 값 및 레이블](assets/save-custom-field-value-label.png)

   사용자 지정 필드는 사용 가능한 필드 목록에 추가되며 기본적으로 활성화됩니다. 의 단계에 따라 사용자 정의 필드를 비활성화할 수 있습니다. [카드 구성](customize-fields-on-card.md#configure-cards) 위의 섹션에서 필드를 편집하거나 모든 카드에서 삭제하십시오.

>[!NOTE]
>
>나중에 Workfront에서 사용자 정의 필드의 이름을 바꾸는 경우 일치시키려면 구성 패널에서 필드 레이블을 편집해야 합니다. 그렇지 않으면 필드가 카드에 표시되지 않습니다.
