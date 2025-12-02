---
title: 레코드 유형 삭제
description: 더 이상 관련이 없는 레코드 유형은 삭제할 수 있습니다. 레코드 유형을 삭제하면 레코드, 필드 및 보기와 같이 레코드 유형과 관련된 모든 정보도 삭제됩니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 476e10f2962f19fd17705cb5f20619d3b636aaa4
workflow-type: tm+mt
source-wordcount: '1062'
ht-degree: 1%

---


<!--keep the global record type reference in yellow till January 2026-->

# 레코드 유형 삭제

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

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
<li><p>모든 워크플로우 및 모든 Planning 패키지</p></li></ul>
<div class="preview">
<p>글로벌 레코드 유형을 삭제하려면</p>
<ul><li><p>모든 Workfront 패키지 및 Planning Plus 패키지</p></li>
또는
<li><p>모든 워크플로우 및 Planning Prime 또는 Ultimate 패키지</p></li></ul>
</div>
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

<div class="preview">

* 다른 작업 영역에 추가된 글로벌 레코드 유형은 삭제할 수 없습니다.

  자세한 내용은 이 문서의 [글로벌 레코드 종류 삭제](#delete-global-record-types) 섹션을 참조하십시오.

</div>

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


1. 확인 상자에 **delete**&#x200B;을(를) 입력한 다음 **영구적으로 삭제**&#x200B;을(를) 클릭합니다. 대/소문자를 구분하지 않습니다.

   선택한 레코드 종류 및 해당 필드, 관련 레코드 및 보기는 삭제되며 복구할 수 없습니다.

<div class="preview">

## 글로벌 레코드 유형 삭제

글로벌 레코드 유형을 삭제할 때 다음과 같은 시나리오가 있습니다.

* 글로벌로 구성된 레코드 유형이 아직 다른 작업 공간에 추가되지 않은 경우 원래 작업 공간에서 삭제할 수 있습니다.

* 글로벌 레코드 유형으로 구성된 레코드 유형이 하나 이상의 다른 작업 영역에 추가된 경우 원래 작업 영역에서 삭제할 수 없습니다. 글로벌 레코드 유형이 추가된 보조 작업 영역에서 글로벌 레코드 유형을 먼저 삭제(삭제)해야 원래 작업 영역에서 글로벌 레코드 유형을 영구적으로 삭제할 수 있습니다.

### 원래 작업 영역에서 글로벌 레코드 유형 삭제

더 이상 관련이 없는 경우 원래 작업 영역에서 레코드 유형을 삭제할 수 있습니다.

1. 원래 작업 영역의 글로벌 레코드 유형으로 이동합니다.

1. (조건부) 글로벌 레코드 유형이 보조 작업 공간에 추가되었는지 여부에 따라 다음 중 하나를 수행합니다.

   * 레코드 종류가 보조 작업 영역에 추가되지 않은 경우 레코드 종류의 카드에서 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭하거나 해당 페이지에서 레코드 종류 이름의 오른쪽에 있는 **삭제**&#x200B;를 클릭하십시오.
   * 레코드 유형이 다른 하나 이상의 보조 작업 영역에 추가된 경우 먼저 보조 작업 영역으로 이동하여 해당 공간에서 글로벌 레코드를 삭제합니다.

     자세한 내용은 이 문서의 [보조 작업 영역에서 글로벌 레코드 종류 삭제](#delete-a-global-record-type-from-a-secondary-workspace) 섹션을 참조하십시오.

1. (조건부) 이 문서의 [레코드 종류 삭제](#delete-record-types-1) 섹션에 설명된 대로 레코드 종류를 계속 삭제합니다.

   다음과 같은 상황이 발생합니다.

   * 글로벌 레코드 유형이 원래 작업 영역에서 제거되고 레코드 유형, 해당 레코드 및 필드는 복구할 수 없습니다.
   * 보조 작업 영역의 모든 글로벌 레코드 유형과 해당 레코드도 제거됩니다.

### 보조 작업 영역에서 글로벌 레코드 유형 삭제

더 이상 필요하지 않은 경우 다른 작업 영역에서 추가한 레코드 유형을 삭제할 수 있습니다.

다음 사항을 고려하십시오.

* 보조 작업 영역에서 글로벌 레코드 유형을 삭제하면 보조 작업 영역에서만 제거됩니다. 레코드 유형은 원본 작업 공간에 남아 있습니다.

* 보조 작업 영역에서 글로벌 레코드 유형을 삭제하면 다음 항목도 삭제됩니다.

   * 보조 작업 영역에서 추가된 레코드입니다.

  <!--Coming later: * The fields added from the secondary workspace.-->

* 보조 작업 영역에서 삭제된 글로벌 레코드 유형은 복구할 수 없습니다.

* 원래 레코드 유형은 원래 작업 영역뿐만 아니라 원래 작업 영역이 추가된 다른 작업 영역에도 유지됩니다.

보조 작업 영역에서 글로벌 레코드 유형을 삭제하려면 다음을 수행합니다.

1. 보조 작업 공간의 글로벌 레코드 유형으로 이동합니다.

1. (선택 사항) 레코드 종류의 카드에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png) 또는 해당 페이지의 레코드 종류 이름 오른쪽에 있는 **삭제**&#x200B;를 클릭합니다.
1. (조건부) 제공된 필드에 **delete**&#x200B;을(를) 입력한 다음 **영구적으로 삭제**&#x200B;을(를) 클릭합니다.

   ![보조 글로벌 레코드 유형 삭제 확인 상자](assets/delete-secondary-global-record-type.png)

   다음과 같은 상황이 발생합니다.

   * 글로벌 레코드 유형에서 만든 레코드 유형이 선택한 작업 영역에서 제거됩니다.
   * 필드가 있는 원래 레코드 유형은 원래 작업 영역에 유지됩니다.
   * 레코드 유형은 추가된 다른 모든 작업 영역에 남아 있습니다.
   * 현재 작업 영역에서 레코드 형식에 추가된 <!--and fields--> 레코드가 삭제됩니다. 글로벌 레코드 유형이 추가된 추가 작업 영역에서 추가된 다른 모든 레코드는 해당 작업 영역과 원래 작업 영역에서 보존됩니다. &lt;!- 필드가 추가된 작업공간에 보존됩니다.

</div>
