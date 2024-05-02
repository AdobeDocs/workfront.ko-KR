---
title: 보고 캔버스에서 테이블 블록 추가 또는 편집
description: 보고 캔버스에서 테이블 블록 추가 또는 편집
hidefromtoc: true
hide: true
exl-id: d706659c-457f-4da0-a6e7-03ea29cab700
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---

# 보고 캔버스에서 테이블 블록 추가 또는 편집

테이블에는 필터링, 그룹화 및 정렬 가능한 열의 필드 정보가 표시됩니다.

## 전제 조건

시작하기 전에 보고 캔버스 베타에 등록해야 합니다. 자세한 내용은 [보고 캔버스 Beta: 개요](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## 테이블 블록 추가 또는 편집

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **보고**.
1. 클릭 **새 보고서**.

   또는

   기존 보고서로 이동하여 **자세히** 아이콘 ![](assets/more-icon-27x15.png) 보고서 헤더에서 를 클릭하고 **편집**.

1. 아래의 화면 오른쪽 **블록 추가**, 다음 중 하나를 수행합니다.

   드래그 **표** 아이콘 ![](assets/table-icon.png) 원하는 위치로 직접 캔버스에 연결합니다.

   또는

   를 두 번 클릭합니다. **표** 아이콘 ![](assets/table-icon.png) 캔버스의 맨 위에 표를 추가합니다.

   >[!TIP]
   >
   >블록 모서리 핸들을 드래그하여 블록을 배치한 후 블록 크기를 변경할 수 있습니다.

1. 클릭 **제목 없는 테이블** 그런 다음 표 머리글에 표의 제목을 입력합니다.

   ![](assets/table-name-350x142.png)

1. 클릭 **편집** 를 클릭하여 테이블을 구성합니다.

   >[!NOTE]
   >
   >테이블이 이미 캔버스에 포함된 경우(예: 기존 보고서를 편집할 때) **편집** 블록의 중앙에 버튼이 표시되지 않습니다. 테이블을 편집하려면 **편집** 아이콘 ![](assets/edit-icon.png) 테이블 머리글에서 을 클릭합니다.
   >![](assets/edit-icon-table-header-350x71.png)

1. 다음에서 **필드** 오른쪽의 패널에서 테이블에 열로 추가할 필드를 찾은 다음 원하는 테이블로 끌거나 더블 클릭하여 테이블의 마지막 열로 추가합니다.

   다음에서 텍스트를 입력할 수 있습니다. **검색** 이름으로 특정 필드를 찾는 상자입니다. 이 상자 아래의 두 드롭다운 메뉴를 사용하여 표시된 필드 목록을 다음 중 하나 또는 둘 다로 좁힐 수도 있습니다.

   * 원하는 필드와 연결된 개체 유형(예: 프로젝트 또는 작업)
   * 날짜 또는 통화와 같이 원하는 필드 유형입니다.

   열로 추가할 각 필드에 대해 이 단계를 반복합니다.

   >[!TIP]
   >
   >선택한 열을 새 위치로 끌어 테이블의 열 순서를 변경할 수 있습니다.

1. 표를 더 구성하려면 다음 중 하나를 수행하십시오.

   * **공식 필드 추가**: 클릭 **신규 +** 의 맨 위에 **필드** 목록을 표시합니다. 수식 필드를 만드는 방법에 대한 자세한 내용은 [보고 캔버스에서 공식 필드 작성](../../../reports-and-dashboards/reporting-canvas/table-blocks/create-formula-field.md).
   * **필터 추가**: 테이블을 필터링할 필드를 **필터** 테이블 위의 섹션에 있는 마지막 항목이 될 필요가 없습니다. 필터 규칙 설정에 대한 자세한 내용은 [보고 캔버스에서 테이블 필터링](../../../reports-and-dashboards/reporting-canvas/table-blocks/configure-filter-rules-for-table.md).
   * **특정 속성별로 행 그룹화**: 테이블을 그룹화할 필드를 **그룹** 테이블 위의 섹션에 있는 마지막 항목이 될 필요가 없습니다. 행 그룹 만들기에 대한 자세한 내용은 [보고 캔버스의 그룹 테이블 행](../../../reports-and-dashboards/reporting-canvas/table-blocks/group-rows-in-table.md).
