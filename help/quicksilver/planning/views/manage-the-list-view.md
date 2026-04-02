---
title: Adobe Workfront Planning에서 목록 보기 관리
description: Adobe Workfront Planning의 레코드의 연결된 레코드 페이지에서 액세스할 때 목록 보기에 객체와 해당 필드를 표시할 수 있습니다. 이 문서에서는 레코드의 연결된 레코드 페이지에서 목록 보기를 만들거나 편집하는 방법에 대해 설명합니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
last-update: 2026-04-01T18:23:03Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
source-git-commit: f4d7484145226eb85bc547e582438e5202dec023
workflow-type: tm+mt
source-wordcount: '1857'
ht-degree: 0%

---


# Adobe Workfront Planning에서 목록 보기 관리

<!--
although list views in Planning are very similar to Workfront enhanced lists, keep this one separate with all the information, because of Planning standalone; some information here is also duplicated in this main Glist article: help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md
-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

{{planning-important-intro}}

Workfront Planning의 다음 영역에서 목록 보기에서 객체를 볼 수 있습니다.

* 레코드 세부 정보 영역의 프로젝트에 대해 연결된 레코드 페이지

  ![목록 보기의 연결된 레코드 페이지에 있는 프로젝트](assets/projects-on-connected-records-page-list-view.png)

* 레코드 유형 수준의 요청 양식 목록

  ![목록 보기의 요청 양식](assets/request-forms-in-list-view.png)

이 문서에서는 Workfront Planning에서 목록 보기를 탐색, 생성 또는 편집하는 방법에 대해 설명합니다.

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

* 연결된 레코드 페이지 목록 보기에 대해 다음 사항을 고려하십시오.

   * 레코드의 연결된 레코드 페이지에 있는 목록 보기에서만 프로젝트를 볼 수 있습니다. 연결된 레코드 페이지의 다른 개체나 레코드 종류에는 목록 보기를 사용할 수 없습니다.

  연결된 레코드 페이지를 만드는 방법에 대한 자세한 내용은 [레코드에 연결된 레코드 페이지 추가](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)를 참조하십시오.
   * 레코드의 연결된 레코드 페이지에서 목록 보기를 보려면 먼저 Workfront 프로젝트를 Planning 레코드 유형과 연결해야 합니다. 자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.
   * 레코드의 연결된 레코드 페이지에서 프로젝트에 대한 목록 보기를 여러 개 만들 수 있습니다.

* 요청 양식 목록 보기에 대해 다음 사항을 고려하십시오.

   * Planning 요청 양식에 대해 추가 목록 보기를 생성하거나 편집할 수 없습니다. Workfront은 요청 양식에 대해 하나의 목록 보기를 만듭니다. <!--this will change-->

     요청 양식에 대한 자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.
* 표시되는 위치에 따라 모든 목록 보기에 이 문서에 설명된 모든 요소가 있는 것은 아닙니다.

## 목록 보기 관리 {#manage-a-list-view}

Workfront Planning 목록 보기는 Workfront의 향상된 목록과 유사합니다. 향상된 보기의 요소 대부분은 Workfront Planning의 목록 보기에도 존재합니다.

자세한 내용은 [향상된 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)을 참조하세요.

<!--
Removed - more direct steps below: 
{{step1-to-planning}}

