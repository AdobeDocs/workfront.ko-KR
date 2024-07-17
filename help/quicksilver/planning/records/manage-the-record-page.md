---
title: 레코드 페이지 레이아웃 관리
description: Adobe Workfront Planning에서 레코드 미리 보기 및 페이지의 레이아웃을 편집할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: f5430d81f1914a3717130de3af54b4b84e0e2d06
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# 레코드 페이지 레이아웃 관리

{{planning-important-intro}}

Adobe Workfront Planning에서 레코드 미리 보기 및 페이지의 레이아웃을 편집할 수 있습니다.

레코드 미리 보기는 레코드 유형 보기에 표시되는 레코드 페이지의 작은 보기입니다.

레코드 미리 보기 및 페이지의 레이아웃을 변경하면 변경 내용은 같은 유형의 모든 레코드의 미리 보기 상자 및 세부 정보 페이지에 영향을 미칩니다.

이 문서에서는 레코드 미리 보기 상자 또는 레코드 페이지의 레이아웃 및 모양을 변경하는 방법에 대해 설명합니다. 레코드 편집에 대한 자세한 내용은 [레코드 편집](/help/quicksilver/planning/records/edit-records.md)을 참조하세요.

레코드 페이지 편집을 시작하려면 먼저 레코드 종류 및 레코드를 만들어야 합니다.

자세한 내용은 다음 문서를 참조하십시오.

* [레코드 유형 만들기](/help/quicksilver/planning/architecture/create-record-types.md)

* [레코드 만들기](/help/quicksilver/planning/records/create-records.md)

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 제품</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 계약</p></td>
   <td>
<p>Workfront Planning의 조기 액세스 단계에 조직을 등록해야 합니다. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>임의</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td>
   <td>
   <p>새로운 기능: 표준</p>
   또는
   <p>현재: 플랜</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Adobe Workfront Planning에 대한 액세스 제어가 없습니다.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 영역</a>에 대한 권한 관리 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 계획 영역을 추가해야 합니다. 자세한 내용은 <a href="/help/quicksilver/planning/access/access-overview.md">액세스 개요</a>를 참조하십시오. </p>  
</td>
  </tr>

</tbody>
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

## 레코드 페이지 편집에 대한 고려 사항

* 기본적으로 레코드의 세부 정보 및 미리보기 페이지에는 레코드와 연관된 모든 필드가 표시됩니다.

* 미리보기 또는 세부 정보 페이지에서 레코드에 대한 새 필드를 추가할 수 없습니다. 미리 보기 및 세부 정보 페이지에 표시하려면 테이블 보기에서 새 필드를 추가해야 합니다.

* 레코드 미리 보기 또는 세부 정보 페이지에 섹션을 추가하여 일반적인 기준별로 정보를 구성하고 쉽게 찾을 수 있습니다.

* 다음 변경 사항은 동일한 유형의 모든 레코드에 영향을 미치며 해당 레코드에 액세스하는 모든 사용자가 볼 수 있습니다.

   * 필드 재정렬
   * 섹션 추가 또는 제거

* 레코드 미리 보기에서 변경한 내용은 레코드 세부 정보 페이지에 즉시 표시됩니다. 레코드 페이지에서 변경한 내용은 레코드 미리 보기 상자도 볼 수 있습니다.

* 레코드에 표지 이미지 또는 썸네일을 추가하는 것은 레코드 미리 보기 또는 페이지의 전체 레이아웃의 일부가 아닙니다. 각 레코드에 고유한 표지 이미지 또는 썸네일을 추가할 수 있습니다. 자세한 내용은 [레코드에 표지 이미지 추가](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) 및 [레코드에 썸네일 추가](/help/quicksilver/planning/records/add-thumbnails-to-records.md)를 참조하십시오.

## 레코드 미리 보기 또는 페이지에 섹션 추가

레코드 페이지에 섹션을 추가할 때 다음 사항을 고려하십시오.

