---
title: 레코드 유형 편집
description: 레코드 유형을 저장한 후 편집할 수 있습니다. 레코드 유형은 Adobe Workfront Planning의 객체 유형입니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 2fb95d37c32984e248767993c4858038d27e0590
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 2%

---


# 레코드 유형 편집

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

{{planning-important-intro}}

레코드 유형은 Adobe Workfront Planning의 객체 유형입니다. 사용자 또는 다른 사용자가 만든 레코드 유형의 모양을 편집할 수 있습니다. Workfront Planning 레코드 유형을 만드는 방법에 대한 자세한 내용은 [레코드 유형 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하십시오.

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
<p>모든 Workfront 및 Planning 패키지</p>
<p>모든 Workfront 및 Planning 패키지</p>
<p><b>메모</b></p>
<p>연결 가능한 레코드 유형을 구성하려면: </p>
<ul> 
<li><p>모든 Workfront 패키지 및 모든 Planning 패키지</p></li>
<p>또는</p>
<li><p>모든 워크플로우 및 Planning Prime 또는 Ultimate 패키지</p></li></ul>

<div class="preview">
<p>글로벌 레코드 유형을 구성하려면 다음을 수행합니다.</p>

<ul> 
<li><p>모든 Workfront 패키지 및 Planning Plus 패키지</p></li>
<p>또는</p>
<li><p>모든 워크플로우 및 Planning Prime 또는 Ultimate 패키지</p></li></ul>
<p>각 Workfront Planning 패키지에 포함된 내용에 대한 자세한 내용은 Workfront 계정 담당자에게 문의하십시오. </p>

</div>
   </td> </tr>
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
   <td>   <p>Manage permissions to a workspace and record type </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p> </td> 
  </tr> 

</tbody> 
</table> -->

## 레코드 유형 편집

{{step1-to-planning}}

1. 레코드 유형을 편집할 작업공간을 클릭합니다.

   작업 영역 페이지가 열리고 레코드 유형이 표시됩니다.
1. 다음 중 하나를 수행하십시오.

   * 레코드 종류의 카드 위에 마우스를 올려 놓고 레코드 종류 카드의 오른쪽 상단에서 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **편집**을 클릭합니다
     <span class="preview">또는 **설정**</span>
또는
   * 레코드 유형 카드를 클릭하여 레코드 유형 페이지를 열고 레코드 유형 이름 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭한 다음 **편집** <span class="preview">또는 **설정**</span>&#x200B;을 클릭합니다.

   <span class="preview">![설정이 있는 레코드 종류 카드의 추가 메뉴 옵션](assets/more-menu-options-from-record-type-card-with-settings-link.png)</span>

1. **레코드 종류 편집** 상자에서 기본적으로 **모양** 탭이 열립니다. <!--update screen shot below at production-->

   ![레코드 종류 상자 모양 편집 탭 ](assets/edit-record-type-box-appearance-tab.png)

   **모양** 탭에서 다음 정보를 업데이트합니다.

   * 필요한 경우 레코드 유형 이름을 편집합니다. <!--did they add a field label for this?-->
   * **설명**: 레코드 형식에 대한 자세한 내용을 포함하여 설명을 편집하거나 추가합니다.
   * 레코드 종류와 관련된 아이콘의 색 및 모양을 편집합니다. 다음을 수행합니다.
      * 레코드 유형을 식별할 색상을 선택합니다. 레코드 유형 아이콘의 색상입니다.
      * 목록에서 아이콘을 선택하거나 아이콘 이름을 입력하여 아이콘이 나타내는 내용을 설명한 다음 표시될 때 선택합니다. 레코드 유형의 아이콘입니다. 기본적으로 파일 아이콘이 선택되어 있습니다.

1. (선택 사항 및 조건부) 시스템 관리자인 경우 **고급 설정** <span class="preview"> 또는 **작업 영역 간 설정**</span> 탭을 클릭하고 레코드 유형의 작업 영역 간 기능에 대한 정보를 업데이트합니다.

   자세한 내용은 [레코드 형식에 대한 작업 영역 간 기능 구성](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)을 참조하십시오. <!--update screen shot at production - Jan 2026-->

   ![고급 설정 탭이 있는 레코드 종류 상자 편집](assets/edit-record-type-box-advanced-settings-tab.png)

1. **저장**&#x200B;을 클릭합니다.

   다른 작업 영역에서 이 레코드에 연결하도록 선택한 경우 **연결 가능한 레코드** 아이콘 ![다른 공간에서 연결 아이콘](assets/connect-from-other-workspaces-icon.png)이 레코드 카드에 표시됩니다.

   <span class="preview">다른 작업 영역에 이 레코드를 추가할 수 있도록 선택한 경우 **글로벌 레코드** 아이콘 ![글로벌 레코드 유형 아이콘](assets/global-icon.png)이 레코드 카드에 표시됩니다. </span>

1. (선택 사항) 작업 영역 영역에서 레코드 유형 카드를 클릭하여 레코드 유형의 페이지를 연 다음 헤더에서 레코드 유형의 이름을 변경합니다.

1. (선택 사항) 다른 레코드 유형을 편집하려면 레코드 유형 페이지에서 레코드 유형 이름의 오른쪽에 있는 아래쪽 화살표를 확장하고 레코드 유형을 검색한 다음 목록에 표시될 때 선택합니다.

   ![검색 상자가 있는 레코드 종류 페이지의 레코드 종류 드롭다운](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
