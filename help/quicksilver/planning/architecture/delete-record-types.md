---
title: 레코드 유형 삭제
description: 더 이상 관련이 없는 레코드 유형은 삭제할 수 있습니다. 레코드 유형을 삭제하면 레코드, 필드 및 보기와 같이 레코드 유형과 관련된 모든 정보도 삭제됩니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 92748bab4eee807d9529a61a9d97ac1c1df9c8cf
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 1%

---


<!--keep the global record type reference in yellow till January 2026-->

# 레코드 유형 삭제

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

더 이상 관련이 없는 레코드 유형은 삭제할 수 있습니다.

그러나 레코드 유형을 삭제하면 레코드 유형과 관련된 모든 정보도 삭제됩니다. 자세한 내용은 이 문서의 [레코드 종류 삭제 시 고려 사항](#considerations-when-deleting-record-types) 섹션을 참조하십시오.

레코드 형식에 대한 자세한 내용은 [레코드 형식 개요](/help/quicksilver/planning/architecture/overview-of-record-types.md)를 참조하십시오.

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
   <td>   <p>작업 공간에 대한 권한 관리</p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  </td> 
  </tr>  
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

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
   <td>   <p>Manage permissions to a workspace and record type</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> 
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

<!--

<div class="preview">

* You cannot delete a global record type that has been added to other workspaces. 
   
   You must first delete it from the secondary workspaces where it's been added, before you can delete it from its original workspace. 

   Deleting a global record type from their secondary workspaces only remove them, their records, and that workspace's fields from the secondary workspace. It does not delete the global record type from its original workspace.

   For information, see the section "Delete a global record type from a secondary workspace" in the article [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md). 

</div>
-->

## 레코드 유형 삭제

{{step1-to-planning}}

1. 레코드 유형을 삭제할 작업 영역을 클릭합니다.

   또는

   작업 영역에서 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 작업 영역을 검색한 다음 목록에 표시될 때 선택합니다.

   작업공간이 열리고 레코드 유형이 표시됩니다.
1. 다음 중 하나를 수행하십시오.

   * 레코드 종류 카드 위에 마우스를 올려 놓고 **자세히** 메뉴를 클릭한 다음 **삭제**&#x200B;합니다.
   * 삭제할 레코드 종류의 카드를 클릭하고 레코드 종류 페이지에서 레코드 종류 이름 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭한 다음 **삭제**&#x200B;를 클릭합니다.

   ![레코드 종류 확인 영구적으로 삭제](assets/permanently-delete-record-type-confirmation.png)

   <!--[!TIP]
   >
   ><span class="preview">You cannot delete global record types added to other workspaces. First, delete the global record types form their secondary workspaces before deleting them from the original workspace.</span>-->


1. 확인 상자에 **delete**&#x200B;을(를) 입력한 다음 **영구적으로 삭제**&#x200B;을(를) 클릭합니다. 대/소문자를 구분하지 않습니다.

   선택한 레코드 종류 및 해당 필드, 관련 레코드 및 보기는 삭제되며 복구할 수 없습니다.


