---
title: 중복 레코드 보기
description: 여러 버전의 보기를 유지하고 버전 간에 약간의 변경을 하려는 경우 Adobe Workfront Planning에서 보기를 복제할 수 있습니다. 이 문서에서는 보기를 복제하는 방법에 대해 설명합니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 441a53d1-ad39-41b7-93fe-2ae1836476c9
source-git-commit: b102960e088f072f10baadcbeca4f7f579daa287
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# 중복 레코드 보기

<!--remove preview and production references-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>


{{planning-important-intro}}

여러 버전의 보기를 유지하고 버전 간에 약간의 변경을 하려는 경우 Adobe Workfront Planning에서 보기를 복제할 수 있습니다.

뷰를 복제하면 기존 뷰의 동일한 복사본이 만들어집니다.

원래 보기의 공유 권한이 복제된 보기로 전송되지 않습니다.

중복 보기는 Workfront Planning의 모든 보기 유형에 대해 동일합니다.

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
   <td>   <p>보기에 대한 권한 관리</p>  
   <p>보기에 대한 권한을 보고 일시적으로 보기 설정을 변경하거나 복제합니다.</p> </td> 
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
   <td>   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings or to duplicate it.</p> </td> 
  </tr> 
</tbody> 
</table> -->

## 레코드 보기 복제

{{step1-to-planning}}

1. 작업 영역의 카드를 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.
기본적으로 선택된 유형의 모든 레코드가 테이블 뷰에 표시됩니다.

1. 사용하는 환경에 따라 다음을 수행합니다.

   * 프로덕션 환경에서 보기 탭의 보기 이름 중 하나를 마우스로 가리킨 다음 보기 이름 왼쪽의 **자세히** ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **복제**&#x200B;를 클릭합니다.
   * <span class="preview">미리 보기 환경에서 현재 보기 이름 옆에 있는 드롭다운 아이콘 ![드롭다운 아이콘](assets/drop-down-icon.png)을 클릭하고 보기 이름을 마우스로 가리킨 다음 **자세히**&#x200B;를 클릭한 다음 **복제**&#x200B;을 클릭합니다.</span>

     ![옵션이 있는 보기의 추가 메뉴](assets/more-menu-for-views-expanded-with-delete-option.png)

     보기가 복제되고 새 보기의 이름이 `Original view's name (Copy)` 패턴을 따릅니다. 새 보기 탭은 모든 보기 탭의 끝에 표시됩니다.
