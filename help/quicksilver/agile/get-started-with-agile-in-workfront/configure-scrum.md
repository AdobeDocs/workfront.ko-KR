---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: 스크럼 구성
description: 팀이 만들어지는 동안 또는 후에 스크럼 애자일 팀에 대해 다음 옵션을 구성할 수 있습니다.
author: Lisa
feature: Agile
exl-id: 7509608e-96af-4601-80d4-791ee29046da
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '1667'
ht-degree: 0%

---

# 구성 [!UICONTROL 스크럼]

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

>[!NOTE]
>
>팀에 현재 진행 중인 이터레이션이 있으면 이 설정을 변경할 수 없습니다.

지점을 사용하거나 시간을 사용하여 추정하도록 스토리를 구성할 수 있습니다.

애자일 팀에 대한 스토리가 예상되는 방식을 구성하려면 다음을 수행하십시오.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!UICONTROL Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

1. 을(를) 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘을 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.
1. 관리할 애자일 팀을 선택합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 메뉴를 선택한 다음 **[!UICONTROL 편집]**.

   팀 구성원만 [!UICONTROL 계획] 또는 [!UICONTROL 작업] 라이센스를 보려면 이 옵션을 참조하십시오.\
   ![팀 편집](assets/edit-team-settings-350x205.png)

1. 에서 **[!UICONTROL 애자일]** 섹션, **[!UICONTROL 에서 스토리 예측]** 영역에서 스토리의 크기(작업 로드)를 추정하는 데 포인트 또는 시간을 사용할지 여부를 선택합니다. 점 을 선택하는 경우 1점과 동일한 시간 수를 지정합니다. (기본값은 1포인트 = 8시간입니다.) 스토리에 추가된 계획 시간 수입니다.

   **예:** 몇 점에서 스토리를 추정하도록 선택했고 1점이 8시간과 같으며 스토리가 3점에서 추정된다면, 24시간의 계획된 시간이 스토리에 추가됩니다.

1. 클릭 **[!UICONTROL 변경 내용 저장]**.

## 애자일 스토리 보드에 상태 열 구성

팀에 할당된 모든 반복 또는 주어진 프로젝트에 대해 애자일 스토리 보드에 표시되는 열을 구성할 수 있습니다.

