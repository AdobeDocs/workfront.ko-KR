---
title: 레코드 종류의 설정 영역 구성
description: 레코드 유형을 설정 페이지에 저장한 후 편집할 수 있습니다.
hide: true
hidefromtoc: true
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 1%

---


<!--add better metadata at release:

title: Configure Record Type Settings
description: You can edit record types after they have been saved in the Settings page. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog 

-->

# 레코드 종류의 설정 영역 구성

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

{{planning-important-intro}}

레코드 유형이 Adobe Workfront Planning에 저장된 후 레코드 유형에 대한 추가 설정을 구성할 수 있습니다.

레코드 유형에 대해 정의하려는 기능에 따라 다음 중 하나를 수행하여 레코드 유형에 대한 추가 설정을 구성할 수 있습니다.

<!--the above will need to be reworded when we add automations and manage request forms to this area-->

* 편집 중

  자세한 내용은 [레코드 종류 편집](/help/quicksilver/planning/architecture/edit-record-types.md)을 참조하세요.

* 레코드 종류의 설정 페이지를 구성합니다.

  이 문서에서는 해당 설정 페이지를 구성하여 레코드 유형을 편집하는 방법에 대해 설명합니다.

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
<ul><li><p>모든 Workfront 패키지</p></li>
<p>And</p>
<li><p>연결 가능한 레코드 유형을 만들기 위한 모든 Planning 패키지</p></li>
<li><p>중앙 집중식 레코드 유형을 만드는 Planning Plus 패키지</p></li>
</ul>
<p>또는:</p>
<ul><li><p>워크플로우 및 계획 Prime 또는 Ultimate 패키지</p> </li></ul>
<p>각 Workfront Planning 패키지에 포함된 내용에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>표준</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역</a>에 대한 권한 관리 </p>  
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
</table> 

-->

## 설정 페이지에서 레코드 유형 정보 구성

해당 설정 페이지에서 정보를 구성하여 레코드 유형에 대한 작업 영역 간 기능을 정의할 수 있습니다.

<!--the intro above will change when we can configure more in this area -->

{{step1-to-planning}}

1. 레코드 유형을 편집할 작업 영역을 클릭합니다.

   작업 영역 페이지가 열리고 레코드 유형이 표시됩니다.
1. 다음 중 하나를 수행하십시오.

   * 레코드 종류의 카드 위에 마우스를 올려 놓고 레코드 종류 카드의 오른쪽 상단에서 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **설정**&#x200B;을 클릭합니다
또는
   * 레코드 유형 카드를 클릭하여 레코드 유형 페이지를 열고 레코드 유형 이름 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭한 다음 **설정**&#x200B;을 클릭합니다.

   <!--update screen shot at release-->

   ![레코드 종류 카드의 추가 메뉴 옵션](assets/more-menu-options-from-record-type-card.png)

1. **작업 영역 간 설정** 섹션이 기본적으로 선택됩니다.
1. 다음 설정 중 하나를 켜거나 끕니다.

   * **이 레코드 형식을 다른 작업 영역에 추가할 수 있도록 허용** 글로벌 레코드 형식임을 나타냅니다.
   * **다른 작업 영역에서 이 레코드 형식에 연결할 수 있도록 허용**&#x200B;하여 연결 가능한 레코드 형식임을 나타냅니다.

   설정은 기본적으로 꺼져 있습니다.

   자세한 내용은 [레코드 형식에 대한 작업 영역 간 기능 구성](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)을 참조하세요.