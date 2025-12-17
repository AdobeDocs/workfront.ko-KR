---
title: 레코드 페이지 레이아웃 관리
description: Adobe Workfront Planning에서 레코드 미리 보기 및 페이지의 레이아웃을 편집할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 5b1993d49ff675b3bab1d470bc756b987fe19d1c
workflow-type: tm+mt
source-wordcount: '1417'
ht-degree: 0%

---


# 레코드 페이지 레이아웃 관리

<!--
<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Adobe Workfront Planning에서 레코드 미리 보기 및 페이지의 레이아웃을 편집할 수 있습니다.

레코드 미리 보기는 레코드 유형 보기에 표시되는 레코드 페이지의 작은 보기입니다.

레코드 미리 보기 및 페이지의 레이아웃을 변경하면 변경 내용은 같은 유형의 모든 레코드의 미리 보기 상자 및 세부 정보 페이지에 영향을 미칩니다.

이 문서에서는 레코드 미리 보기 상자 또는 레코드 페이지의 레이아웃 및 모양을 변경하는 방법에 대해 설명합니다. 레코드 편집에 대한 자세한 내용은 [레코드 편집](/help/quicksilver/planning/records/edit-records.md)을 참조하세요.

레코드 페이지 편집을 시작하려면 먼저 레코드 종류 및 레코드를 만들어야 합니다.

자세한 내용은 다음 문서를 참조하십시오.

* [레코드 유형 만들기](/help/quicksilver/planning/architecture/create-record-types.md)

* [레코드 만들기](/help/quicksilver/planning/records/create-records.md)

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
<p>Any</p>
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
   <td>
   <p>Standard</p>
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
   <td>
   <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> 
  </td>
  </tr>
 </tbody>
</table>-->

## 레코드 페이지 작업에 대한 고려 사항

* 기본적으로 레코드의 세부 정보 페이지에는 레코드와 관련된 모든 필드가 표시됩니다.

* 미리보기 또는 세부 정보 페이지에서 레코드에 대한 새 필드를 추가할 수 없습니다. 미리 보기 및 세부 정보 페이지에 표시하려면 테이블 보기에서 새 필드를 추가해야 합니다.

* 레코드 미리 보기 또는 세부 정보 페이지에 섹션을 추가하여 일반적인 기준별로 정보를 구성하고 쉽게 찾을 수 있습니다.

* 다음 변경 사항은 동일한 유형의 모든 레코드에 영향을 미치며 해당 레코드에 액세스하는 모든 사용자가 볼 수 있습니다.

   * 필드 재정렬
   * 섹션 추가 또는 제거
   * 연결된 레코드 페이지 추가 또는 제거

* 레코드 미리 보기에서 변경한 내용은 레코드 세부 정보 페이지에 즉시 표시됩니다. 레코드 페이지에서 변경한 내용은 레코드 미리 보기 상자도 볼 수 있습니다.

* 레코드에 표지 이미지 또는 썸네일을 추가하는 것은 레코드 미리 보기 또는 페이지의 전체 레이아웃의 일부가 아닙니다. 각 레코드에 고유한 표지 이미지 또는 썸네일을 추가할 수 있습니다. 자세한 내용은 [레코드에 표지 이미지 추가](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) 및 [레코드에 썸네일 추가](/help/quicksilver/planning/records/add-thumbnails-to-records.md)를 참조하십시오.