* [반복에 대한 상태 열 구성](#configure-status-columns-for-iterations)
* [프로젝트에 대한 상태 열 구성](#configure-status-columns-for-projects)

### 반복에 대한 상태 열 구성 {#configure-status-columns-for-iterations}

애자일 팀을 위한 스토리 보드에 있는 상태를 정의할 수 있습니다. 이는 스토리 보드에 표시되는 유일한 상태입니다.

애자일 팀과 연결된 스토리 보드에 사용할 수 있는 상태를 정의하려면

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

1. 을(를) 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

1. 관리할 애자일 팀을 선택합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 메뉴를 선택한 다음 **[!UICONTROL 편집]**.

   팀 구성원만 [!UICONTROL 계획] 또는 [!UICONTROL 작업] 라이센스를 보려면 이 옵션을 참조하십시오.

   ![팀 편집](assets/edit-team-settings-350x205.png)

1. 에서 **[!UICONTROL 애자일]** 섹션에서 **[!UICONTROL 스토리 보드]** 영역.

1. (선택 사항) **[!UICONTROL 열 추가]** 를 눌러 스토리 보드에 상태 열을 추가합니다.
1. (선택 사항) 드래그 앤 드롭 표시기를 사용하여 상태 열을 드래그하여 스토리 보드에서 상태 열을 재정렬합니다. 첫 번째 열은 이동할 수 없으며 첫 번째 열 앞에 있는 다른 열을 드래그할 수 없습니다.

   ![드래그 앤 드롭](assets/agile-story-card-drag-and-drop.png)

1. 작업 및 문제 상태를 모두 선택합니다. 작업 상태는 작업 보드의 각 열에 대한 열 제목으로 표시됩니다. 선택하는 문제 상태는 작업 상태에 매핑됩니다. 즉, 문제를 스토리 보드의 다른 열로 이동할 때 문제 상태는 여기에 표시된 문제 상태로 변경되고 작업 상태를 반영하는 스토리 보드의 열 이름(작업 상태)에는 표시되지 않습니다.

   >[!IMPORTANT]
   >
   >잠긴 시스템 전체 상태만 선택할 수 있습니다. 그룹별 상태는 선택할 수 없습니다. 또한 첫 번째 열의 상태는 항상 **[!UICONTROL 새로 만들기]**.

   다음과 같은 경우 사용자 지정 상태를 추가할 수 있습니다 [!DNL Workfront] 관리자가 구성했습니다. 사용자 지정 상태는 [상태 만들기 또는 편집](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   >[!NOTE]
   >
   >문제 상태를 선택할 때 세 번째 열의 기본값은 항상 입니다 [!UICONTROL 닫힘]. 열이 3개 이상인 경우 적절한 상태를 반영하도록 열을 수동으로 업데이트해야 합니다.

1. 클릭 **[!UICONTROL 변경 내용 저장]**.

### 프로젝트에 대한 상태 열 구성 {#configure-status-columns-for-projects}

프로젝트의 상태 열을 구성하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [만들기 또는 사용자 지정 [!UICONTROL 애자일] 보기](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md#customizing-an-agile-view) 기사 [에서 보기 만들기 또는 편집 [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

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

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!UICONTROL Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

1. 을(를) 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

1. 관리할 애자일 팀을 선택합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 메뉴를 선택한 다음 **[!UICONTROL 편집]**.\
   팀 구성원만 [!UICONTROL 계획] 또는 [!UICONTROL 작업] 라이센스를 보려면 이 옵션을 참조하십시오.

   ![팀 편집](assets/edit-team-settings-350x205.png)

1. 에서 **[!UICONTROL 애자일]** 섹션에서 찾을 필드 이름을 입력합니다.

   ![추가 필드](assets/agile-additional-fields-scrum.png)

1. 추가할 필드 이름을 선택합니다.
1. 을(를) 입력합니다 **[!UICONTROL 표시 이름]** 해당 필드가 스토리 또는 발급 카드에 표시되는지 확인합니다.
1. 클릭 **[!UICONTROL 변경 내용 저장]**.

## 애자일 스토리 보드의 이야기에 색상 표시기가 사용되는 방식을 구성합니다

기본적으로 민첩한 반복의 스토리 보드 타일은 스토리가 연결된 프로젝트에 따라 색상으로 구분됩니다. 각 프로젝트에는 스토리 보드에 색상이 임의로 할당됩니다. 각 애자일 팀에 대해 이 기본 동작을 변경할 수 있습니다. 애자일 스토리의 색상은 스토리 우선 순위, 소유자 등과 연결할 수 있습니다.

애자일 팀을 위한 스토리에 색상을 할당하는 방법의 동작을 변경하려면 다음을 수행하십시오.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

1. 을(를) 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

1. 관리할 애자일 팀을 선택합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 메뉴를 선택한 다음 **[!UICONTROL 편집]**.

   팀 구성원만 [!UICONTROL 계획] 또는 [!UICONTROL 작업] 라이센스를 보려면 이 옵션을 참조하십시오.

   ![팀 편집](assets/edit-team-settings-350x205.png)

1. 에서 [!UICONTROL 애자일] 섹션, [!UICONTROL 카드 색상 연결] 영역에서 다음 선택 사항 중에서 선택합니다.

   * **[!UICONTROL 프로젝트]**: 색상은 스토리가 연결된 프로젝트와 연결됩니다. 스토리를 만들 때는 다음에 설명된 대로 프로젝트와 연결되어야 합니다. [애자일 스토리 만들기](/help/quicksilver/agile/work-in-an-agile-environment/create-an-agile-story.md). 동일한 프로젝트의 모든 작업이 동일한 색상으로 표시됩니다.
   * **[!UICONTROL 자유 형식]**: 사용자가 다음에 설명된 대로 수동으로 색상을 변경할 때까지 기본적으로 모든 카드가 파란색으로 표시됩니다. [[!UICONTROL 색상별로 스토리 분류] 스럼보드](/help/quicksilver/agile/use-scrum-in-an-agile-team//scrum-board/categorize-stories-by-color.md).
   * **[!UICONTROL 우선순위]**: 색상은 다음과 같이 스토리 우선 순위와 연결됩니다.

      * 높음 = 빨강
      * 보통 = 노란색
      * 낮음 = 녹색\

         시스템 관리자가 사용자 지정 우선 순위를 [!DNL Workfront] 시스템이 가장 높은 우선 순위는 빨간색이고 두 번째 순위는 노란색이고 세 번째 가장 높은 곳은 녹색입니다.
   * **[!UICONTROL 작업 소유자]**: 기본 할당자가 같은 모든 스토리는 동일한 색입니다. 기본 할당자는 작업에 처음 할당된 사용자입니다.


1. 클릭 **[!UICONTROL 변경 내용 저장]**.

## 작업 항목을 이터레이션에 추가할 때 날짜가 적용되는 방식을 구성합니다

기본적으로 작업 항목을 스크럼 이터레이션에 추가하면 작업 항목의 계획 시작 날짜 및 계획 완료 날짜가 반복 시작 날짜와 종료 날짜와 일치하도록 수정됩니다. 팀의 모든 작업 항목에 대한 원래 날짜를 유지하도록 선택할 수 있습니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe] Workfront을 클릭한 다음 **[!UICONTROL 팀]**.
1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 막대에서 팀을 검색합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 메뉴를 선택한 다음 **[!UICONTROL 편집]**.\
   팀 구성원만 [!UICONTROL 계획] 또는 [!UICONTROL 작업] 라이센스를 보려면 이 옵션을 참조하십시오.
1. 에서 [!UICONTROL 애자일] 섹션, [!UICONTROL 작업 항목을 이터레이션에 추가할 때] 영역에서 다음 선택 사항 중에서 선택합니다.

   * **[!UICONTROL 반복 시작 및 종료 일자와 일치하도록 계획 시작 일자 및 계획 완료 일자를 수정합니다]**: 작업 항목이 이터레이션에 추가되면 작업 항목 날짜가 반복 날짜로 변경됩니다.\

      날짜를 수정하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [스토리 추가가 작업 날짜에 미치는 영향 이해](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md#understa) 기사 [기존 반복에 스토리 추가](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).
   * **[!UICONTROL 반복 시작 및 종료 일자와 일치하도록 계획 시작 일자 및 계획 완료 일자를 수정하지 마십시오]**: 작업 항목이 이터레이션에 추가되면 작업 항목은 원래 날짜를 유지합니다.

   날짜 옵션을 변경하면 이터레이션에 이미 있는 작업 항목의 날짜가 조정되지 않습니다.

   이러한 옵션은 팀이 각 다른 사람의 반복에 작업 항목을 할당할 때 날짜에 영향을 줄 수 있습니다. 예를 들어 팀 A는 작업 항목 날짜를 반복 날짜로 수정하고 팀 B는 작업 항목 날짜를 수정하지 않습니다. 팀 B가 팀 A의 반복에 작업 항목을 할당하면 작업 항목 날짜가 변경됩니다. 그러나 팀 A가 팀 B의 반복에 작업 항목을 할당하면 날짜가 변경되지 않습니다.

1. 클릭 **[!UICONTROL 변경 내용 저장]**.
