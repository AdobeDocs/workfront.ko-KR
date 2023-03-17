---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 워크플로우 관리
description: 워크스트림은 작업을 공동 작업하기 위해 구성 가능한 보드 및 카드 그룹입니다.
author: Lisa
feature: Agile
source-git-commit: 16e96d55932116cb475eecbe8b6ebfd4661eb494
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 2%

---

# 워크플로우 관리

{{highlighted-preview}}

>[!NOTE]
>
>워크플로우는 미리 보기 환경에서 사용할 수 있고, 이른 기능 옵트인을 통해 프로덕션에서 사용할 수 있습니다 [!UICONTROL [!DNL Workfront] 보드]. 자세한 내용은 [Adobe Workfront 보드에 대한 초기 기능 옵트인](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

워크스트림은 작업을 공동 작업하기 위해 구성 가능한 보드 및 카드 그룹입니다. 워크플로우에는 템플릿에서 만든 다양한 유형의 보드가 포함될 수 있습니다. <span class="preview">그리고 작업 항목의 카드 목록입니다. 워크플로우에서는 반복 또는 스프린트에서 작업을 추적할 수 있습니다.</span>

<span class="preview">자세한 내용은 [카드 목록 사용](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) 및 [반복 만들기](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md).</span>

작업 스트림은 작업 스트림의 일부가 아닌 개별 보드에 액세스할 수 있는 개별 보드와 함께 대시보드에 나타납니다. 보드 대시보드에 대한 자세한 내용은 [보드 대시보드 사용](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). 대시보드에서 보드 이름을 클릭하여 열 수 있습니다.

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

## 작업 스트림 만들기

{{step1-to-boards}}

1. 클릭 **[!UICONTROL 작업 스트림 추가]** 에서 [!UICONTROL Workstreams] 대시보드 영역입니다.
1. 바꿀 이름을 입력합니다 **[!UICONTROL 제목 없는 작업 스트림]** Enter 키를 누릅니다.

   작업 스트림에 보드를 추가하거나 [!UICONTROL **모든 보드**] 를 눌러 대시보드로 돌아갑니다.

## 워크플로우에서 새 보드 만들기

1. 아직 워크플로우에 있지 않은 경우 [!UICONTROL **작업 스트림 보기**] 대시보드에서 기존 작업 스트림을 엽니다.
1. 클릭 **[!UICONTROL 보드 추가]** on [!UICONTROL 보드] 작업 스트림의 탭입니다.
1. 보드의 템플릿을 선택합니다.

| 템플릿 | 설명 |
|---------|----------|
| 기본 보드 | 보드에 기본 열 3개가 제공됩니다. 새 열을 추가하고 기본 열의 이름을 바꾸거나 삭제할 수 있습니다. <p>적용된 열 정책이 없습니다. |
| 칸반 보드 | 보드에 다음 열이 제공됩니다. 백로그, 신규, 진행 중, 완료 및 보류 중 새 열을 추가하고 기본 열의 이름을 바꾸거나 삭제할 수 있습니다.<p>백로그를 사용하려면 취입 열에 대한 필터를 설정해야 합니다. 자세한 내용은 [보드에 흡기 열 추가](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>각 열에 대한 기본 정책을 검토하려면 [!UICONTROL **자세히** 메뉴] 열에서 [!UICONTROL **편집**]. 이러한 사전 설정된 정책을 변경할 수 있습니다. 자세한 내용은 [보드 열 관리](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| Retrospective 보드 | 보드에 다음 열이 제공됩니다. 뭐가 잘 됐어? 개선 가능한 사항? 축하해야 할 사람? 보다 빠른 진행을 위해 할 수 있는 일? 새 열을 추가하고 기본 열의 이름을 바꾸거나 삭제할 수 있습니다. <p>적용된 열 정책이 없습니다. |
| <span class="preview">반복 프로세스</span> | <span class="preview">반복을 정의하고 실행하는 데 사용되는 보드입니다. <p>보드에 다음 열이 제공됩니다. 백로그, 신규, 진행 중, 완료 및 보류 중 보드에 열을 추가할 수 없습니다. <p>각 열에 대한 기본 정책을 검토하려면 [!UICONTROL **자세히**] 열의 메뉴를 선택하고 [!UICONTROL **편집**]. 이러한 사전 설정된 정책을 변경할 수 있습니다. 자세한 내용은 [보드 열 관리](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).</span> |

보드 설정에 대한 자세한 내용은 [보드 만들기 또는 편집](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## 작업 스트림에서 보드 목록 필터링

기본값 이외의 필터가 보드 목록에 적용되면 필터 아이콘에 표시기가 표시됩니다 ![적용된 필터](assets/boards-filterapplied-30x30.png). 클릭 [!UICONTROL **모두 지우기**] 모든 필터를 제거하려면 [!UICONTROL **필터 숨기기**] 를 클릭하여 필터 패널을 닫습니다.

{{step1-to-boards}}

1. 대시보드에서 [!UICONTROL **작업 스트림 보기**] 작업 스트림을 엽니다.
1. 을(를) 클릭합니다. [!UICONTROL **보드**] 아직 표시되지 않은 경우 탭합니다.
1. 클릭 [!UICONTROL **필터**].
1. 상태별로 볼 보드(보관된 보드, 활성 보드 또는 모든 보드)를 선택합니다.
1. 템플릿으로 볼 보드를 선택합니다.

## 작업 스트림에 구성원 추가

사용자 및 팀이 작업 스트림 및 해당 컨텐츠를 볼 수 있으려면 먼저 작업 스트림에 구성원으로 추가되어야 합니다. 작업 스트림 멤버는 작업 스트림에서 멤버를 추가 및 제거하고 작업 스트림에 있는 보드를 확인할 수 있습니다.

>[!NOTE]
>
>작업 스트림 멤버는 특정 보드에 구성원으로 추가될 때까지 작업 스트림에서 보드를 열 수 없습니다.

{{step1-to-boards}}

1. 대시보드에서 [!UICONTROL **작업 스트림 보기**] 작업 스트림을 엽니다.
1. 을(를) 클릭합니다. **[!UICONTROL 멤버 추가]** 아이콘 ![구성원 추가](assets/boards-addmember-spectrum-25x25.png) 작업 스트림에 멤버 및 팀을 추가하려면 다음을 수행합니다.

   이는 보드에 구성원을 추가하는 것과 동일한 프로세스입니다. 자세한 내용은 [보드에서 구성원 추가 또는 제거](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

<div class="preview">

## 작업 스트림 구성

{{step1-to-boards}}

1. 대시보드에서 [!UICONTROL **작업 스트림 보기**] 작업 스트림을 엽니다.
1. 클릭 [!UICONTROL **구성**] 열다 [!UICONTROL 작업 스트림 구성] 패널.
1. (선택 사항) 작업 스트림에 대한 설명을 입력합니다. 이 설명은 대시보드에 표시됩니다.

   카드 목록 섹션에 총 카드 수, 포인트의 카드 수 및 반복 수가 표시됩니다. 클릭 [!UICONTROL **목록 보기**] 목록을 열고 카드를 추가합니다. 자세한 내용은 [카드 목록 사용](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   이터레이션이 정의된 경우 시작 날짜, 카드 수 및 포인트 수가 표시됩니다. 클릭 [!UICONTROL **이터레이션 보드 보기**] 보드를 열려면 자세한 내용은 [반복 만들기](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md).

1. 클릭 [!UICONTROL **소스 추가**] 카드를 워크플로우로 가져올 소스를 정의하려면 현재 사용 가능한 소스는 [!DNL Adobe Workfront].
1. 필터를 추가하여 Workfront에서 작업 및 문제를 카드로 가져옵니다.

   작업 스트림 소스에 대한 필터를 추가하는 것은 기본 보드나 간판 보드의 흡기 열에 대한 필터를 추가하는 것과 같습니다. 자세한 내용은 [보드에 흡기 열 추가](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

</div>
