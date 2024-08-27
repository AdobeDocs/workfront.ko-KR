---
title: 레코드 유형 편집
description: 레코드 유형을 저장한 후 편집할 수 있습니다. 레코드 유형은 Adobe Workfront Planning의 객체 유형입니다.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 83c716dea3815ed9a2ce4c3d0598ef42b128de87
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 2%

---


# 레코드 유형 편집

{{planning-important-intro}}

레코드 유형은 Adobe Workfront Planning의 객체 유형입니다. 사용자 또는 다른 사용자가 만든 레코드 유형의 모양을 편집할 수 있습니다. Workfront Planning 레코드 유형을 만드는 방법에 대한 자세한 내용은 [레코드 유형 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하십시오.

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
   <td>   <p>작업 영역</a>에 대한 권한 관리 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
   <p>시스템 관리자만 다른 작업 영역에서 레코드 유형을 연결할 수 있습니다.</p> </td> 
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
   <p> Adobe Workfront</p> <p>To connect Adobe Workfront Planning record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Business Platform or the Adobe Admin Console.</p> </td>
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
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->

## 레코드 유형 편집

{{step1-to-planning}}

1. 레코드 유형을 편집할 작업 영역을 클릭합니다.

   작업 영역 페이지가 열리고 레코드 유형이 표시됩니다.
1. 다음 중 하나를 수행하십시오.

   * 레코드 종류의 카드 위에 마우스를 올려 놓고 레코드 종류 카드의 오른쪽 상단에서 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 다음 **편집**을(를) 클릭합니다
또는
   * 레코드 유형 카드를 클릭하여 레코드 유형 페이지를 열고 레코드 유형 이름 오른쪽에 있는 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 다음 **편집**&#x200B;을(를) 클릭합니다.

   ![](assets/more-menu-options-from-record-type-card.png)

1. **레코드 종류 편집** 상자에서 기본적으로 **모양** 탭이 열립니다.

   ![](assets/edit-record-type-box-appearance-tab.png)

   **모양** 탭에서 다음 정보를 업데이트합니다.

   * 필요한 경우 레코드 유형 이름을 편집합니다. <!--did they add a field label for this?-->
   * **설명**: 레코드 형식에 대한 자세한 내용을 포함하여 설명을 편집하거나 추가합니다.
   * 레코드 종류와 관련된 아이콘의 색 및 모양을 편집합니다. 다음을 수행합니다.
      * 레코드 유형을 식별할 색상을 선택합니다. 레코드 유형 아이콘의 색상입니다.
      * 목록에서 아이콘을 선택하거나 아이콘 이름을 입력하여 아이콘이 나타내는 내용을 설명한 다음 표시될 때 선택합니다. 레코드 유형의 아이콘입니다. 기본적으로 파일 아이콘이 선택되어 있습니다.

1. (조건부) 시스템 관리자인 경우 **레코드 종류 편집** 상자에서 **고급 설정** 탭을 클릭합니다.

   ![](assets/edit-record-type-box-advanced-settings-tab.png)

1. (조건부) 시스템 관리자는 **고급 설정** 탭에서 다음 정보를 업데이트합니다.

   * **다른 작업 영역에서 연결**: 사용자가 다른 작업 영역에서 이 레코드 형식에 연결할 수 있도록 하려면 이 토글을 선택하십시오. 기본적으로 선택되어 있지 않습니다.
   * **시스템 전체**: 사용자가 시스템의 모든 작업 영역에서 이 레코드에 연결할 수 있도록 하려면 이 옵션을 선택하십시오.
   * **특정 작업 영역**: 사용자가 이 레코드 종류에 연결할 수 있는 작업 영역을 제한하려면 이 옵션을 선택한 다음 드롭다운 메뉴를 확장하고 사용자가 이 레코드 종류에 연결할 작업 영역을 선택하십시오. 작업 공간의 이름을 입력하고 목록에 표시될 때 선택할 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.

   작업 영역의 레코드 유형 카드에 오른쪽 상단 모서리에 연결 아이콘 ![](assets/connect-from-other-workspaces-icon.png)이(가) 표시되어 이제 다른 작업 영역에서 레코드에 액세스할 수 있음을 나타냅니다.

1. (선택 사항) 작업 영역 영역에서 레코드 유형 카드를 클릭하여 레코드 유형의 페이지를 연 다음 헤더에서 레코드 유형의 이름을 변경합니다.

1. (선택 사항) 다른 레코드 유형을 편집하려면 레코드 유형 페이지에서 레코드 유형 이름의 오른쪽에 있는 아래쪽 화살표를 확장하고 레코드 유형을 검색한 다음 목록에 표시될 때 선택합니다.

   ![](assets/record-type-drop-down-on-record-type-page-with-search-box.png)