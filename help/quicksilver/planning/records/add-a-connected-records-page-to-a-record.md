---
title: 레코드에 연결된 레코드 페이지 추가
description: 연결된 레코드 페이지에 대한 탭을 레코드에 추가하여 연결된 레코드 또는 개체에서 정보를 볼 수 있습니다. 이렇게 하면 테이블 보기의 연결된 레코드가 탭에 추가됩니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 6aba4316228a320cf33e419249a64b3cf56e8f39
workflow-type: tm+mt
source-wordcount: '1513'
ht-degree: 1%

---


# 레코드에 연결된 레코드 페이지 추가

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

연결된 레코드 페이지에 대한 탭을 레코드에 추가하여 연결된 레코드 또는 개체에서 정보를 볼 수 있습니다. 이렇게 하면 테이블 보기의 연결된 레코드가 탭에 추가됩니다.

레코드에 연결된 레코드 페이지를 추가할 때는 다음 사항을 고려하십시오.

* 레코드 유형의 테이블 보기에서 레코드나 개체 유형을 레코드 유형에 연결한 후 연결된 레코드 페이지를 레코드에 추가할 수 있습니다.

* 레코드의 미리 보기 영역 또는 레코드 페이지에서 연결된 레코드 페이지를 추가할 수 있습니다.

* 연결된 레코드 페이지에는 연결된 개체나 한 개체 또는 레코드 종류의 레코드만 표시됩니다. 페이지에 해당 유형의 모든 레코드가 표시되지 않습니다.

* 테이블 보기에서 연결된 레코드 페이지에 개체를 표시할 수 있습니다.

<!--replace the above bullet with this: 

* You can display the objects in a connected records page in the following types of views:

   * Table
   * <span class="preview">Timeline</span>
   * <span class="preview">Calendar</span>
-->

* 다음과 같은 연결된 레코드 또는 객체 유형에 대해 연결된 레코드 페이지를 추가할 수 있습니다.

   * Workfront Planning 레코드 유형
   * Workfront 프로젝트, 프로그램, 포트폴리오, 그룹 또는 회사. Workfront에서 연결된 Workfront 개체에 액세스할 수 있는 권한이 없는 경우에도 연결된 개체를 볼 수 있습니다.

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
<p>모든 Workfront 및 모든 Planning 패키지</p>
<p>모든 워크플로우 및 모든 Planning 패키지</p>
<p>각 Workfront Planning 패키지에 포함된 내용에 대한 자세한 내용은 Workfront 계정 담당자에게 문의하십시오. </p> 
   </td> 
<tr>
<td> 
   <p> 추가 제품</p> </td> 
   <td> 
   <p> Adobe Workfront 외에 다음 응용 프로그램의 개체에 대해 연결된 레코드 페이지를 추가하려면 다음 항목이 있어야 합니다.</p>
   <ul><li><p>AEM 에셋을 Planning 레코드 유형과 연결하기 위한 AEM Assets 및 Workfront 간의 통합 및 Adobe Experience Manager Assets 라이선스.</p>
   <p>자세한 내용은 <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Experience Manager Assets 및 Assets Essentials용 Adobe Workfront: 기사 색인</a>을 참조하십시오. </p></li>
   <li><p> 레코드 유형을 GenStudio 브랜드와 연결하는 Adobe GenStudio for Performance Marketing 라이선스</p>
   <p>자세한 내용은 <a href="https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/get-started">Adobe GenStudio for Performance Marketing 시작</a>을 참조하세요.</p></li></ul>
   </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>표준</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>개체 권한</p></td>
   <td>
   <p>작업 공간 및 레코드 유형에 대한 또는 그 이상의 권한 기여 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p> 
  </td>
  </tr>   
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++   

## 레코드에 연결된 레코드 페이지 추가

연결된 레코드 페이지를 레코드에 추가하기 전에 먼저 레코드 유형을 다른 레코드 또는 개체 유형과 연결해야 합니다.

1. 레코드 이름을 클릭하여 레코드 유형 페이지의 모든 보기에서 엽니다.
1. 다음 영역 중 하나에서 **페이지 추가**&#x200B;를 클릭합니다.

   * 레코드의 미리 보기 창
   * 미리 보기 페이지의 오른쪽 상단에 있는 **새 탭에서 열기** 아이콘 ![새 탭에서 세부 정보 열기](assets/open-details-in-a-new-tab-icon.png)을 클릭한 후 레코드의 세부 정보 페이지.

   **페이지 만들기** 상자가 열립니다.

   ![연결된 레코드 추가 페이지 모달](assets/add-connection-view-page-modal.png)

