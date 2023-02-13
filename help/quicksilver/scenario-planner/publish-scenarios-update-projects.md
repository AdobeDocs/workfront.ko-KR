---
product-area: enterprise-scenario-planner-product-area
keywords: 게시,계획,프로젝트,시나리오,시나리오
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 계획자에서 이니셔티브를 게시하여 프로젝트를 업데이트하거나 생성합니다
description: Adobe Workfront Scenario Planner에서 시나리오를 게시하여 기존 이니셔티브에서 프로젝트를 생성하고 이전에 이니셔티브에 연결된 프로젝트를 업데이트할 수 있습니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: 46d3666a-4454-4a84-8c02-a79f3947a18f
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '1694'
ht-degree: 0%

---

# 에서 이니셔티브를 게시하여 프로젝트를 업데이트하거나 만들 수 있습니다 [!DNL Scenario Planner]

에서 시나리오 게시 [!DNL Adobe Workfront Scenario Planner] 다음을 완수합니다.

* 시나리오의 이니셔티브로 프로젝트를 생성하고 함께 연결합니다.
* 시나리오의 이니셔티브에 이미 연결된 프로젝트를 연결된 이니셔티브의 정보로 업데이트합니다. 프로젝트에 프로젝트 를 계획에 가져올 때 이니셔티브에 연결할 수도 있습니다. 자세한 내용은 [계획 로 프로젝트 가져오기 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 플랜*</p> </td> 
   <td>[!UICONTROL Business] 이상</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 라이센스*</p> </td> 
   <td> <p>[!UICONTROL Review] 이상</p> </td> 
  </tr> 
  <tr> 
   <td>제품 </td> 
   <td> <p>에 대한 추가 라이센스를 구입해야 합니다. [!DNL Adobe Workfront Scenario Planner] 을 눌러 이 문서에 설명된 기능에 액세스합니다.</p> <p>를 가져오는 방법에 대한 자세한 내용은 [!DNL Workfront Scenario Planner]를 참조하십시오. <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">을 사용하는 데 필요한 액세스 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p></p> <p>액세스 수준*</p> </td> 
   <td> 
    <ul> 
    <li>[!UICONTROL Edit] 액세스 권한 [!DNL Scenario Planner] 및 프로젝트</li></ul>

<p><b>메모</b>

여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 변경할 수 있습니다. <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p>개체 권한</p> </td> 
   <td> 
    <ul> 
     <li>계획에 대한 [!UICONTROL Manage] 권한 </li> 
     <li>게시된 프로젝트에 대한 [!UICONTROL Manage] 권한</li> 
    </ul> <p>프로젝트에 대한 추가 액세스 요청에 대한 내용은 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> <p>계획에 대한 추가 액세스 요청에 대한 내용은 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">에서 계획에 대한 액세스 요청 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

액세스 권한에 대한 추가 정보 [!DNL Workfront Scenario Planner]를 참조하십시오. [을 사용하는 데 필요한 액세스 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

## 전제 조건

시작하기 전에:

* 이니셔티브를 게시하려면 먼저 계획을 작성하고 저장해야 합니다.

## 프로젝트에 이니셔티브 게시에 대한 고려 사항

* 계획에서 시나리오를 하나만 게시할 수 있습니다.
* 하나의 이니셔티브는 하나의 프로젝트에만 연결할 수 있습니다.
* 이니셔티브가 서로 다른 계획에 속할 때 한 프로젝트가 두 개 이상의 이니셔티브에 연결될 수 있습니다.

   >[!TIP]
   >
   >프로젝트가 여러 계획에 있고 모든 계획에서 프로젝트에 정보를 게시하면 최신 게시가 기존 게시를 덮어씁니다 [!DNL Scenario Planner] 프로젝트에 대한 정보입니다.

* 프로젝트를 계획으로 가져와서 계획에 이니셔티브가 생성된 경우 이니셔티브를 게시하면 연결된 프로젝트도 이니셔티브 정보로 업데이트됩니다.

   >[!TIP]
   >
   >동일한 프로젝트를 여러 계획으로 가져올 수 있습니다. 게시하면 여러 이니셔티브에 연결된 프로젝트의 이니셔티브 정보를 덮어쓸 수 있습니다.

   프로젝트를 가져와서 이니셔티브를 만드는 방법에 대한 자세한 내용은 [계획 로 프로젝트 가져오기 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* 프로젝트에 대한 모든 변경 사항은 연결된 이니셔티브로 전송되지 않습니다.



## 이니셔티브 게시

>[!IMPORTANT]
>
>충돌 해결을 포함하여 계획에 대한 이니셔티브를 변경하는 경우 프로젝트에 새 정보가 표시되도록 하려면 이니셔티브를 다시 게시해야 합니다. 이 정보는 해당 이니셔티브를 게시하는 경우에만 이니셔티브에 연결된 프로젝트에 표시됩니다. 이니셔티브 간 충돌 해결에 대한 자세한 내용은 [에서 이니셔티브 충돌 해결 [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **[!UICONTROL 시나리오]**
1. (선택 사항 및 조건부) 기존 계획에서 게시하려면 **[!UICONTROL 필터]** 아이콘 ![](assets/filter-nwepng.png) 계획의 오른쪽 위 모서리에서 다음 옵션 중 하나를 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>소유하거나 사용자와 공유된 모든 계획을 표시합니다. 기본값입니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 내 계획]</td> 
      <td>생성된 계획을 표시합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 나와 공유]</td> 
      <td> <p>생성하지 않았지만 사용자와 공유된 계획을 표시합니다.</p> <p>중요 사항: 게시하려면 사용자와 공유된 계획에 [!UICONTROL 관리] 권한이 있어야 합니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (선택 사항) **[!UICONTROL 검색]** 아이콘 ![](assets/search-icon.png) 계획 이름을 입력하여 목록에서 빠르게 찾을 수 있습니다.
1. (조건부) 새 계획에서 게시하려면 계획을 만듭니다.

   계획 생성에 대한 자세한 내용은 [에서 계획 생성 및 편집 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) .

1. (선택 사항) 기존 계획의 이름을 클릭하고 계획에 대한 새 시나리오를 생성합니다.

   계획에 대한 시나리오 생성에 대한 자세한 내용은 [에서 계획 시나리오를 만들고 비교합니다. [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (선택 사항) 기존 또는 신규 계획의 이니셔티브를 갱신하거나 신규 계획을 생성합니다.

   이니셔티브 만들기에 대한 내용은 [에서 이니셔티브 만들기 및 편집 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. 클릭 **[!UICONTROL 계획 저장]**.
1. 게시할 시나리오를 **[!UICONTROL 초기 시나리오]** 드롭다운 메뉴를 클릭한 다음 **[!UICONTROL 게시로 이동]** ![](assets/go-to-publish-button-icon.png) 오른쪽 상단 모서리에서

   또는

   클릭 **[!UICONTROL 시나리오 비교]**&#x200B;게시할 시나리오 카드를 마우스로 가리킨 다음 을 클릭합니다. **[!UICONTROL 게시로 이동]** ![](assets/go-to-publish-button-icon.png).

   다음 [!UICONTROL 이니셔티브 게시] 시나리오의 모든 이니셔티브 목록을 보여주는 페이지가 표시됩니다. 이니셔티브가 이전에 게시된 경우 프로젝트 아이콘 ![](assets/project-icon-sp.png) 이름 및 이름 뒤에 표시됩니다. **[!UICONTROL 마지막으로 게시됨]** 날짜가 목록에 채워집니다.

   >[!TIP]
   >
   >프로젝트를 가져와서 만든 이니셔티브에도 프로젝트 아이콘이 표시됩니다 ![](assets/project-icon-sp.png) 그들의 이름의 오른쪽에

   ![](assets/project-icons-and-last-published-date-in-publish-initiative-page-350x63.png)

1. (선택 사항 및 조건부) 기존 계획에서 게시하려면 **[!UICONTROL 필터]** 아이콘 ![](assets/filter-nwepng.png) 계획의 오른쪽 위 모서리에서 다음 옵션 중 하나를 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>선택한 시나리오의 모든 이니셔티브를 표시합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 게시됨]</td> 
      <td>사용자 또는 다른 사용자가 이전에 게시한 이니셔티브를 표시합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 게시 취소]</td> 
      <td> <p>게시되지 않은 이니셔티브를 표시합니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/initiatives-fitler-in-publishing-screen-scenario-planner.png)

1. (선택 사항) **[!UICONTROL 검색]** 아이콘 ![](assets/search-icon.png) 이니셔티브 이름을 입력하여 목록에서 신속하게 찾을 수 있습니다.
1. 프로젝트를 게시 및 만들거나 업데이트할 하나 이상의 이니셔티브를 선택한 다음 **[!UICONTROL 이니셔티브 게시]**.

   게시된 이니셔티브가 이미 프로젝트에 연결되어 있는 경우 선택한 각 이니셔티브 중에서 새 프로젝트를 생성하거나 기존의 연결된 프로젝트를 업데이트합니다.

   >[!TIP]
   >
   >새 프로젝트의 이름은 게시된 이니셔티브와 동일합니다.

1. (조건부) 다음 중 하나를 수행합니다.

   * 이니셔티브를 게시한 경우 **[!UICONTROL 관련 프로젝트 참조]** 이니셔티브에서 만들거나 업데이트한 프로젝트를 열려면 다음을 수행하십시오.
   * 두 개 이상의 이니셔티브를 게시한 경우 **[!UICONTROL 관련 프로젝트 참조]** 이니셔티브에서 게시된 프로젝트 목록을 열려면 다음을 수행하십시오. [!DNL Workfront] 적용 [!DNL Scenario Planner] 프로젝트는 기본적으로 프로젝트 목록으로 필터링됩니다. 가장 최근에 게시된 프로젝트가 목록 맨 위에 표시됩니다.

      ![](assets/scenario-planner-filter-after-publishing-initiatives-350x81.png)

1. 프로젝트에 대한 이니셔티브 정보를 보려면 다음 영역으로 이동하십시오.

   * **다음 [!UICONTROL 업데이트] 섹션**: 업데이트는 프로젝트를 이니셔티브에서 만들거나 업데이트했음을 나타내기 위해 게시됩니다. 갱신에는 프로젝트를 생성 또는 갱신한 이니셔티브의 이름과 이니셔티브가 포함된 계획의 링크된 이름이 포함되어 있습니다. 갱신에서 계획명을 눌러 계획에서 계획을 열 수 있습니다 [!DNL Scenario Planner].

      ![](assets/update-stream-confirmation-of-publish-on-project-350x65.png)

   * **다음 [!UICONTROL 개요] 의 영역 [!UICONTROL 프로젝트 세부 사항] 섹션**: 새로운 [!DNL Scenario Planner] 이 영역에 연결된 이니셔티브의 정보가 포함된 섹션이 만들어집니다.

      ![](assets/scenario-planner-on-project-details-350x135.png)

      다음 이니셔티브 정보는 [!DNL Scenario Planner] 의 영역 [!UICONTROL 프로젝트 세부 사항] 섹션:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Duration]</span> </td> 
        <td><span>프로젝트가 이니셔티브에 연결되어 있을 때 해당 이니셔티브의 기간입니다. 이 필드는 편집할 수 없습니다.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL 마지막으로 게시된 날짜]</span> </td> 
        <td><span>해당 이니셔티브에서 프로젝트를 마지막으로 게시한 날짜입니다.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative 시작 날짜]</span> </td> 
        <td><span>프로젝트가 이니셔티브에 연결되어 있는 이니셔티브 시작 달의 첫 날입니다.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative 종료 날짜]</span> </td> 
        <td><span>프로젝트가 이니셔티브에 연결되어 있는 이니셔티브 마지막 달 하루입니다. </span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL FTE 및 시간의 Initiative Job 역할]</span> </td> 
        <td> <p>이니셔티브에 대한 연관된 작업 역할 및 해당 시간 할당에 대한 정보입니다. 여기에는 다음이 포함됩니다.</p> 
         <ul> 
          <li>작업 역할 이름</li> 
          <li>FTE 수</li> 
          <li> <p>모든 FTE의 시간(시)</p> <p>시간이나 FTE를 사용하여 계획 또는 이니셔티브에 필요한 Job 역할의 양을 예측할 수 있습니다.</p> <p>자세한 내용은 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">시나리오 계획자에서 계획 생성 및 편집</a>. </p> </li> 
         </ul> 
      <p><b>팁</b>

      이니셔티브 내에서 매월 작업 역할 수가 다를 경우 이 필드에는 이니셔티브에 필요한 최대 역할 수가 표시됩니다. 예를 들어, 1월과 2월에 컨설턴트 1명이 필요한 경우 열에는 2FTE와 2개의 FTE에 대한 해당 시간 시간이 모든 달에 표시됩니다.</p> </td>
      </tr> 
      </tbody> 
     </table>

      >[!NOTE]
      >
      >다음을 사용하는 모든 사용자 [!UICONTROL 보기] 프로젝트에 대한 액세스 권한은 [!DNL Scenario Planner] 의 섹션 [!UICONTROL 개요] 영역. 이 영역이 [!UICONTROL 세부 사항] 레이아웃 템플릿을 사용하여 섹션을 만듭니다. 사용자에게 연결된 레이아웃 템플릿이 없는 경우 이 영역이 기본적으로 표시됩니다.
      >
      >   
      >   
      >   * 에서 영역 추가 또는 제거에 대한 자세한 내용은 [!UICONTROL 세부 사항] 레이아웃 템플릿을 사용하는 섹션에서 다음을 참조하십시오. [사용자 지정 [!UICONTROL 세부 사항] 레이아웃 템플릿을 사용하여 보기](../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
      >   * 의 정보 보기에 대한 자세한 내용은 [!UICONTROL 개요] 의 영역 [!UICONTROL 프로젝트 세부 사항]를 참조하십시오. [[!UICONTROL 관리] 프로젝트의 정보 [!UICONTROL 개요] 영역](../manage-work/projects/manage-projects/understand-project-overview-area.md).


   * **다음 [!UICONTROL 역할 할당] 패널의 [!UICONTROL 작업 로드 밸런서] 또는 프로젝트의 작업 목록**: 프로젝트에 대한 역할 할당 외에 이니셔티브의 역할 할당에 대한 정보가 이 영역에 채워집니다.

      자세한 내용은 [프로젝트 및 이니셔티브 간 리소스 할당 조정 개요](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

      ![](assets/role-allocation-panel-350x174.png)

      프로젝트의 날짜 또는 리소스에 대한 변경 사항은 해당 이니셔티브 또는 이니셔티브 정보가 포함된 프로젝트의 영역에 영향을 주지 않습니다.

   * **다음 [!UICONTROL 리소스 예산 책정] 의 영역 [!UICONTROL 비즈니스 사례] 프로젝트**: 을 사용하여 프로젝트 리소스를 관리하는 새로운 옵션 [!DNL Scenario Planner] 정보에 [!UICONTROL 리소스 예산 책정] 의 영역 [!UICONTROL 비즈니스 사례] 프로젝트 구성

      자세한 내용은 [의 예산 리소스 [!UICONTROL 비즈니스 사례] 사용 [!DNL Scenario Planner]](../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

      ![](assets/sp-in-business-case-selected-350x110.png)

1. (선택 사항)에서 다음 정보를 검토하십시오. [!DNL Scenario Planner] 시나리오를 게시한 후:

   * 게시된 시나리오는 이니셔티브를 게시한 후 첫 번째 시나리오가 됩니다.
   * 시나리오를 한 번 이상 게시한 후에는 다른 시나리오에서 게시할 수 없습니다.
   * 다음 [!UICONTROL 게시로 이동] 시나리오에서 하나 이상의 이니셔티브가 게시되면 다른 모든 시나리오에서 옵션이 제거됩니다.
   * 계획에서 게시된 이니셔티브의 프로젝트 아이콘 옆에 녹색 표시기가 표시됩니다.

      ![](assets/indicator-for-published-initiative-icon-350x119.png)

   * 시나리오 상단에 녹색 &quot;게시됨&quot; 표시기가 표시되고 시나리오 카드에 게시됨 필드가 입력되어 게시된 시나리오의 이니셔티브 수를 나타냅니다.

      ![](assets/published-scenario-highlighted-350x632.png)

      >[!TIP]
      >
      >시나리오의 이니셔티브에서 게시된 모든 프로젝트가 삭제되면 시나리오가 게시되었음을 나타내는 지표가 제거됩니다. 자세한 내용은 [프로젝트 삭제](../manage-work/projects/manage-projects/delete-projects.md).

1. (선택 사항) 이니셔티브에 대한 정보를 업데이트하고 위에 설명된 프로세스를 반복하여 이니셔티브를 다시 게시하고 연결된 프로젝트에 대한 이니셔티브 정보를 업데이트합니다.

   이니셔티브 편집에 대한 자세한 내용은 [에서 이니셔티브 만들기 및 편집 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).


