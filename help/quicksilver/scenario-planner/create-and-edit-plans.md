---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 플래너에서 계획 생성 및 편집
description: 회사의 상위 수준 전략에 우선 순위를 지정할 때 Workfront 시나리오 플래너 사용의 일부로 계획을 만들 수 있습니다. 계획에 대한 자세한 내용은 시나리오 계획자의 계획 개요를 참조하십시오.
author: Alina
feature: Workfront Scenario Planner
exl-id: 15c0e519-0164-449d-84f3-470d0d4eb795
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '2396'
ht-degree: 0%

---

# [!DNL Scenario Planner]에서 계획 만들기 및 편집

회사의 상위 수준 전략에 우선 순위를 지정할 때 [!DNL Workfront Scenario Planner]을(를) 사용하는 과정에서 계획을 만들 수 있습니다. 플랜에 대한 자세한 내용은  [!DNL Scenario Planner]](../scenario-planner/plans-overview.md)에서 [플랜 개요를 참조하십시오.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: talk about:</p>
<p>- Show people conflicts >> this impacts the conflicts calculation for initiatives>> link to the conflicts article</p>
<p>- explain what hovering over the green upward-pointing arrow does, with screen shot)</p>
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
   <p>새 Workfront Select 또는 Workfront 플랜에는 시나리오 플래너를 사용할 수 없습니다. </p>
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
   <td> <p>다음에 대한 [!UICONTROL 편집] 액세스 권한: [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>개체 권한 </p> </td> 
   <td> <p>플랜에 대한 [!UICONTROL 관리] 권한</p> <p>플랜에 대한 추가 액세스 요청에 대한 자세한 내용은 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">플랜에 대한 액세스 요청 [!DNL Scenario Planner]</a>을(를) 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서에 대한 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 계획 생성 또는 편집

처음부터 계획을 작성하거나 사용자와 공유된 기존 계획을 편집할 수 있습니다.

>[!NOTE]
>
>계획을 생성한 후에는 계획 생성자 및 소유자로 간주됩니다. 사용자가 비활성화되면 플랜에는 소유자가 없으며 이전에 링크와 공유하지 않는 한 누구에게도 표시되지 않습니다.

이 문서에서는 처음부터 계획을 작성하거나 기존 계획을 편집하는 방법에 대해 설명합니다.

플랜에 사용할 수 있는 정보를 포함하여 플랜에 대한 모든 고려 사항은  [!DNL Scenario Planner]](../scenario-planner/plans-overview.md)에서 [플랜 개요를 참조하십시오.

플랜 삭제에 대한 자세한 내용은 [다음에서 플랜 삭제 [!DNL Scenario Planner]](../scenario-planner/delete-plans.md)를 참조하십시오.

계획을 생성하거나 편집하려면

{{step1-to-scenario-planner}}

생성한 기존 계획 목록이 [!DNL Workfront Scenario Planner]에 표시됩니다.

1. (선택 사항) 계획 목록의 오른쪽 상단에 있는 **[!UICONTROL 필터]** 아이콘 ![](assets/filter-icon-34x37.png)을(를) 클릭하고 다음 중에서 선택합니다.

   | 필터 | 설명 |
   |---|---|
   | [!UICONTROL 모두] | 사용자가 만들었거나 사용자와 공유된 모든 계획을 표시합니다. |
   | [!UICONTROL 내 플랜] | 생성한 계획을 표시합니다. |
   | [!UICONTROL 나와 공유] | 사용자와 공유된 계획을 표시합니다. |

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (선택 사항) **[!UICONTROL 검색]** 아이콘 ![](assets/search-icon.png)을(를) 클릭하여 키워드를 입력하고 목록에서 계획을 빠르게 찾습니다.

1. 기존 계획의 이름을 클릭하여 편집하고 7단계로 진행합니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate) </p>
   -->

   또는

   왼쪽 상단의 **[!UICONTROL 새 계획]**&#x200B;을 클릭하여 계획을 만들고 5단계를 계속합니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate)</p>
   -->

   ![](assets/new-plan-button.png)

   [!UICONTROL 새 플랜] 상자가 표시됩니다.

   ![](assets/new-plan-ui-adding-a-new-plan-350x306.png)

