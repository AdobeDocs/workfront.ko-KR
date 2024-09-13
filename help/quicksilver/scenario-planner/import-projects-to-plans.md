---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 플래너의 플랜으로 프로젝트 가져오기
description: 기존 프로젝트를 플랜으로 가져올 수 있습니다. 가져온 프로젝트는 이니셔티브로 변환되며 새로운 이니셔티브를 관리하는 것처럼 계획 내에서 관리할 수 있습니다. 원래 프로젝트는 새 이니셔티브에 연결된 상태로 유지됩니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: 20429bb1-c158-433b-9790-325cd577248e
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '1690'
ht-degree: 0%

---

# [!DNL Scenario Planner]의 플랜으로 프로젝트 가져오기

기존 프로젝트를 플랜으로 가져올 수 있습니다. 가져온 프로젝트는 이니셔티브로 변환되며 새로운 이니셔티브를 관리하는 것처럼 계획 내에서 관리할 수 있습니다. 원래 프로젝트는 새 이니셔티브에 연결된 상태로 유지됩니다.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: add information about what happens when you import projects and where the info from projects show up;</p>
<p>- the hours/ FTE come from WorkPerDay</p>
<p>- if a task has a Duration of 0, the FTE should be 0 for that asignee but it should still come across) </p>
</div>
-->

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 플랜*</p> </td> 
   <td> <ul></li>
   <li><p>새로운 기능: Ultimate </p></li>
   <p>새 Workfront Select 또는 Workfront Prime 플랜에는 시나리오 플래너를 사용할 수 없습니다. </p>
   <li><p>현재: [!UICONTROL Business] 이상</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 라이센스*</p> </td> 
   <td> <p>새로운 기능: 밝게 또는 높음</p> 
   <p>현재: [!UICONTROL Review] 이상</p> </td> 
  </tr> 
  <tr> 
   <td>제품* </td> 
   <td> <ul><li><p>새로운 Workfront 플랜의 경우:</p><p> Adobe Workfront</li></p>
   <li><p>현재 Workfront 플랜의 경우: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront 시나리오 플래너</p></li></ul>

<p>자세한 내용은 [!DNL Scenario Planner]</a>을(를) 사용하는 데 필요한 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">액세스를 참조하십시오. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>액세스 수준 </td> 
   <td> <p>다음에 대한 [!UICONTROL 편집] 액세스 권한: [!DNL Scenario Planner]</p> <p>프로젝트에 대한 보기 이상의 액세스 권한.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>개체 권한 </p> </td> 
   <td> <p>플랜에 대한 [!UICONTROL 관리] 권한</p> <p>프로젝트에 대한 이상의 권한을 봅니다.</p><p>플랜에 대한 추가 액세스 요청에 대한 자세한 내용은 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">플랜에 대한 액세스 요청 [!DNL Scenario Planner]</a>을(를) 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서에 대한 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 프로젝트를 새 이니셔티브로 플랜에 가져오는 것에 대한 고려 사항

* 프로젝트를 새 이니셔티브로 플랜에 가져오려면 먼저 프로젝트를 만들어야 합니다.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: no caveats for project statuses yet, mentioned in the import steps as a tip) </p>
  -->

