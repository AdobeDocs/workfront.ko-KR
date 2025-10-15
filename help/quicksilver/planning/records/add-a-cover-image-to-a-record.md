---
title: 레코드에 표지 이미지 추가
description: 레코드를 편집할 때 Adobe Workfront Planning의 레코드 페이지에 표지 이미지를 추가하여 레코드를 개인화할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: b102960e088f072f10baadcbeca4f7f579daa287
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 0%

---


# 레코드에 표지 이미지 추가

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

레코드를 편집할 때 Adobe Workfront Planning의 레코드 페이지에 표지 이미지를 추가하여 레코드를 개인화할 수 있습니다.

레코드 편집에 대한 자세한 내용은 [레코드 편집](/help/quicksilver/planning/records/edit-records.md)을 참조하세요.

레코드 만들기 및 편집을 시작하려면 먼저 레코드 유형을 만들어야 합니다.

자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

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
   <td>   <p>작업 공간 및 레코드 유형에 대한 또는 그 이상의 권한 기여  </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p> </td> 
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
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
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
   <td><p> Standard</p>
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
   <td>   <p>Contribute or higher permissions to a workspace and record type  </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## 레코드 페이지 표지 이미지에 대한 고려 사항

표지 이미지를 추가하여 레코드의 페이지를 개인화할 수 있습니다.

다음 사항을 고려하십시오.

* 표지 이미지는 하나의 레코드에 고유하며 동일한 유형의 모든 레코드에 적용되지 않습니다.
* 이미지 파일만 커버 이미지로 추가할 수 있습니다.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* 모든 보기의 레코드 미리 보기 또는 레코드 페이지에서 커버 이미지를 개별 레코드에 추가할 수 있습니다.
* 레코드 보기에서는 표지 이미지를 추가할 수 없습니다.
* Workfront은 레코드를 만들 때마다 표지 이미지를 자동으로 업로드합니다. 나중에 이 이미지를 수정할 수 있습니다.

## 레코드에 표지 이미지 추가

레코드 미리 보기 또는 페이지의 맨 위에 표지 이미지를 추가하여 레코드를 개인화할 수 있습니다.

{{step1-to-planning}}

1. 개인화할 레코드가 있는 작업 영역을 클릭합니다.

   또는

   작업 영역에서 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 작업 영역을 검색한 다음 목록에 표시될 때 선택합니다.

   작업공간이 열리고 레코드 유형이 표시됩니다.

1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.

1. 모든 유형의 보기에서 레코드를 클릭합니다

   또는

   테이블 테이블 보기에서 첫 번째 열의 **세부 정보 열기** 아이콘 ![세부 정보 열기 아이콘](assets/open-details-icon-in-table-name-field.png)을 클릭합니다.

   레코드의 미리보기가 보기에서 열립니다.

   ![세부 정보 미리 보기 상자](assets/details-box.png)


1. (선택 사항) 레코드 미리 보기의 오른쪽 상단에 있는 **새 탭에서 열기** 아이콘 ![새 탭에서 열기](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it-->을(를) 클릭하여 새 탭에서 레코드 페이지를 엽니다.

   레코드 페이지가 열립니다.

   ![세부 정보 페이지](assets/details-page.png)

1. 레코드 미리 보기 또는 세부 정보 페이지에서 레코드 이름 위의 공간을 마우스로 가리킨 다음 **표지 추가**&#x200B;를 클릭합니다.

   또는

   기존 표지 이미지 위로 마우스를 가져간 후 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **업로드**&#x200B;를 클릭합니다. <!--check the casing here; I logged a bug for this-->
**레코드 표지** 상자가 **업로드** 탭에서 열립니다.

   ![업로드를 위한 레코드 표지](assets/record-cover-box-for-upload.png)

1. **이미지 찾아보기**&#x200B;를 클릭하고 컴퓨터에서 그림을 찾아 선택하여 추가합니다.

1. (선택 사항) 이미지를 저장하기 전에 제거하려면 **새 이미지 업로드** 아이콘 ![새 이미지 업로드 아이콘](assets/upload-new-image-icon.png)을 클릭하고 새 이미지를 업로드하십시오.

1. (선택 사항) **갤러리** 탭을 클릭한 다음 이미지 갤러리에서 이미지를 클릭합니다. 이미지 갤러리는 수정할 수 없습니다.

   ![갤러리에 대한 레코드 표지](assets/record-cover-box-for-gallery.png)

1. **이미지 사용**&#x200B;을 클릭합니다.

   이미지는 레코드 미리 보기 또는 세부 사항 페이지의 맨 위에 업로드되고 변경 사항이 자동으로 저장됩니다.

   ![표지 이미지로 페이지 기록](assets/record-page-with-cover-image.png)

1. (선택 사항) 이미지 위로 마우스를 가져간 다음 표지 이미지의 오른쪽 아래 모서리에 있는 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭하고 다음 중 하나를 수행하십시오.

   * 표지 이미지를 바꾸려면 **업로드**&#x200B;를 클릭하고 6단계를 반복하여 새 이미지를 업로드하고 저장합니다.
   * **위치 변경**&#x200B;을 클릭하고 **위치 변경** 도구 ![위치 변경 도구 아이콘](assets/reposition-tool-icon.png)을 사용하여 표지 이미지를 가운데로 설정한 다음 완료되면 **저장**&#x200B;을 클릭합니다.
   * 표지 이미지를 제거하려면 **제거**&#x200B;를 클릭하십시오.

   Workfront은 변경 사항을 자동으로 저장합니다.
