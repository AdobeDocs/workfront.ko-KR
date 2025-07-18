---
title: 레코드 보기 관리
description: Adobe Systems Workfront Planning을 사용할 때 테이블, 타임라인 또는 달력 보기로 레코드를 표시할 수 있습니다. 이 문서에서는 보기를 만들고 기존 보기를 편집하는 방법에 대해 설명합니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 1%

---


# 레코드 보기 관리

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

[Adobe Systems Workfront Planning] 영역에서 레코드 유형을 선택한 후 다음 보기에서 해당 유형의 모든 레코드를 표시할 수 있습니다.

* 테이블

  자세한 내용은 [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)를 참조하십시오.

* 타임라인

  자세한 내용은 [타임라인 보기 관리](/help/quicksilver/planning/views/manage-the-timeline-view.md)를 참조하십시오.

* 캘린더

  자세한 내용은 [일정 보기 관리](/help/quicksilver/planning/views/manage-the-calendar-view.md)를 참조하세요.

이 문서에서는 레코드 보기에 대한 다음 정보를 설명합니다.

* [보기 만들기 및 편집](#create-or-edit-record-views)
* [보기에서 실시간 현재 상태 표시기 사용Enable the real-time presence indicator in a view](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->

Workfront Planning 레코드 보기 관리에 대한 자세한 내용은 다음 문서도 참조하세요.

* [레코드 보기 삭제](/help/quicksilver/planning/views/delete-record-views.md)
* [중복 레코드 보기](/help/quicksilver/planning/views/duplicate-record-views.md)
* [조회수 공유](/help/quicksilver/planning/access/share-views.md)


## 액세스 요구 사항

+++ 액세스 요구 사항을 보려면 확장합니다.

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
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Systems Workfront 플랜*</p></td> 
   <td> 
<p>다음 Workfront 플랜 중 하나:</p> 
<ul><li>선택</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Systems Workfront 계획 패키지*</p></td> 
   <td> 
<p>어떤 </p> 
<p>각 Workfront Planning 플랜에 포함된 항목에 대한 자세한 내용은 Workfront 계정 관리자 관리자에게 문의하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Systems Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning에 액세스하려면 조직의 Workfront 인스턴스가 Adobe Systems 통합 환경에 온보딩되어 있어야 합니다.</p> 
<p>자세한 내용은 Adobe Systems Unified Experience for Workfront<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">를 참조하십시오</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
   <td><p> 보기를 만들고 삭제하는 표준</p>
   <p>기여자 이상: 보기 요소 업데이트</p>
   <p>Workfront Planning은 기존 Workfront 라이선스에 사용할 수 없습니다</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Systems Workfront Planning에 대한 액세스 수준 컨트롤은 없습니다</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 사용 권한</p></td> 
   <td>   <p>보기에 대한 사용 권한 관리</p>  
   <p>보기 설정을 임시로 변경하거나 복제할 수 있는 보기에 대한 보기 권한</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> Light 또는 Contributor 라이센스가 있는 사용자에게는 Planning이 포함된 레이아웃 템플릿 정보가 지정되어야 합니다.
   <p>표준 사용자 및 시스템 관리자는 기본적으로 계획 영역을 사용하도록 설정되어 있습니다.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서[의 액세스 요구 사항을 참조하십시오](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 레코드 뷰로 작업할 때의 고려 사항

* Workfront Planning 보기는 레코드 유형별로 다릅니다. 두 개의 서로 다른 레코드 종류에 동일한 뷰를 적용할 수 없습니다.
* 만든 보기는 사용자와 보기를 공유하는 사용자만 볼 수 있습니다.
* 보기를 수정하거나 삭제하면 보기에 대한 권한이 있는 모든 사용자에 대해 수정 및 삭제됩니다.
* 각 사용자는 최대 100개의 보기를 만들 수 있습니다. 레코드 유형에 대해 100개 이상의 보기를 표시할 수 있지만 한 사용자가 100개의 보기만 만들 수 있습니다.
* 일부 보기 요소는 동일한 레코드에 대한 여러 보기에 적용할 수 있지만 각 레코드 보기에 대해 고유합니다.

   * 필터
   * 그룹화(테이블 및 타임라인 보기용)
   * 막대 모양(타임라인 및 달력 보기용)

  예를 들어 테이블 뷰에서 필터를 만들 때 필터 결과는 선택한 뷰(테이블 뷰)에만 표시되고 레코드 종류와 연결된 모든 뷰에는 표시되지 않습니다.

  >[!TIP]
  >
  >일부 보기 요소는 일부 보기에서만 사용할 수 있습니다.


## 레코드 보기 간의 유사점과 차이점

다음 표에서는 테이블, 타임라인 및 달력 보기 간의 유사점과 차이점을 보여 줍니다.

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| 특징 | 테이블 보기 | 타임라인 보기 | 달력 보기 |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| 목록 또는 테이블에 레코드 표시 | ✓ |              | |
| 기본적으로 모든 필드를 테이블에 열로 표시 | ✓ |              |    |
| 필드(또는 열) 숨기기 또는 표시 | ✓ |               |    |
| 각 레코드의 필드 값 편집 | ✓ |               |             |
| 보기에 새 행으로 레코드 추가 | ✓ |               |        |
| 필드를 뷰의 새 열로 추가 | ✓ |               |         |
| 외부 목록에서 행을 복사하여 표에 붙여넣기 | ✓ |               |          |
| 타임라인 내에 레코드 표시 |            | ✓ |             |
| 레코드 필터링 | ✓ | ✓ | ✓ |
| 달력에 레코드 표시 |           |              | ✓ |
| 그룹 레코드 | ✓ | ✓ |
| 레코드 정렬 | ✓ |              |
| 색상코드 레코드 | ✓ | ✓ | ✓ |
| 색상 코드 그룹화 |           | ✓ |
| 특정 레코드에 대한 Search | ✓ | ✓ |
| 다른 사용자와 뷰 공유 | ✓ | ✓ | ✓ |
| 보기에서 레코드의 페이지 열기 | ✓ | ✓ |    |
| 연도 및 분기별로 레코드 표시 |           | ✓ |    |
| 월별 레코드 표시 |           | ✓ | ✓ |
| 주별 레코드 표시 |           |               | ✓ |
| 보기에서 정보 내보내기 | ✓ |               |    |


## 보기 만들기 또는 편집 {#create-or-edit-views}

{{step1-to-planning}}


1. 작업 영역 카드 클릭

   작업 영역 영역이 열리고 레코드 종류가 카드로 표시됩니다.

1. 레코드 종류 카드 클릭

   레코드 종류 페이지 가 열립니다.

   기본적으로 선택한 유형의 모든 레코드가 테이블 뷰에 표시됩니다.

1. + 보기&#x200B;**를 클릭하여**&#x200B;새 보기를 추가합니다.
1. 다음 유형의 뷰 중에서 선택합니다.

   * 테이블
   * 타임라인
   * 캘린더

   선택한 보기로 새 탭이 만들어집니다.

   화면 너비에 따라 추가 보기가 더 보기&#x200B;**메뉴**&#x200B;의 ![더 보기 메뉴](assets/more-menu.png)에 표시될 수 있습니다.


>[!TIP]
>
>레코드 종류를 만들면 기본적으로 테이블 뷰도 만들어집니다.
>
>타임라인 또는 달력 보기를 만들려면 보기를 빌드 할 레코드 종류에 두 개 이상의 날짜 필드가 있어야 합니다.
>
>그렇지 않으면 타임라인 및 달력 옵션이 흐리게 표시됩니다.
>

![레코드 종류 목록의 보기 종류 드롭다운](assets/view-types-drop-down-from-record-type-list.png)

1. (조건부) 타임라인 또는 달력 보기를 만들 때 다음&#x200B;**을 클릭합니다**.

   기본적으로 Workfront는 보기에 다음 이름 중 하나를 지정합니다.

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   이 숫자는 자동으로 생성된 증분입니다.

1. (조건부) **타임라인 또는 달력 보기에 표시할 레코드의 시작** 및 **종료 날짜를** 선택합니다.

   >[!NOTE]
   >
   >    레코드 날짜 필드에서 선택하거나 연결된 레코드 또는 개체 유형에서 조회 날짜 필드를 선택할 수 있습니다.
   >
   >레코드 종류를 연결할 때 조회 필드를 선택할 때 날짜 필드(MAX 또는 MIN)에 대해 집계자를 사용해야 합니다. 집계를 추가하기만 하면 연결의 날짜를 타임라인 및 달력 보기의 시작 및 종료 날짜로 사용할 수 있습니다.
   >
   >자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

1. Click **Create**.

   보기가 새 탭으로 표시됩니다. 보기가 만들어지거나 사용자와 공유될 때부터 시간 순서대로 표시됩니다.
1. (선택 사항) 선택한 레코드 종류에 대한 모든 보기를 표시하려면 마지막 보기 옆의 **자세히** 메뉴 ![추가 삽입 아래쪽 아이콘 보기](assets/more-caret-down-icon-views.png)를 클릭합니다.

   추가 보기는 마지막 보기 탭 다음에 있는 **자세히** 메뉴 아래에 표시됩니다. 자세히&#x200B;**메뉴 옆의**&#x200B;숫자는 추가 보기 수를 표시합니다.
1. (선택 사항) 보기를 만든 후 이름을 바꾸려면 보기 드롭다운 메뉴를 클릭한 다음 **자세히** 메뉴 ![자세히 메뉴](assets/more-menu.png) > 이름 바꾸기&#x200B;****&#x200B;클릭하여 보기 이름을 업데이트합니다

   또는

   보기 이름을 두 번 클릭하고 새 이름을 입력하기 시작합니다.  <!--ensure there is not another saving step here?!-->

1. (선택 사항) 특정 유형의 보기를 관리하려면 다음 문서를 참조하세요.

   * [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [타임라인 보기 관리](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [달력 보기 관리](/help/quicksilver/planning/views/manage-the-calendar-view.md)

## 보기에서 실시간 현재 상태 표시기 사용Enable the real-time presence indicator in a view

보기의 실시간 현재 상태 표시기를 따라 다른 사용자가 사용자와 동시에 레코드를 편집하고 있는지 확인할 수 있습니다.

기본적으로 모든 레코드 보기의 오른쪽 위 모서리에 표시되는 것과 동시에 레코드 정보를 편집하는 다른 사용자의 아바타입니다.

표 보기를 표시할 때 레코드를 볼 때 다른 사용자가 편집하고 있는 필드를 볼 수도 있습니다.

자세한 내용은 [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)를 참조하십시오.



<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->