* 새 이니셔티브로 프로젝트에 가져오려면 [!UICONTROL 보기] 이상의 권한이 있어야 합니다.
* 동일한 프로젝트를 여러 플랜으로 가져올 수 있습니다.
* 가져오려는 프로젝트의 날짜는 플랜 일정에 포함되어 있어야 합니다. [!UICONTROL 계획된 완료 일자]가 계획 시작보다 빠른거나 [!UICONTROL 계획된 시작 일자]가 계획 종료보다 늦은 프로젝트를 가져올 수 없습니다.
* 한 번에 100개 이상의 프로젝트를 가져올 수 없습니다.
* 일부 프로젝트 정보도 플랜으로 가져와서 이니셔티브 정보가 됩니다. 플랜으로 가져와서 이니셔티브 정보가 되는 프로젝트 정보에 대한 자세한 내용은 이 문서의 [플랜으로 가져온 프로젝트 정보](#project-information-imported-into-the-plan) 섹션을 참조하십시오.
* 연결된 프로젝트에서 발생하는 변경 사항은 계획에 대한 이니셔티브에 영향을 주지 않습니다.
* 플랜의 이니셔티브에 발생한 변경 사항은 연결된 프로젝트에 자동으로 영향을 주지 않습니다. 이니셔티브 변경 사항은 플랜에서 이니셔티브를 게시할 때만 연결된 프로젝트에 영향을 줍니다. 이니셔티브 게시가 연결된 프로젝트에 미치는 영향에 대한 자세한 내용은 [이니셔티브를 게시하여 프로젝트 업데이트 또는 만들기 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)를 참조하십시오.
* 프로젝트를 가져와서 만든 이니셔티브를 삭제해도 프로젝트가 삭제되지 않습니다.
* 이니셔티브에 연결된 프로젝트를 삭제해도 이니셔티브는 삭제되지 않습니다.

## 플랜으로 가져온 프로젝트 정보 {#project-information-imported-into-the-plan}

프로젝트를 플랜으로 가져오면 일부 프로젝트 정보도 플랜으로 가져오고 이니셔티브 정보가 됩니다. 다음 테이블은 프로젝트를 계획으로 가져올 때 어떤 프로젝트 정보가 이니셔티브 정보가 되는지 보여 줍니다.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add what happens if you import a 5 year project to a 1 year plan - how does this display?) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>프로젝트 정보</td> 
   <td>이니셔티브 정보 </td> 
  </tr> 
  <tr> 
   <td>프로젝트 이름</td> 
   <td>이니셔티브 이름</td> 
  </tr> 
  <tr> 
   <td>프로젝트 계획 일자</td> 
   <td> <p>이니셔티브 시작 및 종료 월.</p> <p>프로젝트가 한 달 중간에 시작되거나 종료되는 경우 플랜에서 가져온 날짜가 전체 한 달을 포함하도록 확장됩니다. 예를 들어 프로젝트 계획 일자가 2020년 3월 20일 - 5월 5일인 경우 가져온 이니셔티브의 일자는 2020년 3월 - 5월입니다.</p> <p>계획된 시작 일자 또는 완료 일자가 계획 기간 이후인 경우 임포트된 이니셔티브가 계획 이전 또는 이후에 시작된다는 시각적 표시가 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>작업 및 문제에 할당된 작업 역할</td> 
   <td> <p>이니셔티브 작업 역할. </p> <p>참고:   <p>사용자가 프로젝트 수명 중에 역할을 변경하는 경우 가져오는 역할은 프로젝트를 가져올 때 할당 상태에 따라 다릅니다. 다음과 같은 시나리오가 있습니다.</p> 
     <ul> 
      <li> <p>작업 또는 문제에 할당된 사용자가 할당을 [!UICONTROL 완료]로 표시한 후 역할을 변경한 경우 [!DNL Workfront]은(는) 할당을 [!UICONTROL 완료]로 표시하기 전에 사용자가 이행한 역할을 이니셔티브로 가져옵니다.</p> </li> 
      <li> <p>작업 또는 문제에 할당된 사용자가 프로젝트 수명 동안 역할을 변경했지만 프로젝트를 가져올 때 작업 또는 문제에 할당된 작업이 [!UICONTROL 완료]로 표시되지 않으면 [!DNL Workfront]에서 할당된 사용자의 현재 역할만 가져옵니다. </p> </li> 
     </ul> <p>할당 상태에 대한 자세한 내용은 <a href="../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Adobe 용어집 [!DNL Workfront] 용어</a>의 "할당 상태"를 참조하십시오. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>작업 또는 문제에 할당된 작업 역할과 연결된 프로젝트 [!UICONTROL 계획된 시간]</td> 
   <td> <p><span>FTE를 사용하도록 계획을 설정했는지 또는 시간을 사용했는지 여부에 따라 프로젝트의 작업에서 [!UICONTROL 계획된 시간]이 </span> [!UICONTROL 필수 FTE] <span> 또는 [!UICONTROL 필수 시간]이 됩니다</span>. </p> <p>FTE 또는 시간을 사용할 계획을 설정하는 방법에 대한 자세한 내용은 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">[!DNL Scenario Planner]</a>에서 계획 만들기 및 편집을 참조하십시오. </p> <p>다음 사항을 고려하십시오.</p> 
    <ul> 
     <li> <p>[!DNL Workfront] 은 작업 및 문제에 할당된 작업 역할이나 작업 또는 문제에 할당된 사용자가 프로젝트에서 연결된 작업 역할을 사용하고 이를 새 이니셔티브에 필수 작업 역할로 전송합니다. </p> </li> 
     <li> <p>FTE를 사용하도록 계획을 설정하면 프로젝트의 작업 및 문제에 대한 작업 역할과 연결된 계획된 시간이 먼저 FTE로 변환됩니다. 그런 다음 이 FTE가 이니셔티브의 작업 역할에 할당됩니다. <span>계획된 시간이 [!DNL Workfront]에 균등하게 분배됩니다. 작업 또는 문제가 여러 달에 걸쳐 있는 경우 이니셔티브 기간 내 각 달의 계획된 시간 양은 월별 FTE로 변환되고 이니셔티브의 각 달로 전송됩니다.</span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><span>예를 들어 9월에 계획된 시간 80시간 동안 작업 역할에 작업이 할당되면 가져온 작업 역할에 9월의 이니셔티브에 대해 0.5 FTE가 표시됩니다.</span> </p> </li> 
     <li> <p>[!DNL Workfront] 다음 공식을 사용하여 이니셔티브와 연관된 필수 작업 역할의 FTE를 계산합니다.</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>팁: [!DNL Scenario Planner]은(는) 한 달에 160개의 작업 시간이 있다고 가정합니다.</p> <p>예를 들어 프로젝트의 지속 시간이 1200분이고 프로젝트의 작업 역할이 계획된 시간 600분과 연결된 경우 FTE는 0.5입니다. 프로젝트를 가져올 때 새로 생성된 이니셔티브의 필수 작업 역할 FTE는 이니셔티브의 각 달에 대해 0.5입니다. </p> </li> 
     <li>계획된 시간이 0인 프로젝트의 작업에 작업 역할이 할당되면 이니셔티브의 작업 역할에 대한 필수 FTE는 기본적으로 0입니다. <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         (NOTE: this used to be 1, not zero in Production) 
       </MadCap:conditionalText>
      --></li> 
     <li>[!UICONTROL Duration]이(가) 0인 프로젝트의 작업에 작업 역할이 할당되면 작업에 계획된 시간이 있더라도 이니셔티브의 작업 역할에 대한 필수 FTE <span> 또는 시간</span>은(는) 기본적으로 0입니다. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 플랜에 프로젝트 가져오기

