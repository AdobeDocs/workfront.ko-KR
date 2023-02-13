---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 플래너의 계획에 프로젝트 가져오기
description: 기존 프로젝트를 계획에 가져올 수 있습니다. 가져온 프로젝트는 이니셔티브로 변환되며 새 이니셔티브를 관리할 때처럼 계획 내에서 관리할 수 있습니다. 원래 프로젝트는 새 이니셔티브에 연결되어 있다.
author: Alina
feature: Workfront Scenario Planner
exl-id: 20429bb1-c158-433b-9790-325cd577248e
source-git-commit: 844dddec944b6cfb0957eecf09c2980e9d0577cc
workflow-type: tm+mt
source-wordcount: '1699'
ht-degree: 0%

---

# 계획 로 프로젝트 가져오기 [!DNL Scenario Planner]

기존 프로젝트를 계획에 가져올 수 있습니다. 가져온 프로젝트는 이니셔티브로 변환되며 새 이니셔티브를 관리할 때처럼 계획 내에서 관리할 수 있습니다. 원래 프로젝트는 새 이니셔티브에 연결되어 있다.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: add information about what happens when you import projects and where the info from projects show up;</p>
<p>- the hours/ FTE come from WorkPerDay</p>
<p>- if a task has a Duration of 0, the FTE should be 0 for that asignee but it should still come across) </p>
</div>
-->

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 플랜*</b> </p> </td> 
   <td>[!UICONTROL Business] 이상</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 라이센스*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] 이상</p> </td> 
  </tr> 
  <tr> 
   <td><b>제품</b> </td> 
   <td> <p>에 대한 추가 라이센스를 구입해야 합니다. [!DNL Adobe Workfront Scenario Planner] 을 눌러 이 문서에 설명된 기능에 액세스합니다.</p> <p>를 가져오는 방법에 대한 자세한 내용은 [!DNL Workfront Scenario Planner]를 참조하십시오. <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">을 사용하는 데 필요한 액세스 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>액세스 수준 구성*</strong> </td> 
   <td> <p>[!UICONTROL Edit] 액세스 이상의 [!DNL Scenario Planner]</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 변경할 수 있습니다. <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>개체 권한</strong> </p> </td> 
   <td> <p>계획에 대한 [!UICONTROL Manage] 권한</p> <p>계획에 대한 추가 액세스 요청에 대한 내용은 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">시나리오 플래너의 계획에 대한 액세스 요청</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 프로젝트를 새 이니셔티브로 계획에 가져오는 것에 대한 고려 사항

* 프로젝트를 새 이니셔티브로 계획에 가져오려면 먼저 프로젝트를 생성해야 합니다.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: no caveats for project statuses yet, mentioned in the import steps as a tip) </p>
  -->

