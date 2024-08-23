---
title: 타임라인 보기 관리
description: Adobe Workfront Planning 레코드 유형 페이지의 타임라인 보기에서 레코드에 액세스하고 편집합니다. 필터, 그룹화 및 설정을 사용하여 타임라인을 사용자 지정합니다. 분류 기능을 사용하여 연결된 레코드를 표시합니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: 61cad7dc76ba04ea84ff0bd5052182f040f7b4d9
workflow-type: tm+mt
source-wordcount: '2636'
ht-degree: 0%

---

# 타임라인 보기 관리

<!--
title: Manage the timeline view 
description: You can display records in a timeline view, when accessing the record type page in Adobe Workfront Planning. 
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Adobe Workfront Planning의 레코드 유형 페이지에 액세스할 때 타임라인 보기에 레코드를 표시할 수 있습니다.

레코드 보기에 대한 자세한 내용은 [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md)를 참조하십시오.

## 액세스 요구 사항

<!--Updated for GA-->

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront 계획<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 플랜*</p></td> 
   <td> 
<p>다음 Workfront 플랜 중 하나:</p> 
<ul><li>선택</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다.</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 계획 계획*</p></td> 
   <td> 
<p>임의 </p> 
<p>각 Workfront 계획 계획에 포함된 내용에 대한 자세한 내용은 <a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront 가격 및 패키징</a>을 참조하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning의 모든 기능에 액세스할 수 있으려면 조직의 Workfront 인스턴스가 통합 경험 Adobe에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 통합 경험 Adobe</a>를 참조하십시오. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
   <td> <ul><li><p>임의, Workfront Planning 정보를 보려면</p></li>
   <li><p>표준, 작업 공간 만들기</p></li></ul>
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>보기에 대한 권한 관리</p>  
   <p>보기 설정을 일시적으로 변경하기 위해 보기에 대한 이상의 권한을 봅니다.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>레이아웃 템플릿</p></td> 
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

<!--OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->

+++

## 타임라인 보기 관리 {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

타임라인 보기를 만들 때 선택한 레코드 유형의 모든 레코드가 시간 순서대로 표시됩니다.

다음 사항을 고려하십시오.

* 레코드 유형과 연결된 날짜 필드가 두 개 이상 있는 경우에만 타임라인 보기를 만들 수 있습니다. 레코드 유형과 연관된 날짜 필드가 하나 또는 하나도 없으면 타임라인 보기 옵션이 흐리게 표시됩니다.

  타임라인 보기를 작성할 때 다음 날짜 필드 중에서 선택할 수 있습니다.

   * 날짜 기록
   * 시스템 생성 필드 기록: 생성 날짜, 마지막 수정 날짜
   * 연결된 레코드 또는 개체 유형에서 날짜를 조회합니다.
* 레코드와 연결된 날짜에 따라 다음 시나리오에서 일부 레코드가 타임라인 보기에 표시되지 않을 수 있습니다.

   * 시작 및 종료 날짜에 값이 없는 경우
   * 시작 또는 종료 날짜에 값이 없는 경우
   * 시작 일자가 종료 일자 이후인 경우

타임라인 보기를 관리하려면 다음을 수행합니다.

1. 타임라인을 보려는 레코드 유형 페이지로 이동합니다.
1. [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md) 문서에 설명된 대로 타임라인 보기를 만듭니다.

   ![](assets/timeline-view-example.png)

   선택한 레코드 유형과 연관된 레코드는 타임라인에 막대로 표시되며 기본적으로 시작 날짜의 시간순으로 정렬됩니다.

   >[!TIP]
   >
   >    타임라인에서 레코드 정렬이 약식 보기에 표시되지 않습니다.

1. (선택 사항 및 조건부) 레코드 이름이 잘리면 레코드 막대 위로 마우스를 가져가 레코드의 전체 이름 및 추가 정보를 표시합니다.

1. 다음 중 하나를 수행하여 타임라인을 탐색합니다.

   * 왼쪽 및 오른쪽 아이콘을 클릭하거나 가로 스크롤을 사용하여 타임라인에서 앞뒤로 이동합니다. 페이지를 새로 고치면 선택한 시간대가 유지됩니다.
   * 타임라인을 오늘 날짜로 맞추려면 **오늘**&#x200B;을 클릭하세요.
   * 시간 증분을 업데이트하려면 시간대 드롭다운 메뉴에서 다음 옵션 중 하나를 선택합니다.

      * 년
      * 분기
      * 월
