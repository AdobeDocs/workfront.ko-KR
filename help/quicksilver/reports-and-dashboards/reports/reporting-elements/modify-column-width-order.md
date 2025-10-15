---
product-area: reporting
navigation-topic: reporting-elements
title: 열 너비 및 순서 수정
description: Workfront에서 열 너비 지침 및 열 너비와 순서를 변경하는 방법에 대해 알아보려면 이 문서를 검토하십시오.
author: Nolan
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1004'
ht-degree: 0%

---

# 열 너비 및 순서 수정

<!-- Audited: 11/2024 -->

다음은 Adobe Workfront에서 열 너비가 작동하는 방식에 대한 지침입니다.

* Workfront은 기본적으로 목록 및 보고서의 열 너비를 정의합니다.
* 열의 텍스트 모드에서 별도로 지정하지 않는 한 Workfront은 모든 목록 및 보고서의 `valueformat` 정보에 따라 열의 너비를 자동으로 조정합니다.

  >[!NOTE]
  >
  >Workfront에서는 설정 및 보고서 영역에서 사용할 수 있는 목록의 `valueformat` 정보에 따라 열의 너비를 조정하지 않습니다.

  `valueformat` 값은 열에 표시되는 정보의 종류를 정의합니다. 예를 들어, 숫자를 표시하는 열이 설명 필드를 표시하는 열보다 좁습니다.

* 열에 표시할 정보 유형에 따라 Workfront 목록 및 보고서의 열 너비를 필요에 맞게 사용자 지정할 수 있습니다.

  목록 또는 보고서를 볼 때 일시적으로 또는 뷰 빌더에서 열의 너비를 조정하여 영구적으로 열의 너비를 수정할 수 있습니다. 임시 열 너비 수정에 대한 자세한 내용은 이 문서에서 [임시 열 너비 및 순서 수정 시 고려 사항](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) 섹션을 참조하십시오.

* 기본 제공 보기에 표시되는 열에는 이전에 Workfront으로 하드 코딩된 너비가 있습니다. 이러한 폭을 수정하려면 뷰 빌더에서 텍스트 모드를 사용하여 이러한 열의 폭을 수동으로 업데이트해야 합니다.

  텍스트 모드에서 열을 수정하는 방법에 대한 자세한 내용은 [보기: 열 너비를 영구적으로 편집](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md)을 참조하십시오.

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
   <td role="rowheader">Adobe Workfront 라이선스</strong></td> 
   <td> 
    <p>기여자 이상</p>
    <p>요청 이상</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서에서 보기 편집</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
    <td> <p>보고서에서 보기를 편집하려면 보고서에 대한 권한 관리</p> <p>보기에 대한 편집 권한 관리</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 열 너비 및 순서 수정

다음과 같은 방법으로 보고서에 있는 열의 너비와 순서를 수정할 수 있습니다.

