---
title: 작업 영역 삭제
description: 더 이상 관련이 없는 작업 공간은 삭제할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: 6d9583f8a0e1e0c3712c8a47d68c5d5d321679f9
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 1%

---


# 작업 영역 삭제

{{planning-important-intro}}

Adobe Workfront Planning에서 작업 공간은 팀이 작업을 계획하는 중앙 집중식 위치입니다. 자세한 내용은 [작업 영역 만들기](/help/quicksilver/planning/architecture/create-workspaces.md)를 참조하십시오.

더 이상 관련이 없는 작업 공간은 삭제할 수 있습니다.

삭제하기 전에 다른 작업 영역에서 삭제하려는 작업 영역과 관련된 레코드 유형, 레코드, 필드 및 보기의 일부 또는 전체를 다시 만드는 것이 좋습니다.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항 보기..

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <td role="rowheader"><p>Adobe Workfront 계획 패키지*</p></td> 
   <td> 
<p>임의 </p> 
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning의 모든 기능에 액세스할 수 있으려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p> 
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
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p> </td> 
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
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
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

*For more information about access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->


## 작업 영역 삭제에 대한 고려 사항

* 작업 공간을 삭제하면 모든 레코드 유형, 레코드, 해당 필드 및 보기도 삭제됩니다.
* 삭제된 작업 영역과 여기에 포함된 정보는 복구할 수 없습니다.

## 작업 영역 삭제

{{step1-to-planning}}

1. (조건부) Workfront 관리자인 경우 **내가 속한 작업 영역**&#x200B;을 클릭하여 만든 작업 영역에 액세스하거나 **다른 작업 영역**&#x200B;을 클릭하여 나와 공유된 작업 영역에 액세스합니다.

1. (선택 사항) 추가 작업 영역을 표시하려면 **모두 표시**&#x200B;를 클릭합니다. 작업 영역 카드가 두 개 이상 있는 경우에만 **모두 표시** 링크가 표시됩니다.
1. (선택 사항) 화면에 표시되는 작업 영역의 수를 제한하려면 **간단히 표시**&#x200B;를 클릭합니다.
1. 작업 영역을 삭제하려면 다음 중 하나를 수행합니다.

   * 작업 영역 카드 위로 마우스를 가져간 다음 카드의 오른쪽 상단에 있는 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭합니다
또는
   * 작업 영역 카드를 클릭하여 작업 영역을 연 다음 작업 영역 이름 오른쪽에 있는 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭합니다.
1. **삭제**&#x200B;를 클릭합니다.

   ![](assets/permanently-delete-workspace-confirmation.png)

1. 제공된 공간에 &quot;**delete**&quot;을(를) 입력한 다음 **영구적으로 삭제**&#x200B;을(를) 클릭합니다. 대/소문자를 구분하지 않습니다.

   작업 영역이 삭제되며 복구할 수 없습니다. 모든 레코드 종류, 레코드, 필드 및 연결된 보기도 삭제됩니다. <!--ensure this is right at or before GA-->