1. **표준 보기로 전환** 보기를 클릭하여 레코드를 별도의 줄로 표시합니다. <!--check to see if they updated the name of the setting here-->

   또는

   날짜가 같은 줄에 겹치지 않는 레코드를 표시하려면 **작게 보기로 전환**&#x200B;을 클릭합니다. <!--check to see if they updated the name of the setting here-->

   레코드는 기본적으로 작게 보기에 표시됩니다.

1. 키워드와 일치하는 레코드를 빠르게 찾으려면 다음을 수행하십시오.

   1. **검색** 아이콘 ![](assets/search-icon.png)을(를) 클릭하고 화면에 표시되는 레코드의 필드와 관련된 키워드를 입력하십시오. 검색 항목 옆에 올바른 일치 수가 표시되고 올바른 일치 항목이 있는 레코드가 강조 표시됩니다.

      ![](assets/search-box-and-results-timeline-view.png)

      화면에 표시되는 모든 단어 또는 특수 문자를 사용할 수 있습니다.

      타임라인 보기에 표시되지 않는 필드와 연결된 키워드는 사용할 수 없습니다.

   1. 키보드에서 Enter 키를 눌러 다음 찾은 필드로 이동합니다.
   1. (선택 사항) 일치 항목이 두 개 이상 있는 경우 검색 키워드 오른쪽에 있는 위쪽 및 아래쪽 화살표를 클릭하여 테이블에서 모든 일치 항목을 찾습니다.
   1. 검색 키워드를 지우려면 검색 상자에서 **x** 아이콘을 클릭합니다.

