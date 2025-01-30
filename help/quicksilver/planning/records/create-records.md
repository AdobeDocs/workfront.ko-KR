---
title: 레코드 만들기
description: Adobe Workfront Planning을 사용할 때 레코드는 레코드 유형의 인스턴스입니다. 테이블 보기에 수동으로 추가하거나, 목록에서 가져오거나, 복제하거나, 다른 레코드에 연결할 때 만들어 Workfront Planning에서 각 레코드 유형에 대한 고유한 레코드를 만들 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 928ea5da9955b8c1c98782df81698c49987d4c18
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 레코드 만들기

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Adobe Workfront Planning에서 레코드는 레코드 유형의 인스턴스입니다.

다음 중 하나를 수행하여 레코드를 만들 수 있습니다.

* [테이블 보기의 레코드 유형 페이지에서 레코드 추가](#create-records-by-adding-them-to-a-record-type-in-a-record-type-table)
* [외부 목록에서 레코드 목록 복사 및 붙여넣기](#create-records-by-copying-and-pasting-them-from-an-external-list)
* [테이블 보기에서 레코드 복제](#create-records-by-duplicating-them)
* [다른 레코드와 연결할 때 레코드 만들기](#create-records-as-you-connect-them)
* [요청 양식을 레코드 유형으로 제출하여 만듭니다.](#create-records-by-submitting-a-request-form-to-a-record-type)
* [CSV 또는 Excel 파일에서 레코드 유형을 가져올 때 레코드 만들기](#create-records-when-importing-record-types-from-a-csv-or-excel-file)


테이블 또는 타임라인 보기에서 레코드 관리에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [표 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)
* [타임라인 보기 관리](/help/quicksilver/planning/views/manage-the-timeline-view.md)

## 액세스 요구 사항

+++ 를 확장하여 Workfront Planning에 대한 액세스 요구 사항을 봅니다.

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
   <td role="rowheader"><p>Adobe Workfront 계획 패키지*</p></td> 
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
   <td> 표준
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p> 
   <p>레코드를 연결할 때 만들려는 개체 유형(프로젝트 및 포트폴리오)에 대한 Workfront의 액세스 권한을 편집합니다. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td> <p>레코드를 추가할 작업 영역에 대한 권한을 관리합니다. </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
   <p>하위 개체(프로젝트)를 추가하기 위해 Workfront 개체(포트폴리오)에 대한 권한을 관리합니다.</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>레이아웃 템플릿</p></td> 
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다 </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 레코드 유형 테이블의 레코드 유형에 추가하여 레코드 만들기

레코드 유형 페이지의 표 보기에서 레코드를 만들 수 있습니다.

레코드 정보 편집에 대한 자세한 내용은 [레코드 편집](/help/quicksilver/planning/records/edit-records.md)을 참조하세요.

{{step1-to-planning}}

1. 레코드를 추가할 작업 영역을 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다. 레코드 종류 만들기에 대한 자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

   마지막으로 액세스한 보기에서 레코드 유형 페이지가 열립니다. 기본적으로 레코드 유형 페이지가 표 뷰에 열립니다.
선택한 유형의 모든 레코드가 뷰에 표시됩니다.

1. (조건부) 표시되는 보기에 따라 다음 중 하나를 수행합니다.

   * 테이블 보기에서:

      * 테이블의 마지막 행에서 **새 레코드**&#x200B;을(를) 클릭합니다.

      * 표의 열 또는 행에서 키보드에서 **Shift + Enter**&#x200B;를 클릭합니다. 이렇게 하면 시작한 레코드 아래에 빈 행이 추가됩니다.
      * 레코드의 기본 필드 위에 마우스를 가져다 대고 필드 오른쪽에 있는 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 다음 **위에 레코드 삽입** 또는 **아래에 레코드 삽입**&#x200B;을(를) 클릭합니다.

     ![](assets/adding-a-new-campaign-in-table-row.png)

   * 모든 보기에서:

      * 페이지의 오른쪽 상단에 있는 **새 레코드**&#x200B;을(를) 클릭합니다. 레코드 미리 보기 상자가 열립니다.

     Workfront은 각 새 레코드에 썸네일과 표지 이미지를 자동으로 업로드합니다. 나중에 이러한 이미지를 수정할 수 있습니다. 자세한 내용은 다음 문서를 참조하십시오.

      * [레코드에 표지 이미지 추가](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
      * [레코드에 썸네일 추가](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

1. 미리 보기 상자에 표시되는 필드에 새 레코드에 대한 정보를 입력하십시오.

   >[!NOTE]
   >
   >  * 레코드에 대한 필수 필드가 없습니다. 그러나 레코드를 서로 연결할 때 레코드를 식별하는 데 도움이 되므로 레코드의 기본 필드에 대한 정보를 추가하는 것이 좋습니다. 기본 필드에 대한 자세한 내용은 [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md) 및 [기본 필드 개요](/help/quicksilver/planning/fields/primary-field-overview.md)를 참조하십시오.
   >
   >  * 다른 레코드 종류 또는 계산된 필드를 참조하는 필드는 읽기 전용 필드입니다.

1. (조건부) 표에 레코드를 추가할 때 각 행에 정보를 계속 추가한 다음 키보드에서 **Enter**&#x200B;를 클릭하여 변경 내용을 저장합니다.

   또는

   새 레코드 이름 또는 레코드 이름 왼쪽에 있는 **세부 정보 열기** 아이콘 ![](assets/open-details-icon-in-table-name-field.png)을(를) 클릭합니다. 레코드의 세부 정보가 포함된 미리보기가 테이블에 열립니다.

   >[!TIP]
   >
   >이름 필드가 기본 필드인 경우 레코드의 이름 필드에서만 **세부 정보 열기** 아이콘에 액세스할 수 있습니다.

1. 레코드 미리 보기에서 레코드 정보 편집을 시작합니다. Workfront은 변경 사항을 자동으로 저장합니다.
1. (선택 사항) 레코드 미리 보기의 오른쪽 상단에 있는 **새 탭에서 열기** 아이콘 ![](assets/open-details-in-a-new-tab-icon.png)을(를) 클릭하여 새 탭에서 레코드 페이지를 엽니다. 레코드 페이지에서 레코드 편집을 계속합니다. 자세한 내용은 [레코드 편집](/help/quicksilver/planning/records/edit-records.md)을 참조하세요.

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

## 외부 목록에서 복사하여 붙여 넣어 레코드 만들기

1. 이 문서의 [레코드 형식에 수동으로 추가하여 레코드 만들기](#create-records-by-manually-adding-them-to-a-record-type) 섹션에 설명된 대로 테이블 보기에서 레코드 만들기를 시작합니다.

   테이블 뷰에 새 레코드 정보로 채울 열(또는 필드)이 있는지 확인합니다.

1. 테이블의 마지막 행에서 **새 &lt; 레코드 유형 이름 >**&#x200B;을(를) 클릭하여 새 레코드를 원하는 만큼 테이블에 새 행을 추가합니다.

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

## 복제하여 레코드 만들기

레코드 복제에 대한 자세한 내용은 [레코드 복제](/help/quicksilver/planning/records/copy-or-duplicate-records.md)를 참조하십시오.

## 연결할 때 레코드 만들기

다른 레코드에서 연결할 때 다음 개체 유형을 만들 수 있습니다.

* Workfront 계획 레코드
* Workfront 개체

이 섹션에서는 다른 레코드에서 연결할 때 Workfront Planning 레코드를 만드는 방법에 대해 설명합니다.

>[!NOTE]
>
>Workfront 프로젝트 및 포트폴리오를 Workfront Planning 레코드에 연결할 때 만드는 것은 다른 레코드에서 연결할 때 Planning 레코드를 만드는 것과 비슷합니다.
>
>Workfront Planning에서 Workfront 개체를 만드는 방법에 대한 자세한 내용은 [Workfront Planning에서 Workfront 개체 만들기](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)를 참조하십시오.

기존 레코드에서 새 레코드를 연결하여 추가하려면 먼저 다음 항목이 있어야 합니다.

* 연결된 레코드 종류. 자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.
* 레코드.
* 이 문서의 [액세스 요구 사항](#access-requirements) 섹션에 설명된 대로 Workfront Planning 및 Workfront의 올바른 액세스 및 권한.

다른 레코드에서 연결할 때 레코드를 만들려면 다음 작업을 수행하십시오.

1. [레코드 연결](/help/quicksilver/planning/records/connect-records.md) 문서에 설명된 대로 Workfront Planning 레코드 연결을 시작합니다. Workfront Planning의 다음 영역에 있는 연결 필드에서 레코드를 연결할 수 있습니다.

   * 테이블 보기
   * 레코드의 세부 정보 페이지 또는 미리보기 상자

1. (조건부) 다른 레코드의 연결된 레코드 필드에서 레코드를 추가하려고 할 때 해당 레코드를 찾을 수 없으면 레코드를 검색한 다음 **+ 추가**&#x200B;를 클릭합니다. **+ 추가** 단추 다음에 연결 중인 레코드 형식의 이름이 옵니다. 예: 기존 캠페인에 브랜드를 추가할 때 &quot;브랜드 추가&quot; 입력한 이름도 [추가] 단추 다음에 표시됩니다.

   <!--remove the first part of the step above to say just Click Add when the button will be persistent, for preview and production-->

   ![](assets/add-button-to-create-records-in-context-highlighted.png)

   레코드가 생성되고 연결된 레코드 필드에 추가됩니다.

   <!--
    >[!IMPORTANT]
    >
    >* You can create only projects and portfolios in Workfront when connecting them from a record. 
    >
    >* You cannot create programs, groups, or companies when connecting them from a record in Workfront Planning. 
    >
    >* You cannot create a project from a template when when you create projects by connecting them from a record. You must manually add tasks and project information or a template to the new project after you add it to the record. -->

1. (선택 사항) 레코드를 생성한 레코드 유형의 테이블 뷰로 이동합니다. 새 레코드가 보기의 마지막 행에 표시됩니다.
1. (선택 사항) 테이블 보기에서 새 레코드에 대한 정보 추가를 시작합니다
또는
세부 정보 페이지를 열고 정보를 추가하려면 해당 이름을 클릭합니다.

## 요청 양식을 레코드 유형으로 제출하여 레코드 생성

다른 사용자가 레코드 유형에 대한 요청 양식을 만들고 링크를 공유하면 해당 레코드 유형에 대한 레코드를 만드는 요청을 제출할 수 있습니다.

자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.

Workfront 사용자와 조직 외부의 사용자 모두 요청 양식에 대한 링크가 있는 경우 Planning 레코드 유형에 요청을 제출하고 레코드를 만들 수 있습니다.

자세한 내용은 [레코드를 만들도록 Adobe Workfront Planning 요청 제출](/help/quicksilver/planning/requests/submit-requests.md)을 참조하십시오.

## CSV 또는 Excel 파일에서 레코드 유형을 가져올 때 레코드 만들기

CSV 또는 Excel 파일을 사용하여 레코드 유형을 가져올 때 레코드를 가져올 수 있습니다.

자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