1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card. 
    1. From any view, click the name of a record to open the record's preview or details page. 
    1. Add a **Connected records page** for connected projects as described in the article [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

    The Connected records page displays projects connected to the record in the list view. 

    ![Projects on connected records page in list view](assets/projects-on-connected-records-page-list-view.png)

1. (Conditional) To access a list of request forms, do the following: 

    1. {{step1-to-planning}}

    1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card.
    1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name in the header, then click **Manage request forms**.

        A list of request forms displays.

-->

1. 다음 영역 중 하나의 목록 보기로 이동합니다.

   * 레코드 세부 정보 영역의 프로젝트에 대해 연결된 레코드 페이지
   * 레코드 유형의 요청 양식 페이지

1. (조건부) 사용 가능한 경우 다음 중 하나를 수행하여 목록 보기를 수정합니다.

   1. 목록의 왼쪽 상단 모서리에서 드롭다운 보기 메뉴를 확장하여 다른 보기를 선택하거나 **새 보기**&#x200B;를 클릭하여 다른 보기를 만듭니다.

      >[!TIP]
      >
      >보기가 시스템 전체에서 공유됩니다. 하나의 레코드 유형에 대한 프로젝트 보기를 만드는 경우 연결된 프로젝트를 표시하는 다른 레코드 유형에서 볼 수 있습니다.

   1. 기존 보기의 이름 위로 마우스를 가져간 후 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 후 다음 중 하나를 클릭하십시오.
      * 보기에 새 이름을 지정하려면 **이름 바꾸기**
      * **공유**, 다른 사용자와 보기 공유
      * 보기를 삭제하려면 **삭제**&#x200B;하십시오.

      >[!NOTE]
      >
      >* 편집, 공유 또는 삭제하려면 보기 관리 권한이 있어야 합니다.
      >
      >* 시스템 보기는 수정할 수 없습니다.
      >
      >* <span class="preview">원래 기본 설정을 복원하도록 수정한 후 [보기] 권한만 있는 공유 보기를 재설정하거나 변경 내용과 함께 복사하고 복사본을 공유할 수 있습니다. 자세한 내용은 [향상된 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)을 참조하세요. </span>

   1. 보기에 필터를 추가하려면 **필터** 아이콘 ![필터 아이콘](assets/filter-icon.png)을 클릭하십시오. 결과는 목록에서 즉시 필터링됩니다. 필터를 저장하고 이름을 지정할 수 없습니다. 필터는 나중에 페이지에 액세스할 때 기억되며 공유 보기의 일부입니다.

      >[!TIP]
      >
      ><span class="preview">개인화된 필터를 적용하려면 필드 값에 대해 다음 옵션 중 하나를 선택하십시오.
      >
      ><div class="preview">
      >
      >* **내(로그인한 사용자)**&#x200B;가 사용자를 참조하는 필드에서 로그인한 사용자를 참조합니다.
      >
      >* **내 팀** 또는 **내 홈 팀**&#x200B;에서 팀을 참조하는 필드에 있는 팀을 참조합니다.
      >
      >* **내 그룹** 또는 **내 홈 그룹**&#x200B;에서 그룹을 참조하는 필드에 있는 그룹을 참조합니다.
      >
      >* **내 회사**&#x200B;에서 회사를 참조하는 필드에 회사를 참조합니다.
      > 
      >* **내 역할** 또는 **내 기본 역할**&#x200B;을(를) 참조하여 필드에서 작업 역할을 참조합니다.
      >
      ></div>

   1. 보기에 표시하거나 숨길 열을 선택하려면 **열** 아이콘 ![열 아이콘](assets/columns-icon.png)을 클릭하십시오.
   1. 열 이름 위로 마우스를 가져간 후 열 이름 왼쪽의 아래쪽 화살표를 클릭하고 다음 중 하나를 클릭합니다.
      * 열에 대한 **사용자 지정 레이블**&#x200B;을(를) 추가하려면 **이름 바꾸기**&#x200B;를 하십시오. Workfront의 원래 필드 이름은 변경되지 않습니다.
      * 선택한 필드를 기준으로 목록을 정렬하려면 **정렬**&#x200B;하세요. 정렬의 방향을 나타내는 정렬 아이콘이 열 헤더에 추가됩니다.
   1. 목록의 오른쪽 상단에 있는 **+** 아이콘을 클릭하여 목록에 열을 추가하거나 제거한 다음 **저장**&#x200B;을 클릭합니다.

      **열 관리자**&#x200B;가 열립니다.

      목록 보기에 기존 필드만 추가할 수 있습니다.
첫 번째 열에 표시되는 목록 보기에서 기본 필드를 제거할 수 없습니다.

   1. <span class="preview">셀 서식 지정&#x200B;**아이콘**&#x200B;셀 서식 지정 아이콘![을 클릭합니다. &#x200B;](assets/format-cells-icon.png) **Format** 상자가 열립니다.</span> <!--change the name of the box when they update it-->
      <span class="preview">다음을 수행합니다. </span>

      1. <span class="preview">**조건 추가**.</span>
      1. <span class="preview">**If** 줄에서 필드를 선택하고 필드 값을 선택한 다음 수정자를 추가합니다. 수정자는 선택한 필드 유형에 따라 변경됩니다. </span>

         >[!TIP]
         >
         ><span class="preview">목록 보기에 표시되는 필드만 조건부 서식에 사용할 수 있습니다.</span>

      1. <span class="preview">(선택 사항) 필드 값을 추가하는 대신 **다른 필드와 비교** 아이콘 ![다른 필드와 비교](assets/compare-to-another-field-icon.png)를 클릭하고 선택한 필드의 값과 비교할 필드를 선택합니다. 예를 들어 프로젝트 소유자와 프로젝트 스폰서 필드를 비교할 수 있습니다. </span>

         >[!TIP]
         >
         ><span class="preview">조건부 서식은 목록 보기에 표시되는 필드만 사용할 수 있습니다. 비교하는 필드의 형식은 동일해야 합니다. </span>

      1. <span class="preview">(선택 사항) **If** 줄에서 **조건 추가**&#x200B;를 클릭하여 동일한 규칙에 조건을 더 추가합니다.</span>

         >[!TIP]
         >
         ><span class="preview">조정 규칙에 최대 10개의 조건을 추가할 수 있으며 필드에 최대 20개의 규칙을 사용할 수 있습니다.</span>

      1. <span class="preview">조건 사이에 있는 **Or** 커넥터를 클릭하여 **And**(으)로 변경하고 여러 조건을 동시에 충족해야 함을 나타냅니다. **또는**&#x200B;이(가) 기본 커넥터입니다.</span>
      1. <span class="preview">**서식** 줄에서 서식을 지정할 열을 나타내는 필드를 선택합니다.</span> <!--edit this area, if it changes names??-->
      1. <span class="preview">(선택 사항) 선택한 필드 옆에 있는 **색상 원** 아이콘 ![색상 원 아이콘](assets/color-circle.png)을 클릭하여 확장하고 **셀 채우기** 영역에서 다른 색상을 선택하여 셀의 배경색을 변경하거나 **텍스트 색상** 영역에서 색상을 선택하여 셀의 텍스트 색상을 변경합니다.</span>
      1. <span class="preview">**텍스트 서식** 아이콘 ![텍스트 서식 아이콘](assets/text-format-icon.png)을 클릭하고 다음 옵션 중 하나를 선택하여 셀의 텍스트 서식을 지정합니다.</span>
         * <span class="preview">굵게</span>
         * <span class="preview">기울임꼴</span>

      1. <span class="preview">조건에 맞는 필드의 전체 행에 서식을 적용하려면 **행에 적용** 설정을 켭니다.</span>
      1. <span class="preview">(선택 사항) **형식** 상자에서 **조건 추가**&#x200B;를 클릭하여 다른 필드에 대한 다른 규칙을 추가하고 위의 단계를 반복합니다.</span>
      1. <span class="preview">(선택 사항) **모두 지우기**&#x200B;를 클릭하여 모든 서식을 제거합니다.</span>
      1. <span class="preview">닫으려면 **서식** 상자 바깥쪽을 클릭합니다.</span>

         <span class="preview">목록 보기로 돌아갑니다.</span>
         <span class="preview">서식이 목록 보기에 바로 적용됩니다.</span>
         <span class="preview">**셀 서식 지정** 아이콘 옆에 특수 서식이 적용되었음을 나타내는 파란색 점이 있습니다.</span>

   1. <span class="preview">(선택 사항) **그룹화** 아이콘 ![그룹화 아이콘](assets/grouping-icon.png) &lt;!-이 항목을 &quot;그룹화&quot;??->로 업데이트하여 공통 필드로 목록에 있는 항목을 그룹화했습니다. 옵션 중 하나를 선택하거나 검색 창을 사용하여 필드를 찾습니다.</span>

      <span class="preview">필드를 그룹화하려면 먼저 필드가 목록에 있는 열이어야 합니다. 모든 필드 형식을 그룹화에 사용할 수 있는 것은 아닙니다.</span>

   1. <span class="preview">행의 세로 길이를 업데이트하려면 **행 높이** 아이콘 ![행 높이 아이콘](assets/row-height-icon.png)을 클릭하세요. 다음 옵션 중에서 선택하십시오. </span>

      <div class="preview">

      * 짧음
      * 표준. 이것이 기본 선택입니다.
      * 보통
      * 높음

      </div>

   <!--leave these here, although they duplicate for Enhanced lists in Workfront-->

1. (선택 사항) 목록의 오른쪽 위 모서리에 있는 검색 상자에 키워드를 추가하여 항목을 검색합니다.

   검색어와 일치하는 항목이 목록에서 강조 표시됩니다.

1. (선택 사항 및 조건부) 연결된 프로젝트 <!--change projects to items here when more items will display in the Glist--> 페이지에서 목록에 항목을 더 추가하고 선택한 레코드에 자동으로 연결하려면 다음 중 하나를 수행하십시오.

   * 기존 항목을 추가하려면 목록의 오른쪽 상단에 있는 **레코드 연결**&#x200B;을 클릭합니다.
   * 새 항목을 추가하려면 목록의 맨 아래에 있는 **새 행**&#x200B;을 클릭하세요.
1. 목록에 있는 연결된 항목의 이름을 클릭하여 다른 브라우저 탭에서 엽니다.
1. 목록에서 셀 내부를 두 번 클릭하여 필드의 정보를 편집한 다음 Enter 키를 눌러 변경 사항을 저장합니다.

   일부 필드는 읽기 전용입니다. 예를 들어 프로젝트의 완료율은 시스템에서 계산한 필드이며 수동으로 편집할 수 없습니다.

1. 목록의 항목 이름 위로 마우스를 가져간 후 **추가** 메뉴 [추가 메뉴](assets/more-menu.png)를 클릭하고 **보기**&#x200B;를 클릭하여 다른 탭에서 프로젝트를 엽니다.

   또는

   항목을 하나 이상 선택하고 목록 하단의 작업 표시줄을 확인한 다음, 사용 가능한 경우 다음 중 하나를 클릭합니다. 목록 보기에 액세스하는 영역에 따라 다음 옵션 중 하나를 클릭합니다.

   * 항목을 삭제하려면 **삭제**&#x200B;하십시오. 프로젝트를 삭제하면 레코드에서 연결이 끊기고 Workfront의 휴지통으로 이동합니다. Workfront 관리자는 삭제된 프로젝트를 삭제된 후 최대 30일까지 복구할 수 있습니다. 양식을 삭제해도 양식을 제출할 때 생성된 요청 또는 레코드는 삭제되지 않습니다.
   * 레코드에서 프로젝트의 연결을 끊으려면 **연결을 끊습니다**. 프로젝트의 연결을 해제하면 현재 레코드에서 해당 프로젝트와 해당 조회 필드의 모든 값이 제거됩니다.

     <!--update screen shot at preview release-->

     연결된 레코드 페이지 목록 보기의 ![작업 표시줄](assets/actions-bar-connected-records-page-list-view.png)

   * **양식 편집**: Planning 요청 양식을 열어서 편집할 수 있습니다.
   * **게시 취소**: 요청 양식 게시를 취소합니다. 이렇게 하면 요청 영역에서 양식이 제거되며 사용자는 더 이상 이 레코드 유형에 요청을 추가할 수 없습니다.
   * **공유**: 다른 사용자와 공유할 수 있는 요청 양식의 공유 상자를 엽니다.
   * **링크 복사**: 다른 사용자와 공유할 수 있도록 Planning 요청 양식에 링크를 복사합니다. 양식이 공개적으로 공유되는 경우 Workfront Planning 외부 사용자와 링크를 공유할 수 있습니다.

     Planning 요청 목록의 ![작업 표시줄](assets/actions-bar-in-inake-forms-list.png)