1. 아래 하위 섹션에 설명된 대로 다음 보기 요소를 업데이트합니다.
   * [필터](#add-filters)
   * [그룹화](#add-grouping)
   * [설정](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not yet in timeline; also check the anchor and make sure it's correct-->

1. (선택 사항) 타임라인에 연결된 레코드를 표시하려면 **분류**&#x200B;를 클릭합니다.

   자세한 내용은 [분류 기능을 사용하여 연결된 레코드를 타임라인 보기로 표시](#break-down-connected-records-in-the-timeline-view) 섹션을 참조하십시오.

### 필터 추가

필터를 사용하여 화면에 표시되는 정보의 양을 줄일 수 있습니다.

타임라인 보기에서 필터를 사용하여 작업할 때는 다음 사항을 고려하십시오.

<!-- this list is almost identical to the one for the table view - update both-->

* 타임라인 보기에 대해 만드는 필터는 동일한 레코드 유형에 적용되는 다른 보기의 필터와는 독립적으로 작동합니다.

* 필터는 사용자가 선택한 보기에 고유합니다. 동일한 레코드 종류의 두 타임라인 보기에는 서로 다른 필터가 적용될 수 있습니다.

* 동일한 타임라인 보기를 보는 두 명의 사용자에게 현재 적용된 동일한 필터가 표시됩니다.

* 타임라인 보기를 위해 빌드하는 필터의 이름을 지정할 수 없습니다.

* 필터를 제거하면 사용자와 동일한 레코드 종류에 액세스하고 사용자와 동일한 보기를 표시하는 모든 사용자에서 필터가 제거됩니다.

* 타임라인 보기에서 필터를 추가하는 것은 테이블 보기에서 필터를 추가하는 것과 동일합니다.

  자세한 내용은 문서 [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)의 &quot;필터 추가&quot; 섹션을 참조하십시오.

* 연결된 레코드 필드 또는 조회 필드를 기준으로 필터링할 수 있습니다.
* 여러 값을 표시하는 조회 필드를 기준으로 필터링할 수 있습니다.


### 그룹화 추가

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

보기에 그룹화를 적용할 때 유사한 정보별로 레코드를 그룹화할 수 있습니다.

타임라인 보기에서 그룹화를 추가하는 것은 테이블 보기에 그룹화를 추가하는 것과 비슷합니다.

타임라인 보기에서 그룹화를 사용하여 작업할 때 다음 사항을 고려하십시오.

* 표 및 타임라인 보기에서 그룹화를 적용할 수 있습니다. 테이블 보기의 그룹화는 동일한 레코드 유형의 타임라인 보기의 그룹화와는 독립적입니다.
* 보기에서 3가지 수준의 그룹화를 적용할 수 있습니다. 선택한 그룹화 순서대로 레코드가 그룹화됩니다.
&lt;!—* API를 사용할 때 최대 4가지 수준의 그룹화를 적용할 수 있습니다. —현재 이 항목을 확인하고 있습니다—>
* 그룹화는 선택하는 보기에 대해 고유합니다. 동일한 레코드 종류의 두 테이블 보기에는 서로 다른 그룹화가 적용될 수 있습니다. 동일한 테이블 보기를 보는 두 명의 사용자에게 현재 적용된 동일한 그룹화가 표시됩니다.
* 테이블 보기에 대해 빌드하는 그룹화의 이름을 지정할 수 없습니다.
* 그룹화를 제거하면 사용자와 동일한 레코드 유형에 액세스하거나 사용자와 동일한 보기를 표시하는 모든 사용자에게서 그룹화가 제거됩니다.
* 그룹화 아래에 나열된 레코드를 편집할 수 있습니다.
* 연결된 레코드 필드 또는 조회 필드를 기준으로 그룹화할 수 있습니다.
* 집계자가 요약하지 않은 여러 값이 있는 조회 필드를 기준으로 그룹화하면, 레코드는 각 필드 값의 고유한 조합으로 그룹화됩니다.
* 현재 레코드 유형에서 최대 4개 수준까지 떨어진 필드를 참조할 수 있습니다. 예를 들어, 활동 레코드 유형에 대한 그룹화를 만드는 중에 활동이 Workfront 프로젝트에 연결된 캠페인 레코드 유형에 연결된 제품 레코드 유형에 연결된 경우, 활동 레코드 유형에 대해 만들고 있는 그룹화에서 프로젝트의 상태를 참조할 수 있습니다.
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

타임라인 보기에서 그룹화를 추가하려면 다음을 수행합니다.

1. [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md) 문서에 설명된 대로 레코드 유형에 대한 타임라인 보기를 만듭니다.
1. 타임라인 보기의 오른쪽 상단 모서리에서 **그룹화**&#x200B;을(를) 클릭합니다.

   ![](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. 제안된 필드 중 하나를 클릭하거나 **다른 필드 선택**&#x200B;을 클릭하고 다른 필드를 검색한 다음 목록에 표시될 때 해당 필드를 클릭합니다.

   그룹화는 타임라인에 자동으로 적용되며 그룹화 상자 내에 레코드가 표시됩니다.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (선택 사항) 위의 단계를 반복하여 최대 3개의 그룹화를 추가합니다.

   그룹화를 위해 선택한 필드 수가 그룹화 아이콘 옆에 표시됩니다.

   <!-- update screen shot with view redesign-->

   ![](assets/grouping-applied-in-timeline-view.png)

1. (선택 사항) **레코드 그룹화 기준** 상자 내에서 그룹화를 위해 선택한 필드 오른쪽에 있는 **x** 아이콘을 클릭하여 그룹화를 제거합니다

   또는

   모든 필드를 제거하려면 **모두 지우기**&#x200B;를 클릭하십시오.

1. **레코드 그룹화 기준** 상자 바깥쪽을 클릭하여 닫습니다.
1. (선택 사항) **설정**&#x200B;을 클릭한 다음 **색상**&#x200B;을 클릭하여 색상 코드 그룹화합니다. 자세한 내용은 이 문서의 [타임라인 보기 설정 편집](#edit-the-timeline-view-settings) 섹션을 참조하십시오.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### 타임라인 보기 설정 편집 {#edit-the-timeline-view-settings}

타임라인 보기 설정을 업데이트하여 보기의 타임라인 섹션에 표시되는 정보와 방법을 나타냅니다.

1. [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md) 문서에 설명된 대로 레코드 유형에 대한 타임라인 보기를 만듭니다.
1. **설정**&#x200B;을 클릭합니다.
1. 왼쪽 패널에서 **날짜 및 시간**&#x200B;을 클릭한 다음 타임라인에 표시할 **시작 날짜** 및 **종료 날짜**&#x200B;를 선택하십시오. 기본 시작 및 종료 날짜를 선택하거나 사용 가능한 날짜 필드를 선택할 수 있습니다. 레코드를 나타내는 막대는 시작 날짜에 해당하는 날짜에 시작하여 종료 날짜에 해당하는 날짜에 끝납니다.

   >[!NOTE]
   >
   >시작 또는 종료 날짜에 대한 값이 없거나 시작 날짜가 종료 날짜보다 늦은 레코드는 타임라인 보기에 표시되지 않습니다.

1. 왼쪽 패널에서 **막대 스타일**&#x200B;을 클릭하여 레코드 막대에 표시할 필드를 나타냅니다.

   레코드의 테이블 보기에서 정의된 레코드의 기본 필드(또는 제목)는 기본적으로 선택됩니다. <!--adjust this when the primary field is released??-->

1. (선택 사항 및 조건부) 레코드에 썸네일을 추가한 경우 썸네일 옵션을 선택하여 레코드와 연관된 이미지를 레코드 표시줄에 표시합니다.

   >[!NOTE]
   >
   >    축소판을 타임라인 보기에 표시하려면 먼저 표 보기에 축소판을 추가해야 합니다. 자세한 내용은 [레코드에 썸네일 추가](/help/quicksilver/planning/records/add-thumbnails-to-records.md)를 참조하십시오.

1. 레코드 표시줄에 최대 4개의 필드를 추가하려면 **필드 추가**&#x200B;를 클릭하십시오.
1. **필드 검색** 상자 안을 클릭하고 추가할 필드를 클릭합니다.

   >[!TIP]
   >
   >   * 필드를 레코드 표시줄에 추가하려면 먼저 필드를 만들어야 합니다.
   > 
   >   * 하나 이상의 필드를 선택해야 합니다. 기본적으로 **이름**&#x200B;이(가) 선택되어 있습니다.

   타임라인에서 막대가 어떻게 보이는지에 대한 미리보기가 오른쪽에 표시됩니다.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. 타임라인에서 레코드와 그룹화의 색상을 사용자 지정하려면 왼쪽 패널에서 **색상**&#x200B;을 클릭합니다.

   ![](assets/color-tab-timeline-view.png)

1. (조건부 및 선택 사항) 타임라인 보기에 그룹화를 추가한 경우 **그룹화 색상 설정** 섹션에서 그룹화에 대한 색상을 설정하려면 다음 옵션 중 하나를 선택하십시오.

   * **기본(회색)**: 그룹화의 색상이 회색으로 설정되어 있습니다. 이것이 기본값입니다.
   * **필드 값**: 그룹화의 색상은 그룹화하는 필드의 색과 일치합니다.

     >[!NOTE]
     >
     >    * 색상을 색상으로 구분된 옵션이 있는 필드에만 일치시킬 수 있습니다. 예를 들어 색상을 상태 필드 또는 색상과 연관된 옵션이 있는 필드와 일치시킬 수 있습니다.
     >    
     >    * 연결된 레코드 또는 개체 유형의 조회 필드에 색상을 일치시킬 수 없습니다.


   예를 들어 다중 선택 또는 단일 선택 필드에는 색상으로 구분된 옵션이 있을 수 있습니다.

   색상으로 구분된 옵션이 없는 필드를 기준으로 그룹화하면 그룹화 색상이 회색으로 유지됩니다.

   >[!TIP]
   >
   >타임라인 보기에 그룹화를 추가하지 않은 경우 이 섹션이 표시되지 않습니다.

1. **레코드 색 설정** 섹션에서 다음 옵션 중 하나를 선택하여 레코드의 색을 설정합니다.

   * **레코드 종류**: 레코드 색이 선택한 레코드 종류의 색과 일치합니다. 기본 옵션입니다.
   * **필드 값**: 레코드 색이 지정한 필드 색과 일치합니다. 10단계를 계속합니다. <!--ensure this stays accurate-->
   * **그룹화**: 레코드 색이 그룹화에 지정한 색과 일치합니다. 타임라인 보기에 적용된 그룹화가 없으면 이 옵션은 흐리게 표시됩니다.
   * **없음**: 레코드가 흰색 막대에 표시됩니다.

1. (조건부) 레코드 색으로 **필드 값**&#x200B;을(를) 선택한 경우 **레코드 색과 일치** 드롭다운 메뉴에서 필드를 선택합니다.

   ![](assets/field-selector-drop-down-menu-timeline-view.png)

   색상 코드 옵션이 있는 필드만 드롭다운 메뉴에 표시됩니다.

   예를 들어 다중 선택 또는 단일 선택 필드에는 색상으로 구분된 옵션이 있을 수 있습니다.

   선택한 레코드 유형에 대해 색상으로 구분된 옵션이 있는 필드가 없는 경우 이 옵션은 흐리게 표시됩니다.

1. **저장**&#x200B;을 클릭합니다.

   선택한 사양과 함께 레코드가 타임라인 보기에 표시됩니다.

### 분류 기능을 사용하여 연결된 레코드를 타임라인 보기에 표시합니다

분류 기능을 사용하여 레코드의 타임라인 보기에 연결된 레코드를 표시할 수 있습니다. 레코드와 연결을 분류할 경우 연결된 다른 레코드의 타임라인을 보고 해당 레코드가 성능과 기한에 어떤 영향을 미칠 수 있는지 이해할 수 있습니다.

#### 분류 기능을 사용할 때의 고려 사항

* 타임라인 보기에서 선택한 레코드 유형의 레코드 아래에 연결된 레코드나 개체를 표시할 수 있습니다.
* 분류 기능을 사용하여 타임라인 보기에 다음을 표시할 수 있습니다.
   * 선택한 레코드 유형에 연결된 Workfront Planning 레코드입니다.
   * 선택한 레코드 형식에 연결된 Workfront(************* 또는 AEM Assets *************) 개체 형식입니다.
   * Workfront Planning 레코드 또는 선택한 레코드 유형에 연결된 레코드에 연결된 다른 응용 프로그램의 객체

     예를 들어 캠페인을 포트폴리오에 연결할 수 있습니다. 또한 다른 레코드 유형인 제품을 캠페인뿐만 아니라 프로젝트와 연결할 수도 있습니다. 캠페인 타임라인 보기를 작성할 때 포트폴리오, 제품 및 프로젝트별로 캠페인을 분류할 수 있습니다.

* Workfront의 Workfront 개체에만 연결되어 있지만 Workfront Planning 레코드 유형에는 연결되어 있지 않은 개체 유형은 표시할 수 없습니다. Workfront Planning에서 연결된 객체 또는 레코드 유형만 표시할 수 있습니다.

  예를 들어 작업은 Workfront의 프로젝트에 연결됩니다. 분류 기능을 사용하면 Planning의 캠페인에 연결되어 있지만 Workfront의 프로젝트에 연결된 작업은 아닌 프로젝트를 표시할 수 있습니다.

  Workfront Planning 레코드 유형의 타임라인 보기에 포트폴리오와 프로젝트를 모두 표시하려면 포트폴리오와 프로젝트가 모두 Planning 레코드나 관리하는 Planning 레코드의 타임라인 보기에 연결된 레코드에 연결되어 있어야 합니다.
* 두 개 이상의 날짜 필드와 연결된 레코드 유형만 표시할 수 있습니다.
* 타임라인 보기에 표시할 레코드 종류의 날짜 필드는 선택한 레코드 종류의 표 보기에서 조회 필드로 표시되어야 합니다.
* 타임라인 보기에 표시할 레코드 유형의 시작 날짜와 종료 날짜는 시간 순서대로 표시되어야 합니다. 예를 들어 레코드에 시작 날짜가 1월 31일이고 종료 날짜가 1월 1일인 경우 타임라인 보기에 표시되지 않습니다. 자세한 내용은 이 문서의 [타임라인 보기 관리](#manage-a-timeline-view) 섹션을 참조하십시오.
* 레코드 분류에 포함할 수 있는 레코드 유형은 5개로 제한됩니다.

#### 타임라인 보기에서 연결된 레코드 분류

1. [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md) 문서에 설명된 대로 레코드 유형에 대한 타임라인 보기를 만듭니다.
1. (조건부) 표준 모드에서 타임라인 보기를 보려면 **분류**&#x200B;를 클릭합니다.
1. **연결된 레코드 종류 선택** 상자를 확장하고 연결된 레코드 종류를 선택합니다. <!--add a new screen shot - submitted a bug to remove the "the"-->

   ![](assets/breakdown-picker-and-button-on-timeline.png)

   >[!TIP]
   >
   >    연결된 레코드가 없거나 연결된 레코드에 둘 이상의 날짜 필드가 없는 경우 **연결된 레코드 종류 선택** 상자를 사용할 수 없습니다.

1. **시작 날짜** 및 **종료 날짜 필드**&#x200B;를 선택하세요.

   >[!TIP]
   >
   >    시작 및 종료 날짜는 순차적이어야 합니다. 종료 날짜가 시작 날짜 이전이면 타임라인에 레코드가 표시되지 않습니다.

   다른 레코드와 연결된 경우 타임라인에서 선택한 레코드의 막대에 오른쪽 방향 화살표가 표시됩니다.
1. 레코드 유형을 확장하고 연결을 표시하려면 오른쪽 화살표를 클릭합니다.

   ![](assets/campaigns-broken-down-by-programs-in-timeline-highlighted.png)

1. (선택 사항) 연결된 레코드를 더 추가하려면 위의 단계를 반복합니다.



