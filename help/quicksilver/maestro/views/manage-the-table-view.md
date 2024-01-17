---
title: 표 보기 관리
description: Adobe Maestro의 레코드 유형 페이지에 액세스할 때 테이블 보기에서 레코드와 해당 필드를 표시할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 0dd723b5-d674-4626-8fc2-7da41f3b7f35
source-git-commit: 5f3d5c93c2fc721dda2dd04adac22190ef6a3f29
workflow-type: tm+mt
source-wordcount: '2316'
ht-degree: 3%

---

# 표 보기 관리

<!--
title: Manage the table view
description: You can display records in a table view when using Adobe Maestro. 
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>이 문서의 정보는 Adobe Workfront의 새로운 오퍼링인 Adobe Maestro를 참조합니다.
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 베타 프로그램의 일부입니다. Maestro 기능을 사용하려면 Workfront 고객이어야 합니다.
>
>Maestro용 Beta 프로그램 가입에 대한 자세한 내용은 계정 담당자에게 문의하십시오.
>
>자세한 내용은 [Adobe 마에스트로 개요](../maestro-overview.md).

Adobe Maestro의 레코드 유형 페이지에 액세스할 때 테이블 보기에서 레코드와 해당 필드를 표시할 수 있습니다.

Maestro 보기 및 관리 방법에 대한 자세한 내용은 다음을 참조하십시오. [레코드 보기 관리](../views/manage-record-views.md).

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
<p>Adobe Maestro Closed Beta 프로그램에 조직을 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>임의</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td>
   <td>
   <p>임의</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">액세스 수준 구성</td>
   <td> <p>Maestro에 대한 액세스 수준 제어 없음 </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>보기에 대한 권한 관리</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">레이아웃 템플릿</td>
   <td> <p>시스템 관리자가 레이아웃 템플릿에 마에스트로 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## 표 보기 관리 {#manage-a-table-view}

<!--insert screen shot of table view-->

테이블 뷰를 만들 때 선택한 유형의 모든 레코드가 테이블에 표시됩니다. 각 행은 고유한 레코드이며 각 열은 레코드 필드입니다. 기본적으로 모든 필드와 모든 레코드가 표시됩니다.

테이블 뷰를 관리하려면 다음을 수행합니다.

1. 문서에 설명된 대로 표 보기 만들기 [레코드 보기 관리](../views/manage-record-views.md).

   ![](assets/table-view-example.png)

