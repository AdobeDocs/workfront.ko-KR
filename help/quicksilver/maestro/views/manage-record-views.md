---
title: 레코드 보기 관리
description: Adobe Maestro를 사용할 때 테이블이나 타임라인 보기에서 레코드를 표시할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 74db651f8865965f943bc89e58e7130cffe0c450
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 1%

---

# 레코드 보기 관리

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

Adobe Maestro에서 레코드 유형을 선택한 후 다음 보기에서 해당 유형의 모든 레코드를 표시할 수 있습니다.

* 테이블

  자세한 내용은 [표 보기 관리](../views/manage-the-table-view.md).
* 타임라인

  자세한 내용은 [타임라인 보기 관리](../views/manage-the-timeline-view.md).

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
   <p> Adobe 제품</p> </td>
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
   <td role="rowheader">액세스 수준</td>
   <td> <p>임의</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">레이아웃 템플릿</td>
   <td> <p>시스템 관리자가 레이아웃 템플릿에 마에스트로 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


<!--
When we release permissions to views:

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
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader">Access level configurations</td>
   <td> <p>There are no access controls for Maestro objects</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td> <p>Manage permissions to the view</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

-->


## Maestro 보기 작업 시 고려 사항

* Maestro의 보기는 레코드 유형별로 다릅니다. 동일한 보기를 두 개의 다른 레코드 유형에 적용할 수 없습니다.
* 만든 보기는 Maestro 영역에 액세스하는 모든 사람이 볼 수 있습니다. <!-- edit this when we have permissions and the views will be shared only to be visible by others-->
  <!-- this is not yet possible: * You can share views with others if you want them to also apply them to the same record types.-->
* 운영 레코드 유형에 대한 뷰 작성은 분류 레코드 유형에 대한 뷰 작성과 동일합니다.
* 보기를 수정하거나 삭제하면 Maestro 영역에 액세스할 수 있는 모든 사용자에 대해 수정 및 삭제됩니다.
* 다음 요소는 Maestro의 각 보기에 고유합니다.

   * 필터
   * 그룹화
   * 정렬

  <!-- some of these are not available in all of the views - edit above-->

  예를 들어, 테이블 보기에서 필터를 만들면 필터 결과는 선택한 보기에서만 볼 수 있고 보기 드롭다운 메뉴에 나열된 모든 보기에서는 볼 수 없습니다.

  >[!NOTE]
  >
  > Maestro는 현재 Beta 상태이므로 일부 보기 요소는 두 보기 모두에서 사용할 수 없을 수 있습니다.


이 문서에서는 Maestro 보기에 대한 다음 정보를 설명합니다.

