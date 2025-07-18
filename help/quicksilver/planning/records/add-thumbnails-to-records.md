---
title: 레코드에 썸네일 추가
description: Adobe Systems Workfront Planning에서 레코드 정보를 편집하고 각 레코드를 개별 축소판과 연결하여 쉽게 인식할 수 있도록 할 수 있습니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---


# 레코드에 썸네일 추가

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

Adobe Systems Workfront Planning에서 레코드를 고유 썸네일과 연결하여 쉽게 인식할 수 있도록 할 수 있습니다.

레코드 만들기 및 편집을 시작하려면 먼저 레코드 종류를 만들어야 합니다.
자세한 내용은 레코드 종류[ 만들기 섹션을 참조하세요](/help/quicksilver/planning/architecture/create-record-types.md).

## 액세스 요구 사항

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
   <td role="rowheader"><p>Adobe Systems Workfront 라이선스*</p></td> 
   <td><p> 표준 </p>
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
   <td>   <p>작업 영역 및 레코드 종류에 대한 Contribute 이상의 권한  </p>  
   <p>시스템 관리자는 자신이 생성하지 않은 작업 영역을 포함하여 모든 작업 공간에 대한 권한을 갖습니다</p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서[의 액세스 요구 사항을 참조하십시오](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## 레코드 썸네일에 대한 고려 사항

테이블 보기에서 레코드를 시각적으로 구분하기 위해 고유한 썸네일 이미지를 각 레코드와 연결할 수 있습니다.

고려해야 합니다.

* A thumbnail is unique to one record, and it does not apply to all records of the same type.
* You can add only image files as thumbnails.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* You can add a thumbnail image to individual records in the table view or from the record&#39;s page or preview box.
* Workfront는 레코드를 만들 때마다 썸네일 이미지를 자동으로 업로드합니다. 나중에 이 이미지를 수정할 수 있습니다.
* 썸네일은 레코드 정보에 속하며 레코드가 표시되는 영역에 표시됩니다. 예를 들어 썸네일은 다음 영역에서 레코드 정보와 함께 표시됩니다.

   * 테이블 보기에 있는 레코드의 기본 필드The primary field of a record in the table view
   * 타임라인 보기의 레코드 막대입니다.
   * 레코드의 세부 사항 미리 보기 및 페이지.

## 레코드에 썸네일 추가

썸네일은 다음과 같은 방법으로 추가할 수 있습니다.

* [테이블 보기에서 레코드에 썸네일 추가](#add-a-thumbnail-to-a-record-from-the-table-view)
* [세부 정보 페이지 에서 레코드에 썸네일 추가](#add-a-thumbnail-to-a-record-from-the-details-page)

### 테이블 보기에서 레코드에 썸네일 추가

{{step1-to-planning}}

1. 축소판을 추가할 레코드의 작업 영역을 클릭한 다음, 레코드 종류 카드를 클릭하십시오.

   그러면 레코드 종류 페이지 가 열립니다.
1. 보기&#x200B;**드롭다운 메뉴에서 테이블 보기를**&#x200B;선택합니다. 선택한 유형의 모든 레코드가 테이블에 표시됩니다.
1. 기본 필드 정보 위로 마우스를 가져간 다음 더 **보기** 메뉴 ![더 보기 메뉴를](assets/more-menu.png) 클릭한 다음 썸네일을&#x200B;**클릭합니다**.

   ![Record more menu expanded](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   기본 필드는 테이블 뷰의 첫 번째 열에 표시되는 필드입니다. 기본 필드는 항상 고정되어 있으며 숨김 또는 재배치할 수 없습니다. 썸네일 옵션은 기본 필드가 공식 필드인 경우 [자세히] 메뉴에서 사용할 수 없습니다.

   **[업로드]** 탭 [레코드 썸네일&#x200B;**] 상자에서**&#x200B;기본적으로 열립니다.

   썸네일 업로드에 대한 자세한 내용은 6단계부터 시작하여 이 문서의 세부 정보 페이지[에서 레코드에 썸네일 추가 섹션을 ](#add-a-thumbnail-to-a-record-from-the-details-page)참조하세요.<!--see if this is accurate-->

<!--
   ![Record thumbnail box for upload](assets/record-thumbnail-box-for-upload.png) 

  *****update screen shot with correct casing****

1. Drag and drop a file to add as a thumbnail
   
   Or
   
   Click **Browse images**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) After the image uploads in the **Record thumbnail** box, use the sizing tool to crop and resize the image.
1. (Optional) Click the **Upload new image** icon ![Upload new image icon](assets/upload-new-image-icon.png) to upload another image. 
1. (Optional) To remove a thumbnail before it is saved, click  **Remove uploaded image** icon ![Remove image icon](assets/remove-image-icon.png) to the right of the image. 
1. (Optional) Click the **Gallery** tab, then click an image. The gallery of images cannot be modified.

   ![Record thumbnail box for gallery](assets/record-thumbnail-box-for-gallery.png)
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
   The thumbnail displays in areas of Workfront Planning where the record displays. 

   >[!TIP]
   >
   >   You must enable the Thumbnail field in the table view to display thumbnails in this view. It is disabled by default.

1. (Optional) To remove the thumbnail after it is saved, hover over the primary field and click the **More** menu ![More menu](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![Remove image icon](assets/remove-image-icon.png), then click **Save changes**. -->

### 세부 정보 페이지 에서 레코드에 썸네일 추가

{{step1-to-planning}}

1. 축소판을 추가할 레코드의 작업 영역을 클릭한 다음, 레코드 종류 카드를 클릭하십시오.

   그러면 레코드 종류 페이지 가 열립니다.
1. 보기에서 레코드를 클릭하여 엽니다.

   세부 정보 미리 보기 상자가 표시됩니다.
1. (선택 사항) **오른쪽 상단 모서리에 있는 새 탭** 에서 열기 아이콘 ![새 탭에서 세부 정보 열기 아이콘을](assets/open-details-in-a-new-tab-icon.png) 클릭합니다.

   레코드의 세부 정보 페이지 가 열립니다.

1. (조건부) 레코드 미리 보기 또는 세부 정보 페이지에서 썸네일 이미지 또는 ![아이콘 세부 정보 페이지](assets/record-thumbnail-icon-on-details-page.png)의 레코드 썸네일 아이콘 위로 마우스를 가져간 다음 레코드 이름 위의 공간을 마우스로 가리킨 다음 썸네일&#x200B;**추가 또는**&#x200B;썸네일&#x200B;**편집을 클릭합니다**.

   **[업로드]** 탭 [레코드 썸네일&#x200B;**] 상자에서**&#x200B;기본적으로 열립니다.

   ![업로드할 레코드 썸네일 상자](assets/record-thumbnail-box-for-upload.png)

1. 썸네일로 추가할 파일 드래그 앤 드롭

   또는

   이미지&#x200B;**검색을 클릭한**&#x200B;다음 추가할 이미지 파일을 찾습니다. 파일이 컴퓨터에 저장되어 있어야 합니다.

1. (선택 사항) 이미지가 업로드되면 **[레코드 썸네일** ] 상자에서 크기 조정 도구 를 사용하여 이미지를 자르고 크기를 조정합니다.
1. (선택 사항) **다른 이미지를 업로드하려면 새 이미지** 업로드 아이콘 ![새 이미지 업로드 아이콘을](assets/upload-new-image-icon.png) 클릭합니다.
1. (선택 사항) **갤러리** 탭 을 클릭한 다음 이미지를 클릭합니다. The gallery of images cannot be modified.

   ![Record thumbnail box for gallery](assets/record-thumbnail-box-for-gallery.png)

1. (선택 사항) 저장하기 전에 썸네일을 제거하려면 이미지 오른쪽에 **있는 이미지 제거** 아이콘 ![이미지를 제거 클릭합니다](assets/remove-image-icon.png) .

1. 이미지&#x200B;**사용을 클릭하여**이미지를 썸네일로 추가합니다.
이렇게 하면 레코드 썸네일**상자가 닫힙니다**.
썸네일은 레코드가 표시되는 Workfront Planning 영역에 표시됩니다.

   >[!TIP]
   >
   >   이 뷰에 썸네일을 표시하려면 테이블 뷰에서 썸네일 필드를 활성화해야 합니다. 기본적으로 비활성화되어 있습니다.

1. (선택 사항) 썸네일을 저장한 후 제거하려면 아무 보기에서나 레코드를 클릭하여 세부 정보 페이지 연 다음 썸네일 이미지 위로 마우스를 가져간 다음 자세히 메뉴 **더 보기** 메뉴 아이콘![> ](assets/more-menu.png)제거&#x200B;**아이콘**&#x200B;제거 아이콘을![ 클릭합니다](assets/remove-image-icon.png). 썸네일 이미지가 제거됩니다.


<!--
### Generate a thumbnail for a record

{{step1-to-planning}}

1. Click the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![More menu](assets/more-menu.png), then click **Thumbnail**. 

   ![Record more menu expanded](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

(*************** update the screenshot below*************)
   ![Record thumbnail box for upload](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Generate** tab, and type a prompt describing the type of image you want to add in the space provided. 
1. Click **Generate**. 

   A set of four suggested images displays. 

1. Click an image to select it, then click **Use image**. 

   The Record thumbnail box closes and the thumbnail is attached to the record. All users who can view the records can now see the selected thumbnail. 
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name in the table view, then click **Thumbnail**. 

   The generated image opens in the **Upload** tab where you can modify or remove it, as described in the section [Upload a thumbnail to a record](#upload-a-thumbnail-to-a-record) in this article. 
-->