* 최소한 [!UICONTROL 보기] 프로젝트에 대한 권한을 새 이니셔티브로 가져올 수 있습니다.
* 동일한 프로젝트를 여러 계획으로 가져올 수 있습니다.
* 가져오려는 프로젝트에 계획의 기간에 날짜가 포함되어야 합니다. 와 함께 프로젝트를 가져올 수 없습니다 [!UICONTROL 계획 완료 일자] 계획의 시작 또는 [!UICONTROL 계획 시작 날짜] 계획 종료 보다 늦게.
* 한 번에 100개 이상의 프로젝트를 가져올 수 없습니다.
* 일부 프로젝트 정보는 계획에 가져와서 이니셔티브 정보가 됩니다. 계획에 임포트되어 이니셔티브 정보가 되는 프로젝트 정보에 대한 자세한 내용은 [계획에 가져온 프로젝트 정보](#project-information-imported-into-the-plan) 섹션에 자세히 설명되어 있습니다.
* 연결된 프로젝트에서 발생하는 변경 사항은 계획의 이니셔티브에 영향을 주지 않습니다.
* 계획의 이니셔티브에서 발생하는 변경 사항은 연결된 프로젝트에 자동으로 영향을 주지 않습니다. 프로젝트 변경 사항은 계획에서 이니셔티브를 게시하는 경우에만 연결된 프로젝트에 영향을 줍니다. 게시 이니셔티브가 연결된 프로젝트에 미치는 영향에 대한 자세한 내용은 [에서 이니셔티브를 게시하여 프로젝트를 업데이트하거나 만들 수 있습니다 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
* 프로젝트를 가져와서 만든 이니셔티브를 삭제하면 프로젝트가 삭제되지 않습니다.
* 이니셔티브에 연결된 프로젝트를 삭제해도 이니셔티브가 삭제되지 않습니다.

## 계획에 가져온 프로젝트 정보 {#project-information-imported-into-the-plan}

프로젝트를 계획에 임포트하면 일부 프로젝트 정보도 계획에 임포트되어 이니셔티브 정보가 됩니다. 다음 테이블은 프로젝트를 계획으로 가져올 때 프로젝트 정보가 이니셔티브 정보가 되는 정보를 보여 줍니다.

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
   <td> <p>이니셔티브 시작 및 종료 개월</p> <p>프로젝트가 한 달 중에 시작되거나 종료되는 경우, 가져온 날짜는 계획에서 전체 월을 포함하도록 확장됩니다. 예를 들어, 프로젝트 계획 일자가 2020년 3월 20일~5월 5일인 경우, 임포트된 이니셔티브 일자는 2020년 3월~5월입니다.</p> <p>계획 시작 또는 완료 일자가 계획의 지속 기간을 초과하는 경우, 임포트된 이니셔티브가 계획 이전 또는 종료 후에 시작된다는 시각적 표시가 나타납니다. </p> </td> 
  </tr> 
  <tr> 
   <td>작업 및 문제에 할당된 작업 역할</td> 
   <td> <p>이니셔티브 작업 역할. </p> <p>참고:   <p>사용자가 프로젝트 수명 동안 역할을 변경할 경우 가져온 역할은 프로젝트를 가져올 때 지정 상태에 따라 다릅니다. 다음 시나리오가 있습니다.</p> 
     <ul> 
      <li> <p>작업 또는 문제에 지정된 사용자가 할당을 [!UICONTROL 완료]로 표시한 후 역할을 변경한 경우, [!DNL Workfront] [!UICONTROL 완료]로 표시되기 전에 사용자가 수행한 역할을 이니셔티브에 가져옵니다.</p> </li> 
      <li> <p>작업 또는 문제에 지정된 사용자가 프로젝트 수명 동안 역할을 변경했지만 프로젝트를 가져올 때 해당 작업 또는 문제에 대한 할당이 [!UICONTROL 완료]로 표시되지 않은 경우 [!DNL Workfront] 할당된 사용자의 현재 역할만 가져옵니다. </p> </li> 
     </ul> <p>발령 상태에 대한 자세한 내용은 <a href="../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Adobe 용어집 [!DNL Workfront] 용어</a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>작업 또는 문제에 할당된 작업 역할과 연결된 프로젝트 [!UICONTROL 계획 시간]</td> 
   <td> <p><span>계획이 FTE를 사용하도록 설정되어 있는지 아니면 시간을 사용하도록 설정되어 있는지에 따라 프로젝트의 작업에서 [!UICONTROL 계획 시간]이 다음 중 하나가 됩니다</span> [!UICONTROL 필수 FTE] <span>또는 계획에 대한 [!UICONTROL Required hours]</span>. </p> <p>FTE 또는 시간 사용 계획 설정에 대한 자세한 내용은 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">에서 계획 생성 및 편집 [!DNL Scenario Planner]</a>. </p> <p>다음 사항을 고려하십시오.</p> 
    <ul> 
     <li> <p>[!DNL Workfront] 작업 및 문제에 할당된 작업 역할 또는 프로젝트에서 작업 또는 문제에 할당된 사용자가 연관된 작업 역할을 사용하여 새 이니셔티브에 필수 작업 역할로 전송합니다. </p> </li> 
     <li> <p>FTE를 사용하도록 계획이 설정되면 프로젝트의 작업 및 문제에 대한 작업 역할과 연관된 계획 시간이 FTE로 먼저 변환됩니다. 그러면 이 FTE가 이니셔티브의 Job 역할에 할당됩니다. <span>계획된 시간은 동일하게 [!DNL Workfront]. 태스크 또는 문제가 여러 달에 걸쳐 있을 경우, 이니셔티브 기간 동안의 매월 계획된 시간 금액은 월별 FTE로 변환되어 이니셔티브의 매월 이전됩니다.</span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><span>예를 들어, 9월에 80개의 계획 시간(계획됨 시간)에 대한 작업 역할에 작업이 지정되면, 가져온 작업 롤은 9월에 이니셔티브에 대해 0.5 FTE를 표시합니다.</span> </p> </li> 
     <li> <p>[!DNL Workfront] 다음 공식을 사용하여 이니셔티브와 연관된 필수 작업 역할의 FTE를 계산합니다.</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>팁: 다음 [!DNL Scenario Planner] 에서는 한 달에 160개의 근무 시간이 있다고 가정합니다.</p> <p>예를 들어, 프로젝트에 지속 시간이 1200분이고 프로젝트에 대한 작업 역할이 계획 시간 600분과 연결된 경우 해당 FTE는 0.5입니다. 프로젝트를 가져올 때 새로 생성된 이니셔티브의 필수 작업 역할 FTE는 이니셔티브 매월 0.5입니다. </p> </li> 
     <li>계획 시간이 0인 프로젝트의 작업에 작업 역할이 지정되면 이니셔티브의 작업 역할에 대한 필수 FTE는 기본적으로 0입니다. <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         (NOTE: this used to be 1, not zero in Production) 
       </MadCap:conditionalText>
      --></li> 
     <li>[!UICONTROL 기간]이 0인 프로젝트의 작업에 작업 역할이 할당되면 필수 FTE입니다 <span>또는 시간</span> 이니셔티브 작업 역할에 대해서는 작업에 계획 시간이 있어도 기본적으로 0입니다. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



## 계획에 프로젝트 가져오기

>[!IMPORTANT]
>
>프로젝트를 계획으로 가져온 후 계획에 대한 이니셔티브가 됩니다. 두 항목은 연결되지만 독립 엔티티로 존재하며 업데이트할 때 자동으로 서로 영향을 주지 않습니다.
>
>다음 상황이 발생합니다.
>
>* 프로젝트를 계획에 가져온 후에는 프로젝트 변경 사항이 이니셔티브에 영향을 주지 않습니다. 이러한 변경 사항에는 작업 역할 할당에 대한 변경 사항이 포함됩니다.
>
>  <!--
>  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change if projects will ever affect initiatives automatically) </p>>
>  -->
>
>* 이니셔티브 변경 사항은 [!DNL Scenario Planner] 해당 프로젝트에 이니셔티브를 게시하는 경우에만 프로젝트의 영역입니다. 그렇지 않으면, 이 변수들은 [!UICONTROL 계획 시간] 프로젝트의 작업 및 문제에 대한 정보입니다.
>
>  게시 이니셔티브가 연결된 프로젝트에 미치는 영향에 대한 자세한 내용은  [시나리오 계획자에서 이니셔티브를 게시하여 프로젝트를 업데이트하거나 생성합니다](../scenario-planner/publish-scenarios-update-projects.md).

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Workfront]를 클릭한 다음 [!DNL Scenarios] 에 액세스하려면 [!DNL Scenario Planner].

