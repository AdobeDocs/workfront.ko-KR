---
title: 레코드 삭제
description: 사용자 또는 다른 사용자가 만든 레코드를 삭제할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 2%

---


# 레코드 삭제

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->

{{planning-important-intro}}

Adobe Workfront Planning에서 더 이상 관련이 없는 레코드를 삭제할 수 있습니다. 삭제된 레코드는 삭제된 후 30일 동안 복구할 수 있습니다. 삭제된 레코드 복구에 대한 자세한 내용은 [삭제된 레코드 복구](/help/quicksilver/planning/records/restore-deleted-records.md)를 참조하십시오.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

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
<p>Workfront Planning에 액세스하려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
   <td><p> 표준</p>
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
   <td>   <p>작업 영역 및 레코드 종류 </a>에 대한 권한 이상 제공 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 레코드 삭제에 대한 고려 사항

* 사용자 또는 다른 사용자가 만든 레코드를 삭제할 수 있습니다.
* 본인 또는 다른 사람이 삭제한 삭제된 레코드를 복구할 수 있습니다.
* 삭제된 레코드가 다른 레코드와 연결된 경우 연결된 레코드는 삭제되지 않지만 삭제된 레코드의 정보도 삭제됩니다.
* 타임라인 또는 달력 보기에서는 레코드를 삭제할 수 없습니다.

## 레코드 삭제

다음 영역에서 레코드를 삭제할 수 있습니다.

* [레코드 페이지에서](#delete-a-record-from-the-records-page)
* [레코드 종류의 테이블 보기에서](#delete-a-record-from-the-record-type-table-view)

### 레코드 페이지에서 레코드 삭제

{{step1-to-planning}}

1. 삭제할 레코드가 있는 작업 영역을 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.
1. 다음 중 하나를 수행하십시오.

   * 테이블 보기에서 레코드 이름을 클릭합니다.
   * 테이블 보기에서 레코드 이름 위로 마우스를 가져간 다음 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **보기**&#x200B;를 클릭합니다

     ![레코드 행의 상황에 맞는 메뉴](assets/contextual-menu-for-record-row.png)
   * 타임라인 보기에서 레코드 모음을 클릭합니다.

   레코드 페이지가 열립니다.

1. 레코드 이름의 오른쪽에 있는 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **삭제**&#x200B;를 클릭한 다음 다시 **삭제**&#x200B;를 클릭하여 확인합니다.

   ![레코드 세부 정보 페이지의 추가 메뉴 옵션](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
레코드가 삭제되었습니다.
1. (선택 사항) 레코드 페이지의 테이블 보기로 이동한 다음, 보기의 오른쪽 상단에 있는 **실행 취소** 아이콘 ![실행 취소 아이콘](assets/undo-icon.png)을 클릭한 다음, **최근에 삭제됨**&#x200B;을 클릭하여 삭제된 레코드를 복구합니다.

삭제된 레코드 복구에 대한 자세한 내용은 [삭제된 레코드 복구](/help/quicksilver/planning/records/restore-deleted-records.md)를 참조하십시오.

### 레코드 유형 테이블 보기에서 레코드 삭제

{{step1-to-planning}}

1. 삭제할 레코드가 있는 작업 영역을 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.
1. (조건부) 표의 왼쪽 위 모서리에 있는 **보기** 드롭다운 메뉴에서 표 보기를 선택합니다. 레코드 유형에 마지막으로 액세스했을 때 타임라인 보기에서 확인하지 않은 경우 기본 보기여야 합니다.

   선택한 레코드 유형과 연관된 레코드가 테이블 뷰에 표시됩니다.
1. 다음 중 하나를 수행하십시오.

   * 레코드 행을 마우스 오른쪽 단추로 클릭한 다음 **삭제**&#x200B;를 클릭합니다.
   * 레코드 이름 오른쪽의 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **삭제**&#x200B;를 클릭합니다.

     ![레코드 행의 상황에 맞는 메뉴](assets/contextual-menu-for-record-row.png)

   * **세부 정보 열기** 아이콘 ![테이블 이름 필드의 세부 정보 열기 아이콘](assets/open-details-icon-in-table-name-field.png)을 클릭하여 레코드의 세부 정보가 있는 상자를 열고 레코드 이름 오른쪽에 있는 **자세히** ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **삭제**&#x200B;를 클릭합니다.

   레코드가 삭제되었습니다.

1. (선택 사항) 다음 중 하나를 수행하여 레코드 삭제를 실행 취소하거나 재실행합니다.

   * **실행 취소** 아이콘 ![실행 취소 아이콘](assets/undo-icon.png)을 클릭한 다음 **최근에 삭제됨**&#x200B;을 클릭하여 삭제된 레코드를 복구합니다. 삭제된 레코드 복구에 대한 자세한 내용은 [삭제된 레코드 복구](/help/quicksilver/planning/records/restore-deleted-records.md)를 참조하십시오.
   * 다음 키보드 단축키를 사용하여 레코드 삭제를 실행 취소하거나 재실행할 수 있습니다.

      * 레코드 삭제를 취소하려면 CTRL + Z(⌘ + Z, Mac)
      * Mac 레코드 삭제를 다시 실행하려면 CTRL + Shift + Z(⌘ + Shift + Z)




