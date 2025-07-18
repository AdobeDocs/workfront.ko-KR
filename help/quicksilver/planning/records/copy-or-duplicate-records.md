---
title: 중복 레코드
description: 테이블 보기에서 기존 레코드를 복제할 수 있습니다. 기존 레코드의 동일한 복사본이 레코드 유형 페이지에 추가됩니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2fed8c96-0c9c-4662-a9c4-66dae507ff2a
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 2%

---

# 중복 레코드

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Adobe Workfront Planning에서 레코드는 레코드 유형의 인스턴스입니다.

테이블 보기에서 기존 레코드를 복제할 수 있습니다. 기존 레코드의 동일한 복사본이 레코드 유형 페이지에 추가됩니다.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

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
   <td role="rowheader"><p>Adobe Systems Workfront 플랜*</p></td> 
   <td> 
<p>다음 Workfront 플랜 중 하나:</p> 
<ul><li>선택</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Systems Workfront 계획 패키지*</p></td> 
   <td> 
<p>어떤 </p> 
<p>각 Workfront Planning 플랜에 포함된 항목에 대한 자세한 내용은 Workfront 계정 관리자 관리자에게 문의하십시오. </p> 
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
   <p>Workfront Planning은 기존 Workfront 라이선스에 사용할 수 없습니다</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역 및 레코드 종류</a>에 대한 권한 또는 그 이상을 제공하십시오. </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서[의 액세스 요구 사항을 참조하십시오](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## 레코드 복제 <!--in a record type table (I don't think you can create them elsewhere right now)-->

레코드 종류 페이지 의 테이블 보기에서 기존 레코드를 복제하여 레코드를 만들 수 있습니다. 기존 레코드와 동일한 레코드가 만들어지고 원래 레코드 아래에 추가됩니다.


{{step1-to-planning}}

1. 레코드를 추가할 작업 영역 클릭

   작업 영역 영역이 열리고 레코드 종류가 카드로 표시됩니다.

1. 레코드 종류 카드 클릭 레코드 종류를 만드는 방법에 대한 자세한 내용은 레코드 종류[ 만들기 항목을 참조하십시오](/help/quicksilver/planning/architecture/create-record-types.md).

   레코드 종류 페이지 가 마지막으로 액세스한 보기에서 열립니다. 기본적으로 레코드 종류 페이지 는 테이블 보기에서 열립니다.
선택한 유형의 모든 레코드가 뷰에 표시됩니다.

1. (조건부) 테이블 보기를 선택합니다.

1. 다음 중 하나를 수행하십시오.

   * 레코드 이름 위로 마우스를 가져간 다음 레코드 이름과 인라인으로 **자세히** 메뉴를 클릭한 다음 **복제** 아이콘 ![복제 아이콘 회색](assets/duplicate-icon-gray.png) 을 클릭합니다.

     ![표 보기의 레코드에서 메뉴 더 보기](assets/more-menu-from-record-in-table-view.png)

   * 레코드를 선택한 다음 페이지 하단의 도구 모음에서 **복제** 아이콘 ![복제 아이콘 흰색 및 파란색](assets/duplicate-icon-white-and-blue.png)을 클릭합니다.

     ![테이블 보기의 도구 모음에 있는 중복 아이콘](assets/duplicate-icon-in-toolbar-in-table-view.png)

   원래 레코드 아래에 이름이 같은 동일한 레코드가 만들어집니다. 새 레코드의 모든 필드는 원래 레코드와 동일한 정보로 채워집니다.

1. (선택 사항) 테이블 보기에서 사용할 수 있는 필드에서 새 레코드에 대한 정보 업데이트를 시작하거나 레코드 미리 보기 또는 페이지에서 레코드 및 업데이트 정보를 클릭합니다.

   >[!NOTE]
   >
   >  * 레코드에 대한 필수 필드는 없습니다. 그러나 레코드를 서로 연결할 때 레코드를 식별하는 데 도움이 되므로 레코드의 기본 필드에 대한 정보를 추가하는 것이 좋습니다. 기본 필드에 대한 자세한 내용은 테이블 보기[ 관리 및 ](/help/quicksilver/planning/views/manage-the-table-view.md)기본 필드 개요를[ 참조하세요](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * 다른 레코드 종류 또는 계산된 필드를 참조하는 필드는 읽기 전용 필드입니다.

   레코드 편집에 대한 자세한 내용은 레코드[ 편집을 참조하십시오](/help/quicksilver/planning/records/edit-records.md).

1. (선택 사항) 다음 키보드 단축키를 사용하여 새 레코드 또는 해당 정보를 테이블 보기에 추가할 때 추가를 실행 취소하거나 다시 실행할 수 있습니다.

   * CTRL + Z(⌘ Mac의 경우 + Z)를 사용하여 변경 사항을 실행 취소합니다.
   * CTRL + Shift + Z(⌘ Mac의 경우 + Shift + Z)를 눌러 변경 사항을 다시 실행합니다.
