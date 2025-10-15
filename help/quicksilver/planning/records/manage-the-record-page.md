---
title: 레코드 페이지 레이아웃 관리
description: Adobe Workfront Planning에서 레코드 미리 보기 및 페이지의 레이아웃을 편집할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: b102960e088f072f10baadcbeca4f7f579daa287
workflow-type: tm+mt
source-wordcount: '2395'
ht-degree: 0%

---


# 레코드 페이지 레이아웃 관리

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

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
<ul> 
<li><p>모든 Workfront 및 모든 Planning 패키지</p></li>
또는
<li><p>모든 워크플로우 및 모든 Planning 패키지</li></ul>
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

## 레코드 페이지 편집에 대한 고려 사항

* 기본적으로 레코드의 세부 정보 및 미리보기 페이지에는 레코드와 연관된 모든 필드가 표시됩니다.

* 미리보기 또는 세부 정보 페이지에서 레코드에 대한 새 필드를 추가할 수 없습니다. 미리 보기 및 세부 정보 페이지에 표시하려면 테이블 보기에서 새 필드를 추가해야 합니다.

* 레코드 미리 보기 또는 세부 정보 페이지에 섹션을 추가하여 일반적인 기준별로 정보를 구성하고 쉽게 찾을 수 있습니다.

* 다음 변경 사항은 동일한 유형의 모든 레코드에 영향을 미치며 해당 레코드에 액세스하는 모든 사용자가 볼 수 있습니다.

   * 필드 재정렬
   * 섹션 추가 또는 제거

* 레코드 미리 보기에서 변경한 내용은 레코드 세부 정보 페이지에 즉시 표시됩니다. 레코드 페이지에서 변경한 내용은 레코드 미리 보기 상자도 볼 수 있습니다.

* 레코드에 표지 이미지 또는 썸네일을 추가하는 것은 레코드 미리 보기 또는 페이지의 전체 레이아웃의 일부가 아닙니다. 각 레코드에 고유한 표지 이미지 또는 썸네일을 추가할 수 있습니다. 자세한 내용은 [레코드에 표지 이미지 추가](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) 및 [레코드에 썸네일 추가](/help/quicksilver/planning/records/add-thumbnails-to-records.md)를 참조하십시오.

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

     섹션을 한 위치 아래로 이동하려면 **아래로 이동**을 클릭합니다.
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

연결된 레코드 페이지에 대한 탭을 레코드에 추가하여 연결된 레코드 또는 개체에서 정보를 볼 수 있습니다.

연결된 레코드의 정보는 테이블 보기에서 편집할 수 있습니다. 다른 응용 프로그램에서 연결된 객체의 정보는 테이블 보기에서 편집할 수 없습니다.

레코드에 연결된 레코드 페이지를 추가할 때는 다음 사항을 고려하십시오.

* 레코드 유형의 테이블 보기에서 레코드나 개체 유형을 레코드 유형에 연결한 후 연결된 레코드 페이지를 레코드에 추가할 수 있습니다.

* 프로덕션 환경에서는 레코드의 미리 보기에서 연결된 레코드 페이지를 추가할 수 없습니다.

  <span class="preview">미리 보기 환경에서 레코드의 미리 보기에서 연결된 레코드 페이지를 추가할 수 있습니다.</span>

* 연결된 레코드 페이지는 테이블 보기에서 연결된 개체나 한 개체 또는 레코드 유형의 레코드만 표시합니다. 페이지에 테이블 보기에 해당 유형의 모든 레코드가 표시되지 않습니다.

* 사용하는 환경에 따라 다음을 확인할 수 있습니다.

   * 프로덕션 환경에서는 연결된 레코드 페이지를 레코드에 추가한 후 레코드의 미리 보기 영역에 페이지 탭이 표시되지만 비어 있습니다. 연결된 레코드에 대한 테이블 보기를 보려면 전체 페이지로 이동해야 합니다.
   * <span class="preview">미리 보기 환경에서 연결된 레코드 페이지가 레코드의 미리 보기 영역과 브라우저 탭에서 모두 표시됩니다.</span>

* 다음과 같은 연결된 레코드 또는 객체 유형에 대해 연결된 레코드 페이지를 추가할 수 있습니다.

   * Workfront Planning 레코드 유형
   * Workfront 프로젝트, 프로그램, 포트폴리오, 그룹 또는 회사. Workfront에서 연결된 Workfront 개체에 액세스할 수 있는 권한이 없는 경우에도 연결된 개체를 볼 수 있습니다.

  >[!NOTE]
  >
  >   연결된 AEM Assets 레코드에 대해 연결된 레코드 페이지를 추가할 수 없습니다.

연결된 레코드 페이지를 추가하려면 다음을 수행하십시오.

1. 레코드 이름을 클릭하여 엽니다.
1. 다음 영역 중 하나에서 **페이지 추가**&#x200B;를 클릭합니다.

   * <span class="preview">레코드의 미리 보기 창</span>
   * 미리 보기 페이지의 오른쪽 상단에 있는 **새 탭에서 열기** 아이콘 ![새 탭에서 세부 정보 열기](assets/open-details-in-a-new-tab-icon.png)을 클릭한 후 레코드의 세부 정보 페이지.

   **페이지 만들기** 상자가 열립니다.

   ![연결된 레코드 추가 페이지 모달](assets/add-connection-view-page-modal.png)

1. **페이지 이름**&#x200B;을(를) 추가하고 **연결된 레코드 페이지**&#x200B;을(를) 클릭한 다음 **만들기**&#x200B;를 클릭합니다.

   새 탭이 레코드의 페이지에 추가됩니다.
