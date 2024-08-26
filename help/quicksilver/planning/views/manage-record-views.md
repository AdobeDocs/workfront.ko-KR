---
title: 레코드 보기 관리
description: Adobe Workfront Planning을 사용할 때 표, 타임라인 또는 달력 보기에 레코드를 표시할 수 있습니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: f8ad026582be5b4c89939af8f135151ffaabccfe
workflow-type: tm+mt
source-wordcount: '1212'
ht-degree: 1%

---


# 레코드 보기 관리

{{planning-important-intro}}

Adobe Workfront Planning 영역에서 레코드 유형을 선택한 후 다음 보기에서 해당 유형의 모든 레코드를 표시할 수 있습니다.

* 테이블

  자세한 내용은 [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)를 참조하십시오.

* 타임라인

  자세한 내용은 [타임라인 보기 관리](/help/quicksilver/planning/views/manage-the-timeline-view.md)를 참조하십시오.

* 캘린더

  자세한 내용은 [일정 보기 관리](/help/quicksilver/planning/views/manage-the-calendar-view.md)를 참조하세요.

이 문서에서는 레코드 보기에 대한 다음 정보를 설명합니다.

* [보기 만들기 및 편집](#create-or-edit-record-views)
* [보기 삭제](#delete-views)
* [보기 복제](#duplicate-views)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->


## 액세스 요구 사항

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
   <td> <ul><li><p>Workfront Planning 정보를 보려면 표준, 라이트 또는 기여자</p></li>
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

+++

<!--old: 

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

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->


## 레코드 보기 작업 시 고려 사항

* Workfront Planning 보기는 레코드 유형별로 다릅니다. 동일한 보기를 두 개의 다른 레코드 유형에 적용할 수 없습니다.
* 만든 보기는 사용자와 보기를 공유하는 사용자만 볼 수 있습니다.
* 보기를 수정하거나 삭제하면 보기에 대한 권한이 있는 모든 사용자에 대해 수정 및 삭제됩니다.
* 각 사용자는 최대 100개의 보기를 만들 수 있습니다. 레코드 유형에 대해 100개 이상의 보기를 표시할 수 있지만 한 사용자가 100개의 보기만 만들 수 있습니다.
* 만든 보기를 다른 사용자와 공유할 수 있습니다. 자세한 내용은 [보기 공유](/help/quicksilver/planning/access/share-views.md)를 참조하십시오.
* 다음 요소는 각 레코드 보기에 고유합니다.

   * 필터
   * 그룹화
   * 정렬
   * 막대 모양(타임라인 보기의 경우)

  <!-- some of these are not available in all of the views - edit above-->

  예를 들어, 테이블 보기에서 필터를 만들 때 선택한 보기에서만 필터 결과를 볼 수 있고 레코드 유형과 연관된 모든 보기에서는 볼 수 없습니다.

  >[!NOTE]
  >
  > 일부 보기 요소는 모든 보기에서 사용하지 못할 수 있습니다.


## 레코드 보기 간의 유사성 및 차이점

다음 표는 표, 타임라인 및 달력 보기 간의 유사점과 차이점을 보여 줍니다.

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| 기능 | 표 보기 | 타임라인 보기 | 달력 보기 |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| 목록 또는 테이블에 레코드 표시 | ✓ 덧신 |              | |
| 기본적으로 모든 필드를 테이블에 열로 표시 | ✓ 덧신 |              |    |
| 필드(또는 열) 숨기기 또는 표시 | ✓ 덧신 |               |    |
| 각 레코드의 필드 값 편집 | ✓ 덧신 |               |             |
| 보기에 새 행으로 레코드 추가 | ✓ 덧신 |               |        |
| 보기에 필드를 새 열로 추가 | ✓ 덧신 |               |         |
| 외부 목록에서 행을 복사하여 표에 붙여넣기 | ✓ 덧신 |               |          |
| 타임라인에 레코드 표시 |            | ✓ 덧신 |             |
| 레코드 필터링 | ✓ 덧신 | ✓ 덧신 | ✓ 덧신 |
| 달력에 레코드 표시 |           |              | ✓ 덧신 |
| 그룹 레코드 | ✓ 덧신 | ✓ 덧신 |
| 레코드 정렬 | ✓ 덧신 |              |
| 색상 코드 레코드 |           | ✓ 덧신 | ✓ 덧신 |
| 색상 코드 그룹화 |           | ✓ 덧신 |
| 특정 레코드 검색 | ✓ 덧신 | ✓ 덧신 |
| 다른 사용자와 보기 공유 | ✓ 덧신 | ✓ 덧신 | ✓ 덧신 |
| 보기에서 레코드의 페이지를 엽니다. | ✓ 덧신 | ✓ 덧신 |    |


## 보기 만들기 또는 편집 {#create-or-edit-views}

{{step1-to-planning}}


1. 작업 영역의 카드를 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.

   기본적으로 선택한 유형의 모든 레코드가 테이블 뷰에 표시됩니다.

1. 새 보기를 추가하려면 **+ 보기**&#x200B;를 클릭하십시오.
1. 다음 유형의 뷰 중에서 선택합니다.

   * 테이블
   * 타임라인
   * 캘린더

   선택한 보기로 새 탭이 만들어집니다.

   화면의 너비에 따라 **자세히** 메뉴 ![](assets/more-menu.png)에 추가 보기가 표시될 수 있습니다.


>[!TIP]
>
>레코드 유형을 만들면 기본적으로 테이블 뷰도 만들어집니다.
>
>타임라인 또는 달력 보기를 만들려면 보기를 만드는 레코드 종류에는 최소 두 개 이상의 날짜 필드가 있어야 합니다.
>
>그렇지 않으면 [타임라인] 및 [달력] 옵션이 흐리게 표시됩니다.
>

![](assets/view-types-drop-down-from-record-type-list.png)

1. (조건부) 타임라인 또는 달력 보기를 만들 때 **다음**&#x200B;을 클릭합니다.

   기본적으로 Workfront은 보기에 다음 이름 중 하나를 제공합니다.

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   이 숫자는 자동으로 생성된 증가값입니다.

1. (조건부) 타임라인 또는 달력 보기에 표시할 레코드에 대한 **시작** 및 **종료 날짜**&#x200B;를 선택합니다.

   >[!TIP]
   >
   >    레코드 날짜 필드에서 선택하거나 연결된 레코드 또는 개체 유형에서 날짜 필드를 조회할 수 있습니다. 조회 필드를 타임라인 및 달력 보기의 시작 및 종료 날짜로 선택하는 경우 날짜 필드(MAX 또는 MIN)에 대해 집계자를 사용해야 합니다. 자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

1. Click **Create**.

   보기가 새 탭으로 표시됩니다. 보기가 만들어지거나 사용자와 공유될 때부터 시간 순서대로 표시됩니다.
1. (선택 사항) 선택한 레코드 종류의 모든 보기를 표시하려면 마지막 보기 옆의 **자세히** 메뉴 ![](assets/more-caret-down-icon-views.png)을(를) 클릭합니다.

   마지막 보기 탭 뒤에 **자세히** 메뉴 아래에 추가 보기가 표시됩니다. **자세히** 메뉴 옆의 숫자는 추가 보기 수를 표시합니다.
1. (선택 사항) 보기가 만들어진 후 보기의 이름을 바꾸려면 보기 드롭다운 메뉴를 클릭한 다음 **자세히** 메뉴 ![](assets/more-menu.png) > **이름 바꾸기**&#x200B;를 클릭하여 보기 이름을 업데이트합니다

   또는

   보기 이름을 두 번 클릭하고 새 이름을 입력하십시오.  <!--ensure there is not another saving step here?!-->

1. (선택 사항) 특정 유형의 보기를 관리하려면 다음 문서를 참조하십시오.

   * [표 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [타임라인 보기 관리](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [달력 보기 관리](/help/quicksilver/planning/views/manage-the-calendar-view.md)


## 보기 삭제

{{step1-to-planning}}

1. 작업 영역의 카드를 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.

   기본적으로 선택한 유형의 모든 레코드가 테이블 뷰에 표시됩니다.

1. 보기 탭에서 보기 이름 중 하나를 마우스로 가리킨 다음, 보기 이름 왼쪽의 **자세히** ![](assets/more-menu.png)을(를) 클릭한 다음 **삭제**를 클릭합니다.
먼저, 삭제할 보기를 찾으려면 마지막 탭 왼쪽에 있는 **자세히**&#x200B;를 클릭해야 할 수 있습니다.

1. 확인하려면 **삭제**&#x200B;를 클릭하세요. <!--ensure there is not another saving step here?!-->

   레코드 영역에 액세스할 수 있는 모든 사용자에 대해 보기가 삭제되며 복구할 수 없습니다.

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## 보기 복제

여러 버전의 보기를 유지하고 버전 간에 약간의 변경 내용을 적용하려는 경우 보기를 복제할 수 있습니다.

뷰를 복제하면 기존 뷰의 동일한 복사본이 만들어집니다.

원래 보기의 공유 권한이 복제된 보기로 전송되지 않습니다.

{{step1-to-planning}}

1. 작업 영역의 카드를 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.
기본적으로 선택된 유형의 모든 레코드가 테이블 뷰에 표시됩니다.

1. 복제할 보기의 탭 위로 마우스를 가져간 후 보기 이름 오른쪽에 있는 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 다음 **복제**&#x200B;를 클릭합니다.

   ![](assets/view-more-menu-with-duplicate-option.png)


   보기가 복제되고 새 보기의 이름이 `Original view's name (Copy)` 패턴을 따릅니다. 새 보기 탭은 모든 보기 탭의 끝에 표시됩니다.