1. 프로젝트를 가져올 계획의 이름을 누릅니다.
1. 클릭 **[!UICONTROL 새로운 이니셔티브]**&#x200B;를 클릭한 다음 **[!UICONTROL 프로젝트 가져오기]**.

   다음 [!UICONTROL 프로젝트 가져오기] 상자가 표시됩니다. 계획의 기간에 포함된 날짜가 있는 프로젝트가 목록에 표시됩니다.

   ![](assets/project-import-ui-projects-selected-350x72.png)

   >[!TIP]
   >
   >모든 상태의 프로젝트가 목록에 표시됩니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the status of the projects in the import projects UI might change; right now it's ALL statuses)</p>
   -->

1. (선택 사항) **[!UICONTROL 필터 아이콘]** ![](assets/filter-nwepng.png)목록에서 사용 가능한 필터를 선택하여 목록의 프로젝트 양을 줄입니다. 기본적으로 프로젝트 목록은 프로젝트 목록에서 사용자가 현재 선택한 프로젝트 필터로 필터링됩니다.

1. (선택 사항) **[!UICONTROL 검색 아이콘]** ![](assets/search-icon.png) 화면의 모든 필드에 표시되는 키워드를 추가합니다. 검색어가 포함된 항목은 자동으로 목록에 표시되고 모든 항목이 숨겨집니다.

