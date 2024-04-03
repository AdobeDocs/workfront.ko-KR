---
title: 레코드 페이지 관리
description: Adobe Workfront Planning에서 레코드 상자 및 페이지의 레이아웃을 관리할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 02d20209b8bf53c84308707a89a5abf399494b64
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# 레코드 페이지 관리

{{maestro-important-intro}}

Adobe Workfront Planning에서 레코드 상자 및 페이지의 레이아웃을 관리할 수 있습니다. 레코드 보기에 레코드 상자를 표시할 수 있습니다.

레코드 상자는 레코드 유형 보기에 표시되는 레코드 페이지의 작은 보기입니다.

레코드 상자와 페이지의 레이아웃을 변경하면 같은 유형의 모든 레코드에 대해 상자와 페이지가 변경됩니다.

레코드 페이지 편집을 시작하려면 먼저 레코드 종류 및 레코드를 만들어야 합니다.

자세한 내용은 다음 문서를 참조하십시오.

* [레코드 유형 만들기](../architecture/create-record-types.md)

* [레코드 만들기](/help/quicksilver/maestro/records/create-records.md)

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
<p>조직은 Adobe Workfront Planning Beta 프로그램에 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
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
   <p>새로운 기능: 밝게 또는 높음</p>
   또는
   <p>현재: 작업 시간 이상</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Adobe Workfront Planning에 대한 액세스 제어가 없습니다.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 공간에 대한 이상 권한 관리</a> </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 계획 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 레코드 페이지 편집에 대한 고려 사항

* 레코드 상자 또는 페이지에서 필드를 다시 정렬하면 해당 유형의 모든 레코드와 해당 레코드에 액세스하는 모든 사용자의 필드가 다시 정렬됩니다.
* 레코드에 표지 이미지를 추가하는 것은 레코드 상자 또는 페이지의 전체 레이아웃의 일부가 아닙니다. 각 레코드에 고유한 표지 이미지를 추가할 수 있습니다.

## 레코드 상자 또는 페이지의 필드 다시 정렬

{{step1-to-maestro}}

마지막으로 액세스한 작업공간이 열립니다.

1. (선택 사항) 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 클릭하여 레코드를 업데이트할 작업 영역을 선택합니다.

1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.

1. 모든 유형의 보기에서 레코드 이름을 클릭합니다

   또는

   테이블 테이블 보기에서 **세부 정보 열기** 아이콘 ![](assets/open-details-icon-in-table-name-field.png) 레코드 이름의 왼쪽에 있습니다.

   레코드 상자가 뷰에 열립니다.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >다음을 볼 수 있습니다. **세부 정보 열기** 테이블 보기에서 레코드의 이름 필드 왼쪽에 있는 아이콘은 이름 필드가 기본 필드인 경우에만 해당됩니다.

1. (선택 사항) **새 탭에서 열기** 아이콘 ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> 레코드 상자의 오른쪽 상단 모서리에서 새 탭에서 레코드 페이지를 엽니다.

   레코드 페이지가 열립니다.

   ![](assets/details-page.png)

1. 레코드 상자나 페이지에서 그랩 아이콘을 클릭합니다 ![](assets/grab-icon.png) 필드 이름의 왼쪽으로 드래그하여 원하는 위치에 놓습니다.

   필드의 새 위치는 레코드를 보는 모든 사용자에 대해 동일한 유형의 모든 레코드의 상자와 페이지에서 모두 업데이트됩니다.

   레코드 상자 또는 페이지의 레이아웃에 대한 모든 변경 사항이 자동으로 저장됩니다.


## 레코드 상자 또는 페이지에 표지 이미지 추가

레코드 상자나 페이지 맨 위에 표지 이미지를 추가하여 레코드를 개인화할 수 있습니다.

{{step1-to-maestro}}

마지막으로 액세스한 작업공간이 열립니다.

1. (선택 사항) 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 클릭하여 레코드를 업데이트할 작업 영역을 선택합니다.

1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.

1. 모든 유형의 보기에서 레코드 이름을 클릭합니다

   또는

   테이블 테이블 보기에서 **세부 정보 열기** 아이콘 ![](assets/open-details-icon-in-table-name-field.png) 레코드 이름의 왼쪽에 있습니다.

   레코드 상자가 뷰에 열립니다.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >다음을 볼 수 있습니다. **세부 정보 열기** 테이블 보기에서 레코드의 이름 필드 왼쪽에 있는 아이콘은 이름 필드가 기본 필드인 경우에만 해당됩니다.

1. (선택 사항) **새 탭에서 열기** 아이콘 ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> 레코드 상자의 오른쪽 상단 모서리에서 새 탭에서 레코드 페이지를 엽니다.

   레코드 페이지가 열립니다.

   ![](assets/details-page.png)

1. 레코드 상자 또는 페이지에서 **표지 추가**. <!--check the casing here; I logged a bug for this-->
다음 **레코드 커버** 상자가 열립니다.

1. 클릭 **업로드하려면 선택** 컴퓨터에서 그림을 찾아 선택하고 추가한 다음 **이미지 사용**.

   이미지가 레코드 상자나 페이지 맨 위에 업로드되고 변경 사항이 자동으로 저장됩니다.

   ![](assets/record-page-with-cover-image.png)

1. (선택 사항) 이미지를 마우스로 가리킨 다음, **자세히** 메뉴 ![](assets/more-menu.png) 커버 이미지의 오른쪽 아래 모서리에서 다음 중 하나를 수행합니다.

   * 클릭 **업로드** 표지 이미지를 교체하고 6단계를 반복하여 새 이미지를 업로드하고 저장합니다.
   * 클릭 **위치 변경**, 및 사용 **위치 변경** 도구 ![](assets/reposition-tool-icon.png) 표지 이미지를 가운데로 맞추려면 **저장** 완료 시.
   * 클릭 **제거** 커버 이미지를 제거합니다.

   모든 변경 사항은 즉시 적용됩니다.