1. (조건부) 신규 계획을 생성할 때 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 이름]</td> 
      <td>플랜의 이름을 입력합니다. 필수 필드입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p>중요: <span style="font-weight: normal;">계획을 만들고 저장한 후에는 다음 선택 항목을 수정할 수 없습니다.</span> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>FTE([!UICONTROL Full Time Equivalent]) 또는 [!UICONTROL Hours]</span> </td> 
      <td> <p><span>다음 옵션 중 하나를 선택하여 이 플랜에 대한 작업 역할 정보를 예상할 방법을 지정하십시오.</span> </p> 
       <ul> 
      <li> <p><span><strong>FTE</strong> 기본 </span>입니다. </p> 
      <p><b>중요 사항</b></p>  
      <p>[!DNL Scenario Planner]의 모든 계산에 대해 [!DNL Workfront]은(는) 다음 값을 사용합니다. 1 FTE = 8시간. </p> </li> 
      <li> <p><strong>[!UICONTROL 시간]</strong> </p> </li> 
       </ul> <p><b>중요 사항</b></p>

   여기서 선택하는 옵션은 계획, 계획의 시나리오 및 이니셔티브에 대한 작업 역할 정보가 표시되는 방법을 결정합니다</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 시작 날짜]</td> 
      <td> <p>계획을 시작할 월과 연도를 선택합니다. 이 필드에서는 월만 선택할 수 있습니다. [!DNL Workfront]은(는) 플랜의 시작 날짜가 선택한 월의 첫 날이고 종료 날짜가 해당 기간의 월 마지막 날이라고 가정합니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 기간]</td> 
      <td> <p>드롭다운 메뉴에서 다음 기간 중에서 선택합니다.</p> 
       <ul> 
        <li>1년. 기본 기간입니다. </li> 
        <li>3년</li> 
        <li> <p>5년</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--for table above - how FTE is calcualted: NOTE: snippet below: this is per Ani; it does NOT look at the system FTE.) </p>-->

