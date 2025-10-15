---
title: 중복 레코드
description: 테이블 보기에서 기존 레코드를 복제할 수 있습니다. 기존 레코드의 동일한 복사본이 레코드 유형 페이지에 추가됩니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2fed8c96-0c9c-4662-a9c4-66dae507ff2a
source-git-commit: b102960e088f072f10baadcbeca4f7f579daa287
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 1%

---

# 중복 레코드

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Adobe Workfront Planning에서 레코드는 레코드 유형의 인스턴스입니다.

테이블 보기에서 기존 레코드를 복제할 수 있습니다. 기존 레코드의 동일한 복사본이 레코드 유형 페이지에 추가됩니다.

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
   <td>   <p>작업 공간 및 레코드 유형에 대한 또는 그 이상의 권한 기여  </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p> </td> 
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
   <td>   <p>Contribute or higher permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->


## &#x200B;<!--in a record type table (I don't think you can create them elsewhere right now)--> 레코드 복제

기존 레코드를 복제하여 레코드 유형 페이지의 표 보기에서 레코드를 만들 수 있습니다. 기존 레코드와 동일한 레코드가 생성되어 원본 레코드 아래에 추가됩니다.


{{step1-to-planning}}

1. 레코드를 추가할 작업 영역을 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다. 레코드 종류 만들기에 대한 자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

   마지막으로 액세스한 보기에서 레코드 유형 페이지가 열립니다. 기본적으로 레코드 유형 페이지가 표 뷰에 열립니다.
선택한 유형의 모든 레코드가 뷰에 표시됩니다.

1. (조건부) 테이블 뷰를 선택합니다.

1. 다음 중 하나를 수행하십시오.

   * 레코드 이름 위로 마우스를 가져간 다음 레코드 이름과 인라인으로 **자세히** 메뉴를 클릭한 다음 **복제** 아이콘 ![복제 아이콘 회색](assets/duplicate-icon-gray.png) 을 클릭합니다.

     ![표 보기의 레코드에서 메뉴 더 보기](assets/more-menu-from-record-in-table-view.png)

   * 레코드를 선택한 다음 페이지 하단의 도구 모음에서 **복제** 아이콘 ![복제 아이콘 흰색 및 파란색](assets/duplicate-icon-white-and-blue.png)을 클릭합니다.

     ![테이블 보기의 도구 모음에 있는 중복 아이콘](assets/duplicate-icon-in-toolbar-in-table-view.png)

   원래 레코드 아래에 이름이 같은 동일한 레코드가 만들어집니다. 새 레코드의 모든 필드는 원래 레코드와 동일한 정보로 채워집니다.

1. (선택 사항) 테이블 보기에서 사용할 수 있는 필드에서 새 레코드에 대한 정보 업데이트를 시작하거나 레코드 미리 보기 또는 페이지에서 레코드 및 업데이트 정보를 클릭합니다.

   >[!NOTE]
   >
   >  * 레코드에 대한 필수 필드가 없습니다. 그러나 레코드를 서로 연결할 때 레코드를 식별하는 데 도움이 되므로 레코드의 기본 필드에 대한 정보를 추가하는 것이 좋습니다. 기본 필드에 대한 자세한 내용은 [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md) 및 [기본 필드 개요](/help/quicksilver/planning/fields/primary-field-overview.md)를 참조하십시오.
   >
   >  * 다른 레코드 종류 또는 계산된 필드를 참조하는 필드는 읽기 전용 필드입니다.

   레코드 편집에 대한 자세한 내용은 [레코드 편집](/help/quicksilver/planning/records/edit-records.md)을 참조하세요.

1. (선택 사항) 다음 키보드 단축키를 사용하여 표 보기에서 새 레코드 또는 해당 정보를 추가할 때 해당 추가 작업을 취소하거나 다시 실행합니다.

   * 변경 내용을 실행 취소하려면 CTRL + Z(⌘ + Z, Mac)
   * Mac 변경 내용을 다시 실행하려면 CTRL + Shift + Z(⌘ + Shift + Z)를 누릅니다.
