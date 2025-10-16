---
title: 작업 공간 만들기
description: 작업 영역은 팀에서 사용하는 레코드 유형의 컬렉션으로, 팀의 작업 라이프사이클을 나타냅니다. Adobe Workfront Planning에서 작업 공간을 완전히 사용자 정의할 수 있습니다. 레코드 유형은 작업 영역의 섹션별로 구성됩니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 작업 공간 만들기

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Adobe Workfront Planning에서 작업 공간은 팀이 작업을 계획하는 중앙 집중식 위치입니다.

작업 영역은 팀에서 사용하는 레코드 유형의 컬렉션으로, 팀의 작업 라이프사이클을 나타냅니다. Adobe Workfront Planning에서 작업 공간을 완전히 사용자 정의할 수 있습니다.

작업 영역에 대한 일반적인 정보는 [작업 영역 개요](/help/quicksilver/planning/architecture/workspaces-overview.md)를 참조하십시오.

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
<p>모든 Workfront 및 모든 Planning 패키지</p> <p>모든 워크플로우 및 모든 Planning 패키지</p>
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
   <td>   <p>You receive Manage permissions to the workspaces you create. </p> </td> 
  </tr> 
</tbody> 
</table> -->

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

   ![작업 영역 템플릿 미리 보기](assets/previewing-a-workspace-template.png)

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

   섹션의 이름을 마우스로 가리킨 다음 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **이름 바꾸기**&#x200B;를 클릭하여 섹션의 이름을 변경합니다.

   >[!TIP]
   >
   >섹션을 만들지 않았더라도 작업 영역에서 섹션의 이름을 변경할 수 있습니다.

   작업 영역 섹션 편집을 포함하여 작업 영역 편집에 대한 자세한 내용은 [작업 영역 편집](/help/quicksilver/planning/architecture/edit-workspaces.md)을 참조하십시오.

1. (선택 사항) **레코드 종류 추가**&#x200B;를 클릭하여 모든 섹션의 작업 영역에 레코드 종류를 추가합니다.

   자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

   작업 영역의 레코드 형식을 편집하고 삭제하는 방법에 대한 자세한 내용은 [작업 영역 편집](/help/quicksilver/planning/architecture/edit-workspaces.md)을 참조하십시오.

1. (선택 사항) 새 작업 공간 왼쪽에 있는 뒤로 화살표를 클릭하여 Planning 기본 페이지를 엽니다. **내가 있는 작업 영역** 탭에서 새 작업 영역에 대한 새 작업 영역 카드가 만들어집니다.

   작업공간을 생성한 사용자의 이름은 작업공간 카드에 소유자로 저장됩니다.

   >[!NOTE]
   >
   >현재 IMS(Adobe Identity Management System)로 전환 중인 사용자의 경우 IMS 사용자가 아닌 Workfront 전용 사용자가 만든 작업 영역은 **System**&#x200B;에서 만든 대로 표시됩니다.
   >
   >IMS에 대한 자세한 내용은 [Workfront용 Adobe 통합 환경](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)을 참조하세요.


