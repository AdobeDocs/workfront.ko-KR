---
title: 테이블 보기에서 레코드 내보내기
description: 테이블 보기에서 레코드와 해당 정보를 CSV 또는 Excel 파일로 내보낼 수 있습니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 8f4c1be156094d18df4bc3628d4f1fca90372119
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 2%

---


# 테이블 보기에서 레코드 내보내기

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

테이블 보기에서 Adobe Workfront Planning의 Excel 또는 CSV 파일로 레코드 및 해당 정보를 내보낼 수 있습니다.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

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
<p>Workfront Planning에 액세스하려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
   <td><p> 표준 </p>
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
   <td>   <p>보기에 대한 권한 관리</p>  
   <p>보기에 대한 권한을 보고 보기 설정을 일시적으로 변경하거나 복제하거나 내보냅니다.</p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

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
