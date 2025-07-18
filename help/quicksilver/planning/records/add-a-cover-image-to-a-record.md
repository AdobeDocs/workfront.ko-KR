---
title: 레코드에 표지 이미지 추가
description: 레코드를 편집할 때 Adobe Systems Workfront Planning의 레코드 페이지 페이지에 표지 이미지를 추가하여 레코드를 개인화할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 1%

---


# 레코드에 표지 이미지 추가

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

레코드를 편집할 때 Adobe Systems Workfront Planning의 레코드 페이지 페이지에 표지 이미지를 추가하여 레코드를 개인화할 수 있습니다.

레코드 편집에 대한 자세한 내용은 레코드[ 편집을 참조하십시오](/help/quicksilver/planning/records/edit-records.md).

레코드 만들기 및 편집을 시작하려면 먼저 레코드 종류를 만들어야 합니다.

자세한 내용은 레코드 종류[ 만들기 섹션을 참조하세요](/help/quicksilver/planning/architecture/create-record-types.md).

## 액세스 요구 사항

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
<p>각 Workfront Planning 패키지에 포함된 항목에 대한 자세한 내용은 Workfront 계정 관리자 관리자에게 문의하십시오. </p> 
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
   <td><p> 표준</p>
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

## 레코드 페이지 표지 이미지에 대한 고려 사항

표지 이미지를 추가하여 레코드의 페이지 개별화할 수 있습니다.

고려해야 합니다.

* 표지 이미지는 한 레코드에 고유하며 동일한 유형의 모든 레코드에 적용되는 것은 아닙니다.
* 이미지 파일만 표지 이미지로 추가할 수 있습니다.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* 모든 보기의 레코드 미리 보기 또는 레코드 페이지 또는 개별 레코드에 표지 이미지를 추가할 수 있습니다.
* 레코드 보기에서 표지 이미지를 추가할 수 없습니다.
* Workfront는 레코드를 만들 때마다 표지 이미지를 자동으로 업로드합니다. 나중에 이 이미지를 수정할 수 있습니다.

## 레코드에 표지 이미지 추가

레코드 미리 보기 또는 페이지 상단에 표지 이미지를 추가하여 레코드를 개인화할 수 있습니다.

{{step1-to-planning}}

1. 레코드를 개인화할 작업 영역,

   또는

   작업 영역에서 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 화살표를 확장하고, 작업 영역 검색한 다음, 목록에 표시되면 선택합니다.

   작업 영역 영역이 열리고 레코드 종류가 표시됩니다.

1. 레코드 종류 카드 클릭

   레코드 종류 페이지 가 열립니다.

1. 모든 유형의 보기에서 레코드를 클릭합니다

   또는

   테이블 테이블 보기에서 첫 번째 열의 세부 정보&#x200B;**열기 아이콘**&#x200B;세부 정보 열기 아이콘을![ 클릭합니다](assets/open-details-icon-in-table-name-field.png).

   레코드의 미리 보기가 보기에서 열립니다.

   ![세부 정보 미리 보기 상자](assets/details-box.png)


1. (선택 사항) **레코드 미리 보기의 오른쪽 위 모서리에 있는 새 탭에서 열기 아이콘**&#x200B;새 탭![에서 열기 아이콘을](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> 클릭하여 새 탭에서 레코드의 페이지 엽니다.

   레코드 페이지 가 열립니다.

   ![세부 정보 페이지](assets/details-page.png)

1. 레코드 미리보기 또는 세부정보 페이지 에서 레코드 이름 위의 공백 위로 마우스를 가져간 다음 Add cover(커버&#x200B;**추가)를 클릭합니다**.

   또는

   기존 표지 이미지 위로 마우스를 가져간 후 더 **보기** 메뉴 ![더 보기 메뉴를](assets/more-menu.png) 클릭하고 업로드&#x200B;**를 클릭합니다**. <!--check the casing here; I logged a bug for this-->**[업로드] 탭 에서**&#x200B;[레코드 표지&#x200B;**]** 상자가 열립니다.

   ![업로드 용 레코드 표지 상자](assets/record-cover-box-for-upload.png)

1. 이미지 검색(Browse images **)을 클릭하고**&#x200B;컴퓨터에서 사진을 찾아 선택하고 추가합니다.

1. (선택 사항) 저장하기 전에 이미지를 제거하려면 새 이미지&#x200B;**업로드 아이콘**&#x200B;새 이미지 업로드 아이콘![ 을 클릭하고 ](assets/upload-new-image-icon.png)새 이미지를 업로드합니다.

1. (선택 사항) **갤러리** 탭 을 클릭한 다음, 이미지 갤러리에서 이미지를 클릭합니다. 이미지 갤러리는 수정할 수 없습니다.

   ![갤러리용 레코드 표지 상자](assets/record-cover-box-for-gallery.png)

1. 이미지&#x200B;**사용을 클릭합니다**.

   이미지는 레코드 미리보기 또는 세부 정보 페이지 상단에 업로드되고 변경 사항이 자동으로 저장됩니다.

   ![표지 이미지로 페이지 기록](assets/record-page-with-cover-image.png)

1. (선택 사항) 이미지 위에 마우스를 올려 놓은 다음, 표지 이미지의 오른쪽 하단에 있는 더 보기&#x200B;**메뉴**&#x200B;더![ 보기를 클릭하고 ](assets/more-menu.png)다음 중 하나를 수행하십시오.

   * 표지 이미지를 바꾸려면 [업로드&#x200B;**]를 클릭하고** 6단계를 반복하여 새 이미지를 업로드 및 저장합니다.
   * [위치 변경]을 클릭하고 **[**&#x200B;위치&#x200B;**변경 도구] 도구**&#x200B;[위치 변경] 도구 아이콘을![ 사용하여 표지 이미지를 가운데에 맞춘 다음, 완료되면 [저장]](assets/reposition-tool-icon.png)을 클릭합니다&#x200B;**.**
   * [제거]&#x200B;**를 클릭하여**&#x200B;표지 이미지를 제거합니다.

   Workfront는 변경 사항을 자동으로 저장합니다.
