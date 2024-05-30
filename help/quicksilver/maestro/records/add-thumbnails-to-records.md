---
title: 레코드에 썸네일 추가
description: Adobe Workfront Planning에서 레코드 정보를 편집하고 각 레코드를 쉽게 인식할 수 있도록 개별 썸네일과 연결할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: 1369269bcb64bd32f26603608782dc996b079cb9
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

<!--update the metadata with real information-->

# 레코드에 썸네일 추가

{{planning-important-intro}}

레코드를 Adobe Workfront Planning에서 고유한 썸네일과 연결하여 쉽게 인식할 수 있습니다.

레코드 만들기 및 편집을 시작하려면 먼저 레코드 유형을 만들어야 합니다.
자세한 내용은 [레코드 유형 만들기](../architecture/create-record-types.md).

## 액세스 요구 사항

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Workfront Planning에 대한 액세스 제어가 없습니다. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 영역에 대한 상위 권한 기여 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td>  <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> <p>자세한 내용은 <a href="/help/quicksilver/maestro/access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## 레코드 썸네일에 대한 고려 사항

테이블 보기에서 레코드를 시각적으로 구별하기 위해 고유한 썸네일 이미지를 각 레코드와 연결할 수 있습니다.

다음 사항을 고려하십시오.

* 이미지 파일만 썸네일로 추가할 수 있습니다.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* 표 보기에서 개별 레코드에 축소판 이미지를 추가할 수 있습니다.
* 썸네일은 레코드 정보에 속하며 레코드가 표시되는 뷰에 표시됩니다. 예를 들어 축소판은 다음 영역의 레코드 정보와 함께 표시됩니다.

   * 테이블 보기에서 레코드의 기본 필드
   * 타임라인 보기의 레코드 모음
* 레코드 페이지나 다른 유형의 보기에서 레코드 축소판을 추가할 수 없습니다.
* 썸네일은 레코드의 페이지에 표시되지 않습니다.

## 레코드에 썸네일 추가

{{step1-to-maestro}}

1. 썸네일을 추가할 레코드가 있는 작업 영역을 선택한 다음 레코드 유형 카드를 클릭합니다.

   그러면 레코드 유형 페이지가 열립니다.
1. 다음에서 표 보기 선택 **보기** 드롭다운 메뉴. 선택한 유형의 모든 레코드가 테이블에 표시됩니다.
1. 기본 필드 정보를 마우스로 가리킨 다음 **자세히** 메뉴 ![](assets/more-menu.png)을 클릭한 다음 을 클릭합니다 **축소판**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   기본 필드는 테이블 뷰의 첫 번째 열에 표시되는 필드입니다. 기본 필드는 항상 고정되어 있으므로 숨기거나 재배치할 수 없습니다.

   다음 **레코드 썸네일** 상자가 열립니다.

   ![](assets/record-thumbnail-box-for-upload.png)

   <!--update screen shot with correct casing-->

1. 다음에서 **업로드** 탭하거나, 파일을 드래그 앤 드롭하여 썸네일로 추가하거나 **업로드하려면 선택**&#x200B;을 클릭한 다음 추가할 이미지 파일을 찾습니다. 파일을 컴퓨터에 저장해야 합니다.
1. (선택 사항) 크기 조정 도구를 사용하여 이미지를 자르고 크기를 조정합니다.
1. 클릭 **이미지 사용** 이미지를 썸네일로 추가합니다.
이 옵션을 닫으면 **레코드 썸네일** 상자.
1. (조건부) 테이블 보기에 대해 적어도 기여 권한이 있는 경우 **필드** 테이블 보기의 오른쪽 위 모서리에서 참조할 수 있습니다.
1. 다음 항목 선택 **축소판** 썸네일을 표시하려면 전환합니다. 기본적으로 선택되어 있지 않습니다.

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   기본 필드 값의 왼쪽에 썸네일이 표시됩니다.
1. (선택 사항 및 조건부) 보기에 대한 Contribute 이상의 권한이 없는 경우 **보기** 드롭다운 메뉴 또는 뷰를 만듭니다.
1. (선택 사항) 썸네일을 제거하려면 기본 필드 위로 마우스를 가져간 다음 **자세히** 메뉴 ![](assets/more-menu.png)> **축소판** > **제거** 아이콘 ![](assets/remove-image-icon.png)을 클릭한 다음 을 클릭합니다 **변경 내용 저장**.

<!--
Replace the section above with the following when we release generate thumbnails:

## Add a thumbnail to a record

You can add a thumbnail to a record in the following ways:

* Upload a file from your computer
* Generate an image with a prompt

### Upload a thumbnail to a record

{{step1-to-maestro}}

1. Select the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![](assets/more-menu.png), then click **Thumbnail**. 

   ![](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

   ![](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Upload** tab, and drag and drop a file to add as a thumbnail
   Or
   Click **Select to upload**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) Use the sizing tool to crop and resize the image.
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
1. (Conditional) If you have at least Contribute permissions to the table view, click **Fields** in the upper-right corner of the table view. 
1. Select the **Thumbnail** toggle to display the thumbnail. This is deselected by default. 

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   The thumbnail displays to the left of the primary field value. 
1. (Optional and conditional) If you do not have Contribute or higher permissions to the view, select a new view from the **View** drop-down menu, or create a view. 
1. (Optional) To remove the thumbnail, hover over the primary field and click the **More** menu ![](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![](assets/remove-image-icon.png), then click **Save changes**.

### Generate a thumbnail for a record

{{step1-to-maestro}}

1. Select the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![](assets/more-menu.png), then click **Thumbnail**. 

   ![](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

(*************** update the screenshot below*************)
   ![](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Generate** tab, and type a prompt describing the type of image you want to add in the space provided. 
1. Click **Generate**. 

   A set of four suggested images displays. 

1. Click an image to select it, then click **Use image**. 

   The Record thumbnail box closes and the thumbnail is attached to the record. All users who can view the records can now see the selected thumbnail. 
1. (Optional) Click the **More** menu ![](assets/more-menu.png) to the right of the record name in the table view, then click **Thumbnail**. 

   The generated image opens in the **Upload** tab where you can modify or remove it, as described in the section [Upload a thumbnail to a record](#upload-a-thumbnail-to-a-record) in this article. 
-->