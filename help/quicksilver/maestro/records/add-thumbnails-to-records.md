---
title: 레코드에 썸네일 추가
description: Adobe 마에스트로에서 레코드 정보를 편집하고 각 레코드를 쉽게 인식할 수 있도록 개별 썸네일과 연결할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: dda00a43c5122a233ce2849d828d2e5e4555d2d9
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

<!--update the metadata with real information-->

# 레코드에 썸네일 추가

>[!IMPORTANT]
>
>이 문서의 정보는 Adobe Workfront의 새로운 오퍼링인 Adobe Maestro를 참조합니다.
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 베타 프로그램의 일부입니다. Maestro 기능을 사용하려면 Workfront 고객이어야 합니다.
>
>Maestro용 Beta 프로그램 가입에 대한 자세한 내용은 계정 담당자에게 문의하십시오.
>
>자세한 내용은 [Adobe 마에스트로 개요](../maestro-overview.md).

Adobe Maestro에서 레코드를 고유한 썸네일과 연결하여 쉽게 인식할 수 있습니다.

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
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Maestro에 대한 액세스 제어가 없습니다. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 영역에 대한 상위 권한 기여 </p>  
   <p>테이블 보기에 대한 상위 권한 기여 </p> 
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 마에스트로 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>

</tbody>
</table>


## 레코드 썸네일에 대한 고려 사항

테이블 보기에서 레코드를 시각적으로 구별하기 위해 고유한 썸네일 이미지를 각 레코드와 연결할 수 있습니다.

다음 사항을 고려하십시오.

* 이미지 파일만 썸네일로 추가할 수 있습니다.
* 표 보기에서 개별 레코드에 축소판 이미지를 추가할 수 있습니다.
* 레코드의 세부 정보 페이지나 타임라인 보기에서는 레코드 축소판을 추가할 수 없습니다.
* 축소판 이미지는 필드 유형에 관계없이 각 레코드의 기본 필드 왼쪽에 항상 표시됩니다.

  한 줄 텍스트, 숫자 또는 수식인 필드를 기본 필드로 지정할 수 있습니다.
자세한 내용은 [표 보기 관리](/help/quicksilver/maestro/views/manage-the-table-view.md).

<!--above: when you know exactly what type of files are allowed, add the exact extensions above-->

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
1. 테이블 보기의 오른쪽 위 모서리에 있는 필드 를 클릭합니다.
1. 다음 항목 선택 **축소판** 썸네일을 표시하려면 전환합니다. 기본적으로 선택되어 있지 않습니다.

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   기본 필드 값의 왼쪽에 썸네일이 표시됩니다.
1. (선택 사항) 썸네일을 제거하려면 기본 필드 위로 마우스를 가져간 다음 **자세히** 메뉴 ![](assets/more-menu.png)> **축소판** > **제거** 아이콘 ![](assets/remove-image-icon.png)을 클릭한 다음 을 클릭합니다 **변경 내용 저장**.
