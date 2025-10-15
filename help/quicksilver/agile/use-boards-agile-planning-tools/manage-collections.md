---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 작업 스트림 관리
description: 작업 스트림은 작업에 대해 공동 작업하기 위해 구성 가능한 보드 및 카드 그룹입니다.
author: Lisa
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 1%

---

# 작업 스트림 관리

>[!IMPORTANT]
>
>작업 스트림은 특정 고객 그룹만 사용할 수 있습니다.

작업 스트림은 작업에 대해 공동 작업하기 위해 구성 가능한 보드 및 카드 그룹입니다. 작업 스트림에는 템플릿과 작업 항목의 카드 목록에서 생성된 다양한 유형의 보드가 포함될 수 있습니다. 워크스트림에서 반복 또는 스프린트로 작업을 추적할 수 있습니다.

자세한 내용은 [카드 목록 사용](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) 및 [워크플로에서 반복 만들기](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md)를 참조하십시오.

작업 스트림은 작업 스트림의 일부가 아닌 액세스 권한이 있는 개별 보드와 함께 대시보드에 표시됩니다. 보드 대시보드에 대한 자세한 내용은 [보드 대시보드 사용](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md)을 참조하세요. 대시보드에서 보드 이름을 클릭하여 열 수 있습니다.

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

## 작업 스트림 만들기

{{step1-to-boards}}

1. 대시보드의 **[!UICONTROL 작업 스트림]** 영역에서 [!UICONTROL 작업 스트림 추가]를 클릭합니다.
1. **[!UICONTROL 제목 없는 작업 스트림]**&#x200B;을 바꿀 이름을 입력하고 Enter 키를 누르십시오.

   워크스트림에 보드를 추가하거나 [!UICONTROL **모든 보드**]&#x200B;를 클릭하여 대시보드로 돌아갈 수 있습니다.

## 워크스트림에 새 보드 만들기

1. 아직 작업 스트림에 있지 않은 경우 대시보드에서 [!UICONTROL **작업 스트림 보기**]&#x200B;를 클릭하여 기존 작업 스트림을 엽니다.
1. 작업 스트림의 **[!UICONTROL 보드]** 탭에서 [!UICONTROL 보드 추가]를 클릭합니다.
1. 보드에 사용할 템플릿을 선택합니다.

| 템플릿 | 설명 |
|---------|----------|
| 기본 보드 | 보드에는 세 개의 기본 열이 제공됩니다. 새 열을 추가하고 기본 열의 이름을 바꾸거나 삭제할 수 있습니다. <p>열 정책이 적용되지 않습니다. |
| 칸반 보드 | 백로그, 신규, 진행 중, 완료 및 보류 중 열이 보드에 제공됩니다. 새 열을 추가하고 기본 열의 이름을 바꾸거나 삭제할 수 있습니다.<p>백로그를 사용하려면 접수 열에 대한 필터를 설정해야 합니다. 자세한 내용은 [보드에 접수 열 추가](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)를 참조하십시오. <p>각 열의 기본 정책을 검토하려면 열에서 [!UICONTROL **자세히** 메뉴]를 클릭하고 [!UICONTROL **편집**]&#x200B;을 선택합니다. 이러한 사전 설정된 정책을 변경할 수 있습니다. 자세한 내용은 [보드 열 관리](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)를 참조하십시오. |
| Retrospective 보드 | 게시판에는 다음과 같은 열이 제공됩니다. 무엇이 잘 되었습니까? 무엇을 개선할 수 있을까요? 축하해야 할 사람이 누구죠? 더 빨리 움직이기 위해 우리가 할 수 있는 일은 무엇인가? 새 열을 추가하고 기본 열의 이름을 바꾸거나 삭제할 수 있습니다. <p>열 정책이 적용되지 않습니다. |
| 반복 프로세스 | 반복을 정의하고 실행하는 데 사용되는 보드입니다. <p>백로그, 신규, 진행 중, 완료 및 보류 중 열이 보드에 제공됩니다. 보드에 열을 추가할 수 없습니다. <p>각 열의 기본 정책을 검토하려면 열에서 [!UICONTROL **자세히**] 메뉴를 클릭하고 [!UICONTROL **편집**]&#x200B;을 선택합니다. 이러한 사전 설정된 정책을 변경할 수 있습니다. 자세한 내용은 [보드 열 관리](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)를 참조하십시오. |

보드 설정에 대한 자세한 내용은 [보드 만들기 또는 편집](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md)을 참조하세요.

## 작업 스트림에서 보드 목록 필터링

