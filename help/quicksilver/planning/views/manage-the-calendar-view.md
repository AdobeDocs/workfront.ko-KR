---
title: 달력 보기 관리
description: 달력 보기에서 레코드와 해당 필드를 표시할 수 있습니다. 이 문서에서는 달력 보기를 만들고 기존 달력 보기를 편집하거나 삭제하는 방법에 대해 설명합니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 1%

---

# 달력 보기 관리

{{planning-important-intro}}

레코드 유형 페이지에서 레코드와 해당 필드를 달력 보기에 표시할 수 있습니다.

Adobe Workfront Planning 보기 및 관리 방법에 대한 자세한 내용은 [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md)를 참조하십시오.

## 액세스 요구 사항

+++ 를 확장하여 Workfront Planning에 대한 액세스 요구 사항을 봅니다.

Workfront Planning에 액세스하려면 다음 항목이 있어야 합니다.

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
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
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
   <td><p> 표준 </p>
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
   <p>보기에 대한 권한을 보고 일시적으로 보기 설정 변경</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>레이아웃 템플릿</p></td> 
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

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

## 달력 보기 관리 {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

다음 사항을 고려하십시오.

* 레코드 유형과 연결된 날짜 필드가 두 개 이상 있는 경우에만 달력 보기를 만들 수 있습니다. 레코드 유형과 연결된 날짜 필드가 하나 또는 없으면 달력 보기 옵션이 흐리게 표시됩니다.

  레코드 날짜 필드에서 선택하거나 연결된 레코드 또는 개체 유형에서 날짜 필드를 조회할 수 있습니다.
* 다음과 같은 시나리오가 있습니다.

   * 시작 날짜와 종료 날짜에 값이 없으면 레코드가 달력에 표시되지 않습니다
   * 시작 또는 종료 날짜에 값이 없으면 레코드가 1일 이벤트로 표시됩니다
   * 시작 날짜가 종료 날짜 이후인 경우 기록이 캘린더에 표시되지 않습니다.

달력 보기를 관리하려면:

1. 달력을 보려는 레코드 유형 페이지로 이동합니다.
1. [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md) 문서에 설명된 대로 일정 보기를 만듭니다.

   ![](assets/calendar-view-example.png)

   선택한 레코드 유형과 연관된 레코드가 달력에 막대로 표시됩니다. 막대의 색상은 레코드 아이콘의 색상과 일치합니다.

1. 다음 중 하나를 수행하여 달력을 탐색합니다.

   * 왼쪽 및 오른쪽 아이콘을 클릭하거나 가로 스크롤을 사용하여 달력에서 앞뒤로 이동합니다.
   * **오늘**&#x200B;을 클릭하여 캘린더를 오늘 날짜로 가운데로 맞춥니다.
   * 시간 증가를 업데이트하려면 시간대 드롭다운 메뉴에서 다음 옵션 중 하나를 선택합니다.

      * 월
1. 아래 하위 섹션에 설명된 대로 다음 보기 요소를 업데이트합니다.
   * [필터](#add-filters)
   * [설정](#edit-the-calendar-view-settings)
     <!--* [Grouping](#add-grouping)-->
     <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### 필터 추가

필터를 사용하여 화면에 표시되는 정보의 양을 줄일 수 있습니다.

달력 보기에서 필터를 사용할 때는 다음 사항을 고려하십시오.

<!-- this list is almost identical to the one for the table view - update both-->

* 달력 보기를 위해 만든 필터는 동일한 레코드 유형에 적용되는 다른 보기의 필터와는 독립적으로 작동합니다.

* 필터는 사용자가 선택한 보기에 고유합니다. 동일한 기록 유형의 두 달력 보기에는 서로 다른 필터가 적용될 수 있습니다.

* 동일한 달력 보기를 보고 있는 두 명의 사용자에게 현재 적용된 동일한 필터가 표시됩니다.

* 달력 보기를 위해 빌드하는 필터의 이름을 지정할 수 없습니다.

* 필터를 제거하면 사용자와 동일한 레코드 종류에 액세스하고 사용자와 동일한 보기를 표시하는 모든 사용자에서 필터가 제거됩니다.

* 달력 보기에서 필터를 추가하는 것은 표 보기에서 필터를 추가하는 것과 동일합니다.

  자세한 내용은 문서 [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)의 &quot;필터 추가&quot; 섹션을 참조하십시오.

* 연결된 레코드 필드 또는 조회 필드를 기준으로 필터링할 수 있습니다.

* 여러 값을 표시하는 조회 필드를 기준으로 필터링할 수 있습니다.

### 달력 보기 설정 편집

달력 보기 설정을 편집하는 것은 타임라인 보기의 설정을 편집하는 것과 동일합니다.

자세한 내용은 문서 [타임라인 보기 관리](/help/quicksilver/planning/views/manage-the-timeline-view.md)의 &quot;타임라인 보기 설정 편집&quot; 섹션을 참조하십시오.
