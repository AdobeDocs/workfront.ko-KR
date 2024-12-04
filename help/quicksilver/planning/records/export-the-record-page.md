---
title: 레코드 페이지 내보내기
description: 레코드의 미리 보기 또는 세부 정보 페이지를 Word로 내보낼 수 있습니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8de68b70-dd87-4aad-9137-980ea9fc0d69
source-git-commit: 5db940b197364e30ef6e1ea3e3c94ae3bda5b20c
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 1%

---

# 레코드의 세부 사항 내보내기

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).</span>-->


Workfront 계정이 없을 수도 있는 다른 사용자와 더 효율적으로 공동 작업하려면 레코드의 세부 사항을 파일로 내보내고 해당 사용자와 공유할 수 있습니다.

## 액세스 요구 사항

+++ 를 확장하여 Workfront Planning에 대한 액세스 요구 사항을 봅니다.

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
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront 계획<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 플랜*</p></td> 
   <td> 
<p>다음 Workfront 플랜 중 하나:</p> 
<ul><li>선택</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다.</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 계획 패키지*</p></td> 
   <td> 
<p>임의 </p> 
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning의 모든 기능에 액세스할 수 있으려면 조직의 Workfront 인스턴스가 통합 경험 Adobe에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 통합 경험 Adobe</a>를 참조하십시오. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
   <td> <p>표준</p>
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역 </a>에 대한 이상의 권한 보기 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>레이아웃 템플릿</p></td> 
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 레코드 세부 정보 내보내기에 대한 고려 사항:

* 레코드의 세부 사항을 다음 파일 형식으로 내보낼 수 있습니다.

   * .docx Word
   * .pdf

* 레코드 페이지 또는 미리 보기 영역의 세부 정보 탭만 내보낼 수 있습니다.

* 내보낸 파일은 축소판 및 표지 이미지를 포함하여 레코드 페이지의 레이아웃을 유지합니다.

## 레코드의 세부 사항 내보내기

{{step1-to-planning}}

1. 작업 영역의 카드를 클릭합니다.

   작업공간이 열리고 기록 유형이 카드에 표시됩니다.

1. 레코드 유형 카드를 클릭합니다.
레코드 유형 페이지가 열리고 해당 유형의 모든 레코드가 표시됩니다.

1. 보기에서 레코드 이름을 클릭합니다.

   레코드의 미리보기 상자가 열립니다.

1. (선택 사항) **새 탭에서 열기** 아이콘 ![](assets/open-details-in-a-new-tab-icon.png)을 클릭하여 레코드 페이지를 엽니다.

1. **세부 정보** 탭을 선택합니다. 기본적으로 세부 정보 탭이 열립니다.

1. 미리 보기 또는 레코드 페이지에서 **내보내기** 메뉴 ![](assets/export-icon-in-record-details-page.png)을(를) 클릭한 후 다음 중 하나를 클릭합니다.

   * **Microsoft Word**
   * **Adobe PDF**

   Word(.docx) 또는 PDF 파일을 다운로드하여 컴퓨터에 저장합니다.

   내보낸 파일의 이름은 레코드의 기본 필드입니다.

   ![](assets/exported-word-file.png)

   >[!NOTE]
   >
   >    기록 세부 정보 영역에서 자세히 표시를 클릭한 후에만 표시되는 페이지에 표시되지 않는 추가 정보는 내보낸 PDF 파일에 표시되지 않습니다. 페이지에 표시되는 정보만 내보낸 파일에 표시됩니다.


1. (선택 사항) 다운로드한 파일로 이동하여 열고 편집하거나(Word 파일인 경우) 다른 사용자와 공유합니다.