1. 아래 하위 섹션에 설명된 대로 다음 보기 요소를 업데이트합니다.
   * [열(또는 필드)](#add-columns-or-fields)
   * [행(또는 레코드)](#add-rows-or-records)
   * [필터](#add-filters)
   * [그룹화](#add-groupings)
   * [정렬](#sort-information)


### 열(또는 필드) 추가 {#add-columns}

Maestro 테이블 보기의 열 헤더에는 보기의 레코드와 관련된 필드가 표시됩니다. 표 보기에 표시된 동일한 필드가 Maestro 레코드의 세부 정보 섹션에도 표시됩니다. 자세한 내용은 [레코드 편집](../records/edit-records.md).

<!--this is not available yet:You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default.-->

보기에 열을 추가하는 것은 레코드 유형에 필드를 추가하는 것과 같습니다.

테이블 보기에서 최대 500개의 필드(또는 열)를 추가할 수 있습니다.

1. 레코드 유형 페이지로 이동하여 **표** 보기 드롭다운 메뉴에서 보기
1. 문서에 설명된 대로 필드(또는 열) 추가 시작 [필드 만들기](../fields/create-fields.md).

   추가한 열은 레코드 유형에 액세스하는 모든 사용자가 볼 수 있으며 선택한 레코드 유형의 레코드에 대한 세부 정보 페이지에서 새 필드로 추가됩니다.

1. 다음 중 하나를 수행하여 테이블의 열 순서를 변경합니다.

   * 열 머리글을 잡고 원하는 위치에 끌어서 놓습니다. 테이블을 다시 조정할 때까지 이동한 열이 파란색 배경에 잠시 표시됩니다.

   * 클릭 **필드** 테이블의 도구 모음에서 필드를 원하는 순서로 드래그 앤 드롭한 다음, **필드 가시성 및 순서** 상자를 닫으십시오.

     ![](assets/fields-setting-table-view-toolbar-expanded.png)


     >[!TIP]
     >
     >* 이름 필드는 기본적으로 항상 테이블 보기의 첫 번째 필드입니다. 이는 기본 필드로 간주됩니다.
     >
     >* 다른 필드를 기본 필드로 지정하지 않는 한 이름 필드를 다른 위치로 이동할 수 없습니다. 자세한 내용을 보려면 4단계를 계속 진행하십시오. <!--accurate?-->
     >
     >* 기본 필드는 숨기거나 삭제할 수 없습니다.
     >
     >* 기본 필드가 고정되어 있고 가로 스크롤의 일부가 아닙니다.

   * 기본 필드를 변경하여 첫 번째 열의 필드를 다른 필드로 바꿉니다. 자세한 내용을 보려면 4단계를 계속 진행하십시오. <!--accurate?-->

1. (선택 사항) 테이블의 첫 번째 열에 표시되지 않는 필드의 열 헤더에 있는 필드 이름을 마우스로 가리키고 필드 이름의 오른쪽에 있는 아래쪽 방향 화살표를 클릭한 다음 를 클릭합니다 **기본 필드로 설정**.

   ![](assets/set-as-primary-field-option-table-view.png)

1. 클릭 **필드 설정** 확인할 수 있습니다.

   필드는 기본 필드가 되어 테이블 보기의 첫 번째 열로 표시됩니다. 이전 기본 필드가 두 번째 열로 이동합니다.

   >[!NOTE]
   >
   >   * 다음 유형의 필드만 기본 필드가 될 수 있습니다.
   >
   >       * 한 줄 텍스트
   >       * 숫자
   >       * 공식
   >
   >   * 기본 필드는 항상 고정되어 있으므로 이동할 수 없습니다. 기본 필드를 다른 위치로 이동해야 하는 경우 다른 필드를 선택하여 기본 필드를 대체할 수 있습니다.
   >
   >   * 테이블 보기의 기본 필드를 변경하면 기본 필드를 선택하는 다른 모든 사용자의 보기에 영향을 줍니다.
   >
   >   * 테이블 보기에서 기본 필드를 변경하면 모든 테이블 보기에 영향을 줍니다.
   >
   >   * 기본 필드는 삭제하거나 숨길 수 없습니다.

1. 열 구분선을 클릭하고 드래그하여 원하는 위치에 놓아 열의 너비를 늘립니다.

   >[!TIP]
   >
   >열 너비 및 순서에 대한 변경 사항은 영구적이며 레코드 유형에 액세스하는 모든 사용자에게 표시됩니다.

1. 열 머리글 위로 마우스를 가져간 다음 아래쪽을 가리키는 화살표를 클릭하고 **필드 숨기기**

   또는

   클릭 **필드** 테이블 도구 모음에서 를 클릭하고 숨길 필드(또는 열)와 관련된 토글을 비활성화합니다. 다음 **필드 가시성 및 순서** 상자가 표시됩니다.

   >[!TIP]
   >
   >도구 모음의 필드 아이콘 왼쪽에 숨겨진 필드 수가 표시됩니다.


1. 다음을 클릭합니다. **필드** 아이콘을 클릭하고 테이블의 열에 표시할 필드와 관련된 토글을 활성화합니다. 기본적으로 모든 필드가 표시됩니다.

1. 키워드와 일치하는 레코드를 빠르게 찾으려면 다음을 수행하십시오.

   1. 다음을 클릭합니다. **검색** 아이콘 ![](assets/search-icon.png) 화면에 표시되는 레코드의 필드와 연결된 키워드를 입력하십시오. 검색 항목 옆에 올바른 일치 항목 수가 표시되고 올바른 일치 항목이 있는 필드가 강조 표시됩니다.

      ![](assets/search-box-with-results-blue-outline-table-view.png)

      화면에 표시되는 모든 단어 또는 특수 문자를 사용할 수 있습니다.

      테이블 보기에서 숨겨진 필드와 연결된 키워드는 사용할 수 없습니다.

   1. 누르기 **입력** 키보드에서 다음 찾은 필드로 이동합니다.

   1. (선택 사항) 일치 항목이 두 개 이상 있는 경우 검색 키워드 오른쪽에 있는 위쪽 및 아래쪽 화살표를 클릭하여 테이블에서 모든 일치 항목을 찾습니다.

   1. 다음을 클릭합니다. **x** 아이콘을 클릭하여 검색 키워드를 지웁니다.


### 행(또는 레코드) 추가 {#add-rows}

Maestro 테이블 보기의 행에는 선택한 레코드 유형의 개별 레코드가 표시됩니다.

Maestro에서 레코드 유형에 대해 최대 10,000개의 레코드(또는 행)를 가질 수 있습니다.

1. 레코드 유형 페이지로 이동하여 **표** 보기 드롭다운 메뉴에서 보기
1. 문서에 설명된 대로 레코드(또는 행) 추가를 시작합니다 [레코드 만들기](../records/create-records.md).

   테이블 보기에서 추가하는 레코드는 즉시 저장되며 작업 공간에 대한 보기 이상의 권한이 있는 모든 사용자에게 표시됩니다.

1. (선택 사항) 한 행에서 하나 이상의 레코드를 선택한 다음 **핸들** 아이콘 ![](assets/handle-icon.png) 레코드 이름 왼쪽에 행 순서를 변경합니다.

   >[!NOTE]
   >
   >테이블 뷰에 정렬을 하나 이상 적용하면 행 순서를 재정렬할 수 없습니다.

   <!-- this is not possible right now:

    1. To reorder the rows, click the row header, drag and drop it in the desired location. 

        The changes you make to the row order are permanent and visible to all users who access the record type
    -->

### 필터 추가 {#add-filters}

<!-- this section links from the timeline view; consider splitting them if they become different-->

필터는 화면에 표시되는 정보의 양을 줄이는 데 도움이 됩니다.

표 보기에서 필터를 사용하여 작업할 때는 다음 사항을 고려하십시오.
<!-- this list is almost identical to the one for the table view - update both-->

* 테이블 보기에 대해 만든 필터는 동일한 레코드 유형에 적용될 때 타임라인 보기의 필터와는 독립적으로 작동합니다.

* 필터는 사용자가 선택한 보기에 고유합니다. 동일한 레코드 종류의 두 테이블 보기에는 서로 다른 필터가 적용될 수 있습니다. 동일한 테이블 보기를 보는 두 명의 사용자에게 현재 적용된 동일한 필터가 표시됩니다.

* 테이블 보기에 빌드하고 적용하는 필터의 이름을 지정할 수 없습니다.

* 필터를 제거하면 사용자와 동일한 레코드 유형에 액세스하는 모든 사람에서 필터가 제거되며 사용하는 것과 동일한 보기를 사용합니다.

* 테이블 보기에 필터를 추가하는 것은 타임라인 보기에 필터를 추가하는 것과 같습니다.

테이블 보기에 필터를 추가하려면 다음 작업을 수행하십시오.

1. 문서에 설명된 대로 레코드 유형 페이지에 대한 테이블 보기를 만듭니다 [레코드 보기 관리](../views/manage-record-views.md).
1. 테이블 뷰를 선택한 다음 **필터** 테이블 오른쪽 위 모서리에서 참조할 수 있습니다.
1. 클릭 **조건 추가** 다음 정보를 추가합니다.

   * 필터링 기준으로 사용할 필드 선택 <!-- the tip below might change-->

   * 옵션(또는 필터 수정자)을 선택하여 필드가 충족해야 하는 조건 종류를 정의합니다

     아래 표에는 각 필드 유형에 사용할 수 있는 수정자가 표시됩니다.

     >[!TIP]
     >
     > 연결된 필드는 선택할 수 없습니다. 자세한 내용은 [필드 만들기](../fields/create-fields.md).

     <table>
        <thead>
        <tr>
            <th><b>필드 유형</b></th>
            <th><b>수정자</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>한 줄, 단락, 공식 </td>
            <td><p>다음을 포함함</p>
            <p>다음을 포함하지 않음</p>
            <p>다음과 같음</p>
            <p>다음이 아님</p>
            <p>비어 있음</p>
            <p>비어 있지 않음</p></td>
        </tr>
        <tr><td>단일 선택</td>
            <td><p>다음과 같음</p>
            <p>다음이 아님</p>
            <p>다음 중 하나</p>
            <p>다음에 해당하지 않음</p>
            <p>비어 있음</p>
            <p>비어 있지 않음</p></td>
        </tr>
        <tr>
            <td>다중 선택, 사람</td>
            <td><p>다음 중 하나 포함</p>
            <p>다음을 모두 포함</p>
            <p>정확함</p>
            <p>다음 중 어느 것도 포함하지 않음</p>
            <p>비어 있음</p>
            <p>비어 있지 않음</p></td>
        </tr>
        <tr>
            <td>숫자, 백분율, 통화</td>
            <td><p>=</p>
            <p>≠</p>
            <p> &lt; </p>
            <p>&gt;</p>
            <p>≤</p>
            <p>≥</p>
            <p>비어 있음</p>
            <p>비어 있지 않음</p></td>
        </tr>
        <tr>
            <td>일자</td>
            <td><p>다음과 같음</p>
            <p>다음이 아님</p>
            <p>다음 이후</p>
            <p>다음 이전</p>
            <p>다음 사이에 있음</p><p>다음 사이에 없음</p>
            <p>비어 있음</p><p>비어 있지 않음</p></td>
        </tr>

     <tr>
            <td>확인란</td>
            <td><p>다음과 같음</p>
        </tr>
        </tbody>
        </table>

   * 선택한 필드의 값을 선택합니다.

   ![](assets/filter-ui-table-view.png)

   추가할 수 있는 필터링 조건 수에는 제한이 없습니다.

1. (선택 사항) **조건 추가** 다른 필터링 옵션을 추가하고 위의 단계를 반복합니다. 적용된 필터 수는 필터 아이콘 왼쪽에 표시됩니다.
1. 다음 연산자를 클릭하여 필터 조건이 조인되고 적용되어야 하는 방식을 나타냅니다.

   * **및**: 지정된 모든 조건이 충족되어야 합니다.
   * **또는**: 지정된 조건을 모두 충족해야 합니다. 기본 옵션입니다.

   레코드 목록은 자동으로 필터링됩니다.  <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. (선택 사항) **필터**&#x200B;을(를) 클릭하고 **x** 아이콘을 클릭하여 필터를 제거합니다. <!--right now you cannot "clear all" for filters, but this might come later-->

### 그룹화 추가 {#add-groupings}

<!--this section exists in the timeline view too, but the display is slightly different, so I kept both steps; consider updating both sections if any updates to groupings are introduced-->

보기에 그룹화를 적용할 때 유사한 정보별로 레코드를 그룹화할 수 있습니다.

표 보기에서 그룹화를 추가하는 것은 타임라인 보기에 그룹화를 추가하는 것과 비슷합니다.

다음 사항을 고려하십시오.

* 표 및 타임라인 보기에서 그룹화를 적용할 수 있습니다. 테이블 보기의 그룹화는 동일한 레코드 유형의 타임라인 보기의 그룹화와는 독립적입니다.
* Maestro 보기에서 3가지 수준의 그룹화를 적용할 수 있습니다. 선택한 그룹화 순서대로 레코드가 그룹화됩니다.
&lt;!—* API를 사용할 때 최대 4가지 수준의 그룹화를 적용할 수 있습니다. —현재 이 항목을 확인하고 있습니다—>
* 그룹화는 선택하는 보기에 대해 고유합니다. 동일한 레코드 종류의 두 테이블 보기에는 서로 다른 그룹화가 적용될 수 있습니다. 동일한 테이블 보기를 보는 두 명의 사용자에게 현재 적용된 동일한 그룹화가 표시됩니다.
* 테이블 보기에 대해 빌드하는 그룹화의 이름을 지정할 수 없습니다.
* 그룹화를 제거하면 사용자와 동일한 레코드 유형에 액세스하거나 사용자와 동일한 보기를 표시하는 모든 사용자에게서 그룹화가 제거됩니다.
* 그룹화 아래에 나열된 레코드를 편집할 수 있습니다.
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

그룹화를 추가하려면:

1. 문서에 설명된 대로 레코드 유형에 대한 타임라인 보기를 만듭니다 [레코드 보기 관리](../views/manage-record-views.md).
1. 클릭 **그룹화** 을 클릭합니다.

   ![](assets/grouping-ui-table-view.png)

1. 제안된 필드 중 하나를 클릭하거나 **다른 필드 선택**&#x200B;에서 다른 필드를 검색한 다음 목록에 표시되면 해당 필드를 클릭합니다.

   >[!TIP]
   >
   >연결된 필드는 선택할 수 없습니다.

   그룹화가 테이블에 자동으로 적용되며 그룹화 구분선 아래에 레코드가 표시됩니다

1. (선택 사항) 위의 단계를 반복하여 최대 3개의 그룹화를 추가합니다.

   그룹화를 위해 선택한 필드 수가 그룹화 아이콘 옆에 표시됩니다.

   ![](assets/grouping-applied-in-table-view.png)

1. (선택 사항) **레코드 그룹화 기준** 상자를 클릭하고 **x** 그룹화를 제거하기 위해 선택한 필드 오른쪽의 아이콘

   또는

   클릭 **모두 지우기** 모든 필드를 제거합니다.

1. 바깥쪽을 클릭합니다. **레코드 그룹화 기준** 상자를 닫으십시오.
1. (선택 사항) **+ 신규 &lt; 레코드 유형 이름 >** 그룹화가 끝날 때 새 레코드를 추가한 다음 페이지를 새로 고쳐 새 레코드를 적절한 그룹화에 추가합니다. <!--this might need to be changed when they add the Refresh button on the toolbar of the table view-->

### 정렬 추가 {#sort-information}

정렬을 적용하여 주어진 순서로 정보를 구성할 수 있습니다.

다음 정보를 정렬할 수 있습니다.

* 테이블 보기의 모든 레코드. <!--or timeline view. ***********verify this is the case for the timeline view*********************-->
  <!--* All groupings. - this is not available yet-->

표 보기에서 레코드를 정렬할 때는 다음 사항을 고려하십시오.

<!-- if this is available for the timeline view, update both when you update one-->

* 정렬은 선택하는 보기에 고유합니다. 동일한 레코드 종류의 두 테이블 보기에는 서로 다른 정렬 기준이 적용될 수 있습니다. 동일한 테이블 보기를 보는 두 명의 사용자에게 현재 적용된 동일한 정렬이 표시됩니다.

* 작성하여 테이블 보기에 적용하는 정렬 이름은 지정할 수 없습니다.

* 정렬은 이동할 때 유지됩니다.

* 레코드 유형의 테이블 보기에 표시되는 수만큼 필드를 정렬할 수 있습니다.

* 정렬 기준을 제거하면 사용자와 동일한 레코드 유형에 액세스하는 모든 사람에서 정렬 기준이 제거되며 사용하는 것과 동일한 보기를 사용합니다.

정렬하려면 <!--ungrouped (add this when sorting for groupings will be available--> 레코드, 다음을 수행합니다.

1. 문서에 설명된 대로 표 보기 만들기 [레코드 보기 관리](../views/manage-record-views.md).
1. 다음을 클릭합니다. **정렬** 아이콘 ![](assets/sort-icon.png) 표의 오른쪽 위 모서리

   또는

   테이블 보기에서 열 이름 위로 마우스를 가져간 후 열 헤더 이름 오른쪽에 있는 아래쪽 화살표를 클릭한 다음 을 클릭합니다 **이 필드별로 정렬**. 필드는 표 보기의 오른쪽 위 모서리에 있는 정렬 아이콘에서 정렬 선택 항목으로 추가됩니다.
1. 다음에서 **레코드 정렬 기준** 상자를 클릭하고 추천 필드 중 하나를 클릭하거나 **다른 필드 선택** 다른 필드를 검색하여 목록에 표시되면 클릭합니다.

   정렬은 테이블 보기에 자동으로 적용되며 선택한 기준에 따라 정렬된 레코드가 표시됩니다.

   <!-- add a step that you can rearrange the sorting fields here, when this will be possible-->

1. (선택 사항) 추가 필드를 기준으로 정렬하려면 위의 단계를 반복합니다.

   정렬하려는 필드 수는 도구 모음의 오른쪽 위 모서리에 있는 정렬 아이콘 왼쪽에 표시됩니다. 테이블 뷰의 열에 표시되는 필드만 선택할 수 있습니다.

   >[!TIP]
   >
   > 연결된 필드는 선택할 수 없습니다. 자세한 내용은 [필드 만들기](../fields/create-fields.md).

1. (선택 사항) **레코드 정렬 기준** 상자를 클릭하고 **x** 정렬을 제거할 정렬 필드 오른쪽의 아이콘

   또는

   클릭 **모두 지우기** 정렬에서 모든 필드를 제거합니다.

1. 바깥쪽을 클릭합니다. **레코드 정렬 기준** 상자를 닫으십시오.

   ![](assets/sorting-in-table-view.png)

   표에 표시된 정보는 선택한 기준에 따라 정렬됩니다.

   정렬하기 위해 선택한 필드에는 정렬 아이콘이 표시되고 그 뒤에 정렬이 적용되는 순서를 나타내는 숫자가 표시됩니다.

<!-- this is not available yet: 

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. ************************* add steps here for sorting grouped records****************

-->