1. (조건부) **[!UICONTROL 다음]**&#x200B;을 클릭합니다.

   플랜의 타임라인이 **[!UICONTROL 초기 시나리오]**(으)로 표시됩니다.

   추가 시나리오 만들기에 대한 자세한 내용은 [계획 시나리오 만들기 및 비교 [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md)를 참조하십시오.

1. (선택 사항) 타임라인 드롭다운 메뉴에서 다음 표의 옵션 중 하나를 선택하여 계획의 타임라인 보기 방법을 변경합니다.

   ![](assets/month-dropdown-with-all-options.png)

   | 드롭다운 메뉴 옵션 | 설명 |
   |---|---|
   | [!UICONTROL 개월] | 월별 시간표를 표시합니다. 1년 계획의 기본값이자 유일한 옵션입니다. |
   | [!UICONTROL 분기] | 분기별로 타임라인을 표시합니다. 이 옵션은 플랜의 [!UICONTROL 기간]이 3년 또는 5년인 경우에만 사용할 수 있습니다. 3년 계획의 기본 옵션입니다. |
   | [!UICONTROL 년] | 연도별로 타임라인을 표시합니다. 이 옵션은 플랜의 [!UICONTROL 기간]이 5년인 경우에만 사용할 수 있습니다. 5년 계획의 기본 옵션입니다. |

1. (선택 사항) 왼쪽에서 오른쪽으로 스크롤하여 계획의 전체 기간을 봅니다.
1. (선택 사항) 현재 날짜로 돌아가려면 **[!UICONTROL 오늘]** 표시줄을 클릭합니다.

   ![](assets/today-indicator-350x160.png)

1. 계획 헤더에 있는 **[!UICONTROL 작업 역할]** 상자를 클릭하여 계획을 실행하는 데 사용할 수 있는 작업 역할을 추가합니다.

   [!UICONTROL 작업 역할] 상자의 세부 정보가 표시됩니다.

   >[!TIP]
   >
   >[!DNL Workfront]이(가) 이 계획에 사용하는 역할 할당 단위(FTE 또는 시간)가 상자 제목의 괄호로 표시됩니다.

   ![](assets/adding-people-to-plan-350x206.png)

1. **[!UICONTROL 작업 역할 입력 시작]** 필드를 클릭하고 목록에서 역할을 선택하거나 활성 작업 역할의 이름을 입력하십시오.

   이 필드를 누르면 시스템의 모든 활성 작업 역할이 나열됩니다.

   작업 역할 열에 작업 역할이 추가됩니다.

1. 작업 역할에 대해 다음 정보를 업데이트하거나 검토합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max available] (FTE의 경우) </p> <p role="rowheader">또는 </p> <p role="rowheader"><span>[!UICONTROL 총 사용 가능](시간)</span> </p> </td> 
      <td> <p><span>플랜에 시간을 사용할지 FTE를 사용할지 여부에 따라 다음 필드에 플랜에 대한 작업을 실행하는 데 사용할 수 있는 작업 역할 FTE 수 <span>또는 시간</span>을(를) </span>입력하십시오. </p> 
       <ul> 
        <li> <p style="font-weight: normal;"><strong>[!UICONTROL Total available]</strong>(시간): 시나리오가 진행되는 동안 모든 달의 총 시간을 나타냅니다. 기본적으로 [!DNL Workfront]은(는) 시나리오 기간 동안 사용 가능한 총 수를 모든 달에 균등하게 나눕니다. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span>Designer에 1200시간을 입력하면 계획 [!UICONTROL Duration]이 1년일 때 계획 기간 동안 매월 100시간 동안 Designer을 사용할 수 있습니다. </p> </li> 
        <li> <p><b>[!UICONTROL 최대 사용 가능]</b>(FTE의 경우): 플랜 기간 동안 매월 작업 역할을 사용할 수 있는 FTE 수를 나타냅니다. 기본적으로 <strong>Workfront</strong>은(는) 시나리오 기간 동안 각 달에 [!UICONTROL Max available] 숫자를 할당합니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span>컨설턴트에게 1개의 FTE를 입력하면, 컨설턴트는 플랜 기간 동안 매달 1개의 FTE에 사용할 수 있습니다. </p> <p>1FTE보다 작은 숫자를 입력할 수 있습니다. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span>0.5 컨설턴트 작업 역할로 인해 컨설턴트는 FTE의 절반(일반적으로 4시간, 8시간은 FTE 1시간)을 이 플랜에 할애하게 됩니다. 시나리오 플래너의 모든 계산에 대해 Workfront은 다음 값을 사용합니다. 1 FTE = 8 시간. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL 최대 필요] (FTE의 경우)</p> <p role="rowheader">또는 </p> <p role="rowheader"><span>[!UICONTROL 총 필요](시간)</span> </p> </td> 
      <td> <p><span>플랜에 시간을 사용할지 FTE를 사용할지 여부에 따라 시나리오에서 이니셔티브를 완료하는 데 필요한 작업 역할 FTE 수 <span>또는 시간</span>을(를) 검토</span>하십시오. 다음 필드를 검토하십시오.</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Total required]</strong>(시간): 플랜 기간 동안 모든 달에 필요한 총 시간입니다.</p> </li> 
        <li> <p><strong>[!UICONTROL 최대 필요]</strong>(FTE의 경우): 플랜 기간 동안 필요한 최대 FTE 수. </p> </li> 
       </ul> <p>팁: 이니셔티브를 추가하기 시작한 후에 해당 작업 역할에 필요한 <span>최대</span> FTE 수 <span>또는 총 시간</span>이 표시됩니다. 계획에 이니셔티브를 추가하는 방법에 대한 자세한 내용은 <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">이니셔티브 만들기 및 편집([!DNL Scenario Planner]</a>)을 참조하십시오.</p> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">[!UICONTROL Avg utilization]</td> 
       <td> <p>(NOTE: this field was removed in 21.2 - May 2021) </p> <p>[!DNL Workfront] calculates the average utilization for each job role using the job role FTEs associated with initiatives (required) and the job role FTEs associated with the plan (available). </p> <p> [!DNL Workfront] calculates the job role utilization percentage for a plan using the following formula: </p> <p><code>Job role utilization percentage = Sum [(Required job roles for each month of the plan *100)/ (Available job roles for each month of the plan)] / Number of months in the Duration of the plan</code> </p> 
        <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Example: </b></span></span> 
         <p>For example, if you have a plan with a duration of 12 months and an initiative with the duration of 2 months, where you use 1 Designer for your initiative (required job role) and there are 2 Designers available on the plan (available), the Utilization percentage for the Designer job role is calculated as follows:</p> 
         <p><code>Designer utilization percentage = [(1/2 + 1/2) * 100] / 12 = 100 / 12 = 8.3%</code> </p> 
        </div> <p>As you add job roles to the plan and indicate the Available amount for each one, the [!UICONTROL Utilization] value for each role also updates and [!DNL Workfront] calculates a utilization percentage for the plan. For information about how [!DNL Workfront] calculates the Job Role Utilization for a plan, see <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Plans overview in the [!DNL Scenario Planner]</a>. </p> <p>Tip: The Utilization percentage is rounded and has one decimal. </p> </td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">[!UICONTROL 시간당 요금]</td> 
      <td> <p>작업 역할에 대한 [!UICONTROL 비용 시간] 비율입니다. 시간별 요금은 시스템 통화로 표시됩니다. 시스템의 환율 설정에 대한 자세한 내용은 <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">환율 설정</a>을 참조하십시오.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 역할 정보를 업데이트한 후 작업 역할의 이름 위에 마우스를 가져다 대거나 탭을 클릭한 다음 **[!UICONTROL 휴지통 아이콘]** ![](assets/delete.png)을(를) 클릭하여 계획에서 제거합니다.
