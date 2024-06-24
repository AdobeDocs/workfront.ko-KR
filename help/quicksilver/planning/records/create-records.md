---
title: 레코드 만들기
description: Adobe Workfront Planning을 사용할 때 레코드는 레코드 유형의 인스턴스입니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: f5430d81f1914a3717130de3af54b4b84e0e2d06
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 레코드 만들기

{{planning-important-intro}}

Adobe Workfront Planning에서 레코드는 레코드 유형의 인스턴스입니다.

다음 중 하나를 수행하여 레코드를 만들 수 있습니다.

* 레코드 유형에 대해 수동으로 만들기
* 외부 목록에서 정보를 복사하여 붙여 넣어 레코드를 만듭니다.

이 문서에서는 레코드를 만드는 방법을 설명합니다. 테이블 또는 타임라인 보기에서 레코드 관리에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [표 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)
* [타임라인 보기 관리](/help/quicksilver/planning/views/manage-the-timeline-view.md)

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
   <p>현재: 플랜</p>  
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Adobe Workfront Planning에 대한 액세스 제어가 없습니다. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 영역에 대한 상위 권한 기여</a> </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 계획 영역을 추가해야 합니다. 자세한 내용은 <a href="/help/quicksilver/planning/access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*자세한 내용은 [Workfront 설명서에 대한 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/planning/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 수동으로 레코드 유형에 추가하여 레코드 만들기 <!--in a record type table (I don't think you can create them elsewhere right now)-->

레코드 유형 페이지의 표 보기에서 레코드를 만들 수 있습니다.

레코드 정보 편집에 대한 자세한 내용은 [레코드 편집](/help/quicksilver/planning/records/edit-records.md).

{{step1-to-planning}}

1. 레코드를 추가할 작업 영역을 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다. 레코드 종류 만들기에 대한 내용은 [레코드 유형 만들기](/help/quicksilver/planning/architecture/create-record-types.md).

   마지막으로 액세스한 보기에서 레코드 유형 페이지가 열립니다. 기본적으로 레코드 유형 페이지가 표 뷰에 열립니다.
선택한 유형의 모든 레코드가 뷰에 표시됩니다.

1. (조건부) 표시되는 보기에 따라 다음 중 하나를 수행합니다.

   * 테이블 보기에서:

      * 클릭 **새 레코드** 테이블의 마지막 행에서

      * 클릭 **Shift + Enter** 표의 열 또는 행에서 키보드에 있는 경우 빈 행이 표시됩니다.

     ![](assets/adding-a-new-campaign-in-table-row.png)

   * 모든 보기에서:

      * 클릭 **새 레코드** 페이지의 오른쪽 상단 모서리에서 을 참조하십시오. 레코드 미리 보기 상자가 열립니다.

     Workfront은 각 새 레코드에 썸네일과 표지 이미지를 자동으로 업로드합니다. 나중에 이러한 이미지를 수정할 수 있습니다. 자세한 내용은 다음 문서를 참조하십시오.

      * [레코드에 표지 이미지 추가](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
      * [레코드에 썸네일 추가](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

1. 미리 보기 상자에 표시되는 필드에 새 레코드에 대한 정보를 입력하십시오.

   >[!NOTE]
   >
   >  * 레코드에 대한 필수 필드가 없습니다. 그러나 레코드를 서로 연결할 때 레코드를 식별하는 데 도움이 되므로 레코드의 기본 필드에 대한 정보를 추가하는 것이 좋습니다. 기본 필드에 대한 자세한 내용은 [표 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md) 및 [기본 필드 개요](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * 다른 레코드 종류 또는 계산된 필드를 참조하는 필드는 읽기 전용 필드입니다.

1. (조건부) 테이블에서 레코드를 추가할 때 각 행에 대한 정보를 계속 추가한 다음 을 클릭합니다 **입력** 키보드에서 을(를) 클릭하여 변경 내용을 저장합니다.

   또는

   새 레코드의 이름 또는 **세부 정보 열기** 아이콘 ![](assets/open-details-icon-in-table-name-field.png) 레코드 이름 왼쪽에 있습니다. 레코드의 세부 정보가 포함된 미리보기가 테이블에 열립니다.

   >[!TIP]
   >
   >다음에 액세스할 수 있습니다. **세부 정보 열기** ( 이름 필드가 기본 필드인 경우 레코드의 이름 필드에서만) 아이콘으로 표시됩니다.

1. 레코드 미리 보기에서 레코드 정보 편집을 시작합니다. Workfront은 변경 사항을 자동으로 저장합니다.
1. (선택 사항) **새 탭에서 열기** 아이콘 ![](assets/open-details-in-a-new-tab-icon.png) 레코드 미리 보기의 오른쪽 상단 모서리에서 새 탭에서 레코드 페이지를 엽니다. 레코드 페이지에서 레코드 편집을 계속합니다. 자세한 내용은 [레코드 편집](/help/quicksilver/planning/records/edit-records.md).

1. (선택 사항) 다음 키보드 단축키를 사용하여 표 보기에서 새 레코드 또는 해당 정보를 추가할 때 해당 추가 작업을 취소하거나 다시 실행합니다.

   * CTRL+Z(Mac의 경우 ⌘+Z)
   * 변경 내용을 재실행하려면 CTRL+Shift+Z(Mac의 경우 ⌘+Shift+Z)

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    The following items are created in Workfront Planning:

    * A read-only record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Planning record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Planning records you're linking from. 
   
-->

## 외부 목록에서 정보를 복사하여 붙여 넣어 레코드 만들기

1. 섹션에 설명된 대로 테이블 보기에서 레코드 만들기를 시작합니다. [수동으로 레코드 유형에 추가하여 레코드 만들기](#create-records-by-manually-adding-them-to-a-record-type) 이 문서에서.

   테이블 뷰에 새 레코드 정보로 채울 열(또는 필드)이 있는지 확인합니다.

1. 클릭 **새로 만들기 &lt; 레코드 유형 이름 >** 테이블의 마지막 행에 새 레코드를 원하는 만큼 추가합니다.

   예를 들어 다른 응용 프로그램에서 10개의 새 레코드에 대한 정보를 붙여넣으려면 10개의 행을 테이블 보기에 추가합니다.

1. 다른 응용 프로그램에서 가져올 레코드 목록을 만듭니다.

   예를 들어 Excel 스프레드시트를 사용하여 목록을 만들 수 있습니다.

   목록에는 표 형식의 정보가 포함되어야 합니다.

   >[!TIP]
   >
   > 목록의 열에는 Workfront에 있는 기존 필드에 대한 정보가 포함되어야 합니다.
   >
   > 원하는 필드가 Workfront에서 이미 만들어져 있고 시트의 정보가 Workfront의 각 필드와 일치하는 올바른 형식으로 표시되는지 확인하십시오.

1. 다른 응용 프로그램에서 여러 행과 열을 선택한 다음 첫 번째 새 레코드부터 시작하여 레코드 유형 테이블 보기에 정보를 붙여 넣습니다.

   Workfront 계획 영역에 다음 정보를 가져옵니다.

   * 행에는 새 레코드가 포함됩니다
   * 열은 레코드의 필드에 대한 정보를 채웁니다.
