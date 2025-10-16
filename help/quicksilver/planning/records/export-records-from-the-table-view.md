---
title: 테이블 보기에서 레코드 내보내기
description: 테이블 보기에서 레코드와 해당 정보를 CSV 또는 Excel 파일로 내보낼 수 있습니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d8ac4d94-28b5-41d6-acb8-259696897c8a
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 1%

---

# 테이블 보기에서 레코드 내보내기

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

테이블 보기에서 Adobe Workfront Planning의 Excel 또는 CSV 파일로 레코드 및 해당 정보를 내보낼 수 있습니다.

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
   <td> <p>작업 공간 및 레코드 유형에 대한 이상의 권한 보기</p>   
   <p>보기에 대한 보기 이상의 권한</p>

</td> 
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
   <td><p> Light or higher </p>
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
   <td>   <p>View or higher permissions to a view</p>  
   </td> 
  </tr> 
</tbody> 
</table> -->


## 테이블 보기에서 레코드 내보내기

테이블 뷰를 내보낼 때는 다음 사항을 고려하십시오.

* Excel 파일로 내보낸 정보는 Workfront Planning의 테이블 보기에 적용된 필터, 그룹화 및 정렬을 유지합니다. 그룹화는 CSV 파일에 표시되지 않습니다.

* 내보낸 파일에는 축소판 및 사용자 정의 행 색상이 지원되지 않습니다.

* Workfront 인터페이스에 표시된 필드만 내보내집니다. 숨겨진 필드는 내보내지 않습니다.

테이블 뷰 또는 레코드 유형에서 정보를 내보내려면 다음을 수행합니다.

1. 레코드 유형 페이지로 이동하고 표 보기 탭을 클릭합니다.
1. 다음 중 하나를 수행하십시오.

   * 테이블 보기 탭의 이름을 마우스로 가리킨 다음 보기 이름의 오른쪽에 있는 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **내보내기**&#x200B;를 클릭합니다.

   ![보기에 있는 기타 메뉴](assets/view-more-menu-with-duplicate-option.png)

   * **공유** > **현재 보기 내보내기**&#x200B;를 클릭합니다. 이 옵션은 테이블 뷰를 표시하는 경우에만 사용할 수 있습니다.

   ![레코드 종류 및 보기 공유 옵션이 있는 공유 단추](assets/share-button-with-record-type-and-view-sharing-options.png)

1. 다음 형식 중 하나를 선택합니다.

   * **Excel**
   * **CSV**

   >[!IMPORTANT]
   >
   >다른 보기를 화면에 표시할 때는 표 보기에서 정보를 내보낼 수 없습니다. 기타 메뉴의 내보내기 옵션에 액세스하려면 내보낼 테이블 뷰를 표시해야 합니다.

   파일이 컴퓨터에 다운로드됩니다.

1. (선택 사항) 컴퓨터의 다운로드 폴더로 이동하여 다운로드한 파일을 찾습니다.

   내보낸 파일의 이름은 다음 형식을 따릅니다.

   `Name of the view - name of the record type`

   예를 들어 Campaigns 레코드 형식의 테이블 보기는 이름이 `Table view - Campaigns`인 파일을 생성합니다.

   파일에는 다음 정보가 표시됩니다.

   * 열 머리글은 Excel 파일에서 검은색으로 강조 표시됩니다
   * Workfront 인터페이스에 표시되는 모든 필드를 동일한 기준으로 정렬 및 필터링합니다
   * 그룹화는 Excel 파일에서 유지됩니다

   이제 내보낸 파일을 다른 사용자와 공유하거나 모든 통신에 첨부할 수 있습니다.

</div>