1. **[!UICONTROL 작업 역할 분배]**&#x200B;를 클릭합니다.

   작업 역할 분배 패널이 시나리오 기간 내의 모든 달에 대해 표시됩니다.

   ![](assets/job-role-monthly-distribution-box-fte-350x144.png)

1. **[!UICONTROL 작업 역할 입력 필드]**&#x200B;에서 계획에 추가할 작업 역할 이름을 입력한 다음 목록에 나타나면 [입력]을 클릭하십시오. [!UICONTROL 작업 역할] 열에 작업 역할을 추가합니다.
1. 시나리오의 각 달에 대한 다음 정보를 업데이트하거나 검토합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 작업 역할] (FTE 또는 시간)</td> 
      <td>시나리오에 사용할 수 있는 작업 역할과 시나리오의 이니셔티브에 필요한 작업 역할이 모두 작업 역할 분배 패널에 표시됩니다. 작업 역할 예상이 FTE에 있는지 또는 열 헤더에 시간이 있는지 여부가 표시됩니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 사용 가능](최대 &lt;FTE 수&gt;) </p> 
       <div> 
        <p>또는</p> 
        <p>[!UICONTROL 사용 가능] (총 &lt;시간 수&gt;) </p> 
       </div> </td> 
      <td> <p><span>플랜에 시간을 사용할지 FTE를 사용할지 여부에 따라 </span> 다음 필드의 시나리오에 사용할 수 있는 월별 작업 역할 FTE 수 <span>또는 시간</span>을(를) 검토하거나 업데이트하십시오.</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL 사용 가능](최대 &lt;FTE 수&gt;)</strong>: 괄호로 묶인 숫자는 시나리오의 어느 한 달에 사용할 수 있는 최대 역할 수를 표시합니다. 시나리오의 각 달에 대한 FTE 수를 검토하거나 업데이트합니다. 월별 할당을 변경하면 괄호 안에 있는 FTE 수가 업데이트될 수 있습니다. </p> </li> 
        <li> <p><span><strong>[!UICONTROL 사용 가능](총 &lt;시간 수&gt;)</strong>: 괄호로 묶인 숫자는 시나리오의 모든 달에 사용할 수 있는 총 시간을 표시합니다. 시나리오의 각 달에 대한 시간 수를 검토하거나 업데이트합니다. 월별 할당을 변경하면 괄호 안의 시간 수가 업데이트됩니다.</span> </p> </li> 
       </ul> <p>월별 작업 역할 할당을 수동으로 업데이트하는 것은 시나리오에서 이니셔티브 간 작업 역할 충돌을 해결하는 또 다른 방법입니다. </p> <p>팁:   <p><span>월별 역할 가용성을 여러 달 동안 업데이트하려면 특정 월의 [!UICONTROL 사용 가능] 필드에 시간 또는 FTE 수를 입력한 다음 필드의 모서리를 인접한 개월 위로 끌어 놓아 각 달에 대해 동일한 값을 복사합니다. 모든 월을 업데이트하려면 삭제하세요.</span> </p> <p> <img src="assets/job-role-distribution-draggable-corner-highlighted-350x83.png" style="width: 350;height: 83;"> </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL 필수] (최대 &lt;숫자&gt;)</p> 
       <div> 
        <p role="rowheader">또는</p> 
        <p role="rowheader">[!UICONTROL Required] (total &lt;number&gt;)</p> 
       </div> </td> 
      <td> <p><span>플랜에 시간을 사용할지 FTE를 사용할지 여부에 따라 </span> 다음 필드에서 시나리오에 필요한 월별 작업 역할 FTE 수 또는 시간을 검토하십시오. </p> 
       <ul> 
        <li> <p><strong>[!UICONTROL 필수](최대 &lt;FTE 수&gt;)</strong>: 괄호 안의 숫자는 시나리오의 어느 한 달에 필요한 최대 역할 수를 표시합니다. </p> </li> 
        <li> <p><span><strong>[!UICONTROL 필수](총 &lt;시간 수&gt;)</strong>: 괄호 안의 숫자는 시나리오의 모든 달에 필요한 총 시간을 표시합니다.</span> </p> </li> 
       </ul> <p>팁: 작업 역할에 필요한 FTE 수 <span> 또는 시간</span>을(를) 수정할 수 없습니다. 이니셔티브 및 해당 작업 역할 요구 사항 추가를 시작하면 이 숫자가 시나리오에 대해 채워집니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Difference]</td> 
      <td> 
       <div> 
        <p>시나리오에 필요한 작업 역할과 사용 가능한 작업 역할의 월별 차이입니다. [!DNL Workfront]은(는) 다음 수식을 사용하여 각 달의 각 작업 역할에 대한 차이를 계산합니다.</p> 
        <p><code>Monthly role difference = Monthly required roles - Monthly available roles</code> (FTE 또는 시간 단위) </p> 
        <p>팁: 차이가 음수를 표시할 경우 시나리오에는 계획을 사용할 수 있는 것보다 더 많은 작업 역할이 필요합니다. 리소스가 초과 할당되었습니다. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 사용률] %</td> 
      <td> 
       <div> 
        <p>사용률은 시나리오의 이니셔티브에서 사용 가능한 작업 역할 중 실제로 사용되는(또는 필요한) 작업 역할의 수를 표시합니다. </p> 
        <p>[!DNL Workfront] 다음 공식을 사용하여 월별 작업 역할당 가동률을 계산합니다. </p> 
        <p><code>Monthly role utilization % = Monthly required roles / Monthly available roles * 100</code> </p> 
        <p>활용률 비율은 리소스 할당에 따라 다음 색상으로 표시될 수 있습니다.</p> 
        <ul> 
         <li> <p><b>녹색</b>: 사용 가능한 작업 역할과 필요한 작업 역할 수가 일치합니다. 자원이 완전히 할당되고 활용률은 100%입니다. </p> </li> 
         <li> <p><b>빨강</b>: 계획을 사용할 수 있는 것보다 더 많은 필수 작업 역할이 있습니다. 자원이 과다 할당되고 활용 비율이 100%보다 높다.</p> </li> 
         <li> <p><b>파란색</b>: 사용 가능한 작업 역할이 필요 이상으로 많습니다. 자원이 과소 할당되고 활용 비율은 100%보다 낮다. </p> </li> 
        </ul> 
       </div> <p> <img src="assets/utilization-percent-colors-sp-350x61.png" style="width: 350;height: 61;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 월별 작업 역할 분포를 저장하려면 **[!UICONTROL 적용]**&#x200B;을 클릭하십시오.

   또는

   작업 역할 배포 목록을 닫고 시나리오로 돌아가려면 **[!UICONTROL 취소]**&#x200B;를 클릭하십시오.