* 페이지에 포함할 수 있는 섹션 수에는 제한이 없습니다.
* 빈 섹션은 가질 수 없습니다. 섹션에 하나 이상의 필드가 있어야 합니다.
* 한 섹션에서 다른 섹션으로 필드를 끌어다 놓을 수 있습니다. 자세한 내용은 이 문서의 [레코드 미리 보기 또는 세부 정보 페이지에서 필드 다시 정렬](#rearrange-fields-in-the-record-preview-or-details-page) 섹션을 참조하십시오.
* 섹션에서 모든 필드를 제거하면 섹션이 자동으로 삭제되어 복구할 수 없습니다.

레코드 미리 보기 또는 페이지에 섹션을 추가하려면 다음 작업을 수행하십시오.

{{step1-to-planning}}

1. 작업 영역의 카드를 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.

1. 모든 유형의 보기에서 레코드 이름을 클릭합니다

   또는

   테이블 테이블 보기에서 첫 번째 열의 **세부 정보 열기** 아이콘 ![](assets/open-details-icon-in-table-name-field.png)을(를) 클릭합니다.

   레코드의 미리보기가 보기에서 열립니다.

   ![](assets/details-box.png)

1. (선택 사항) 레코드 미리 보기의 오른쪽 상단에 있는 **새 탭에서 열기** 아이콘 ![](assets/open-details-in-a-new-tab-icon.png)을(를) 클릭하여 새 탭에서 레코드 페이지를 엽니다.

   레코드 페이지가 열립니다.

   ![](assets/details-page.png)

1. 레코드 미리 보기 또는 페이지에서 필드 왼쪽의 공백 위로 마우스를 가져간 다음 **섹션 추가** 아이콘 ![](assets/add-section-icon.png)을(를) 클릭하여 섹션을 추가합니다.
1. 섹션 이름 내부를 클릭하고 **제목 없는 섹션**&#x200B;을(를) 이름으로 바꾼 다음 Enter를 클릭합니다. 섹션 아래에 표시되는 필드는 자동으로 새 섹션의 일부입니다.
1. 이 문서의 [레코드 미리 보기 또는 세부 정보 페이지에서 필드 다시 정렬](#rearrange-fields-in-the-record-preview-or-details-page) 섹션에 설명된 대로 필드를 새 섹션으로 끌어다 놓습니다.

1. (선택 사항) 섹션 이름 위에 마우스를 놓고 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭합니다.

   ![](assets/more-menu-options-for-section-on-record-page.png)
1. (선택 사항) 다음 중 하나를 수행하여 섹션을 편집합니다.

   * 섹션 이름을 변경하려면 **이름 바꾸기**&#x200B;를 클릭하십시오.

     >[!TIP]
     >
     > 이름을 클릭하여 섹션의 이름을 인라인으로 바꿀 수 있습니다.

   * 섹션을 한 위치 위로 이동하려면 **위로 이동**&#x200B;을 클릭하십시오.

     또는

     섹션을 한 위치 아래로 이동하려면 **아래로 이동**을 클릭합니다.
섹션의 모든 필드가 섹션과 함께 이동합니다.

   * 섹션을 삭제하려면 **삭제**&#x200B;를 클릭하십시오. 섹션이 삭제되어 복구할 수 없습니다. 이 유형의 레코드에 액세스하는 모든 사용자가 더 이상 삭제된 섹션을 볼 수 없습니다.

1. 섹션 이름의 왼쪽에 있는 아래쪽 방향 화살표를 클릭하여 축소하거나 오른쪽 방향 화살표를 클릭하여 확장합니다.
기본적으로 모든 섹션이 확장되어 있습니다.

1. (선택 사항) 섹션 이름의 왼쪽에 있는 **grab** 아이콘 ![](assets/grab-icon.png)을(를) 클릭한 다음 원하는 위치에 끌어다 놓습니다.

   새 섹션 위치는 레코드를 보는 모든 사용자에 대해 동일한 유형의 모든 레코드의 미리보기 및 페이지에서 모두 업데이트됩니다.

   섹션과 필드 순서에 대한 모든 변경 사항은 자동으로 저장됩니다.

## 레코드 미리 보기 또는 세부 정보 페이지에서 필드 다시 정렬

{{step1-to-planning}}

1. 작업 영역의 카드를 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.

1. 모든 유형의 보기에서 레코드 이름을 클릭합니다

   또는

   테이블 테이블 보기에서 첫 번째 열의 **세부 정보 열기** 아이콘 ![](assets/open-details-icon-in-table-name-field.png)을(를) 클릭합니다.

   레코드의 미리보기가 보기에서 열립니다.

   ![](assets/details-box.png)

1. (선택 사항) 레코드 미리 보기의 오른쪽 상단에 있는 **새 탭에서 열기** 아이콘 ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it-->을(를) 클릭하여 새 탭에서 레코드 페이지를 엽니다.

   레코드 페이지가 열립니다.

   ![](assets/details-page.png)

1. 레코드 미리 보기 또는 페이지에서 필드 이름 왼쪽에 있는 **grab** 아이콘 ![](assets/grab-icon.png)을(를) 클릭한 다음 원하는 위치에 끌어다 놓습니다. <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   필드의 새 위치는 레코드를 보는 모든 사용자에 대해 동일한 유형의 모든 레코드의 미리보기 및 페이지에서 모두 업데이트됩니다.

   레코드 미리 보기 또는 페이지의 레이아웃에 대한 모든 변경 사항이 자동으로 저장됩니다.