>[!IMPORTANT]
>
>프로젝트를 플랜으로 가져온 후 플랜에서 이니셔티브가 됩니다. 두 항목은 연결되어 있지만 독립적인 엔티티로 존재하며 업데이트할 때 서로 자동으로 영향을 주지 않습니다.
>
>다음이 발생합니다.
>
>* 프로젝트를 플랜으로 가져온 후에는 프로젝트 변경 사항이 이니셔티브에 영향을 주지 않습니다. 이러한 변경 사항에는 작업 역할 할당에 대한 변경 사항이 포함됩니다.
>
>  <!--
>  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change if projects will ever affect initiatives automatically) </p>>
>  -->
>
>* 이니셔티브를 변경하면 해당 프로젝트에 이니셔티브를 게시하는 경우에만 프로젝트의 [!DNL Scenario Planner] 영역에 있는 정보에 영향을 줍니다. 그렇지 않으면 프로젝트의 작업 및 문제에 대한 [!UICONTROL 계획된 시간] 정보에 영향을 주지 않습니다.
>
>  이니셔티브 게시가 연결된 프로젝트에 미치는 영향에 대한 자세한 내용은 [시나리오 플래너에서 이니셔티브를 게시하여 프로젝트 업데이트 또는 만들기](../scenario-planner/publish-scenarios-update-projects.md)를 참조하십시오.
>

{{step1-to-scenario-planner}}

1. 프로젝트를 가져올 플랜의 이름을 클릭합니다.
1. **[!UICONTROL 새 이니셔티브]**&#x200B;를 클릭한 다음 **[!UICONTROL 프로젝트 가져오기]**&#x200B;를 클릭합니다.

   [!UICONTROL 프로젝트 가져오기] 상자가 표시됩니다. 플랜의 시간대에 포함된 날짜가 있는 프로젝트가 목록에 표시됩니다.

   ![](assets/project-import-ui-projects-selected-350x72.png)

   >[!TIP]
   >
   >모든 상태의 프로젝트가 목록에 표시됩니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the status of the projects in the import projects UI might change; right now it's ALL statuses)</p>
   -->