1. **페이지 이름**&#x200B;을(를) 추가하고 **연결된 레코드 페이지**&#x200B;을(를) 클릭한 다음 **만들기**&#x200B;를 클릭합니다.

   연결된 새 레코드 페이지가 레코드의 페이지에 새 탭으로 추가됩니다.

   현재 레코드에 연결된 레코드가 테이블 뷰에 표시됩니다.

   >[!TIP]
   >
   >연결된 레코드를 연결된 레코드 페이지에 표시하려면 먼저 레코드의 테이블 또는 세부 정보 영역에 연결된 레코드를 추가해야 합니다.

   <!--All fields of the connected record display in the table view of the connected record's tab.-->

   연결된 레코드의 처음 5개 필드는 기본적으로 표시됩니다. <!--No lookup fields display by default.-->

   ![캠페인 세부 정보 아래의 대상자 연결 테이블 보기](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (선택 사항) 연결된 레코드 또는 개체 유형의 이름을 클릭하거나 목록에서 해당 이름을 검색한 다음 목록에 표시될 때 클릭합니다.

1. (선택 사항 및 조건부) 테이블 보기 또는 레코드의 세부 정보 페이지에 표시되는 연결된 필드가 두 개 이상 있는 경우 연결된 레코드 페이지에 표시할 레코드가 있는 필드를 클릭합니다.

   선택한 연결된 레코드 유형의 테이블 보기가 연결된 레코드 페이지에 추가됩니다.

1. (선택 사항 및 조건부) 연결된 Planning 레코드에 대해 연결된 레코드 페이지를 만들 때 다음 중 하나를 수행합니다. <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

   * 레코드 이름을 클릭합니다. 새 탭에서 레코드 페이지가 열립니다.
   * 기존 레코드를 연결하려면 테이블 보기 아래쪽에 있는 **연결**&#x200B;을 클릭하고 연결 상자에서 선택한 다음 상자 바깥쪽을 클릭하여 닫습니다. 레코드는 자동으로 표에 추가됩니다. 레코드를 추가하려면 먼저 해당 레코드가 있어야 합니다.

   자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하세요.
   * 테이블 보기에서 인라인으로 연결된 레코드의 모든 정보를 편집합니다.

   * 연결된 레코드의 이름을 마우스로 가리킨 다음 **추가** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭합니다

     또는

     레코드 중 하나를 선택한 다음 목록 하단의 파란색 막대에서 다음 옵션 중 하나를 클릭합니다.

      * 새 탭에서 레코드 페이지를 열려면 **보기**
      * 레코드 페이지에 대한 링크를 복사하려면 **링크 복사**
      * **축소판 편집**: **레코드 축소판** 상자를 열고 레코드의 축소판 이미지를 편집합니다.
      * **복제**&#x200B;하여 연결된 레코드를 복제합니다. 복제된 레코드는 현재 레코드에도 연결됩니다.
      * **위 또는 아래에 레코드를 삽입**&#x200B;하여 연결된 레코드 형식에 새 레코드를 추가합니다. 여기에 추가된 새 레코드도 현재 레코드와 연결됩니다. 이 옵션은 테이블에서 레코드를 선택할 때 파란색 막대에서 사용할 수 없습니다.
      * 레코드를 삭제하려면 **삭제**&#x200B;하십시오. 연결된 레코드를 삭제하면 레코드 종류 및 레코드가 연결된 모든 위치에서 해당 레코드가 삭제됩니다.

        표 보기에서 레코드를 편집하는 방법에 대한 자세한 내용은 [레코드 편집](/help/quicksilver/planning/records/edit-records.md)을 참조하십시오.

        >[!TIP]
        >
        >둘 이상의 레코드 또는 개체를 선택하여 삭제할 수 있습니다.

   * 연결된 레코드 페이지의 표에 있는 모든 Planning 레코드를 인라인 편집합니다.

1. (선택 사항 및 조건부) 다음 Workfront 개체 유형에 대해 연결된 레코드 페이지를 만들 때:

   * 포트폴리오
   * 프로그램
   * 그룹
   * 회사

   연결된 레코드 페이지의 표 보기에서 다음 중 하나를 수행합니다.

   * 개체의 이름을 클릭합니다. 그러면 새 탭에서 개체의 페이지가 열립니다.
   * 기존 개체를 연결하려면 표 보기 아래쪽에 있는 **연결**&#x200B;을 클릭하고 연결 상자에서 선택한 다음 상자 바깥쪽을 클릭하여 닫습니다. 객체는 자동으로 테이블에 추가됩니다. 개체를 추가하려면 먼저 개체가 있어야 합니다.

   자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하세요.

   * 테이블 뷰에서 객체 중 하나를 선택한 다음 목록 하단의 파란색 막대에서 다음 옵션 중 하나를 클릭합니다.

   * 새 탭에서 레코드 페이지를 열려면 **보기**
   * 레코드 페이지에 대한 링크를 복사하려면 **링크 복사**
   * 현재 보고 있는 레코드에서 개체의 연결을 끊으려면 **연결을 끊습니다**.

   >[!TIP]
   >
   >두 개 이상의 레코드 또는 개체를 선택하여 연결을 끊을 수 있습니다.

1. (선택 사항 및 조건부) 연결된 Workfront 프로젝트에 대해 연결된 레코드 페이지를 만들 때:

   * 연결된 레코드 페이지의 오른쪽 상단에서 **레코드 연결**&#x200B;을 클릭하여 기존 프로젝트를 연결합니다.

   자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하세요.
   * 테이블에서 프로젝트 정보를 인라인 편집합니다.
   * 템플릿 없이 프로젝트를 만들려면 **새 행**&#x200B;을 클릭하세요. 새 프로젝트가 현재 레코드에 즉시 연결됩니다.

     자세한 내용은 [레코드에 연결할 때 Workfront Planning에서 Workfront 개체 만들기](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)를 참조하십시오.
   * 프로젝트 위로 마우스를 가져간 후 **추가** 메뉴를 클릭합니다. [추가 메뉴](assets/more-menu.png)

     또는

     프로젝트를 하나 이상 선택하고 목록 하단의 파란색 막대를 확인한 후 다음 중 하나를 클릭합니다.

      * 프로젝트를 삭제하려면 **삭제**&#x200B;하십시오. 프로젝트를 삭제하면 레코드에서 연결이 끊기고 Workfront의 휴지통으로 이동합니다.
      * 레코드에서 프로젝트의 연결을 끊으려면 **연결을 끊습니다**. 프로젝트의 연결을 해제하면 현재 레코드에서 해당 프로젝트와 해당 조회 필드의 모든 값이 제거됩니다.

     >[!TIP]
     >
     >연결을 끊거나 삭제할 프로젝트를 두 개 이상 선택할 수 있습니다.
   * 테이블 보기의 오른쪽 위 모서리에 있는 **+** 아이콘을 클릭하여 기존 필드를 테이블에 추가합니다. 필드를 추가하려면 먼저 해당 필드가 있어야 합니다.

     **열 관리자** 상자가 열립니다. 다음을 수행합니다.

      1. **사용 가능** 열에서 기존 개체 필드를 검색한 다음 필드 이름 오른쪽의 **+**&#x200B;을(를) 클릭하여 **선택됨** 열에 추가합니다.

         선택한 필드가 연결된 레코드 페이지의 표 보기에 추가됩니다.
      1. 테이블 보기에서 제거하려면 **선택됨** 열의 필드 오른쪽에 있는 **-**&#x200B;을(를) 클릭합니다.
      1. **저장**&#x200B;을 클릭하여 연결된 레코드 페이지 테이블 보기를 저장합니다.

1. (선택 사항) **연결된 레코드 페이지** 탭의 이름을 두 번 클릭합니다

   또는

   탭 이름을 마우스로 가리킨 다음 **자세히** ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **이름 바꾸기**&#x200B;를 클릭하여 새 연결된 보기 탭으로 이름을 바꿉니다.
1. (선택 사항) 연결된 레코드 페이지의 도구 모음에서 다음 보기 요소를 사용하여 테이블 보기를 관리합니다.

   * 필터
   * 정렬. 프로젝트에는 사용할 수 없습니다.
   * 그룹화. 프로젝트에는 사용할 수 없습니다.
   * 열, 필드 표시, 숨기기 또는 재배열
   * 행 높이. 프로젝트에는 사용할 수 없습니다.
   * 검색

   자세한 내용은 [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)를 참조하십시오.

   >[!NOTE]
   >
   >연결된 레코드 탭의 표 보기에서 필드를 만들거나 편집하거나 삭제할 수 없습니다.

   <!--1. <span class="preview">(Optional) Click the dropdown menu to the right of the view name, then click **New view** to add a view. For more information, see the section [Manage multiple views from the connected records page](#manage-multiple-views-from-the-connected-records-page) in this article. </span>-->

1. (선택 사항) 연결된 레코드 페이지 탭의 이름을 마우스로 가리키고 **자세히** ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **삭제**&#x200B;를 클릭하여 탭으로 제거합니다.

<!--
<div class="preview">

## Manage multiple views from the connected records page

You can add and manage multiple view types from the connected records page of a record. 

The views you create in the Connected records page of a record type are available everywhere in Workfront Planning where that record type page displays. Views created for the same record type anywhere else in Workfront Planning are also accessible in all connected records pages of that record type. 

To manage multiple views from the connected records page: 

1. From the connected records page of a record, click the dropdown menu to the right of the view name, then click **New view** to add a view, then select from the following options: 

   * **Table**. For more information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 
   * **Timeline**. For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).
   * **Calendar**. For more information, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md). 

1. (Optional) Hover over the name of a view in the Connected records page, then click the **More** menu ![More menu](assets/more-menu.png), then click one of the following: *************check to make sure these are all possible*********

   * **Rename**
   * **Share**. For more information, see [Share views](/help/quicksilver/planning/access/share-views.md).

   >[!TIP]
   >
   >Sharing views from Connected records pages makes them accessible to users in all areas of Workfront Planning where the view displays. 
   >Also, if a view is shared from any other area of Workfront Planning, it is also available to the same users in Connected records pages. 

   * **Export** 
   * **Duplicate**. For more information, see [Duplicate record views](/help/quicksilver/planning/views/duplicate-record-views.md).

      >[!TIP]
      >
      >Duplicating a view from Connected records pages makes it available in all other areas of Workfornt planning, when viewing the same record types. 

</div> -->