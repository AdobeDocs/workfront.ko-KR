---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 보드 만들기 또는 편집
description: 에서 [!UICONTROL 보드] 대시보드에서 새 보드를 만들거나 기존 보드를 편집할 수 있습니다.
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: 966a88b8c7761b257a1ad0b2fdb3400f78c5d4f7
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 보드 만들기 또는 편집

{{highlighted-preview}}

에서 [!UICONTROL 보드] 대시보드에서 새 보드를 만들거나 기존 보드를 편집할 수 있습니다.

작업 스트림에 보드를 추가하려면 다음을 참조하십시오 [워크플로우 관리](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
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

## 새 보드 만들기

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 보드]**.
1. 독립형 보드를 만들려면 **[!UICONTROL 보드 추가]** 에서 [!UICONTROL 보드] 영역. 작업 스트림에 보드를 추가하려면 다음을 참조하십시오 [워크플로우 관리](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

1. 보드의 템플릿을 선택합니다.

   | 템플릿 | 설명 |
   |---------|----------|
   | 기본 보드 | 보드에 기본 열 3개가 제공됩니다. 새 열을 추가하고 기본 열의 이름을 바꾸거나 삭제할 수 있습니다. <p>보드에 기본 열 3개가 제공됩니다. 새 열을 추가하고 기본 열의 이름을 바꾸거나 삭제할 수 있습니다. |
   | 칸반 보드 | 보드에 다음 열이 제공됩니다. 백로그, 신규, 진행 중, 완료 및 보류 중 새 열을 추가하고 기본 열의 이름을 바꾸거나 삭제할 수 있습니다.<p>백로그를 사용하려면 취입 열에 대한 필터를 설정해야 합니다. 자세한 내용은 [보드에 흡기 열 추가](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>각 열에 대한 기본 정책을 검토하려면 [!UICONTROL **자세히** 메뉴] 열에서 [!UICONTROL **편집**]. 이러한 사전 설정된 정책을 변경할 수 있습니다. 자세한 내용은 [보드 열 관리](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | Retrospective 보드 | 보드에 다음 열이 제공됩니다. 뭐가 잘 됐어? 개선 가능한 사항? 축하해야 할 사람? 보다 빠른 진행을 위해 할 수 있는 일? 새 열을 추가하고 기본 열의 이름을 바꾸거나 삭제할 수 있습니다. <p>적용된 열 정책이 없습니다. |
   | <span class="preview">동적 보드</span> | <span class="preview">보드에 다음 열이 제공됩니다. 선택되지 않음, 신규, 진행 중, 보류 중 및 완료 새 열을 추가하고 기본 열의 이름을 바꾸거나 삭제할 수 있습니다. (선택하지 않은 열의 이름은 변경할 수 있지만 삭제할 수는 없습니다. 이 열에는 다른 열 상태와 일치하지 않는 상태가 있는 모든 카드가 포함됩니다. <p>기본 열 정책은 상태를 기준으로 열에 카드를 할당합니다. 자세한 내용은 [보드 열 관리](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).</span> |

1. <span class="preview">동적 보드의 경우에만 설정 마법사 단계를 수행합니다.</span>

   <div class="preview">

   1. 보드 이름을 입력하고 를 클릭합니다 [!UICONTROL **다음**].
   1. 클릭 [!UICONTROL **소스 추가**].
   1. 클릭 [!UICONTROL **필터 소스**] 을(를) 선택합니다. [!UICONTROL **작업**] 또는 [!UICONTROL **문제**].

      >[!NOTE]
      >
      >작업 및 문제를 모두 포함하도록 보드를 필터링할 수 있지만 각 개체 유형에 대해 필터를 별도로 설정해야 합니다.
      >
      >또한 저장된 필터 및 시스템 기본 필터를 선택할 수 있습니다.

   1. 보드를 연결된 카드로 가져올 개체를 정의하는 필터를 만듭니다.

      이것은 흡입 열에 필터를 만드는 것과 동일한 프로세스입니다. 자세한 내용은 [보드에 흡기 열 추가](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

   1. 필터를 추가한 후 [!UICONTROL **보드 만들기**].

   </div>

1. 에 보드의 이름을 입력합니다 **[!UICONTROL 보드]** 필드를 입력하고 Enter 키를 누릅니다.
1. 필요에 따라 보드를 구성합니다.

   자세한 내용은 [보드에서 구성원 추가 또는 제거](../../agile/get-started-with-boards/add-members-to-board.md), [보드 열 관리](../../agile/get-started-with-boards/manage-board-columns.md), [보드에 임시 카드 추가](../../agile/get-started-with-boards/add-card-to-board.md), 및 [보드에서 연결된 카드 사용](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. 클릭 **[!UICONTROL 모든 보드]** 보드 대시보드로 돌아갑니다.

   현재 보드의 이름으로 표시된 드롭다운 메뉴를 찾아 클릭하여 다른 보드로 전환할 수도 있습니다.

   ![보드 목록](assets/boards-button-list-of-boards-350x188.png)

## 기존 보드 편집

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 보드]**.
1. 대시보드에서 열 보드를 선택합니다.
1. 필요에 따라 보드를 편집합니다. 보드 이름을 클릭하여 이름을 바꿀 수 있습니다.

   자세한 내용은 [보드에서 구성원 추가 또는 제거](../../agile/get-started-with-boards/add-members-to-board.md), [보드 열 관리](../../agile/get-started-with-boards/manage-board-columns.md), 및 [보드에 카드 추가](../../agile/get-started-with-boards/add-card-to-board.md).

1. 클릭 **[!UICONTROL 모든 보드]** 보드 대시보드로 돌아갑니다.

   현재 보드의 이름으로 표시된 드롭다운 메뉴를 찾아 클릭하여 다른 보드로 전환할 수도 있습니다.