보드 목록에 기본값이 아닌 필터가 적용되면 필터 아이콘 ![적용된 필터](assets/boards-filterapplied-30x30.png)에 표시기가 표시됩니다. 모든 필터를 제거하려면 [!UICONTROL **모두 지우기**]&#x200B;를 클릭하고 필터 패널을 닫으려면 [!UICONTROL **필터 숨기기**]&#x200B;를 클릭합니다.

{{step1-to-boards}}

1. 대시보드에서 [!UICONTROL **작업 스트림 보기**]&#x200B;를 클릭하여 작업 스트림을 엽니다.
1. 아직 표시되지 않은 경우 [!UICONTROL **보드**] 탭을 클릭하십시오.
1. [!UICONTROL **필터**]&#x200B;를 클릭합니다.
1. 상태별로 보려는 보드(보관된 보드, 활성 보드 또는 모든 보드)를 선택합니다.
1. 템플릿별로 보려는 보드를 선택합니다.

## 워크스트림에 구성원 추가

작업 스트림 및 해당 컨텐츠를 보려면 먼저 사람 및 팀을 구성원으로 작업 스트림에 추가해야 합니다. 작업 스트림 구성원은 작업 스트림에 구성원을 추가 및 제거하고 작업 스트림에 있는 보드를 확인할 수 있습니다.

>[!NOTE]
>
>작업 스트림 구성원은 특정 보드에 구성원으로 추가될 때까지 작업 스트림에서 보드를 열 수 없습니다.

{{step1-to-boards}}

1. 대시보드에서 [!UICONTROL **작업 스트림 보기**]&#x200B;를 클릭하여 작업 스트림을 엽니다.
1. 워크스트림에 구성원 및 팀을 추가하려면 **[!UICONTROL 구성원 추가]** 아이콘 ![구성원 추가](assets/boards-addmember-spectrum-25x25.png)를 클릭하십시오.

   이는 보드에 멤버를 추가하는 것과 동일한 프로세스입니다. 자세한 내용은 [보드에서 구성원 추가 또는 제거](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md)를 참조하십시오.

## 워크스트림에 소스 추가

소스는 작업 스트림의 카드 출처를 결정합니다.

{{step1-to-boards}}

1. 카드를 작업 스트림으로 가져올 소스를 정의하려면 [!UICONTROL **소스**] 아이콘 ![소스 아이콘](assets/sources-icon.png)을(를) 클릭하십시오. 현재 사용 가능한 원본은 [!DNL Adobe Workfront]뿐입니다.
1. 필터를 추가하여 Workfront에서 작업 및 문제를 카드로 가져옵니다.

   작업 스트림 소스에 대한 필터를 추가하는 것은 기본 보드 또는 Kanban 보드에서 접수 열에 대한 고급 필터를 추가하는 것과 같습니다. 자세한 내용은 [보드에 접수 열 추가](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)를 참조하십시오.

## 작업 스트림 구성

{{step1-to-boards}}

1. 대시보드에서 [!UICONTROL **작업 스트림 보기**]&#x200B;를 클릭하여 작업 스트림을 엽니다.
1. [!UICONTROL **구성**]&#x200B;을 클릭하여 [!UICONTROL 작업 스트림 구성] 패널을 엽니다.
1. (선택 사항) [!UICONTROL **작업 스트림**]&#x200B;을 확장하고 작업 스트림에 대한 설명을 입력합니다. 이 설명은 대시보드에 표시됩니다.
1. (선택 사항) [!UICONTROL **반복**]&#x200B;을 확장하여 이 워크스트림에 대한 반복 프로세스를 정의합니다.

   카드 목록 섹션에 총 카드 수, 뾰족한 카드 수 및 반복 횟수가 표시됩니다. 목록을 열고 카드를 추가하려면 [!UICONTROL **목록 보기**]&#x200B;를 클릭하세요. 자세한 내용은 [카드 목록 사용](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md)을 참조하세요.

   반복이 이미 정의된 경우 해당 시작 날짜, 카드 수 및 포인트 수가 표시됩니다. [!UICONTROL **보드 보기**]&#x200B;를 클릭하여 반복 보드를 엽니다. 자세한 내용은 [워크플로에서 반복 만들기](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md)를 참조하십시오.

1. (선택 사항) [!UICONTROL **태그**]&#x200B;를 확장하여 작업 스트림에 태그를 추가합니다. 태그를 검색하거나 검색 상자에 새 태그 이름을 입력하고 Enter 키를 눌러 태그를 만듭니다.
