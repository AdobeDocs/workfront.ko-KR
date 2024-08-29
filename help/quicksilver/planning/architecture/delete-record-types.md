---
title: 레코드 유형 삭제
description: 더 이상 관련이 없는 레코드 유형은 삭제할 수 있습니다. 레코드 유형을 삭제하면 레코드, 필드 및 보기와 같이 레코드 유형과 관련된 모든 정보도 삭제됩니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 425c3d3afb892ac83a10bbd36efb4c7d9712c4dc
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 2%

---


# 레코드 유형 삭제

{{planning-important-intro}}

더 이상 관련이 없는 레코드 유형은 삭제할 수 있습니다.

그러나 레코드 유형을 삭제하면 레코드 유형과 관련된 모든 정보도 삭제됩니다. 자세한 내용은 이 문서의 [레코드 종류 삭제 시 고려 사항](#considerations-when-deleting-record-types) 섹션을 참조하십시오.

레코드 형식에 대한 자세한 내용은 [레코드 형식 개요](/help/quicksilver/planning/architecture/overview-of-record-types.md)를 참조하십시오.

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
   <td><p> 표준</p>
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
   <td>   <p>작업 영역</a>에 대한 권한 관리 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>레이아웃 템플릿</p></td> 
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--

OLD: 

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
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->


## 레코드 유형 삭제 시 고려 사항

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* 관리 권한이 있는 작업 공간에서는 레코드 유형만 삭제할 수 있습니다.
* 레코드 유형을 삭제하면 레코드 유형과 관련된 다음 정보가 제거됩니다.

   * 해당 유형의 모든 레코드.
   * 레코드 유형과 연결된 모든 필드.
   * 레코드 종류의 모든 보기(필터, 그룹화 및 정렬 기준 포함).
* 기록 유형은 작업 영역에 액세스하는 모든 사용자에서 제거됩니다.
* 삭제된 레코드 종류 또는 해당 정보는 복구할 수 없습니다.
* 삭제하기 전에 다른 레코드 유형에서 삭제하려는 레코드 유형과 연관된 레코드 및 필드를 다시 만드는 것이 좋습니다.

## 레코드 유형 삭제

{{step1-to-planning}}

1. 레코드 유형을 삭제할 작업 영역을 클릭합니다.

   또는

   작업 영역에서 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 작업 영역을 검색한 다음 목록에 표시될 때 선택합니다.

   작업공간이 열리고 레코드 유형이 표시됩니다.
1. 다음 중 하나를 수행하십시오.

   * 레코드 종류 카드 위에 마우스를 올려 놓고 **자세히** 메뉴를 클릭한 다음 **삭제**&#x200B;합니다.
   * 삭제할 레코드 종류의 카드를 클릭하고 레코드 종류 페이지에서 레코드 종류 이름의 오른쪽에 있는 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 다음 **삭제**&#x200B;를 클릭합니다.

   ![](assets/permanently-delete-record-type-confirmation.png)

1. 확인 상자에 **delete**&#x200B;을(를) 입력한 다음 **영구적으로 삭제**&#x200B;을(를) 클릭합니다. 대/소문자를 구분하지 않습니다.

   선택한 레코드 종류 및 해당 필드, 관련 레코드 및 보기는 삭제되며 복구할 수 없습니다.
