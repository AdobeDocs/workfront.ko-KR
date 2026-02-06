---
title: Adobe Workfront Planning에서 목록 보기 관리
description: Adobe Workfront Planning의 레코드의 연결된 레코드 페이지에서 액세스할 때 목록 보기에 객체와 해당 필드를 표시할 수 있습니다. 이 문서에서는 레코드의 연결된 레코드 페이지에서 목록 보기를 만들거나 편집하는 방법에 대해 설명합니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
source-git-commit: b2f1bbfbbec23a5400552eb0f989e0a0dc58413c
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 0%

---


# Adobe Workfront Planning에서 목록 보기 관리

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Adobe Workfront Planning의 레코드의 연결된 레코드 페이지에서 액세스할 때 목록 보기에 객체와 해당 필드를 표시할 수 있습니다.

이 문서에서는 레코드의 연결된 레코드 페이지에서 목록 보기를 만들거나 편집하는 방법과 보기에서 개체를 편집하는 방법에 대해 설명합니다.

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
<p>모든 Workfront 및 모든 Planning 패키지</p>
<p>모든 워크플로우 및 모든 Planning 패키지</p>
<p>각 Workfront Planning 패키지에 포함된 내용에 대한 자세한 내용은 Workfront 계정 담당자에게 문의하십시오. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p> 보기를 만들고 삭제하는 표준</p>
   <p>기여자 이상: 보기 요소 업데이트</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>보기에 대한 권한 관리</p>  
   <p>보기에 대한 권한을 보고 일시적으로 보기 설정을 변경하거나 복제합니다.</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> 라이트 또는 기여자 라이선스가 있는 사용자에게 Planning이 포함된 레이아웃 템플릿을 할당해야 합니다.
   <p>표준 사용자 및 시스템 관리자에게는 기본적으로 계획 영역이 활성화되어 있습니다.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++ 

## 목록 보기에 대한 고려 사항

* 목록 보기에서 레코드 유형 페이지의 레코드를 볼 수 없습니다. 다음 객체는 레코드의 연결된 레코드 페이지에서 볼 때만 목록 보기에 표시할 수 있습니다.

   * Workfront 프로젝트

  연결된 레코드 페이지를 만드는 방법에 대한 자세한 내용은 [레코드에 연결된 레코드 페이지 추가](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)를 참조하십시오.
* 레코드의 연결된 레코드 페이지에서 목록 보기를 보려면 먼저 Workfront 프로젝트를 Planning 레코드 유형과 연결해야 합니다. 자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.
* 목록 보기는 고급 목록과 유사합니다. 자세한 내용은 [향상된 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)을 참조하세요.


## 목록 보기 관리 {#manage-a-list-view}

Workfront의 목록 보기 관리에 대한 자세한 내용은 [향상된 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)을 참조하세요.

{{step1-to-planning}}

1. 작업 영역 카드를 클릭한 다음 레코드 유형 카드를 클릭합니다.
1. 보기에서 레코드 이름을 클릭하여 레코드의 미리 보기 또는 세부 정보 페이지를 엽니다.
1. **레코드에 연결된 레코드 페이지 추가** 문서에 설명된 대로 연결된 프로젝트에 대해 [연결된 레코드 페이지](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)를 추가하십시오.

   연결된 레코드 페이지는 목록 보기의 레코드에 연결된 프로젝트를 표시합니다.

   ![목록 보기의 연결된 레코드 페이지에 있는 프로젝트](assets/projects-on-connected-records-page-list-view.png)

