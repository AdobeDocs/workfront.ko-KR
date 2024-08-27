---
title: 작업 공간 만들기
description: 작업 영역은 팀에서 사용하는 레코드 유형의 컬렉션으로, 팀의 작업 라이프사이클을 나타냅니다. Adobe Workfront Planning에서 작업 공간을 완전히 사용자 정의할 수 있습니다. 레코드 유형은 작업 영역의 섹션별로 구성됩니다.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 83c716dea3815ed9a2ce4c3d0598ef42b128de87
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 작업 공간 만들기

{{planning-important-intro}}

Adobe Workfront Planning에서 작업 공간은 팀이 작업을 계획하는 중앙 집중식 위치입니다.

작업 영역은 팀에서 사용하는 레코드 유형의 컬렉션으로, 팀의 작업 라이프사이클을 나타냅니다. Adobe Workfront Planning에서 작업 공간을 완전히 사용자 정의할 수 있습니다.

작업 영역에 대한 일반적인 정보는 [작업 영역 개요](/help/quicksilver/planning/architecture/workspaces-overview.md)를 참조하십시오.

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
   <td>   <p>작성한 작업 공간에 대한 관리 권한을 받습니다. </p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>레이아웃 템플릿</p></td> 
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!---
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
   Or
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>You receive Manage permissions to the workspaces you create. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>You must add the Planning area to your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

For more information about access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 
-->

## 작업 영역 만들기

작업공간을 만들고 여기에 레코드 유형을 추가하여 Workfront Planning에서 객체를 구성할 수 있습니다. 작업 영역 편집에 대한 자세한 내용은 [작업 영역 편집](/help/quicksilver/planning/architecture/edit-workspaces.md)을 참조하십시오.

{{step1-to-planning}}

1. **작업 영역 만들기** 클릭

   작업 공간 만들기 상자가 표시됩니다. 작업공간을 처음부터 만들거나 사용 가능한 템플릿 중 하나를 사용하여 만들 수 있습니다.

1. (선택 사항 및 조건부) 미리 정의된 다음 작업 영역 템플릿 내에서 **미리 보기**&#x200B;를 클릭합니다.

   * 기본: 마케팅 관리
   * 고급: 마케팅 관리
   * 엔터프라이즈: 마케팅 관리
   * 영업 관리
   * 제품 관리

   템플릿 미리보기 상자가 열립니다.

   각 템플릿과 연관된 운영 레코드 유형, 분류 및 필드 수가 표시됩니다.

   ![](assets/previewing-a-workspace-template.png)

   Workfront Planning 작업 영역 템플릿에 대한 자세한 내용은 [작업 영역 템플릿 목록](/help/quicksilver/planning/architecture/workspace-templates.md)을 참조하십시오.

1. 템플릿 미리 보기 상자에서 **템플릿 사용**&#x200B;을 클릭하여 선택한 템플릿에서 작업 영역 만들기를 시작합니다

   또는

   **뒤로**&#x200B;를 클릭한 다음 **새 작업 영역**&#x200B;을 클릭하여 작업 영역을 처음부터 만듭니다.

   다음 유형의 작업 공간에 대한 하나가 만들어집니다.

   * 처음부터 작업 영역을 만들 때 레코드 형식을 수동으로 추가할 수 있는 빈 작업 영역(**제목 없는 Workspace**)입니다.
   * 선택한 템플릿 이름을 따라 이름이 지정되고 샘플 레코드 유형으로 채워진 작업 영역입니다. 레코드 유형 및 작업 영역을 추가로 사용자 지정할 수 있습니다.

   Workfront 관리자의 경우 새 작업 영역이 내가 있는 **작업 영역** 탭에 표시됩니다.

   작업 영역을 만들 수 있는 다른 모든 사용자의 경우 **작업 영역** 영역에 새 작업 영역이 표시됩니다.

1. 새 작업 영역의 헤더에서 작업 영역 이름 내부를 클릭하여 이름을 변경한 다음 Enter 키를 누릅니다.

1. (선택 사항 및 조건부) 템플릿에서 작업 영역을 만든 경우 **작업 레코드 종류** 또는 **분류** 섹션의 이름 내부를 클릭합니다

   또는

   섹션의 이름을 마우스로 가리킨 다음 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 다음 **이름 바꾸기**&#x200B;를 클릭하여 섹션의 이름을 변경합니다.

   >[!TIP]
   >
   >섹션을 만들지 않았더라도 작업 영역에서 섹션의 이름을 변경할 수 있습니다.

   작업 영역 섹션 편집을 포함하여 작업 영역 편집에 대한 자세한 내용은 [작업 영역 편집](/help/quicksilver/planning/architecture/edit-workspaces.md)을 참조하십시오.

1. (선택 사항) **레코드 종류 추가**&#x200B;를 클릭하여 모든 섹션의 작업 영역에 레코드 종류를 추가합니다.

   자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

   작업 영역의 레코드 형식을 편집하고 삭제하는 방법에 대한 자세한 내용은 [작업 영역 편집](/help/quicksilver/planning/architecture/edit-workspaces.md)을 참조하십시오.