1. 플랜 헤더에서 **[!UICONTROL 재무]** 상자를 클릭하여 이 플랜에 대한 예산을 추가합니다.

   [!UICONTROL Financial] 상자에 대한 세부 정보가 표시됩니다.

   >[!TIP]
   >
   >[!DNL Workfront]이(가) 이 플랜에 사용하는 통화는 상자 제목에서 괄호로 표시됩니다.

1. **[!UICONTROL 연간 예산]**&#x200B;을 지정하십시오.

   >[!NOTE]
   >
   >계획이 여러 연도에 걸쳐 있는 경우 각 연도의 예산 금액을 지정해야 합니다.

1. Enter 키를 눌러 연간 예산을 저장한 다음 [!UICONTROL Tab]을 눌러 다음 연도로 이동합니다.

   연간 예산은 선택한 연도의 각 달에 대해 자동으로 균등하게 분배됩니다.

1. 월별 예산 분포를 보려면 **[!UICONTROL 고급]**&#x200B;을 클릭하세요. 연간 및 월별 예산은 항상 반올림된 숫자입니다. 소수로 인해 1년 내의 모든 달에 예산 금액을 균등하게 분배할 수 없는 경우 **[!UICONTROL 남은]** 표시기가 연간 예산 분배 아래에 표시됩니다.

   ![](assets/adanced-and-remaining-links-on-plan-budget-350x507.png)