* [보기 만들기 및 편집](#create-or-edit-record-views)
* [보기 삭제](#delete-views)
  <!--* [Duplicate a view](#duplicate-views)-->
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
  <!--* [Share a view](#share-views) - not possible yet-->

## 테이블 및 타임라인 보기의 유사점과 차이점

다음 표는 Maestro의 테이블 보기와 타임라인 보기 간의 유사점과 차이점을 보여 줍니다.

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| 기능 | 표 보기 | 타임라인 보기 |
|-----------------------------------------------------------------------|------------|---------------|
| 목록 또는 테이블에 레코드 표시 | ✓ 덧신 |              |
| 기본적으로 모든 필드를 테이블에 열로 표시 | ✓ 덧신 |              |
| 필드(또는 열) 숨기기 또는 표시 | ✓ 덧신 |               |
| 각 레코드의 필드 값 편집 | ✓ 덧신 |               |
| 보기에 새 행으로 레코드 추가 | ✓ 덧신 |               |
| 보기에 필드를 새 열로 추가 | ✓ 덧신 |               |
| 외부 목록에서 행을 복사하여 표에 붙여넣기 | ✓ 덧신 |               |
| 타임라인에 레코드 표시 |            | ✓ 덧신 |
| 레코드 필터링 | ✓ 덧신 | ✓ 덧신 |
| 그룹 레코드 |           | ✓ 덧신 |
| 레코드 정렬 | ✓ 덧신 |              |
| 색상 코드 레코드 |           | ✓ 덧신 |
| 색상 코드 그룹화 |           | ✓ 덧신 |
| 레코드 검색 | ✓ 덧신 | ✓ 덧신 |

<!--| Sort groupings                                                        | ✓          | ✓             |-->
<!--| Display a limited number of fields as columns, by default                      | ✓          |               |-->

## 보기 만들기 또는 편집 {#create-or-edit-views}

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-workfront.png) 오른쪽 상단 또는 **메인 메뉴** 아이콘 ![](assets/main-menu-shell.png) 왼쪽 위 모서리에서 사용 가능한 경우 을(를) 클릭합니다. **마에스트로** ![](assets/maestro-icon.png).
마지막으로 액세스한 작업공간은 기본적으로 열립니다. 작업 공간 만들기에 대한 자세한 내용은 [작업 공간 만들기](../architecture/create-workspaces.md).
1. 레코드 유형 카드를 클릭합니다. 레코드 종류 만들기에 대한 내용은 [레코드 유형 만들기](../architecture/create-record-types.md).

   기본적으로 선택한 유형의 모든 레코드가 테이블 뷰에 표시됩니다.

1. 다음을 클릭합니다. **보기** 드롭다운 메뉴를 사용하여 기존 메뉴 중 하나 선택 **표 보기** ![](assets/table-view-icon.png) 또는 클릭 **뷰 만들기 > 테이블** 테이블 뷰 생성하기

   또는

   기존 항목 선택 **타임라인 보기** ![](assets/timeline-view-icon.png) 보기 또는 클릭 **보기 만들기 > 타임라인** 을 클릭하여 타임라인 보기를 만듭니다.

   ![](assets/view-types-drop-down-from-record-type-list.png)

   >[!NOTE]
   >
   >    타임라인 보기를 만들려면, 보기를 만드는 레코드 종류에는 최소 두 개 이상의 날짜 필드가 있어야 합니다. 그렇지 않으면 [타임라인] 옵션이 흐리게 표시됩니다.

1. (선택 사항) 보기의 이름을 업데이트한 다음 **만들기** 저장하려고.

   기본적으로 Maestro는 &quot;Table &lt; number >&quot; 또는 &quot;Timeline &lt; number >&quot; 보기 이름을 지정합니다. 이 숫자는 자동으로 생성된 증가값입니다.

1. (선택 사항) 뷰를 만든 후 이름을 변경하려면 뷰 드롭다운 메뉴를 클릭한 다음, **자세히** 메뉴 ![](assets/more-menu.png) > **이름 바꾸기** 를 클릭하여 뷰 이름을 업데이트합니다. <!--ensure there is not another saving step here?!-->
1. (선택 사항) 보기를 관리하려면 다음 문서를 참조하십시오.

   * [표 보기 관리](../views/manage-the-table-view.md)
   * [타임라인 보기 관리](../views/manage-the-timeline-view.md)


<!--# Add a view as a favorite - this is not possible yet-->

<!-- ## Share views - not possible yet-->

## 보기 삭제

{{step1-to-maestro}}

마지막으로 액세스한 작업공간은 기본적으로 열립니다. 작업 공간 만들기에 대한 자세한 내용은 [작업 공간 만들기](../architecture/create-workspaces.md).

1. 레코드 유형 카드를 클릭합니다.

   레코드 종류 만들기에 대한 내용은 [레코드 유형 만들기](../architecture/create-record-types.md).

   기본적으로 선택한 유형의 모든 레코드가 테이블 뷰에 표시됩니다.

1. 보기 드롭다운 메뉴를 클릭하고 목록의 보기 중 하나를 마우스로 가리킨 다음, **자세히** 메뉴 ![](assets/more-menu.png) > **삭제**.
1. 클릭 **삭제** 확인할 수 있습니다. <!--ensure there is not another saving step here?!-->

   보기는 Maestro 영역에 액세스할 수 있는 모든 사용자에 대해 삭제되며 복구할 수 없습니다.

<!--not possible yet - August 30, 2023: 

## Duplicate views

If you want to keep multiple versions of a view and make slight changes between the version, you can duplicate a view. Duplicating a view creates identical copies of an existing view. 

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) to the right of the view name > **Duplicate**. (**********ensure there is not another saving step here?! also, add how this view is named; the button to duplicate was there but not the functionality yet************)
    
    The view is duplicated and visible to all users who can access the Maestro area. 

-->
