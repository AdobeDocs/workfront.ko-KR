---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 보드 만들기 또는 편집
description: 다음에서 [!UICONTROL 게시판] 대시보드에서 새 보드를 만들거나 기존 보드를 편집할 수 있습니다.
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: d593d288546abb4a674646519c6245563673b938
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 보드 만들기 또는 편집

<!-- Audited: 12/2023 -->

다음에서 [!UICONTROL 게시판] 대시보드에서 새 보드를 만들거나 기존 보드를 편집할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td> <p>새로운 기능: 기여자 이상 </p>
 <p>또는</p> 
<p>현재: [!UICONTROL Request] 이상 </p> 
</td> 
  </tr>
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 새 게시판 만들기

{{step1-to-boards}}

1. 클릭 **[!UICONTROL 보드 추가]**.

1. 보드에 사용할 템플릿을 선택합니다.

   | 템플릿 | 설명 |
   |---------|----------|
   | 기본 보드 | 보드에는 세 개의 기본 열이 제공됩니다. 새 열을 추가하고 기본 열의 이름을 바꾸거나 삭제할 수 있습니다. <p>보드에는 세 개의 기본 열이 제공됩니다. 새 열을 추가하고 기본 열의 이름을 바꾸거나 삭제할 수 있습니다. |
   | 칸반 보드 | 백로그, 신규, 진행 중, 완료 및 보류 중 열이 보드에 제공됩니다. 새 열을 추가하고 기본 열의 이름을 바꾸거나 삭제할 수 있습니다.<p>백로그를 사용하려면 접수 열에 대한 필터를 설정해야 합니다. 자세한 내용은 [보드에 접수 열 추가](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>각 열에 대한 기본 정책을 검토하려면 [!UICONTROL **자세히** 메뉴] 열에서 [!UICONTROL **편집**]. 이러한 사전 설정된 정책을 변경할 수 있습니다. 자세한 내용은 [보드 열 관리](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | Retrospective 보드 | 게시판에는 다음과 같은 열이 제공됩니다. 무엇이 잘 되었습니까? 무엇을 개선할 수 있을까요? 축하해야 할 사람이 누구죠? 더 빨리 움직이기 위해 우리가 할 수 있는 일은 무엇인가? 새 열을 추가하고 기본 열의 이름을 바꾸거나 삭제할 수 있습니다. <p>열 정책이 적용되지 않습니다. |
   | 동적 보드 | 보드에 선택되지 않음, 새로 만들기, 진행 중, 보류 및 완료 열이 제공됩니다. 새 열을 추가하고 기본 열의 이름을 바꾸거나 삭제할 수 있습니다. 선택 해제됨 열의 이름은 변경할 수 있지만 삭제할 수는 없습니다. 이 열에는 다른 열 상태와 일치하지 않는 상태의 모든 카드가 포함됩니다.) <p>기본 열 정책은 상태에 따라 열에 카드를 할당합니다. 자세한 내용은 [보드 열 관리](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

1. 동적 보드에 대해서만 설정 마법사 단계를 수행합니다.

   1. 보드 이름을 입력하고 [!UICONTROL **다음**].
   1. 검색 및 선택 [!DNL Workfront] [!UICONTROL **프로젝트**] 작업 및 문제를 게시판으로 가져오기
   1. 검색 및 선택 [!UICONTROL **할당**] 작업 및 문제를 게시판으로 가져오기

      모든 개체는 보드에 연결된 카드로 표시됩니다.

      다음 [!UICONTROL **카드 추가 중**] 카운터는 보드에 표시될 카드의 수를 보여줍니다. 예를 들어 작업 및 문제가 100개인 프로젝트를 선택하면 카운터에 100개가 표시됩니다. 사용자 할당을 추가하고 해당 사람이 프로젝트에서 5개의 작업에 할당되면 카운터에 5개가 표시됩니다.

      >[!NOTE]
      >
      >동적 보드에 대한 카드 제한은 총 1,400개의 카드에 대해 작업 700개, 문제 700개입니다. 보드에 있는 카드 수가 많으면 보드 성능에 영향을 줄 수 있습니다.

   1. (선택 사항) 선택 [!UICONTROL **완료된 카드 보관 안 함**] 완료된 작업 및 문제를 완료됨 열에 표시되는 카드로 보드에 가져오기. 이 옵션을 선택하지 않으면 보드 생성 시 완료된 카드가 보드로 제공됩니다.

      >[!NOTE]
      >
      >기본적으로 보관된 카드는 보드에 표시되지 않습니다. 보관된 카드를 표시하려면 구성 설정을 켠 다음 보드를 필터링하여 보관된 카드를 표시해야 합니다. 자세한 내용은 [카드에 표시할 필드 사용자 지정](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md) 및 [보드에서 필터링 및 검색](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   1. (선택 사항) [!UICONTROL **고급 필터 사용**] 추가 필터 옵션을 표시합니다.

      이 프로세스는 접수 열에 필터를 만드는 프로세스와 동일합니다. 자세한 내용은 [보드에 접수 열 추가](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

      동적 보드를 만든 후 필터를 업데이트하면 Workfront 작업 또는 문제(예: 태그)에 포함되지 않은 카드 설정이 재설정됩니다.

   1. 필터를 추가한 후 다음을 클릭합니다. [!UICONTROL **보드 만들기**].

1. 보드에 대한 이름을 입력합니다. **[!UICONTROL 보드]** 필드를 입력하고 Enter 키를 누릅니다.
1. 필요에 따라 보드를 구성합니다.

   자세한 내용은 [보드에서 구성원 추가 또는 제거](../../agile/get-started-with-boards/add-members-to-board.md), [보드 열 관리](../../agile/get-started-with-boards/manage-board-columns.md), [보드에 애드혹 카드 추가](../../agile/get-started-with-boards/add-card-to-board.md), 및 [보드에서 연결된 카드 사용](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. 클릭 **[!UICONTROL 모든 게시판]** 을 눌러 보드 대시보드로 돌아갑니다.

   현재 보드 이름으로 레이블이 지정된 드롭다운 메뉴를 찾은 다음 클릭하여 다른 보드로 전환할 수도 있습니다.

   ![보드 목록](assets/boards-button-list-of-boards-350x188.png)

## 기존 게시판 편집

{{step1-to-boards}}

1. 대시보드에서 열 보드를 선택합니다.
1. 필요에 따라 보드를 편집합니다. 보드 이름을 클릭하여 이름을 바꿀 수 있습니다.

   자세한 내용은 [보드에서 구성원 추가 또는 제거](../../agile/get-started-with-boards/add-members-to-board.md), [보드 열 관리](../../agile/get-started-with-boards/manage-board-columns.md), 및 [보드에 카드 추가](../../agile/get-started-with-boards/add-card-to-board.md).

1. 클릭 **[!UICONTROL 모든 게시판]** 을 눌러 보드 대시보드로 돌아갑니다.

   현재 보드 이름으로 레이블이 지정된 드롭다운 메뉴를 찾은 다음 클릭하여 다른 보드로 전환할 수도 있습니다.
