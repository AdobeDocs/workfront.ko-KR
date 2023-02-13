---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: 간판 구성
description: 팀이 생성되는 동안 또는 이후에 간판 애자일 팀에 대해 다음 옵션을 구성할 수 있습니다.
author: Lisa
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 0%

---

# 구성 [!UICONTROL 간판]

팀 생성 중 또는 이후에 애자일 팀에 대해 다음 옵션을 구성할 수 있습니다. 에서 애자일 팀(간판 또는 스크럼)을 생성합니다 [!DNL Adobe Workfront] 에 설명된 대로 [애자일 팀 만들기](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

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
   <td> <p>[!UICONTROL Work] 이상</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 확인하려면 [!DNL Workfront] 관리자

## 스토리가 몇 포인트 또는 몇 시간 단위로 예상되는지 구성

지점을 사용하거나 시간을 사용하여 추정하도록 스토리를 구성할 수 있습니다.

애자일 팀에 대한 스토리가 예상되는 방식을 구성하려면 다음을 수행하십시오.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

1. 을(를) 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘을 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.
1. 관리할 애자일 팀을 선택합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 메뉴를 선택한 다음 **[!UICONTROL 편집]**.

   팀 구성원만 [!UICONTROL 계획] 또는 [!UICONTROL 작업] 라이센스를 보려면 이 옵션을 참조하십시오.\
   ![팀 편집](assets/edit-team-settings-350x205.png)

1. 에서 **[!UICONTROL 애자일]** 섹션, **[!UICONTROL 에서 스토리 예측]** 영역에서 스토리의 크기(작업 로드)를 추정하는 데 포인트 또는 시간을 사용할지 여부를 선택합니다. 점 을 선택하는 경우 1점과 동일한 시간 수를 지정합니다. (기본값은 1포인트 = 8시간입니다.) 스토리에 추가된 계획 시간 수입니다.

   **예:** 몇 점에서 스토리를 추정하도록 선택했고 1점이 8시간과 같으며 스토리가 3점에서 추정된다면, 24시간의 계획된 시간이 스토리에 추가됩니다.

1. 클릭 **[!UICONTROL 변경 내용 저장]**.

## 애자일 스토리 보드에 상태 열 구성

애자일 팀을 위한 스토리 보드에 있는 상태를 정의할 수 있습니다. 이는 스토리 보드에 표시되는 유일한 상태입니다.

애자일 팀과 연결된 스토리 보드에 사용할 수 있는 상태를 정의하려면

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!UICONTROL Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

1. 을(를) 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

1. 관리할 애자일 팀을 선택합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 메뉴를 선택한 다음 **[!UICONTROL 편집]**.

   팀 구성원만 [!UICONTROL 계획] 또는 [!UICONTROL 작업] 라이센스를 보려면 이 옵션을 참조하십시오.

   ![팀 편집](assets/edit-team-settings-350x205.png)

1. 에서 **[!UICONTROL 애자일]** 섹션에서 **[!UICONTROL 스토리 보드]** 영역.

1. (선택 사항) **[!UICONTROL 열 추가]** 를 눌러 스토리 보드에 상태 열을 추가합니다.
1. (선택 사항) 드래그 앤 드롭 표시기를 사용하여 상태 열을 드래그하여 스토리 보드에서 상태 열을 재정렬합니다. 첫 번째 열은 이동할 수 없으며 첫 번째 열 앞에 있는 다른 열을 드래그할 수 없습니다.

   ![드래그 앤 드롭](assets/agile-story-card-drag-and-drop.png)

1. 작업 상태를 선택합니다.

   >[!IMPORTANT]
   >
   >잠긴 시스템 전체 상태만 선택할 수 있습니다. 그룹별 상태는 선택할 수 없습니다. 또한 첫 번째 열의 상태는 항상 **[!UICONTROL 새로 만들기]**.

   다음과 같은 경우 사용자 지정 상태를 추가할 수 있습니다 [!DNL Workfront] 관리자가 구성했습니다. 사용자 지정 상태는 [상태 만들기 또는 편집](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. 클릭 **[!UICONTROL 변경 내용 저장]**.

## 애자일 스토리 보드에 스토리 카드에 표시할 추가 필드를 구성합니다

스토리 카드에 필드를 추가하면 필드가 채워질 때 보기 전용이고 표시 전용입니다.

기본적으로 작업 및 문제에 대한 다음 유형의 데이터가 스토리 카드에 표시됩니다.

* 작업 또는 문제에 직접 연결되는 링크가 있는 스토리 이름
* 프로젝트에 직접 연결되는 링크가 있는 프로젝트 이름
* 이 링크는 하위 작업이 아니라 스토리에 대해서만 표시됩니다
* 작업 또는 문제 설명
* 현재 약정
* 완료 퍼센트를 직접 조정하거나 완료된 포인트 또는 시간 수를 조정하여 완료 비율을 보고 편집합니다
* 할당된 사용자

스토리 카드에 추가 데이터(사용자 지정 데이터 포함)를 표시할 수 있습니다. 여러 가지 이유로 스토리 카드에 추가 필드를 표시할 수 있습니다. 예를 들어, 반복 내에서 여러 고객을 위한 스토리에 작업하거나 프로젝트 시작 날짜 또는 프로젝트 완료 날짜를 표시하려는 경우 고객 ID를 표시할 수 있습니다.

>[!NOTE]
>
>스토리 카드에서 사용자 지정 필드를 사용하는 경우 이름에 마침표/점을 포함할 수 없습니다.

추가 필드를 표시하도록 애자일 팀에 할당된 스토리 카드를 구성하려면:

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

1. 을(를) 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

1. 관리할 애자일 팀을 선택합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 메뉴를 선택한 다음 **[!UICONTROL 편집]**.\
   팀 구성원만 [!UICONTROL 계획] 또는 [!UICONTROL 작업] 라이센스를 보려면 이 옵션을 참조하십시오.

   ![팀 편집](assets/edit-team-settings-350x205.png)

1. 에서 **[!UICONTROL 애자일]** 섹션에서 찾을 필드 이름을 입력합니다.

   ![추가 필드](assets/agile-additional-fields-kanban.png)

1. 추가할 필드 이름을 선택합니다.
1. 을(를) 입력합니다 **[!UICONTROL 표시 이름]** 해당 필드가 스토리 또는 발급 카드에 표시되는지 확인합니다.
1. 클릭 **[!UICONTROL 변경 내용 저장]**.

## 진행 중인 작업(WIP) 제한 구성

간판 [!DNL Workfront] 에 나타날 수 있는 작업 수를 제한하여 팀에서 현재 작업 중인 작업 양을 제어할 수 있습니다 [!UICONTROL 진행 중] 열 [!UICONTROL 간판] 보드.

WIP 제한이 구성되면, WIP 제한을 조회하거나, WIP에서 갱신할 수도 있습니다. [!UICONTROL 간판] 애자일 스토리보드 [WIP(진행 중인 작업) 제한을 [!UICONTROL 간판] 보드](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

간판 팀의 WIP를 제한하려면

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

1. 을(를) 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

1. 관리할 간판 팀을 선택합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 메뉴를 선택한 다음 **[!UICONTROL 편집]**.

   팀 구성원만 [!UICONTROL 계획] 또는 [!UICONTROL 작업] 라이센스를 보려면 이 옵션을 참조하십시오.

   ![팀 편집](assets/edit-team-settings-350x205.png)

1. 에서 **[!UICONTROL 애자일]** 섹션, **[!UICONTROL 방법론]** 섹션에서 간판이 선택되었는지 확인합니다.

1. 에서 **[!UICONTROL 스토리 보드]** 섹션, **[!UICONTROL WIP 제한]** 필드에서 각 열에 허용되는 최대 항목 수를 지정합니다 [!UICONTROL 간판] 애자일 스토리보드 각 열에 대해 다른 제한을 설정할 수 있습니다. 각 열에 설정할 수 있는 최대 제한은 100개입니다.\
   설정된 경우 WIP 제한에 경고 메시지가 표시됩니다 [!UICONTROL 간판] 스토리 보드의 모든 열에 대해 제한이 초과될 때마다 애자일 스토리 보드. 이 경고 메시지는 WIP 제한을 처음 초과할 때만 표시됩니다. 이 경고 메시지는 상태와 같은 상태가 있는 열에는 표시되지 않습니다 [!UICONTROL 완료].\
   WIP 제한은 단순한 시각적 경고이며, 사용자가 설정한 제한보다 하나의 열에 더 많은 항목이 있는 것을 제한하지 않습니다.

   ![WIP 제한](assets/wip-limit-350x193.png)

1. 클릭 **변경 내용 저장**.

## 백로그에서 자동으로 추가할 스토리를 구성합니다

백로그에서 스토리를 구성하여 페이지의 첫 번째 열에 자동으로 추가할 수 있습니다 [!UICONTROL 간판] 항목이 해당 열에서 이동되면 즉시 게시합니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

1. 을(를) 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

1. 관리할 간판 팀을 선택합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 메뉴를 선택한 다음 **[!UICONTROL 편집]**.

   팀 구성원만 [!UICONTROL 계획] 또는 [!UICONTROL 작업] 라이센스를 보려면 이 옵션을 참조하십시오.

   ![팀 편집](assets/edit-team-settings-350x205.png)

1. 선택 **[!UICONTROL 백로그에서 다음 스토리 자동 추가]** 백로그에서 페이지의 첫 번째 열에 자동으로 추가할 스토리를 구성하려면 [!UICONTROL 간판] 스토리 보드

   이 작업은 스토리가 전체 상태(완료와 동일한 상태)를 나타내는 스토리 보드의 열로 이동할 때마다 발생합니다. 백로그에서 추가하면 우선 순위가 가장 높은 스토리가 스토리 보드에 추가됩니다. 이 옵션을 선택하여 백로그에 자동으로 추가할 다음 항목을 구성합니다 **[!UICONTROL 진행 중]** 항목을 **[!UICONTROL 진행 중]** 열.

1. 클릭 **[!UICONTROL 변경 내용 저장]**.

## 카드가 [!UICONTROL 간판] 보드

완성된 카드가 [!UICONTROL 간판] 보드. 작업 [!UICONTROL 간판] 원래 프로젝트에서 보드에 계속 액세스할 수 있습니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 선택한 다음 드롭다운 메뉴에서 새 간판 팀을 선택하거나 검색 막대에서 팀을 검색합니다.
1. 간판 팀을 선택합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 메뉴를 선택한 다음 **Edit**.

   팀 구성원만 [!UICONTROL 계획] 또는 [!UICONTROL 작업] 라이센스를 보려면 이 옵션을 참조하십시오.

   ![팀 편집](assets/edit-team-settings-350x205.png)

1. 에서 **[!UICONTROL 완료된 카드가 간판 보드에 남아 있는 일 수]** 드롭다운 메뉴에서 값을 선택합니다.
1. 클릭 **[!UICONTROL 변경 내용 저장]**.