1. 목록에서 연결된 레코드 이름 또는 개체 유형을 검색하거나 클릭합니다.
선택한 레코드 유형의 테이블 뷰는 새 페이지에 표시되고 연결된 레코드는 테이블 뷰에 표시됩니다.
연결된 레코드의 모든 필드는 연결된 레코드 탭의 테이블 보기에 표시됩니다.

   연결된 레코드 테이블의 처음 5개 필드는 기본적으로 표시됩니다. 기본적으로 표시되는 조회 필드가 없습니다.

   ![캠페인 세부 정보 아래의 대상자 연결 테이블 보기](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (선택 사항) 연결된 레코드의 표 보기에서 다음 중 하나를 수행합니다.

   * 레코드 이름을 클릭합니다. 새 탭에서 레코드 페이지가 열립니다.

     그러면 레코드의 미리보기 페이지가 열립니다. 오른쪽 상단의 **새 탭에서 열기** 아이콘 ![새 탭에서 열기](assets/open-details-in-a-new-tab-icon.png)을 클릭하여 연결된 레코드의 페이지를 엽니다.

   * **연결**&#x200B;을 클릭하여 더 많은 레코드를 연결한 다음 연결 상자 바깥쪽을 클릭하여 닫습니다. 새 레코드는 자동으로 표에 추가됩니다.
   * 표 보기 내에서 연결된 레코드의 모든 정보를 편집합니다.

   * 연결된 레코드의 이름을 마우스로 가리킨 다음 **추가** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 다음 다음 옵션 중 하나를 클릭합니다.
      * 보기
      * 링크 복사
      * 썸네일 편집
      * 복제
      * 위 또는 아래에 레코드 삽입
      * 삭제
   * 레코드 중 하나를 선택한 다음 화면 하단의 파란색 막대에서 다음 옵션 중 하나를 클릭합니다.
      * 보기
      * 링크 복사
      * 썸네일 편집
      * 복제
      * 삭제. [삭제]는 둘 이상의 레코드를 선택할 때 사용할 수 있는 유일한 옵션입니다.

     표 보기에서 레코드를 편집하는 방법에 대한 자세한 내용은 [레코드 편집](/help/quicksilver/planning/records/edit-records.md)을 참조하십시오.

   * 연결된 레코드 페이지의 표에 있는 모든 레코드를 인라인 편집합니다.

     프로덕션 환경에서는 모든 Workfront 개체가 읽기 전용 테이블 보기에 표시되며 편집할 수 없습니다.

     <span class="preview">미리 보기 환경에서 연결된 레코드 페이지에서 프로젝트를 인라인 편집할 수 있습니다.</span>

1. <span class="preview">(조건부) 연결된 프로젝트 목록을 볼 때 다음 중 하나를 수행하십시오.</span>

   * <span class="preview">연결된 레코드 페이지의 오른쪽 상단에서 **레코드 연결**&#x200B;을 클릭하여 기존 프로젝트를 연결합니다.</span>
   * <span class="preview">테이블의 프로젝트 정보를 인라인 편집합니다.</span>
   * <span class="preview">템플릿 없이 프로젝트를 만들려면 **새 행**&#x200B;을 클릭합니다. 새 프로젝트가 현재 레코드에 즉시 연결됩니다.</span>

     자세한 내용은 [레코드에 연결할 때 Workfront Planning에서 Workfront 개체 만들기](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)를 참조하십시오.
   * <span class="preview">프로젝트 위로 마우스를 가져간 후 **자세히** 메뉴 [추가 메뉴](assets/more-menu.png)를 클릭한 후 다음 중 하나를 클릭하십시오.</span>
      * 프로젝트를 삭제하려면 <span class="preview">**삭제**&#x200B;하십시오. 프로젝트를 삭제하면 레코드에서 연결이 끊기고 Workfront의 휴지통으로 이동합니다. </span>
      * 레코드에서 프로젝트의 연결을 끊으려면 <span class="preview">**연결을 끊습니다**. 프로젝트의 연결을 해제하면 현재 레코드에서 해당 프로젝트와 해당 조회 필드의 모든 값이 제거됩니다. </span>

1. (선택 사항) 연결된 레코드 페이지 탭의 이름을 두 번 클릭합니다

   또는

   탭 이름을 마우스로 가리킨 다음 **자세히** ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **이름 바꾸기**&#x200B;를 클릭하여 새 연결된 보기 탭으로 이름을 바꿉니다.
1. (선택 사항) 도구 모음에서 다음 뷰 요소를 사용하여 테이블 뷰를 관리합니다.

   * 필터
   * 정렬
   * 그룹화
   * 필드, 필드를 표시, 숨기기 또는 다시 정렬

   자세한 내용은 [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)를 참조하십시오.

   >[!NOTE]
   >
   >   연결된 레코드 탭의 표 보기에서 필드를 만들거나 편집하거나 삭제할 수 없습니다.
   >

1. (조건부) 더 많은 레코드나 개체를 연결하려면 다음 중 하나를 수행합니다.

   * 테이블 하단의 **연결**&#x200B;을 클릭하여 레코드 또는 프로젝트를 제외한 모든 Workfront 개체 <span class="preview">를 추가하거나 제거합니다.</span>
   * <span class="preview">미리 보기 환경에서 연결된 레코드 페이지의 오른쪽 위 모서리에 있는 **레코드 연결**&#x200B;을 클릭하여 기존 프로젝트를 연결하거나 테이블 하단에 있는 **새 행**&#x200B;을 클릭하여 프로젝트를 만들고 현재 레코드에 자동으로 연결합니다.</span>

   자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하세요.
1. (선택 사항) 연결된 레코드 페이지 탭의 이름을 마우스로 가리키고 **자세히** ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **삭제**&#x200B;를 클릭하여 탭으로 제거합니다.




<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



