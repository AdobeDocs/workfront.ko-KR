---
title: 작업 영역 삭제
description: 더 이상 관련이 없는 작업 공간은 삭제할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/yzpirNfY0Hsp0cbClQA8dFqhgqbpK8ZryIyeq4tBAgw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 347c3e87fea0289616bf1a52779c07501a8ec69d
workflow-type: tm+mt
source-wordcount: 459
ht-degree: 2%

---

# 작업 영역 삭제

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

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
<p>Planning 패키지가 있는 모든 Workfront 또는 워크플로우</p> 
또는
<p>독립 실행형 제품으로 구입할 경우 모든 Workfront Planning</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>Any</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Planning 라이선스</p></td> 
   <td><p>Any</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>워크플로우와 Planning 패키지가 모두 있는 경우 액세스 레벨에 워크플로우와 Planning 라이선스 유형을 모두 추가해야 합니다.</p>   
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

<!--
Old:

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
   <td> <p>You must add both a Workflow and a Planning license type to the access level when you have both a Workflow and a Planning package</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table>
-->

## 작업 영역 삭제에 대한 고려 사항

* 작업 공간을 삭제하면 모든 레코드 유형, 레코드, 해당 필드 및 보기도 삭제됩니다.
* 삭제된 작업 영역과 여기에 포함된 정보는 복구할 수 없습니다.

## 작업 영역 삭제

{{step1-to-planning}}

1. (조건부) Workfront 관리자인 경우 다음 중 하나를 클릭합니다.

   * 생성한 작업 영역에 액세스하기 위해 **내가 속한 작업 영역**
   * **모든 작업 영역** 사용자와 공유된 작업 영역 또는 사용자가 만든 작업 영역에 액세스할 수 있습니다.

   >[!NOTE]
   >
   >**샘플 작업 영역** 탭에서 작업 영역을 삭제할 수 없습니다. 다중 작업 영역 템플릿 번들을 사용하여 샘플 작업 영역 탭의 작업 영역과 유사한 작업 영역을 만드는 것이 좋습니다. 자세한 내용은 [작업 영역 만들기](/help/quicksilver/planning/architecture/create-workspaces.md)를 참조하십시오.

1. (선택 사항) 추가 작업 영역을 표시하려면 **모두 표시**&#x200B;를 클릭합니다. 작업 영역 카드가 두 개 이상 있는 경우에만 **모두 표시** 링크가 표시됩니다.
1. (선택 사항) 화면에 표시되는 작업 영역의 수를 제한하려면 **간단히 표시**&#x200B;를 클릭합니다.
1. 작업 영역을 삭제하려면 다음 중 하나를 수행합니다.

   * 작업 영역 카드 위로 마우스를 가져간 다음 카드의 오른쪽 상단에 있는 **추가** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭합니다
     또는
   * 작업 영역 페이지의 오른쪽 위 모서리에 있는 **검색** 아이콘 ![검색 아이콘](assets/search-icon.png)을 클릭하여 이름으로 작업 영역을 검색하고 작업 영역 카드를 클릭하여 작업 영역을 연 다음 작업 영역 이름 오른쪽에 있는 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭합니다.

   >[!TIP]
   >
   >다음 키보드 조합을 사용하여 Workfront Planning 페이지에서 글로벌 검색 상자를 열고 작업 공간을 검색할 수 있습니다.
   >
   >* Windows의 경우 CTRL+K
   >* Mac의 경우 ⌘+K

1. **삭제**&#x200B;를 클릭합니다.

   ![작업 영역 영구적으로 삭제 확인](assets/permanently-delete-workspace-confirmation.png)

1. 제공된 공간에 &quot;**delete**&quot;을(를) 입력한 다음 **영구적으로 삭제**&#x200B;을(를) 클릭합니다. 대/소문자를 구분하지 않습니다.

   작업 영역이 삭제되며 복구할 수 없습니다. 모든 레코드 종류, 레코드, 필드 및 연결된 보기도 삭제됩니다. <!--ensure this is right at or before GA-->


