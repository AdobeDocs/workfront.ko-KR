---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 작업 로드 밸런서에서 정보 필터링
description: 작업 항목을 효율적으로 찾고 관리하는 사용자 또는 항목에 집중할 수 있도록 작업 로드 밸런서에서 필터를 사용하는 것이 좋습니다.
author: Alina
feature: Resource Management
exl-id: f8ffb40e-4e71-45fe-bcae-801d45d75a21
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '2464'
ht-degree: 0%

---

# 작업 로드 밸런서에서 정보 필터링

<!--
(when they add custom fields to fitlering, add the caveat you added for the Resource Planner : only field NAMES and not LABELS are to be found in the drop-down >> ADD THIS IN THE STEP BELOW WHEN ADDING A FILTER)
-->

리소스 관리자는 작업 로드 밸런서를 사용하여 사용자의 작업 로드를 보고 관리할 수 있습니다. 작업 로드 밸런서에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [작업 로드 밸런서 개요](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
* [작업 로드 밸런서 탐색](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>작업 항목을 효율적으로 찾고 관리하는 사용자 또는 항목에 집중할 수 있도록 작업 로드 밸런서에서 필터를 사용하는 것이 좋습니다. 이렇게 하면 자원 지정 관리를 시작하기 전에 올바른 정보를 표시할 수 있습니다.
>
>새 필터를 저장하고 적용한 다음 작업 로드 밸런서에서 멀리 탐색하면 로그오프하고 다시 로그온한 후에도 필터가 유지됩니다.


이 문서에는 작업 로드 밸런서의 필터에 대한 정보가 포함되어 있습니다. Workfront의 필터에 대한 자세한 내용은 [Adobe Workfront의 필터 개요](../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 계획</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>리소스 영역에서 작업 로드 밸런서를 사용할 계획</p>
   <p>작업, 팀 또는 프로젝트의 작업 로드 밸런서를 사용할 때</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>다음 항목에 대한 액세스 권한 보기 이상:</p> 
    <ul> 
     <li> <p>리소스 관리</p> </li> 
     <li> <p>프로젝트</p> </li> 
     <li> <p>작업</p> </li> 
     <li> <p>문제</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>필터, 보기 및 그룹화</p> </li> 
    </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span>필터를 빌드하거나 편집할 때 필터, 보기 및 그룹화에 대한 액세스 편집</span> </p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트, 작업, 문제에 대한 권한 보기 이상</p>
   <p>편집하거나 삭제할 필터에 대한 권한 관리</p>
     </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 작업 로드 밸런서의 필터 개요

작업 로드 밸런서에서 필터를 사용할 때 다음 사항을 고려하십시오.

* 작업 로드 밸런서에 액세스하는 위치에 따라 Workfront에서 이미 정보를 필터링하고 있을 수 있습니다. 사전 적용된 필터에 대한 자세한 내용은 섹션을 참조하십시오 [작업 로드 밸런서에서 미리 적용된 필터](#pre-applied-filters-in-the-workload-balancer) 참조하십시오.
* 필터를 저장하지 않고 만들고 적용할 수 있고, 필터를 저장하여 나중에 다시 사용할 수 있습니다.
* 필터를 저장하지 않고 적용할 때 페이지를 새로 고쳐 원래 목록으로 되돌릴 수 있습니다.
* 만든 필터 또는 다른 사용자가 만들고 공유한 필터를 볼 수 있습니다.
* 공유 필터를 삭제하거나 편집할 때 공유 필터를 공유하는 모든 사용자에 대해 필터가 삭제되거나 편집됩니다.
* 작업 로드 밸런서에서 한 영역에 필터를 만들면 다른 영역에서 사용할 수 없습니다.

   예를 들어, [리소스] 영역에서 만들어진 필터는 프로젝트 또는 팀의 작업 로드 밸런서에서 사용할 수 없습니다.

   작업 로드 밸런서를 찾을 위치에 대한 자세한 내용은 [작업 로드 밸런서를 찾습니다.](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

* 선택한 필터와 일치하는 항목만 작업 로드 밸런서의 화면에 표시된 타임라인 내의 날짜와 일치시킬 수 있습니다.

## 작업 로드 밸런서에서 미리 적용된 필터 {#pre-applied-filters-in-the-workload-balancer}

작업 로드 밸런서는 다음 두 가지 분리된 영역에 정보를 표시합니다.

* **할당되지 않은 작업 영역**: 사용자에게 아직 할당되지 않은 작업 항목입니다.
* **지정된 작업 영역**: 사용자에게 할당된 작업 항목입니다.

   각 영역에 표시되는 내용에 대한 자세한 내용은 [작업 로드 밸런서 탐색](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

>[!IMPORTANT]
>
>작업 로드 밸런서의 각 영역에는 서로 독립적으로 작동하는 자체 필터 세트가 있습니다. 두 필터를 모두 구성하여 각 영역에 표시할 정보를 표시해야 합니다.

작업 로드 밸런서에는 사용자와 작업 항목이 표시됩니다.
사용자에게 할당된 작업 항목은 항목의 날짜가 화면에 표시된 기간과 일치하는 경우에만 표시됩니다.

작업 로드 밸런서에 액세스하는 위치에 따라 다음 표에 설명된 것처럼 [지정되지 않음] 및 [지정된 영역]이 이미 특정 기준으로 필터링됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>작업 로드 밸런서에 액세스하는 Workfront 영역</strong></td> 
   <td><b>기본적으로 지정되지 않은 작업 영역에 표시되는 항목</b> </td> 
   <td><b>기본적으로 지정된 작업 영역에 표시되는 항목</b> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">리소스 영역</td> 
   <td>기본적으로 여기에 표시되는 항목이 없습니다. 이 영역에서 작업 항목을 보려면 필터를 사용자 지정해야 합니다.</td> 
   <td>팀 및 해당 작업 항목의 멤버인 사용자. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">팀</td> 
   <td>팀이나 팀 및 Job 역할에 할당된 작업 항목입니다. </td> 
   <td> <p>선택한 팀의 구성원인 사용자 및 해당 작업 항목</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">프로젝트</td> 
   <td> <p>선택한 프로젝트의 팀 또는 작업 역할에 할당된 할당되지 않은 작업 항목 또는 항목이 이 영역에 표시됩니다.</p> </td> 
   <td> <p>시스템 기본 필터를 사용할 때 선택한 프로젝트에서 하나 이상의 작업 항목과 프로젝트의 작업 항목에 할당된 사용자 <b>이 프로젝트의 작업 항목</b> 이 선택되어 있습니다. </p>

<p>시스템 기본 필터가 <b>이 프로젝트의 작업 항목</b> 이 선택 해제되면 프로젝트의 [지정된 작업 영역]에 선택한 프로젝트의 하나 이상의 항목에 할당된 사용자의 모든 작업 항목이 표시됩니다.  </p> 이 필터는 기본적으로 선택되어 있지 않습니다.

<b>메모</b>
<p>프로젝트의 작업 로드 밸런서에서 모든 사용자 표시 옵션을 활성화하여 시스템의 모든 사용자를 표시할 수 있습니다. 자세한 내용은 <a href="../workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">작업 로드 밸런서 탐색</a></p>

</td> 
  </tr> 
 </tbody> 
</table>

## 작업 로드 밸런서 필터 만들기

작업 로드 밸런서에서 지정되지 않은 작업 영역 및 할당된 작업 영역에 대한 필터를 생성하는 프로세스는 작업 로드 밸런서에 액세스하는 위치에 관계없이 동일합니다. 작업 로드 밸런서 찾기에 대한 자세한 내용은 [작업 로드 밸런서를 찾습니다.](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

필터를 처음부터 만들거나 사전 정의된 필터 중 하나를 편집할 수 있습니다. 편집할 수 있는 기존 필터에 대한 자세한 내용은 [작업 로드 밸런서에서 기존 필터 편집](#edit-an-existing-filter-in-the-workload-balancer) 섹션에 자세히 설명되어 있습니다.

1. 작업 로드 밸런서로 이동합니다.

   작업 로드 밸런서 액세스에 대한 자세한 내용은 [작업 로드 밸런서 탐색](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. 을(를) 클릭합니다. **필터** 아이콘 ![](assets/filter-icon.png) 어느 쪽의 오른쪽 위 모서리에서 **할당되지 않은 작업** 또는 **지정된 작업 시간** 영역.

   필터 빌더 상자가 오른쪽에 표시됩니다. 필터를 만드는 영역의 이름은 상자의 헤더에 표시됩니다.

   ![](assets/filters-list-wb-assigned-work-with-filters-listed-nwe-350x377.png)

1. (선택 사항 및 조건부) 자원 관리 영역에서 작업 로드 밸런서에 액세스하면 사전 정의된 기본 필터가 이미 지정된 작업 영역에 적용될 수 있습니다. 기본 필터의 복사본을 편집하고 저장할 수 있습니다.

   >[!TIP]
   >
   >기본 필터는 팀 및 해당 작업 항목에 속하는 사용자를 표시합니다. 이 필터의 복사본을 편집할 수 있습니다.

   에 액세스하면 [!UICONTROL 작업 로드 밸런서] 프로젝트에서 &quot;[!UICONTROL 이 프로젝트의 작업 항목]필터를 이미 적용했을 수 있습니다. 이 프로젝트의 사용자에게 할당된 작업 항목만 표시됩니다. 이 필터의 복사본을 복제하고 저장할 수 있습니다.

   기본적으로 [!UICONTROL 작업 로드 밸런서] 프로젝트의 모든 사용자에게 할당된 모든 작업 항목이 표시됩니다.


1. 클릭 **새 필터.**

   ![](assets/new-filters-empty-panel-workload-balancer-350x460.png)

1. 필터를 만들려면 다음을 수행하십시오.

   1. 첫 번째 드롭다운 메뉴에서 필드 이름을 선택하거나 **필드 찾아보기** 을 입력하여 기본적으로 표시되지 않는 필드의 이름을 입력할 수 있습니다.

      >[!IMPORTANT]
      >
      >사용자 지정 필드를 참조할 때는 필드 레이블이 아니라 필드 이름을 입력해야 합니다. 필드 레이블은 개체에 첨부된 사용자 지정 양식에 표시됩니다. 레이블과 사용자 지정 필드 이름의 차이에 대한 자세한 내용은 [사용자 지정 양식 만들기 또는 편집](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   1. (조건부) **필드 찾아보기**&#x200B;를 채울 때 **검색** 필드를 선택하고 목록에 표시될 때 선택합니다.

      ![](assets/new-filters-search-for-a-field-highlighted-wb-nwe-350x386.png)

      >[!TIP]
      >
      >다음 섹션에서 필드를 선택할 수 있습니다.
      >
      >* **최근 선택**: 최근에 필터링한 필드입니다.
      >* **추천 필드**: 가장 일반적으로 사용되는 필드입니다.



   1. 두 번째 드롭다운 메뉴에서 수정자를 선택합니다. Workfront 필터 수정자에 대한 자세한 내용은 [필터 및 조건 수정자](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).
   1. 필터링할 필드 값을 선택하거나 입력합니다.

      >[!NOTE]
      >
      > 특정 포트폴리오의 작업 개체를 표시하려면 다음 필터를 적용할 수 있습니다. &quot;Portfolio 이름에 마케팅이 포함됩니다.&quot; 이름에 &quot;marketing&quot;이 포함된 포트폴리오에 속하는 작업 항목을 표시합니다.
      >
      >![](assets/portfolio-name-filter-statement-wb-350x262.png)

   1. (선택 사항) **삭제** 아이콘 ![](assets/delete.png) 필터 기준을 제거하려면 다음을 수행하십시오.

1. (선택 사항) **필터 추가** 다른 필터 기준을 추가하려면 4단계에서 작업을 반복합니다.

   <!--(NOTE: ensure this stays correct)-->

1. 클릭 **적용** 필터 결과를 저장하지 않고 선택한 작업 로드 밸런서 영역에 적용하려면

   왼쪽의 작업 항목 목록이 업데이트됩니다.

   >[!IMPORTANT]
   >
   >추가한 모든 필터 문이 동시에 true이면 작업 로드 밸런서에 결과가 표시됩니다.

   필터는 페이지를 새로 고칠 때까지 유지됩니다.

   다음 **적용** 단추가 **새 이름으로 저장** 버튼을 클릭합니다.

1. 클릭 **새 이름으로 저장** 나중에 사용할 수 있도록 필터를 저장합니다.

   ![](assets/new-filters-save-as-box-unassigned-area-wb-350x467.png)

   >[!TIP]
   >
   >클릭 **취소** 언제든지 필터 빌딩 영역으로 돌아갑니다.

1. 선택 **제목 없는 필터** 새 필터 이름을 대신 입력합니다.
1. 새 필터의 아이콘을 **아이콘** 드롭다운 메뉴

   ![](assets/new-filters-select-icon-expanded-drop-down-wb.png)

1. (선택 사항) 필터에 대한 설명을 추가하여 고유한 사항을 나타냅니다. 설명은 필터 목록의 필터 이름 아래에 표시됩니다.
1. **저장**&#x200B;을 클릭합니다.

   저장된 필터는 필터 상자의 내 필터 영역에 표시됩니다.

   저장된 필터 적용에 대한 자세한 내용은 섹션을 참조하십시오 [작업 로드 밸런서에서 저장된 필터 삭제](#delete-a-saved-filter-in-the-workload-balancer) 참조하십시오.

1. (조건부) 마우스를 **필터 아이콘** ![](assets/filter-icon.png) 오른쪽 위 모서리에서 **할당되지 않은 작업** 또는 **지정된 작업 시간** 영역 - 현재 적용된 필터 수나 이름이 있는 도구 설명을 표시합니다.

   ![](assets/filter-icon-with-number-and-tooltip-with-name-of-filter-wb-nwe-350x98.png)

## 필터 복제

필터를 복제하고 편집하여 새 필터를 만들 수 있습니다.

1. 작업 로드 밸런서로 이동합니다.

   작업 로드 밸런서 액세스에 대한 자세한 내용은 [작업 로드 밸런서 탐색](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. 을(를) 클릭합니다. **필터** 아이콘 ![](assets/filter-icon.png) 어느 쪽의 오른쪽 위 모서리에서 **할당되지 않은 작업** 또는 **지정된 작업 시간** 영역.

   필터 빌더 상자가 오른쪽에 표시됩니다. 필터를 만드는 영역의 이름은 상자의 헤더에 표시됩니다.

1. 기존 필터 위에 마우스를 놓고 **자세히** 메뉴 ![](assets/more-menu.png)를 클릭한 다음 **복제**.

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > 필터를 편집하는 동안 **자세히** 필터 편집 상자의 왼쪽 아래 모서리에 있는 메뉴를 클릭한 다음 **복제**.

1. 복제된 필터에 대한 다음 정보를 편집합니다.

   * 이름

      기본적으로 새 필터 이름은 &quot;(원래 필터 이름) Copy&quot;입니다.

   * 아이콘
   * 설명
   * 모든 필드, 수정자 또는 값

1. (선택 사항) **필터 추가** 를 눌러 복제된 필터에 명령문을 추가합니다.
1. 클릭 **저장** 중복된 필터를 **내 필터** 영역.

   원본 필터는 변경되지 않고 중복되는 필터가 새 필터로 저장됩니다.

## 작업 로드 밸런서에서 기존 필터 편집 {#edit-an-existing-filter-in-the-workload-balancer}

작업 로드 밸런서에서 저장된 필터를 편집할 수 있습니다.

>[!TIP]
>
>다른 사용자와 공유된 필터를 편집하면 변경한 내용이 표시됩니다.

1. 작업 로드 밸런서로 이동합니다.

   작업 로드 밸런서 액세스에 대한 자세한 내용은 [작업 로드 밸런서 탐색](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. 을(를) 클릭합니다. **필터 아이콘** ![](assets/filter-icon.png) 오른쪽 위 모서리에서 **지정되지 않음** 또는 **지정된 작업 시간** 영역.\
   필터 빌더가 오른쪽에 표시됩니다.

1. 편집할 필터 위로 마우스를 가져간 다음 **편집** ![](assets/wb-edit-filter-icon.png).

   ![](assets/filter-more-menu-options-wb.png)

1. 다음 중 하나를 수행하십시오.

   * 필터 문을 수정합니다
   * 클릭 **필터 추가** 새 필터 문을 추가하려면
   * 을(를) 클릭합니다. **삭제** 아이콘 ![](assets/delete.png) 기존 필터 문을 제거하려면 다음을 수행하십시오.

1. (선택 사항) **적용**.

   왼쪽에 있는 작업 로드 밸런서에서 결과가 업데이트되어 필터에 대한 변경 사항을 보여 줍니다.

1. 클릭 **저장.**

   왼쪽의 작업 로드 밸런서에서 결과가 업데이트되고 선택한 새 정보로 필터가 업데이트됩니다.

## 작업 로드 밸런서에서 저장된 필터 삭제 {#delete-a-saved-filter-in-the-workload-balancer}

필터를 삭제하기 전에 다음 사항을 고려하십시오.

* 삭제된 필터는 복구할 수 없습니다.
* 사전 정의된 필터는 삭제할 수 없습니다.
* 저장하지 않은 필터는 삭제할 수 없습니다. Workfront에서 로그아웃한 후 다시 로그인하면 자동으로 제거됩니다.
* 공유 필터를 삭제하면 공유 필터가 있는 모든 사용자에 대해서도 삭제됩니다.
* 저장된 필터를 모두 삭제하면 작업 로드 밸런서가 원래 기본값으로 표시됩니다.

>[!NOTE]
>
>다른 사람과 공유된 필터를 삭제하면 해당 필터가 삭제되기도 합니다.

1. 작업 로드 밸런서로 이동
1. 을(를) 클릭합니다. **필터 아이콘** ![](assets/filter-icon.png) 오른쪽 위 모서리에서 **할당되지 않은 작업** 또는 **지정된 작업 시간** 영역.\
   필터 빌더 상자가 오른쪽에 표시됩니다.

1. 필터를 마우스로 가리킨 다음 **자세히** 메뉴 ![](assets/more-menu.png)를 클릭한 다음 **삭제**.
   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   >필터를 편집하는 동안 **자세히** 필터 편집 상자의 왼쪽 아래 모서리에 있는 메뉴를 클릭한 다음 **삭제**.

1. (선택 사항) **취소** 삭제하지 않고 필터 목록으로 돌아갑니다.
1. 클릭 **삭제** 를 클릭하여 삭제를 확인합니다.

   필터가 사용자와 이 필터에 대한 권한이 있는 모든 사용자에 대해 삭제됩니다.

## 작업 로드 밸런서에서 필터 공유

사용자가 만들었거나 다른 사용자가 사용자와 공유한 필터를 공유할 수 있습니다.

작업 로드 밸런서에서 필터를 공유할 때 다음 사항을 고려하십시오.

* 활성 사용자, 팀, 역할 및 회사와 필터를 공유하거나 Workfront 인스턴스의 모든 사람에게 필터를 표시할 수 있습니다.
* 리소스 영역에서 공유하는 필터는 프로젝트 또는 팀의 작업 로드 밸런서에 표시되지 않습니다.
* 다른 사용자와 공유하는 작업 로드 밸런서 필터는 Workfront의 다른 영역에 표시되지 않습니다.

필터를 공유하려면 다음을 수행하십시오.

1. 작업 로드 밸런서로 이동
1. 을(를) 클릭합니다. **필터 아이콘** ![](assets/filter-icon.png) 오른쪽 위 모서리에서 **할당되지 않은 작업** 또는 **지정된 작업 시간** 영역.\
   필터 빌더 상자가 오른쪽에 표시됩니다.

1. 필터를 마우스로 가리킨 다음 **자세히** 메뉴 ![](assets/more-menu.png)를 클릭한 다음 **공유.**

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > 필터를 편집하는 동안 **자세히** 필터 편집 상자의 왼쪽 아래 모서리에 있는 메뉴를 클릭한 다음 **공유**.

   필터 공유 상자가 표시됩니다.

1. 를 활성화합니다 **시스템 전체 보기** 설정 이렇게 하면 Workfront의 모든 사용자가 필터를 볼 수 있는 권한이 제공됩니다.

   또는

   에서 필터를 공유할 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력합니다 **액세스 권한 부여** 필드.

   ![](assets/new-filters-sharing-ui-wb-350x422.png)

1. (선택 사항) 필터에 대한 권한을 편집할 엔티티 이름 옆에 있는 오른쪽 화살표 를 클릭한 다음, **보기** 또는 **관리** 선택 사항입니다.

   ![](assets/new-filters-granular-permissions-for-manage-wb-350x107.png)

1. (선택 사항) 다음 중 하나를 수행하여 엔티티에 대한 추가 권한을 활성화하거나 비활성화합니다.

   1. 클릭 **보기** 및 **공유** 선택 사항입니다. 기본적으로 활성화되어 있습니다.

   1. 클릭 **관리** 및 **공유** 또는 **삭제** 선택 사항입니다. 기본적으로 활성화되어 있습니다.
   >[!TIP]
   >
   >사용자는 액세스 수준보다 높은 권한을 받을 수 없습니다. 액세스 수준에서 편집 필터에 액세스할 수 없는 사용자는 필터를 관리할 권한을 받을 수 없습니다. Workfront이 이러한 사용자에 대한 관리 옵션을 비활성화하고 옵션이 흐리게 표시됩니다.

1. 클릭 **공유**. 필터는 지정한 엔터티와 공유됩니다.

   공유한 필터가 **나와 공유** 필터 상자의 영역.

   ![](assets/new-filters-shared-with-me-area-wb-350x236.png)

<!--   

## Add a filter to your favorites list

You can mark a filter as a favorite for quicker access to it. 

The filters that you mark as a favorite do not count towards your system Favorites list. There is no limit for how many filters you can favorite. 

1. Go to the Workload Balancer
1. Click the **Filter** icon ![](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or **Assigned Work** areas. The filter builder box displays on the right. 
1. Mouse over a filter, then click the **Favorite** ![](assets/favorites-icon-small.png). 
(NOTE: insert screen shot here with Favorite as part of this menu - same as above ones but with Favorite)
1. The filter is listed in the **Favorited** section inside the filter panel. 
1. (Optional) Click the **Favorite** icon again to remove the filter from the list of favorite filters
(I logged bugs for "Favorited" and "Unfavorite" wordings - make sure these have not updated)
-->
