---
title: 레코드 공유
description: 다른 사용자와 레코드를 공유하여 공동 작업을 향상시킬 수 있습니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: cf42511263ec1cffd90d1e4bdcd43521b7fe6a30
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 1%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

# 레코드 공유

{{planning-important-intro}}

다른 사용자와 공동 작업하려면 레코드를 다른 사용자와 공유할 수 있습니다.

다음과 같은 방법으로 Adobe Workfront Planning 레코드를 공유할 수 있습니다.

* 페이지가 열릴 때 브라우저에서 레코드 페이지의 링크를 복사합니다.

* 레코드 유형의 표 보기에서 레코드를 볼 때 레코드의 페이지에 대한 링크를 복사합니다.

* 작업 영역을 공유하면 작업 영역의 모든 레코드를 다른 사용자와 공유할 수 있습니다. 자세한 내용은 [작업 영역 공유](/help/quicksilver/planning/access/share-workspaces.md)를 참조하십시오.

이 문서에서는 레코드 유형의 표 보기에서 레코드 페이지에 링크를 복사하는 방법에 대해 설명합니다.

## 액세스 요구 사항

+++ 를 확장하여 Workfront Planning에 대한 액세스 요구 사항을 봅니다.

Workfront Planning에 액세스하려면 다음 항목이 있어야 합니다.

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
   <td role="rowheader"><p>Adobe Workfront 계획 계획*</p></td> 
   <td> 
<p>임의 </p> 
<p>각 Workfront 계획 계획에 포함된 내용에 대한 자세한 내용은 <a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront 가격 및 패키징</a>을 참조하십시오. </p> 
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
   <td><p> 기여자, 라이트 또는 표준 </p>
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
   <td>  <p>링크를 사용하여 레코드를 공유할 수 있는 작업 영역에 대한 이상의 권한 보기 </p>
   <p>레코드가 속한 작업 영역을 공유하면서 레코드를 공유할 수 있는 작업 영역 권한 관리 </p>
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>레이아웃 템플릿</p></td> 
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


<!--OLD:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace to share a record using a link </p>
   <p>Manage permissions to a workspace to share records while sharing the workspace the record belongs to </p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

-->

## 레코드 유형 테이블 보기에서 레코드 링크 공유

{{step1-to-planning}}

마지막으로 액세스한 작업 영역이 열립니다.
1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.
1. (조건부) 표의 오른쪽 위 모서리에 있는 **보기** 드롭다운 메뉴에서 표 보기를 선택합니다. 레코드 유형에 마지막으로 액세스했을 때 타임라인 보기에서 확인하지 않은 경우 기본 보기여야 합니다.

   선택한 레코드 유형과 연관된 레코드가 테이블 뷰에 표시됩니다.
1. 레코드 행을 마우스 오른쪽 단추로 클릭

   또는

   레코드 이름 위에 마우스를 올려 놓고 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 다음 **링크 복사**&#x200B;를 클릭합니다.

   ![](assets/contextual-menu-for-record-row.png)

   링크가 클립보드에 복사됩니다.

1. 링크를 이메일 또는 채팅 창에 붙여넣어 다른 사용자와 공유할 수 있습니다. 사용자가 링크를 받으면 레코드 페이지가 열립니다.

   >[!TIP]
   >
   >레코드 페이지의 필드는 레코드의 테이블 보기에서 사용할 수 있는 필드와 동일합니다.


   <!--add there when it will be available: if they have access to this record-->

## 작업 영역을 공유하여 작업 영역의 모든 레코드 공유

다른 사용자와 작업 영역을 공유할 때 작업 영역의 모든 레코드를 공유할 수 있습니다.

작업 영역에 대한 관리 권한이 있는 사용자만 다른 사용자와 공유할 수 있습니다.

자세한 내용은 [작업 영역 공유](/help/quicksilver/planning/access/share-workspaces.md)를 참조하십시오.
