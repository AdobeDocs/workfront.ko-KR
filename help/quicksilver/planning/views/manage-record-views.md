---
title: 레코드 보기 관리
description: Adobe Workfront Planning을 사용할 때 표, 타임라인 또는 달력 보기에 레코드를 표시할 수 있습니다. 이 문서에서는 보기를 만들고 기존 보기를 편집하는 방법에 대해 설명합니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: b102960e088f072f10baadcbeca4f7f579daa287
workflow-type: tm+mt
source-wordcount: '1245'
ht-degree: 1%

---


# 레코드 보기 관리

<!-- take preview and production references out at production-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>


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
* [보기에서 실시간 현재 상태 표시기를 사용하도록 설정](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->

Workfront Planning 레코드 보기 관리에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [레코드 보기 삭제](/help/quicksilver/planning/views/delete-record-views.md)
* [중복 레코드 보기](/help/quicksilver/planning/views/duplicate-record-views.md)
* [보기 공유](/help/quicksilver/planning/access/share-views.md)


## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<ul> 
<li><p>모든 Workfront 및 모든 Planning 패키지</p></li>
또는
<li><p>모든 워크플로우 및 모든 Planning 패키지</li></ul>
<p>각 Workfront Planning 패키지에 포함된 내용에 대한 자세한 내용은 Workfront 계정 담당자에게 문의하십시오. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p> 보기를 만들고 삭제하는 표준</p>
   <p>기여자 이상: 보기 요소 업데이트</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>보기에 대한 권한 관리</p>  
   <p>보기에 대한 권한을 보고 일시적으로 보기 설정을 변경하거나 복제합니다.</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> 라이트 또는 기여자 라이선스가 있는 사용자에게 Planning이 포함된 레이아웃 템플릿을 할당해야 합니다.
   <p>표준 사용자 및 시스템 관리자에게는 기본적으로 계획 영역이 활성화되어 있습니다.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard to create and delete views</p>
   <p>Contributor or higher to update view elements</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings or to duplicate it</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table>-->

## 레코드 보기 작업 시 고려 사항

* Workfront Planning 보기는 레코드 유형별로 다릅니다. 동일한 보기를 두 개의 다른 레코드 유형에 적용할 수 없습니다.
* 만든 보기는 사용자와 보기를 공유하는 사용자만 볼 수 있습니다.
* 보기를 수정하거나 삭제하면 보기에 대한 권한이 있는 모든 사용자에 대해 수정 및 삭제됩니다.
* 각 사용자는 최대 100개의 보기를 만들 수 있습니다. 레코드 유형에 대해 100개 이상의 보기를 표시할 수 있지만 한 사용자가 100개의 보기만 만들 수 있습니다.
* 일부 보기 요소는 동일한 레코드에 대한 여러 보기에 적용할 수 있지만 각 레코드 보기에 대해 고유합니다.

   * 필터
   * 그룹화(테이블 및 타임라인 보기)
   * 막대 모양(타임라인 및 달력 보기의 경우)

  예를 들어, 테이블 보기에서 필터를 만들 때 선택한 보기(테이블 보기)에서만 필터 결과가 표시되고 레코드 유형과 연관된 모든 보기에서는 표시되지 않습니다.

  >[!TIP]
  >
  >일부 보기 요소는 모든 보기에서 사용할 수 없습니다.


## 레코드 보기 간의 유사성 및 차이점

다음 표는 표, 타임라인 및 달력 보기 간의 유사점과 차이점을 보여 줍니다.

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| 기능 | 테이블 보기 | 타임라인 보기 | 캘린더 보기 |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| 목록 또는 테이블에 레코드 표시 | ✓ |              | |
| 기본적으로 모든 필드를 테이블에 열로 표시 | ✓ |              |    |
| 필드(또는 열) 숨기기 또는 표시 | ✓ |               |    |
| 각 레코드의 필드 값 편집 | ✓ |               |             |
| 보기에 새 행으로 레코드 추가 | ✓ |               |        |
| 보기에 필드를 새 열로 추가 | ✓ |               |         |
| 외부 목록에서 행을 복사하여 표에 붙여넣기 | ✓ |               |          |
| 타임라인에 레코드 표시 |            | ✓ |             |
| 레코드 필터링 | ✓ | ✓ | ✓ |
| 달력에 레코드 표시 |           |              | ✓ |
| 그룹 레코드 | ✓ | ✓ |
| 레코드 정렬 | ✓ |              |
| 색상 코드 레코드 | ✓ | ✓ | ✓ |
| 색상 코드 그룹화 |           | ✓ |
| 특정 레코드 검색 | ✓ | ✓ |
| 다른 사용자와 보기 공유 | ✓ | ✓ | ✓ |
| 보기에서 레코드의 페이지를 엽니다. | ✓ | ✓ |    |
| 연도 및 분기별 레코드 표시 |           | ✓ |    |
| 월별 레코드 표시 |           | ✓ | ✓ |
| 주별 레코드 표시 |           |               | ✓ |
| 보기에서 정보 내보내기 | ✓ |               |    |
| <span class="preview">전체 화면으로 표시</span> | ✓ | ✓ | ✓ |
| <span class="preview">보기에서 레코드 만들기</span> | ✓ | ✓ | ✓ |

## 보기 만들기 또는 편집 {#create-or-edit-views}

{{step1-to-planning}}


1. 작업 영역의 카드를 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.

   기본적으로 선택한 유형의 모든 레코드가 테이블 뷰에 표시됩니다.

1. 사용하는 환경에 따라 다음을 수행합니다.

   * 프로덕션 환경에서 **+보기** 탭을 클릭합니다.
   * <span class="preview">미리 보기 환경에서 현재 보기 이름 옆에 있는 드롭다운 아이콘 ![드롭다운 아이콘](assets/drop-down-icon.png)을 클릭한 다음 **+새 보기**&#x200B;를 클릭합니다.</span>

1. 다음 유형의 뷰 중에서 선택합니다.

   * 테이블
   * 타임라인
   * 캘린더

   프로덕션 환경에서는 선택한 뷰로 새 탭이 만들어집니다.

   화면의 너비에 따라 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)에 추가 보기가 표시될 수 있습니다.

   >[!TIP]
   >
   >레코드 유형을 만들면 기본적으로 테이블 뷰도 만들어집니다.
   >
   >타임라인 또는 달력 보기를 만들려면 보기를 만드는 레코드 종류에는 최소 두 개 이상의 날짜 필드가 있어야 합니다.
   >
   >그렇지 않으면 [타임라인] 및 [달력] 옵션이 흐리게 표시됩니다.
   >

   <span class="preview">미리 보기 환경에서 보기 유형을 선택한 다음 **만들기**&#x200B;를 클릭합니다. 드롭다운 메뉴에 새 보기가 추가됩니다. </span>

   <span class="preview">![보기 상자 만들기](assets/create-view-box.png)</span>