* 다음 유형의 페이지를 레코드의 페이지에 추가할 수 있습니다.

   * 연결된 레코드 페이지

     자세한 내용은 [레코드에 연결된 레코드 페이지 추가](#add-a-connected-records-page-to-a-record) 섹션을 참조하십시오.

## 레코드 미리 보기 또는 페이지에 섹션 추가

레코드 페이지에 섹션을 추가할 때 다음 사항을 고려하십시오.

* 페이지에 포함할 수 있는 섹션 수에는 제한이 없습니다.
* 빈 섹션은 가질 수 없습니다. 섹션에 하나 이상의 필드가 있어야 합니다.
* 한 섹션에서 다른 섹션으로 필드를 끌어다 놓을 수 있습니다. 자세한 내용은 이 문서의 [레코드 미리 보기 또는 세부 정보 페이지에서 필드 다시 정렬](#rearrange-fields-in-the-record-preview-or-details-page) 섹션을 참조하십시오.
* 섹션에서 모든 필드를 제거하면 섹션이 자동으로 삭제되어 복구할 수 없습니다.

레코드 미리 보기 또는 페이지에 섹션을 추가하려면 다음 작업을 수행하십시오.

{{step1-to-planning}}

1. 작업 영역의 카드를 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.

1. 모든 유형의 보기에서 레코드 이름을 클릭합니다

   또는

   테이블 테이블 보기에서 첫째 열의 테이블 이름 필드에 있는 **세부 정보 열기** 아이콘 ![세부 정보 열기 아이콘](assets/open-details-icon-in-table-name-field.png)을 클릭합니다.

   레코드의 미리보기가 보기에서 열립니다.

   ![세부 정보 상자](assets/details-box.png)

1. (선택 사항) 레코드 미리 보기의 오른쪽 상단에 있는 **새 탭에서 열기** 아이콘 ![새 탭에서 세부 정보 열기](assets/open-details-in-a-new-tab-icon.png)을 클릭하여 새 탭에서 레코드 페이지를 엽니다.

   레코드 페이지가 열립니다. 기본적으로 세부 정보 탭이 열립니다.

   ![세부 정보 페이지](assets/details-page.png)

1. 레코드 미리 보기 또는 페이지의 **세부 정보** 탭에서 필드 왼쪽의 공백 위로 마우스를 가져간 다음 **섹션 추가** 아이콘 ![섹션 추가 아이콘](assets/add-section-icon.png)을 클릭하여 섹션을 추가합니다.
1. 섹션 이름 내부를 클릭하고 **제목 없는 섹션**&#x200B;을(를) 이름으로 바꾼 다음 Enter를 클릭합니다. 섹션 아래에 표시되는 필드는 자동으로 새 섹션의 일부입니다.
1. 이 문서의 [레코드 미리 보기 또는 세부 정보 페이지에서 필드 다시 정렬](#rearrange-fields-in-the-record-preview-or-details-page) 섹션에 설명된 대로 필드를 새 섹션으로 끌어다 놓습니다.

1. (선택 사항) 섹션 이름 위에 마우스를 놓고 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭합니다.

   ![레코드 페이지의 섹션에 대한 추가 메뉴 옵션](assets/more-menu-options-for-section-on-record-page.png)
1. (선택 사항) 다음 중 하나를 수행하여 섹션을 편집합니다.

   * 섹션 이름을 변경하려면 **이름 바꾸기**&#x200B;를 클릭하십시오.

     >[!TIP]
     >
     > 이름을 클릭하여 섹션의 이름을 인라인으로 바꿀 수 있습니다.

   * 섹션을 한 위치 위로 이동하려면 **위로 이동**&#x200B;을 클릭하십시오.

     또는

     섹션을 한 위치 아래로 이동하려면 **아래로 이동**&#x200B;을 클릭합니다.
섹션의 모든 필드가 섹션과 함께 이동합니다.

   * 섹션을 삭제하려면 **삭제**&#x200B;를 클릭하십시오. 섹션이 삭제되어 복구할 수 없습니다. 이 유형의 레코드에 액세스하는 모든 사용자가 더 이상 삭제된 섹션을 볼 수 없습니다.

1. 섹션 이름의 왼쪽에 있는 아래쪽 방향 화살표를 클릭하여 축소하거나 오른쪽 방향 화살표를 클릭하여 확장합니다.
기본적으로 모든 섹션이 확장되어 있습니다.

1. (선택 사항) 섹션 이름의 왼쪽에 있는 **그랩** 아이콘 ![그랩 아이콘](assets/grab-icon.png)을 클릭한 다음 원하는 위치에 끌어다 놓습니다.

   새 섹션 위치는 레코드를 보는 모든 사용자에 대해 동일한 유형의 모든 레코드의 미리보기 및 페이지에서 모두 업데이트됩니다.

   섹션과 필드 순서에 대한 모든 변경 사항은 자동으로 저장됩니다.

1. (선택 사항) **내보내기** 메뉴 ![레코드 세부 정보 페이지의 내보내기 아이콘](assets/export-icon-in-record-details-page.png)을 클릭하여 세부 정보 탭을 Word 또는 PDF 파일로 내보냅니다. 자세한 내용은 [레코드 세부 정보 내보내기](/help/quicksilver/planning/records/export-the-record-page.md)를 참조하십시오.

1. (선택 사항) **세부 정보** 탭 옆에 있는 **연결** 탭을 클릭합니다. **연결** 탭을 클릭하기 전에 **자세히**&#x200B;를 클릭해야 할 수 있습니다.

   선택한 레코드에 연결된 모든 레코드 또는 개체는 레코드 유형 또는 해당 레코드가 속한 응용 프로그램의 이름 아래에 표시됩니다.

   ![Workfront Planning의 레코드에 있는 연결 탭](assets/connections-tab-on-record-in-workfront-planning.png)

1. (선택 사항) [연결] 탭의 오른쪽 상단 모서리에서 **모든 레코드 표시** 설정을 선택합니다. 아직 연결된 레코드가 없는 레코드 종류를 포함하여 연결된 모든 레코드 종류가 표시됩니다. 기본적으로 토글이 선택 해제되고 연결된 레코드가 없는 레코드 유형이 숨겨집니다.

1. (선택 사항) 연결된 레코드 형식에 레코드를 더 추가하려면 **연결**&#x200B;을 클릭합니다. 자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하세요.

1. (선택 사항) 레코드 카드 위로 마우스를 가져간 다음 레코드 연결 끊기 아이콘 **-**&#x200B;을 클릭한 다음 **연결 끊기**&#x200B;를 클릭합니다. <!--this is copied to the Manage the Planning page in Workfront article; update in both articles-->
다음과 같은 상황이 발생합니다.
   * 레코드가 더 이상 Workfront 개체에 연결되어 있지 않습니다.
   * Workfront 개체는 Workfront Planning에서 레코드의 연결된 필드에서도 제거됩니다.
   * 계획 레코드에 연결된 Workfront 조회 필드의 값도 삭제됩니다.

## 레코드의 세부 정보 탭에서 필드 다시 정렬

{{step1-to-planning}}

1. 작업 영역의 카드를 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.

1. 모든 유형의 보기에서 레코드 이름을 클릭합니다

   또는

   테이블 테이블 보기에서 첫째 열의 테이블 이름 필드에 있는 **세부 정보 열기** 아이콘 ![세부 정보 열기 아이콘](assets/open-details-icon-in-table-name-field.png)을 클릭합니다.

   레코드의 미리보기가 보기에서 열립니다.

   ![세부 정보 상자](assets/details-box.png)

1. (선택 사항) 레코드 미리 보기의 오른쪽 상단에 있는 **새 탭에서 열기** 아이콘 ![새 탭에서 세부 정보 상자 열기](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it-->을 클릭하여 새 탭에서 레코드 페이지를 엽니다.

   레코드의 **세부 정보** 탭이 기본적으로 열립니다.

   ![세부 정보 페이지](assets/details-page.png)

1. 레코드 **세부 정보** 탭에서 필드 이름 왼쪽에 있는 **grab** 아이콘 ![Grab 아이콘](assets/grab-icon.png)을 클릭한 다음 원하는 위치에 끌어다 놓습니다.

   >[!TIP]
   >
   >필드를 다른 섹션으로 끌어다 놓을 수 있습니다.
   >섹션에 하나 이상의 필드가 있어야 합니다.
   >

   필드의 새 위치는 레코드를 보는 모든 사용자에 대해 동일한 유형의 모든 레코드의 미리보기 및 페이지에서 모두 업데이트됩니다.

   레코드 미리 보기 또는 페이지의 레이아웃에 대한 모든 변경 사항이 자동으로 저장됩니다.

## 레코드에 연결된 레코드 페이지 추가

연결된 레코드 페이지에 대한 탭을 레코드에 추가하여 연결된 레코드 또는 개체에서 정보를 볼 수 있습니다. 이렇게 하면 테이블 보기의 연결된 레코드가 탭에 추가됩니다.

자세한 내용은 [레코드에 연결된 레코드 페이지 추가](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)를 참조하십시오.

<!--this content has been moved to the page linked above
Consider the following when adding a Connected records page to a record: 

* You can add a Connected records page to a record after you connected record or object types to the record type from the table view of a record type.

* You can add a Connected records page from a record's preview area or the record's page.

* Connected records pages display only the connected objects or records from one object or record type in a table view. The page does not display all records of that type. 

* You can add Connected records pages for the following connected record or object types:

   * Workfront Planning record types
   * Workfront projects, programs, portfolios, groups, or companies. You can view the connected Workfront objects even when you do not have permissions to access them in Workfront. 

To add a Connected records page:

1. Click the name of the record to open it from any view of a record type page. 
1. Click **Add page** from one of the following areas: 

   * The record's preview window
   * The record's details page, after clicking the **Open in new tab** icon ![Open details in a new tab icon](assets/open-details-in-a-new-tab-icon.png) in the upper-right corner of the preview page.  

   The **Create page** box opens.

   ![Add Connected records page modal](assets/add-connection-view-page-modal.png) 

1. Add the **Page name**, click **Connected records page**, then click **Create**.

   A new connected records page is added as a new tab to the record's page.
   
   The records that are connected to the current record display in the table view.  

      >[!TIP]
      >
      >You must add connected records in the table or Details area of a record before you can display them in a connected records page.

   (^^^^^^All fields of the connected record display in the table view of the connected record's tab.^^^^^^^^)
   
   The first five fields of the connected records display by default. (^^^^No lookup fields display by default.^^^^^^^)

   ![Audience connected table view under campaign details](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Optional) Search for or click the name of a connected record or object type in the list.

1. (Optional and conditional) In the table view of the connected records page, do any of the following when viewing connected Planning records or any Workfront objects except for projects: 

   * Click the name of a record. This opens the record's page in a new tab. 

   * Click **Connect** at the bottom of the table view to connect more records, then click outside the connection box to close it. The new records are automatically added to the table. 

      For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
   * Edit any information from the connected records inline in the table view. 

   * Hover over a connected record's name, then click the **More** menu ![More menu](assets/more-menu.png)
   
      Or 
      
      Select one of the records, then click one of the following options in the blue bar at the bottom of the list: 

      * **View** to open the record page in a new tab
      * **Copy link** to copy a link to the record page
      * **Edit thumbnail** to open the **Record thumbnail** box and edit the record's thumbnail image
      * **Duplicate** to duplicate the connected record. The duplicated record is also connected to the current record.
      * **Insert record above or below** to add new records to the connected record type. New records added here are also connected to the current record. This option is not available in the blue bar when selecting a record in the table.
      * **Delete** to delete the record. Deleting a connected record deletes it from its record type and from everywhere where the record is connected.

      For information about editing records in the table view, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 

      >[!TIP]
      >
      >You can select more than one record or object to delete them.

   * Inline edit any of the Planning records in the table on the Connected records page. 
   
      All other Workfront objects display in a read-only table view and you cannot edit them. 
   
1. (Optional and conditional) In the table view of the connected records page, do any of the following when viewing connected Workfront projects:

     * Click **Connect records** in the upper-right corner of the connected record page to connect existing projects.

      For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
     * Inline edit project information in the table.
     * Click **New row** to create a project without a template. The new project is connected to the current record immediately.

         For more information, see [Create Workfront objects from Workfront Planning as you connect them to records](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)
     * Hover over a project and click the **More** menu [More menu](assets/more-menu.png)
     
         Or

         Select one or more projects, and notice the blue bar at the bottom of the list, then click one of the following:
         
         * **Delete** to delete the project. Deleting a project disconnects it from the record and moves it to the Workfront's Recycle Bin. 
         * **Disconnect** to disconnect the project from the record. Disconnecting a project removes it and all the values of its lookup fields from the current record.
      
1. (Optional) Double-click the name of the **Connected records page** tab

   Or

   Hover over the name of the tab, then click **More** ![More menu](assets/more-menu.png), then click **Rename** to rename to new Connected view tab.
1. (Optional) Use any of the following view elements in the toolbar of a connected record page to manage the table view:

   * Filters
   * Sort
   * Grouping
   * Fields, to display, hide, or rearrange fields
   * Row height
   * Search

   For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 

   >[!NOTE]
   >
   >You cannot create, edit, or delete fields in the table view of a connected record's tab.
   
1. (Optional)  Hover over the name of the Connected records page tab, click **More** ![More menu](assets/more-menu.png), then click **Delete** to remove to tab.-->


<!--
## Add a Brief page to a record

(^^^^^^^^^^move this content to its own article, like you did above - leave the header here with a link^^^^^^^^^^^^)

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