* [일시적으로 열 너비와 순서 수정](#modify-width-and-order-of-columns-temporarily)
* [열 너비와 순서를 영구적으로 수정](#modify-width-and-order-of-columns-permanently)

### 임시로 열 너비 및 순서 수정 {#modify-width-and-order-of-columns-temporarily}

열 테두리를 드래그하여 열의 크기를 조정하고, 열을 드래그 앤 드롭하여 Workfront 사이트 전체 대부분의 목록에서 열의 순서를 일시적으로 변경할 수 있습니다. 여기에는 보고서, 보기, 대시보드의 보고서 및 간트 보기가 포함됩니다.

Workfront 목록에 대한 자세한 내용은 문서 [Adobe Workfront 목록 시작](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)을 참조하십시오.

* [열의 너비와 순서를 일시적으로 수정할 때 고려 사항](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [일시적으로 열 크기 조정](#resize-columns-temporarily)
* [일시적으로 열 순서 바꾸기](#reorder-columns-temporarily)

#### 열의 너비 및 순서를 일시적으로 수정할 때 고려 사항 {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

보기를 편집하지 않고 목록의 열 너비와 순서를 임시로 수정할 수 있습니다.

열의 크기를 일시적으로 조정하고 순서를 지정할 때 다음 사항을 고려하십시오.

* 열 크기를 조정할 때 새 열 크기는 브라우저의 로컬 저장소에 저장되고 기본적으로 저장됩니다. 다른 브라우저를 사용하거나 캐시를 지우거나 데이터를 검색하면 열 크기가 기본값으로 되돌아갑니다. 페이지를 새로 고치면 열 너비에 대한 변경 사항이 유지됩니다.

>[!NOTE]
> 
>열 너비는 브라우저 창의 크기로 제한됩니다. 페이지를 새로 고치면 모든 열이 수평 스크롤하지 않고 창에 들어갈 수 있을 때까지 열의 너비가 줄어듭니다. 열을 브라우저에 맞는 너비보다 넓게 유지하려면 [열 너비와 순서 영구적으로 수정](#modify-width-and-order-of-columns-permanently)에 설명된 대로 텍스트 모드에서 열 너비를 설정하고 테두리를 드래그하여 열 너비를 수동으로 조정하지 않아야 합니다.
>

* 열을 재정렬할 때 선택한 순서는 목록에서 나가거나 브라우저 페이지를 새로 고칠 때까지만 유지됩니다. 목록에서 다른 위치로 이동하거나 브라우저 페이지를 새로 고치면 열이 기본 순서로 돌아갑니다.
* 최적의 성능을 위해 재정렬하려는 열에는 목록에 100개를 초과하는 항목이 없어야 합니다.
* 열 크기를 조정하면 변경 사항은 현재 사용 중인 보기에만 적용되며 사용자에게만 표시됩니다. 다른 사용자와 보기를 공유해도 정의한 열 크기는 공유되지 않습니다.
* 열 테두리를 오른쪽으로 끌어 열 크기를 조정하면 인접한 열의 너비는 다음을 제외하고 유지됩니다.

   * 설정 영역
   * 보고서 영역
   * 문서 목록 및 보고서

  >[!NOTE]
  >
  >열의 왼쪽 테두리를 목록의 인접한 열의 왼쪽 테두리를 지나서 이동할 수 없습니다.

* 목록을 파일로 내보내면 열의 임시 순서가 내보낸 파일로 전송되지 않습니다. 내보낸 파일은 원래 목록에 있는 열의 순서를 재정렬하기 전에 표시합니다.

목록 및 보고서에서 데이터를 내보내는 방법에 대한 자세한 내용은 문서 [데이터 내보내기](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)를 참조하십시오.

#### 일시적으로 열 크기 조정 {#resize-columns-temporarily}

1. 수정할 목록으로 이동합니다.
1. 열이 원하는 크기에 도달할 때까지 열 머리글의 테두리를 드래그합니다.\
   ![열 크기 조정](assets/column-resize-350x124.png)

#### 일시적으로 열 순서 바꾸기 {#reorder-columns-temporarily}

1. 수정할 목록으로 이동합니다.
1. 이동할 열 헤더를 클릭하여 원하는 위치로 드래그합니다.

>[!TIP]
>
>간트 차트와 목록 보기를 동시에 볼 때 특히 유용합니다. 간트 차트를 볼 때 열이 숨겨질 수 있습니다. 간트 차트가 표시되는 동안 열을 보려면 보려는 열을 드래그하여 페이지 왼쪽에 표시하면 됩니다.

### 열 너비와 순서를 영구적으로 수정 {#modify-width-and-order-of-columns-permanently}

열의 순서를 영구적으로 조정하려면 문서 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view)에서 [표준 보기 만들기 또는 사용자 지정](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md) 섹션을 참조하십시오.

텍스트 모드를 사용해야만 열의 너비를 영구적으로 수정할 수 있습니다.

텍스트 모드를 사용하고 열의 너비를 영구적으로 수정하는 방법에 대한 자세한 내용은 문서 [텍스트 모드의 일반적인 사용 개요](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)를 참조하십시오.
