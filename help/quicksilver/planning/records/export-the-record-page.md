---
title: 레코드 페이지 내보내기
description: 레코드의 미리 보기 또는 세부 사항 페이지를 Adobe Workfront Planning에서 Microsoft Word 파일로 내보낼 수 있습니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8de68b70-dd87-4aad-9137-980ea9fc0d69
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# 레코드의 세부 사항 내보내기

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->


Workfront 계정이 없을 수도 있는 다른 사용자와 더 효율적으로 공동 작업하려면 레코드의 세부 사항 페이지를 Microsoft Word 파일로 내보내 공유할 수 있습니다.

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
<p>모든 Workfront 및 모든 Planning 패키지</p> <p>모든 워크플로우 및 모든 Planning 패키지</p>
<p>각 Workfront Planning 패키지에 포함된 내용에 대한 자세한 내용은 Workfront 계정 담당자에게 문의하십시오. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>밝거나 높음</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역 및 레코드 종류</a>에 대한 이상의 사용 권한 보기 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p> </td> 
  </tr> 
  </tr> 
  <tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> 라이트 또는 기여자 라이선스가 있는 사용자에게 Planning이 포함된 레이아웃 템플릿을 할당해야 합니다.
   <p>표준 사용자 및 시스템 관리자에게는 기본적으로 계획 영역이 활성화되어 있습니다.</p></div></li></ul>
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
<p>Any </p> 
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
   <td> <p>Light or higher</p>
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
   <td>   <p>View or higher permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->


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

1. (선택 사항) 레코드의 페이지를 열려면 **새 탭에서 열기** 아이콘 ![새 탭에서 세부 정보 열기](assets/open-details-in-a-new-tab-icon.png)를 클릭합니다.

1. **세부 정보** 탭을 선택합니다. 기본적으로 세부 정보 탭이 열립니다.

1. 미리 보기 또는 레코드 페이지에서 **내보내기** 메뉴 ![레코드 세부 정보 페이지의 내보내기 아이콘](assets/export-icon-in-record-details-page.png)을 클릭하고 다음 중 하나를 클릭합니다.

   * **Microsoft Word**
   * **Adobe PDF**

   Word(.docx) 또는 PDF 파일이 다운로드되고 컴퓨터에 저장됩니다.

   내보낸 파일의 이름은 레코드의 기본 필드입니다.

   ![내보낸 word 파일](assets/exported-word-file.png)

   >[!NOTE]
   >
   >    기록 세부 정보 영역에서 자세히 표시를 클릭한 후에만 표시되는 페이지에 표시되지 않는 추가 정보는 내보낸 PDF 파일에 표시되지 않습니다. 페이지에 표시되는 정보만 내보낸 파일에 표시됩니다.


1. (선택 사항) 다운로드한 파일로 이동하여 열고 편집하거나(Word 파일인 경우) 다른 사용자와 공유합니다.