1. <span class="preview">기존 보기를 편집하려면 **검색** 필드에 보기 이름을 입력하고 키보드에서 Enter 키를 누르십시오.</span>
1. <span class="preview">보기 드롭다운 메뉴에서 원하는 순서대로 보기를 끌어서 놓습니다.</span>

   <span class="preview">![레코드 형식 목록의 보기 형식 드롭다운](assets/view-types-drop-down-from-record-type-list.png)</span>

1. (조건부) 타임라인 또는 달력 보기를 만들 때 **다음**&#x200B;을 클릭합니다.

   기본적으로 Workfront은 보기에 다음 이름 중 하나를 제공합니다.

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   이 숫자는 자동으로 생성된 증가값입니다.

1. (조건부) 타임라인 또는 달력 보기에 표시할 레코드에 대한 **시작** 및 **종료 날짜**&#x200B;를 선택합니다.

   >[!NOTE]
   >
   >    레코드 날짜 필드에서 선택하거나 연결된 레코드 또는 개체 유형에서 날짜 필드를 조회할 수 있습니다.
   >
   >레코드 유형을 연결할 때 조회 필드를 선택할 때에는 날짜 필드(MAX 또는 MIN)에 집계자를 사용해야 합니다. 집계자만 추가하면 연결의 날짜를 타임라인 및 달력 보기의 시작 및 종료 날짜로 사용할 수 있습니다.
   >
   >자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

1. Click **Create**.

   보기가 새 탭으로 표시됩니다. 보기가 만들어지거나 사용자와 공유될 때부터 시간 순서대로 표시됩니다.
1. (선택 사항) 선택한 레코드 종류에 대한 모든 보기를 표시하려면 마지막 보기 옆의 **자세히** 메뉴 ![추가 삽입 아래쪽 아이콘 보기](assets/more-caret-down-icon-views.png)를 클릭합니다.

   마지막 보기 탭 뒤에 **자세히** 메뉴 아래에 추가 보기가 표시됩니다. **자세히** 메뉴 옆의 숫자는 추가 보기 수를 표시합니다.
1. (선택 사항) 보기가 만들어진 후 보기의 이름을 바꾸려면 보기 드롭다운 메뉴를 클릭한 다음 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png) > **이름 바꾸기**&#x200B;를 클릭하여 보기 이름을 업데이트합니다

   또는

   보기 이름을 두 번 클릭하고 새 이름을 입력하십시오.  <!--ensure there is not another saving step here?!-->

1. <span class="preview">(선택 사항) **전체 화면** 아이콘 ![전체 화면 열기 아이콘](assets/open-full-screen-icon.png)을 클릭하여 전체 화면에서 보기를 연 다음 **전체 화면 종료** 아이콘 ![전체 화면 종료 아이콘](assets/exit-full-screen-icon.png) 또는 키보드에서 Esc 키를 눌러 전체 화면을 종료합니다.  </span>

1. (선택 사항) 특정 유형의 보기를 관리하려면 다음 문서를 참조하십시오.

   * [표 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [타임라인 보기 관리](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [달력 보기 관리](/help/quicksilver/planning/views/manage-the-calendar-view.md)

## 보기에서 실시간 현재 상태 표시기 활성화

보기의 실시간 상태 표시기를 따라 다른 사용자가 사용자와 동시에 레코드를 편집하고 있는지 확인할 수 있습니다.

기본적으로 모든 레코드 보기의 오른쪽 위 모서리에 표시함과 동시에 레코드 정보를 편집하는 다른 사용자의 아바타입니다.

표 보기를 표시할 때 레코드를 볼 때 다른 사용자가 편집하고 있는 필드를 볼 수도 있습니다.

자세한 내용은 [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)를 참조하십시오.



<!--## Add a view as a favorite - this is not possible yet-->
