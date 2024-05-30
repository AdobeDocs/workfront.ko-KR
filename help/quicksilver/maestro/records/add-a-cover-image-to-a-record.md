---
title: 레코드에 표지 이미지 추가
description: 레코드를 편집할 때 Adobe Workfront Planning의 레코드 페이지에 표지 이미지를 추가하여 레코드를 개인화할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---


<!--update the metadata with real information-->

# 레코드에 표지 이미지 추가

{{planning-important-intro}}

레코드를 편집할 때 Adobe Workfront Planning의 레코드 페이지에 표지 이미지를 추가하여 레코드를 개인화할 수 있습니다.

레코드 편집에 대한 자세한 내용은 [레코드 편집](/help/quicksilver/maestro/records/edit-records.md).

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

## 레코드 페이지 표지 이미지에 대한 고려 사항

표지 이미지를 추가하여 레코드의 페이지를 개인화할 수 있습니다.

다음 사항을 고려하십시오.

* 표지 이미지는 하나의 레코드에 고유하며 동일한 유형의 모든 레코드에 적용되지 않습니다.
* 이미지 파일만 커버 이미지로 추가할 수 있습니다.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* 모든 보기의 레코드 미리 보기 또는 레코드 페이지에서 커버 이미지를 개별 레코드에 추가할 수 있습니다.
* 레코드 보기에서 표지 이미지를 인라인으로 추가할 수 없습니다.

## 레코드에 표지 이미지 추가

레코드 미리 보기 또는 페이지의 맨 위에 표지 이미지를 추가하여 레코드를 개인화할 수 있습니다.

{{step1-to-maestro}}

마지막으로 액세스한 작업공간이 열립니다.

1. (선택 사항) 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 클릭하여 레코드를 업데이트할 작업 영역을 선택합니다.

1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.

1. 모든 유형의 보기에서 레코드 이름을 클릭합니다

   또는

   테이블 테이블 보기에서 **세부 정보 열기** 아이콘 ![](assets/open-details-icon-in-table-name-field.png) 레코드 이름의 왼쪽에 있습니다.

   레코드의 미리보기가 보기에서 열립니다.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >다음을 볼 수 있습니다. **세부 정보 열기** 테이블 보기에서 레코드의 이름 필드 왼쪽에 있는 아이콘은 이름 필드가 기본 필드인 경우에만 해당됩니다.

1. (선택 사항) **새 탭에서 열기** 아이콘 ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> 레코드 미리 보기의 오른쪽 상단 모서리에서 새 탭에서 레코드 페이지를 엽니다.

   레코드 페이지가 열립니다.

   ![](assets/details-page.png)

1. 레코드 미리 보기 또는 페이지에서 **표지 추가**. <!--check the casing here; I logged a bug for this-->
다음 **레코드 커버** 상자가 열립니다.

1. 클릭 **업로드하려면 선택** 컴퓨터에서 그림을 찾아 선택하고 추가한 다음 **이미지 사용**.

   이미지가 레코드 미리 보기 또는 페이지 맨 위에 업로드되고 변경 사항이 자동으로 저장됩니다.

   ![](assets/record-page-with-cover-image.png)

1. (선택 사항) 이미지를 마우스로 가리킨 다음, **자세히** 메뉴 ![](assets/more-menu.png) 커버 이미지의 오른쪽 아래 모서리에서 다음 중 하나를 수행합니다.

   * 클릭 **업로드** 표지 이미지를 교체하고 6단계를 반복하여 새 이미지를 업로드하고 저장합니다.
   * 클릭 **위치 변경**, 및 사용 **위치 변경** 도구 ![](assets/reposition-tool-icon.png) 표지 이미지를 가운데로 맞추려면 **저장** 완료 시.
   * 클릭 **제거** 커버 이미지를 제거합니다.

   Workfront은 변경 사항을 자동으로 저장합니다.