1. (선택 사항) 목록 보기를 수정하려면 다음 중 하나를 수행합니다.

   1. 목록의 오른쪽 상단 모서리에서 드롭다운 보기 메뉴를 확장하여 다른 보기를 선택하거나 **새 보기**&#x200B;를 클릭하여 다른 보기를 만듭니다.

      보기가 시스템 전체에서 공유됩니다. 하나의 레코드 유형에 대한 프로젝트 보기를 만드는 경우 연결된 프로젝트를 표시하는 다른 레코드 유형에서 볼 수 있습니다.

   1. 기존 보기의 이름 위로 마우스를 가져간 후 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 후 다음 중 하나를 클릭하십시오.
      * 보기에 새 이름을 지정하려면 **이름 바꾸기**
      * **공유**, 다른 사용자와 보기 공유
      * 보기를 삭제하려면 **삭제**&#x200B;하십시오.

      >[!NOTE]
      >
      >편집, 공유 또는 삭제하려면 보기 관리 권한이 있어야 합니다.
      >
      >시스템 보기는 수정할 수 없습니다.
      >
   1. 보기에 필터를 추가하려면 **필터** 아이콘 ![필터 아이콘](assets/filter-icon.png)을 클릭하십시오. 결과는 목록에서 즉시 필터링됩니다. 필터를 저장하고 이름을 지정할 수 없습니다. 필터는 나중에 페이지에 액세스할 때 기억되며 공유 보기의 일부입니다.
   1. 보기에 표시하거나 숨길 열을 선택하려면 **열** 아이콘 ![열 아이콘](assets/columns-icon.png)을 클릭하십시오.
   1. 열 이름 위로 마우스를 가져간 후 열 이름 왼쪽의 아래쪽 화살표를 클릭하고 다음 중 하나를 클릭합니다.
      * 열에 대한 **사용자 지정 레이블**&#x200B;을(를) 추가하려면 **이름 바꾸기**&#x200B;를 하십시오. Workfront의 원래 필드 이름은 변경되지 않습니다.
      * 선택한 필드를 기준으로 목록을 정렬하려면 **정렬**&#x200B;하세요. 정렬의 방향을 나타내는 정렬 아이콘이 열 헤더에 추가됩니다.
   1. 목록의 오른쪽 상단에 있는 **+** 아이콘을 클릭하여 목록에 열을 추가하거나 제거한 다음 **저장**&#x200B;을 클릭합니다.

      **열 관리자**&#x200B;가 열립니다.

      목록 보기에 기존 필드만 추가할 수 있습니다.
첫 번째 열에 표시되는 목록 보기에서 기본 필드를 제거할 수 없습니다.
1. (선택 사항) 목록의 오른쪽 위 모서리에 있는 검색 상자에 키워드를 추가하여 항목을 검색합니다.

   검색어와 일치하는 항목이 목록에서 강조 표시됩니다.
1. (선택 사항) 목록에 항목을 더 추가하고 선택한 레코드에 자동으로 연결하려면 다음 중 하나를 수행하십시오.

   * 기존 항목을 추가하려면 목록의 오른쪽 상단에 있는 **레코드 연결**&#x200B;을 클릭합니다.
   * 새 항목을 추가하려면 목록의 맨 아래에 있는 **새 행**&#x200B;을 클릭하세요.
1. 목록에 있는 연결된 항목의 이름을 클릭하여 다른 브라우저 탭에서 엽니다.
1. 목록에서 셀 내부를 두 번 클릭하여 필드의 정보를 편집한 다음 Enter 키를 눌러 변경 사항을 저장합니다.

   일부 필드는 읽기 전용입니다. 예를 들어 프로젝트의 완료율은 시스템에서 계산한 필드이며 수동으로 편집할 수 없습니다.

1. 목록의 항목 이름 위로 마우스를 가져간 후 **추가** 메뉴 [추가 메뉴](assets/more-menu.png)를 클릭하고 **보기**&#x200B;를 클릭하여 다른 탭에서 프로젝트를 엽니다.

   또는

   항목을 하나 이상 선택하고 목록 하단의 작업 표시줄을 확인한 후 다음 중 하나를 클릭합니다.

   * 프로젝트를 삭제하려면 **삭제**&#x200B;하십시오. 프로젝트를 삭제하면 레코드에서 연결이 끊기고 Workfront의 휴지통으로 이동합니다. Workfront 관리자는 삭제된 프로젝트를 삭제된 후 최대 30일까지 복구할 수 있습니다.
   * 레코드에서 프로젝트의 연결을 끊으려면 **연결을 끊습니다**. 프로젝트의 연결을 해제하면 현재 레코드에서 해당 프로젝트와 해당 조회 필드의 모든 값이 제거됩니다.

   연결된 레코드 페이지 목록 보기의 ![작업 표시줄](assets/actions-bar-connected-records-page-list-view.png)