1. (선택 사항) **[!UICONTROL 필터 아이콘]** ![](assets/filter-nwepng.png)을 클릭하고 목록에서 사용 가능한 필터를 선택하여 목록의 프로젝트 양을 줄이십시오. 기본적으로 프로젝트 목록은 프로젝트 목록에서 사용자가 현재 선택한 프로젝트 필터로 필터링됩니다.

1. (선택 사항) **[!UICONTROL 검색 아이콘]** ![](assets/search-icon.png)을 클릭하고 화면의 필드에 표시된 키워드를 추가합니다. 검색어를 포함하는 항목이 목록에 자동으로 표시되고 모든 항목이 숨겨집니다.

1. (조건부) **[!UICONTROL X 아이콘]**&#x200B;을 클릭하여 검색을 제거하고 모든 프로젝트를 표시합니다.
1. 최대 100개의 프로젝트를 선택하고 **[!UICONTROL 가져오기]**&#x200B;를 클릭합니다.

   프로젝트를 새 이니셔티브로 가져옵니다.

   다음 사항에 주목하십시오.

   * 이니셔티브 이름 오른쪽에 프로젝트 아이콘 ![](assets/project-icon-sp.png)이(가) 표시됩니다.
   * 프로젝트 타임라인이 플랜 기간을 초과하는 경우 이니셔티브의 막대는 왼쪽(시작 일자가 플랜 일자보다 빠른 경우) 또는 오른쪽(종료 일자가 플랜 일자보다 늦은 경우)에 뾰족한 여백으로 끝납니다.

     ![](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)

   * 개월 수와 작업 역할이 프로젝트의 개월 수와 일치하도록 업데이트되었습니다.

   >[!TIP]
   >
   >작업 역할과 관련된 비용은 이니셔티브 수준에서 업데이트되며 프로젝트에서 가져오지 않습니다.

1. 새 이니셔티브를 나타내는 막대를 클릭하여 오른쪽에 이니셔티브 세부 사항 패널을 엽니다.

   ![](assets/initiative-duration-with-project-duration-details-panel-350x292.png)

   **[!UICONTROL 이니셔티브 기간]** 영역에서 다음 정보를 검토하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Duration]</td> 
      <td>이니셔티브 기간(단위: 월)입니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative]</td> 
      <td>이니셔티브의 시작 및 종료 날짜입니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 프로젝트]</td> 
      <td> <p>연결된 프로젝트의 [!UICONTROL 계획된 시작] 및 [!UICONTROL 완료 일자].</p> <p>팁: [!UICONTROL Project] 정보가 누락된 경우 프로젝트가 삭제되었습니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 이니셔티브의 이름을 편집합니다. 기본적으로 프로젝트의 이름과 일치합니다.
1. (선택 사항) 다음 중 하나를 수행합니다.

   * **[!UICONTROL 필수 작업 역할]** 섹션에서 작업 역할 업데이트
   * **[!UICONTROL 비용]** 섹션에서 **[!UICONTROL 고정 비용]** 업데이트

   * 플랜에 대한 새 이니셔티브와 다른 이니셔티브 간의 충돌을 해결하려면 **[!UICONTROL 사용 가능한 작업 역할 업데이트]** 또는 **[!UICONTROL 사용 가능한 예산 업데이트]**&#x200B;를 클릭하십시오.

1. (조건부) **[!UICONTROL 적용]**&#x200B;을 클릭하여 이니셔티브에 변경 내용을 저장합니다.
1. **[!UICONTROL 플랜 저장]**&#x200B;을 클릭하여 플랜에 대한 변경 내용을 저장합니다.
1. (선택 사항) 이니셔티브의 변경 사항을 가져온 프로젝트로 다시 업데이트하려면 플랜에서 프로젝트를 게시합니다. 게시 계획에 대한 자세한 내용은 [이니셔티브를 게시하여 프로젝트 업데이트 또는 만들기 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)를 참조하십시오.
1. (선택 사항) 프로젝트 아이콘을 클릭하여 연결된 프로젝트에 액세스합니다.

   ![](assets/project-icon-on-initiative-highlighted-350x49.png)
