---
title: 작업 영역 삭제
description: 더 이상 관련이 없는 작업 공간은 삭제할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: ba5089fd02ca099d25ce0d3c2c2c039c2c6e2fe2
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 2%

---


# 작업 영역 삭제

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

{{planning-important-intro}}

Adobe Workfront Planning에서 작업 공간은 팀이 작업을 계획하는 중앙 집중식 위치입니다. 자세한 내용은 [작업 영역 만들기](/help/quicksilver/planning/architecture/create-workspaces.md)를 참조하십시오.

더 이상 관련이 없는 작업 공간은 삭제할 수 있습니다.

삭제하기 전에 다른 작업 영역에서 삭제하려는 작업 영역과 관련된 레코드 유형, 레코드, 필드 및 보기의 일부 또는 전체를 다시 만드는 것이 좋습니다.

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
<li><p>모든 워크플로우 및 모든 Planning 패키지</p></li></ul>
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
   <td><p> Standard </p>
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
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## 작업 영역 삭제에 대한 고려 사항

* 작업 공간을 삭제하면 모든 레코드 유형, 레코드, 해당 필드 및 보기도 삭제됩니다.
* 삭제된 작업 영역과 여기에 포함된 정보는 복구할 수 없습니다.

## 작업 영역 삭제

{{step1-to-planning}}

1. (조건부) Workfront 관리자인 경우 다음 중 하나를 클릭합니다.

   * 생성한 작업 영역에 액세스하기 위해 **내가 속한 작업 영역**
   * 다른 사용자와 공유된 작업 영역에 액세스할 수 있는 **다른 작업 영역**
또는
     <span class="preview">**나와 공유된 작업 영역 또는 사용자가 만든 작업 영역에 액세스할 수 있는 모든 작업 영역**</span>

1. (선택 사항) 추가 작업 영역을 표시하려면 **모두 표시**&#x200B;를 클릭합니다. 작업 영역 카드가 두 개 이상 있는 경우에만 **모두 표시** 링크가 표시됩니다.
1. (선택 사항) 화면에 표시되는 작업 영역의 수를 제한하려면 **간단히 표시**&#x200B;를 클릭합니다.
1. 작업 영역을 삭제하려면 다음 중 하나를 수행합니다.

   * 작업 영역 카드 위로 마우스를 가져간 다음 카드의 오른쪽 상단에 있는 **추가** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭합니다
또는
   * <span class="preview"> 작업 영역 페이지의 오른쪽 위 모서리에 있는 **검색** 아이콘 ![검색 아이콘](assets/search-icon.png)을 클릭하여 이름으로 작업 영역을 검색하고</span> 작업 영역 카드를 클릭하여 작업 영역을 연 다음 작업 영역 이름 오른쪽에 있는 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭합니다.
1. **삭제**&#x200B;를 클릭합니다.

   ![작업 영역 영구적으로 삭제 확인](assets/permanently-delete-workspace-confirmation.png)

1. 제공된 공간에 &quot;**delete**&quot;을(를) 입력한 다음 **영구적으로 삭제**&#x200B;을(를) 클릭합니다. 대/소문자를 구분하지 않습니다.

   작업 영역이 삭제되며 복구할 수 없습니다. 모든 레코드 종류, 레코드, 필드 및 연결된 보기도 삭제됩니다. <!--ensure this is right at or before GA-->