1. 초과 금액을 제거하기 위해 월별 예산을 수동으로 조정합니다.

   모든 월별 예산 금액의 합계가 연간 예산보다 큰 경우 연간 예산 분포 아래에 **[!UICONTROL 초과]** 경고 표시기가 표시됩니다. 월별 예산 금액이 계획에 대해 사용 가능한 예산과 같거나 낮을 때까지 수동으로 조정합니다.

   ![](assets/exceeding-budget-warning-on-plan-350x483.png)

1. **[!UICONTROL 인력 비용 포함]** 설정을 비활성화하여 작업 역할과 관련된 비용을 계획의 전체 비용 계산에서 제외합니다. 고정 비용은 항상 계획의 전체 비용에 포함됩니다. 이 설정은 기본적으로 활성화되어 있으며 플랜의 모든 시나리오에 영향을 줍니다.
1. 닫으려면 [!UICONTROL 재무] 상자 외부의 아무 곳이나 클릭하십시오. 입력한 정보가 자동으로 저장됩니다.

   이제 플랜에 대한 이니셔티브를 생성하고 시나리오를 추가할 수 있습니다.

1. (권장) 새 이니셔티브를 추가하려면 **[!UICONTROL 새 이니셔티브]**&#x200B;를 클릭합니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Should this include information on how to create scenarios - see also information about scenarios in Manage Plans?)</p>
   -->

   이니셔티브 추가에 대한 자세한 내용은 문서 [이니셔티브 만들기 및 편집 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md)을 참조하십시오.

1. (선택 사항) 기존 시나리오의 복사본을 만들어 동일한 계획의 새 시나리오를 만듭니다. 여러 시나리오를 만들고 작업하는 방법에 대한 자세한 내용은 [계획 시나리오 만들기 및 비교 [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md)를 참조하십시오.
1. **[!UICONTROL 플랜 저장]**&#x200B;을 클릭합니다.

   플랜이 생성되거나 업데이트됩니다.

1. (선택 사항) 플랜 이름 오른쪽에 있는 **[!UICONTROL 즐겨찾기 아이콘]** ![](assets/favorites-icon-small.png)을 클릭하여 즐겨찾기 목록에 플랜을 추가합니다.

1. (선택 사항) 플랜의 URL을 복사하여 검토하거나 업데이트해야 할 다른 사용자에게 보냅니다. 플랜을 보려면 액세스 수준에 [!UICONTROL 보기] 이상의 액세스 권한이 있어야 합니다. 편집하려면 [!UICONTROL 편집] 액세스 권한이 있어야 합니다. 예산, 비용 및 작업 역할 비율 정보와 같은 계획에 대한 재무 정보를 검토해야 하는 경우 액세스 수준의 [!UICONTROL 재무 데이터]에도 액세스할 수 있어야 합니다. [!DNL Scenario Planner]에 필요한 액세스에 대한 자세한 내용은 [을(를) 사용하는 데 필요한 액세스 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md)을(를) 참조하십시오.