1. (조건부) **[!UICONTROL X 아이콘]** 을 클릭하여 검색을 제거하고 모든 프로젝트를 표시합니다.
1. 최대 100개의 프로젝트를 선택하고 **[!UICONTROL 가져오기]**.

   그 프로젝트는 새로운 이니셔티브로 수입된다.

   다음 사항에 주의하십시오.

   * 프로젝트 아이콘 ![](assets/project-icon-sp.png) 이니셔티브 이름의 오른쪽에 표시됩니다.
   * 프로젝트 타임라인이 계획의 기간을 초과하는 경우, 이니셔티브 막대는 왼쪽(시작 일자가 계획 일자 이전일 경우) 또는 오른쪽(종료 일자가 계획 일자 이후일 경우)에 대해 뾰족한 마진으로 끝납니다.

      ![](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)

   * 월 및 작업 역할이 프로젝트의 역할과 일치하도록 업데이트되었습니다.
   >[!TIP]
   >
   >작업 역할과 연관된 비용은 이니셔티브 레벨에서 갱신되며 프로젝트에서 임포트되지 않습니다.

1. 새 이니셔티브를 나타내는 표시줄을 클릭하여 오른쪽에 이니셔티브 세부 사항 패널을 엽니다.

   ![](assets/initiative-duration-with-project-duration-details-panel-350x292.png)

   에서 **[!UICONTROL 이니셔티브 기간]** 영역: 다음 정보를 검토합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Duration]</td> 
      <td>이것은 몇 달 동안 이니셔티브의 기간이다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative]</td> 
      <td>이니셔티브 시작 및 종료 날짜입니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Project]</td> 
      <td> <p>연결된 프로젝트의 [!UICONTROL 계획 시작] 및 [!UICONTROL 완료 날짜].</p> <p>팁: [!UICONTROL Project] 정보가 없으면 프로젝트가 삭제되었습니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 이니셔티브의 이름을 편집합니다. 기본적으로 프로젝트 이름과 일치합니다.
1. (선택 사항) 다음 중 하나를 수행합니다.

   * 에서 작업 역할 업데이트 **[!UICONTROL 필수 작업 역할]** 섹션
   * 업데이트 **[!UICONTROL 고정 비용]** 에서 **[!UICONTROL 비용]** 섹션

   * 클릭 **[!UICONTROL 사용 가능한 작업 역할 업데이트]** 또는 **[!UICONTROL 사용 가능한 예산 업데이트]** 그 계획에 대한 새로운 주제와 다른 주제의 간의 갈등을 해결하기 위해.

1. (조건부) 클릭 **[!UICONTROL 적용]** 이니셔티브에 변경 사항을 저장합니다.
1. 클릭 **[!UICONTROL 계획 저장]** 계획 변경 사항을 저장하려면 다음을 수행합니다.
1. (선택 사항) 이니셔티브에 대한 변경 사항을 다시 가져온 프로젝트로 업데이트하려면 계획에서 프로젝트를 게시합니다. 계획 게시에 대한 자세한 내용은 [에서 이니셔티브를 게시하여 프로젝트를 업데이트하거나 만들 수 있습니다 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
1. (선택 사항) 프로젝트 아이콘을 클릭하여 연결된 프로젝트에 액세스합니다.

   ![](assets/project-icon-on-initiative-highlighted-350x49.png)
