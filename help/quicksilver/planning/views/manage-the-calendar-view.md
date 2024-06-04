---
title: 달력 보기 관리
description: 달력 보기에서 레코드와 해당 필드를 표시할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: 278d740303b0fa2f1d1b10801634ce76ce0f5739
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# 달력 보기 관리

<!--
title: Manage the calendar view
description: You can display records in a calendar view.
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

레코드 유형 페이지에서 레코드와 해당 필드를 달력 보기에 표시할 수 있습니다.

Adobe Workfront Planning 기능 보기 및 관리 방법에 대한 자세한 내용은 다음을 참조하십시오. [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md).

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
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td>
   <td>
   <p>임의</p> 
   <p>시스템 관리자는 자신이 만들었거나 자신과 공유된 보기에만 액세스할 수 있습니다. </p>
  </td>
  </tr>

<tr>
   <td role="rowheader">액세스 수준 구성</td>
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>보기에 대한 권한 관리</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">레이아웃 템플릿</td>
   <td> <p>시스템 관리자가 레이아웃 템플릿에 계획 영역을 추가해야 합니다. 자세한 내용은 <a href="/help/quicksilver/planning/access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


## 달력 보기 관리 {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

다음 사항을 고려하십시오.

* 레코드 유형과 연결된 날짜 필드가 두 개 이상 있는 경우에만 달력 보기를 만들 수 있습니다. 레코드 유형과 연결된 날짜 필드가 하나 또는 없으면 달력 보기 옵션이 흐리게 표시됩니다.
* 다음과 같은 시나리오가 있습니다.

   * 시작 날짜와 종료 날짜에 값이 없으면 레코드가 달력에 표시되지 않습니다
   * 시작 또는 종료 날짜에 값이 없으면 레코드가 1일 이벤트로 표시됩니다
   * 시작 날짜가 종료 날짜 이후인 경우 기록이 캘린더에 표시되지 않습니다.

달력 보기를 관리하려면:

1. 달력을 보려는 레코드 유형 페이지로 이동합니다.
1. 문서에 설명된 대로 달력 보기를 만듭니다 [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md).

   ![](assets/calendar-view-example.png)

   선택한 레코드 유형과 연관된 레코드가 달력에 막대로 표시됩니다. 막대의 색상은 레코드 아이콘의 색상과 일치합니다.

1. 다음 중 하나를 수행하여 달력을 탐색합니다.

   * 왼쪽 및 오른쪽 아이콘을 클릭하거나 가로 스크롤을 사용하여 달력에서 앞뒤로 이동합니다.
   * 클릭 **오늘** 캘린더를 오늘 날짜로 맞춰야 합니다.
   * 시간 증가를 업데이트하려면 시간대 드롭다운 메뉴에서 다음 옵션 중 하나를 선택합니다.

      * 월
1. 아래 하위 섹션에 설명된 대로 다음 보기 요소를 업데이트합니다.
   * [필터](#add-filters)
     <!--* [Grouping](#add-grouping)-->
     <!--* [Settings](#edit-the-calendar-view-settings)-->
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

  자세한 내용은 문서의 &quot;필터 추가&quot; 섹션을 참조하십시오 [표 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md).

* 연결된 레코드 필드나 조회 필드를 기준으로 필터링할 수 있지만 여러 레코드에 연결할 수 있는 필드는 필터링할 수 없습니다.
