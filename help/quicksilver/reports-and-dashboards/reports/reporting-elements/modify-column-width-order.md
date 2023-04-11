---
product-area: reporting
navigation-topic: reporting-elements
title: 열 너비 및 순서 수정
description: Workfront에서 열 너비 지침 및 열 너비 및 순서를 변경하는 방법에 대해 알려면 이 문서를 검토하십시오.
author: Nolan
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 0%

---

# 열 너비 및 순서 수정

다음은 Adobe Workfront에서 열 너비가 작동하는 방식에 대한 지침입니다.

* Workfront은 기본적으로 목록 및 보고서의 열 너비를 정의합니다.
* Workfront은 열 너비를 `valueformat`열의 텍스트 모드에서 별도로 지정하지 않는 한, 모든 목록 및 보고서에 대한 정보입니다.

   >[!NOTE]
   >
   >Workfront은 열 너비를 `valueformat` 설정 및 보고서 영역에서 사용할 수 있는 목록의 정보입니다.

   다음 `valueformat` 값은 열에 표시되는 정보의 종류를 정의합니다. 예를 들어, 숫자를 표시하는 열은 설명 필드를 표시하는 열보다 좁습니다.

* 열에 표시할 정보의 종류에 따라 Workfront 목록 및 보고서의 열 너비를 사용자 지정할 수 있습니다.

   목록 또는 보고서를 보는 동안 또는 보기 빌더에서 열 너비를 조정하여 일시적으로 열 너비를 수정하거나 영구적으로 변경할 수 있습니다. 임시 열 너비 수정에 대한 자세한 내용은 [열의 너비와 순서를 일시적으로 수정할 때의 고려 사항](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) 섹션에 자세히 설명되어 있습니다.

* 기본 제공 보기에 표시되는 열의 너비는 하드 코딩된 Workfront에서 이전에 정의한 너비를 갖습니다. 이러한 너비를 수정하려면 보기 빌더에서 텍스트 모드를 사용하여 이러한 열의 너비를 수동으로 업데이트해야 합니다.

   텍스트 모드에서 열 수정에 대한 자세한 내용은 [보기: 열 너비를 영구적으로 편집](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이선스*</strong></td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 달력에 대한 액세스를 편집하여 보고서의 보기를 편집합니다</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>보고서에 대한 권한을 관리하여 보고서의 보기를 편집합니다</p> <p>보기에 대한 권한을 관리하여 편집합니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 열 너비 및 순서 수정

다음과 같은 방법으로 보고서에서 열의 너비와 순서를 수정할 수 있습니다.

* [일시적으로 열 너비 및 순서를 수정합니다](#modify-width-and-order-of-columns-temporarily)
* [열의 폭 및 순서를 영구적으로 수정](#modify-width-and-order-of-columns-permanently)

### 일시적으로 열 너비 및 순서를 수정합니다 {#modify-width-and-order-of-columns-temporarily}

열 테두리를 끌어 열 크기를 조정하고 열을 끌어다 놓아 Workfront 사이트 전체의 대부분의 목록에서 일시적으로 열 순서를 변경할 수 있습니다. 여기에는 보고서, 보기, 대시보드의 보고서 및 간트 보기가 포함됩니다.

Workfront 목록에 대한 자세한 내용은 문서를 참조하십시오 [Adobe Workfront에서 목록 시작](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* [열의 너비와 순서를 일시적으로 수정할 때의 고려 사항](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [일시적으로 열 크기 조정](#resize-columns-temporarily)
* [일시적으로 열 재정렬](#reorder-columns-temporarily)

#### 열의 너비와 순서를 일시적으로 수정할 때의 고려 사항 {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

뷰를 편집하지 않고 목록의 열 너비와 순서를 일시적으로 수정할 수 있습니다.

열 크기를 일시적으로 조정하고 순서를 지정할 때 다음 사항을 고려하십시오.

* 열 크기를 변경하면 새 열 크기가 브라우저의 로컬 저장소에 저장되고 기본적으로 저장됩니다. 다른 브라우저를 사용하거나, 캐시를 지우거나, 검색 데이터를 지우면 열 크기가 기본값으로 되돌려집니다. 페이지를 새로 고치면 열 너비에 대한 변경 사항이 유지됩니다.
* 열 순서를 변경할 때 선택한 순서는 목록에서 이동하거나 브라우저 페이지를 새로 고칠 때까지 유지됩니다. 목록에서 이동하거나 브라우저 페이지를 새로 고치면 열이 기본 순서로 반환됩니다.
* 최적의 성능을 위해 순서를 변경하는 열에는 목록에 100개 이상의 항목이 없어야 합니다.
* 열 크기를 변경하면 변경 사항은 현재 사용 중인 보기에만 적용되며 사용자만 볼 수 있습니다. 다른 사용자와 보기를 공유해도 정의한 열 크기가 공유되지 않습니다.
* 테두리를 오른쪽으로 끌어 열 크기를 조정하면 인접한 열의 너비가 다음과 같이 유지됩니다.

   * 설정 영역
   * 보고서 영역
   * 문서 목록 및 보고서

   >[!NOTE]
   >
   >목록의 인접 열의 왼쪽 테두리를 지나면 열의 왼쪽 테두리를 이동할 수 없습니다.

* 목록을 파일로 내보내면 열의 임시 순서가 내보낸 파일로 전송되지 않습니다. 내보낸 파일은 열을 다시 정렬하기 전에 원래 목록의 열 순서를 표시합니다.

목록 및 보고서에서 데이터를 내보내는 방법에 대한 자세한 내용은 문서를 참조하십시오 [데이터 내보내기](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

#### 일시적으로 열 크기 조정 {#resize-columns-temporarily}

1. 수정할 목록으로 이동합니다.
1. 열이 원하는 크기에 도달할 때까지 열의 테두리를 드래그합니다.\
   ![](assets/column-resize-350x124.png)

#### 일시적으로 열 재정렬 {#reorder-columns-temporarily}

1. 수정할 목록으로 이동합니다.
1. 열을 선택하려면 다른 위치로 이동할 열을 클릭합니다.
1. 열을 올바른 위치로 드래그합니다.
1. 열을 위치에 놓아 이동합니다.

   ![](assets/column-reorder-350x118.png)

>[!TIP]
>
>간트 차트와 목록 보기를 동시에 볼 때 특히 유용합니다. 간트 차트를 볼 때 열이 숨겨질 수 있습니다. 간트 차트가 표시되는 동안 열을 보려면 페이지의 왼쪽에 표시되도록 보려는 열을 드래그하기만 하면 됩니다.

### 열의 폭 및 순서를 영구적으로 수정 {#modify-width-and-order-of-columns-permanently}

열을 영구적으로 재정렬하려면 섹션을 참조하십시오 [표준 보기 만들기 또는 사용자 지정](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view) 기사 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

텍스트 모드를 사용해야만 열의 너비를 영구적으로 수정할 수 있습니다.

텍스트 모드를 사용하고 열의 너비를 영구적으로 수정하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [텍스트 모드에 대한 일반적인 사용 개요](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
