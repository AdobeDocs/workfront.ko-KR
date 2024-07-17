---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 플래너에서 이니셔티브 만들기 및 편집
description: Adobe Workfront Scenario Planner를 사용할 때 생성했거나 공유한 계획에 이니셔티브를 생성할 수 있습니다. 이니셔티브를 생성하면 더 작은 조직 단위가 계획 완료에 기여하는 정도를 알 수 있습니다. 예를 들어, 조직에서 새로운 시장으로 확장하기 위한 향후 3년간의 계획을 가지고 있는 경우, 각 부서에 대해 이 계획 내에 이니셔티브를 생성하여 이 계획을 달성하기 위한 인력 및 예산에 대한 각 부서의 필요성을 추정할 수 있습니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: a811bad0-d3c0-4cba-8b78-d9a14ffc8482
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '1649'
ht-degree: 0%

---

# [!DNL Scenario Planner]에서 이니셔티브 만들기 및 편집

[!UICONTROL Adobe Workfront Scenario Planner]를 사용하는 경우 만들었거나 사용자와 공유된 플랜에서 이니셔티브를 만들 수 있습니다. 이니셔티브를 생성하면 더 작은 조직 단위가 계획 완료에 기여하는 정도를 알 수 있습니다. 예를 들어, 조직에서 새로운 시장으로 확장하기 위한 향후 3년간의 계획을 가지고 있는 경우, 각 부서에 대해 이 계획 내에 이니셔티브를 생성하여 이 계획을 달성하기 위한 인력 및 예산에 대한 각 부서의 필요성을 추정할 수 있습니다.

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
   <td> <p>[!DNL Adobe Workfront] 라이센스* </p> </td> 
   <td> <p>[!UICONTROL Review] 이상</p> </td> 
  </tr> 
  <tr> 
   <td>제품 </td> 
   <td> <p>이 문서에 설명된 기능에 액세스하려면 [!DNL Adobe Workfront Scenario Planner]에 대한 추가 라이선스를 구입해야 합니다. </p> <p>[!DNL Workfront Scenario Planner]을(를) 얻는 방법에 대한 자세한 내용은 [!DNL Scenario Planner]</a>을(를) 사용하는 데 필요한 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">액세스를 참조하십시오. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>액세스 수준 구성* </td> 
   <td> <p>다음에 대한 [!UICONTROL 편집] 액세스 이상: [!DNL Scenario Planner]</p> <p>아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하십시오. [!DNL Workfront] 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>개체 권한 </p> </td> 
   <td> <p>플랜에 대한 [!UICONTROL 관리] 권한</p> <p>플랜에 대한 추가 액세스 요청에 대한 자세한 내용은 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">플랜에 대한 액세스 요청 [!DNL Scenario Planner]</a>을(를) 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하십시오.

## 전제 조건

플랜을 작성하거나 다른 사용자가 플랜을 공유해야 해당 플랜 내에서 이니셔티브를 작성할 수 있습니다. 계획 만들기에 대한 자세한 내용은 [계획 만들기 및 편집 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)을 참조하세요.

이니셔티브가 무엇인지에 대한 자세한 내용은  [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md)에서 [이니셔티브 개요 를 참조하십시오.

## 이니셔티브 만들기

다음과 같은 방법으로 이니셔티브를 생성할 수 있습니다.

* 처음부터.
* 플랜으로 프로젝트 가져오기

  계획에서 이니셔티브로 프로젝트를 가져오는 방법에 대한 자세한 내용은 [계획으로 프로젝트 가져오기 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)를 참조하십시오.

* 기존 이니셔티브를 복사하여

  이니셔티브 복사에 대한 자세한 내용은 [의 이니셔티브 복사 [!DNL Scenario Planner]](../scenario-planner/copy-initiatives.md)를 참조하십시오.

이니셔티브를 처음부터 생성하려면:

1. **[!UICONTROL 주 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 [!UICONTROL 시나리오]를 클릭합니다.

1. 이니셔티브를 생성할 계획의 이름을 누릅니다.
1. **[!UICONTROL 새 이니셔티브]**&#x200B;의 왼쪽에 있는 **+ 아이콘**&#x200B;을 클릭합니다.

   또는

   **[!UICONTROL 새 이니셔티브]** 드롭다운 메뉴를 클릭하고 **[!UICONTROL 새 이니셔티브]** 또는 **[!UICONTROL 프로젝트 가져오기]를 선택합니다.**

1. **[!UICONTROL 제목 없는 이니셔티브]** 필드에 이니셔티브 이름을 입력한 다음 Enter 키를 누르거나 페이지의 다른 위치를 클릭합니다.

   이니셔티브가 계획의 타임라인에 파란색 막대로 표시됩니다. 기본적으로 이니셔티브 기간은 1개월이며 항상 플랜의 첫 달에 시작됩니다.

1. (선택 사항) 왼쪽 패널과 타임라인 사이에 분리 막대를 드래그하여 왼쪽 패널의 크기를 조정합니다.

1. (선택 사항) 이니셔티브 막대의 끝을 드래그하여 기간을 1개월 이상으로 늘린 다음 이니셔티브의 종료 월을 원하는 위치에 놓습니다.
1. (선택 사항 및 조건부) 이니셔티브 기간이 계획의 기간보다 짧은 경우 이니셔티브 막대를 계획의 타임라인에서 다른 위치에 끌어다 놓아 다른 시간대로 이동합니다.

   ![](assets/move-initiative-back-and-forth-on-the-timeline-350x71.png)

   >[!IMPORTANT]
   >
   >기간은 월 단위로만 선택할 수 있습니다. 처음부터 만드는 이니셔티브의 기간은 플랜 기간을 초과할 수 없습니다.

1. (선택 사항) **[!UICONTROL 월]** 드롭다운 메뉴에서 다음 옵션 중 하나를 선택하여 계획의 타임라인을 변경합니다.

   | 드롭다운 메뉴 옵션 | 설명 |
   |---|---|
   | [!UICONTROL 개월] | 월별 시간표를 표시합니다. 1년 계획의 기본 옵션입니다. |
   | [!UICONTROL 분기] | 분기별로 타임라인을 표시합니다. 이 옵션은 플랜의 [!UICONTROL 기간]이 3년 또는 5년인 경우에만 사용할 수 있습니다. 3년 계획의 기본 옵션입니다. |
   | [!UICONTROL 년] | 연도별로 타임라인을 표시합니다. 이 옵션은 플랜의 [!UICONTROL 기간]이 5년인 경우에만 사용할 수 있습니다. 5년 계획의 기본 옵션입니다. |


1. (선택 사항) 왼쪽에서 오른쪽으로 스크롤하여 이니셔티브의 전체 지속 시간을 확인합니다.
1. (선택 사항) 현재 날짜로 돌아가려면 **[!UICONTROL 오늘]** 표시줄을 클릭합니다.

   ![](assets/today-indicator-350x160.png)

   >[!TIP]
   >
   >플랜이 미래나 과거에 있고 현재 날짜를 포함하지 않는 경우 오늘 표시기가 표시되지 않습니다.

1. 이니셔티브의 막대를 클릭합니다. 오른쪽에 이니셔티브 세부 정보 패널이 열립니다.

   ![](assets/initiative-details-panel-multiple-months-350x626.png)

   다음 정보를 지정하거나 검토합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">이니셔티브 기간</td> 
      <td>이니셔티브 기간(단위: 월). </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">시작 및 종료 날짜</td> 
      <td>이니셔티브의 시작 및 종료 날짜.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">필수 작업 역할 섹션 </td> 
      <td> <p><strong>[!UICONTROL 작업 역할 입력 시작]</strong> 필드를 클릭하고 목록에서 역할을 선택하거나 <span>n 활성</span> 작업 역할의 이름을 입력하십시오. </p> <p><span>FTE를 사용하도록 계획을 설정했는지 또는 시간에 따라 </span> 이니셔티브의 각 달에 대해 FTE <span><span>또는 시간</span></span><span>에서 이 이니셔티브에 필요한 작업 역할의 수를 추가</span>합니다. <span>이니셔티브의 처음 3개월은 기본적으로 표시됩니다.</span></p> <p><span>이니셔티브에 대한 작업 역할 정보를 업데이트하면 플랜에 대한 필수 작업 역할 정보도 업데이트됩니다.</span> </p> <p>FTE 또는 시간을 사용하도록 계획을 설정하는 방법에 대한 자세한 내용은 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">[!DNL Scenario Planner]</a>에서 계획 만들기 및 편집을 참조하십시오. </p>
      <p><b>중요 사항</b></p>  
      <p>[!DNL Scenario Planner]의 모든 계산에 대해 [!DNL Workfront]은(는) 다음 값을 사용합니다. 1 FTE = 8시간. </p>

   <p><b>팁</b></p>

   <ul> 
       <li> <p><span>다음 달로 이동하려면 [!UICONTROL Tab] 키를 사용합니다.</span> </p> </li> 
      <li> <p> 이 필드를 클릭하면 시스템의 모든 <span>활성</span> 작업 역할이 나열됩니다. </p> </li> 
       <li> <p>플랜의 사용 가능한 작업 역할에 이미 추가된 작업 역할이 먼저 표시됩니다. 계획에 사용 가능한 작업 역할을 추가하는 방법에 대한 자세한 내용은 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">시나리오 플래너에서 계획 만들기 및 편집</a>을 참조하십시오. </p> </li> 
       <li> <p>[!DNL Workfront] 는 한 달에 160시간이 풀타임에 해당하는 것으로 간주합니다. </p> <p>시나리오 플래너의 모든 계산에 대해 Workfront은 다음 값을 사용합니다. 1 FTE = 8 시간. </p></li> 
      </ul> </p> <p>FTE <span>또는</span> <span>시간</span>에 대해 1FTE보다 낮은 숫자 또는 10진수를 입력할 수 있습니다. 예를 들어, 0.5 컨설턴트 작업 역할은 컨설턴트가 이 이니셔티브에 대한 작업에 자신의 FTE의 절반(일반적으로 4시간, 여기서 8시간은 1FTE)을 할애한다는 의미입니다. </p>  </td> 
     </tr> 
     <tr> 
      <td rowspan="3" role="rowheader">비용 섹션</td> 
      <td> <p>이니셔티브의 총 비용은 [!UICONTROL Costs] 섹션의 오른쪽에 표시됩니다. [!DNL Workfront]은(는) 다음 수식을 사용하여 이니셔티브의 비용을 계산합니다.</p> <p><code>[!UICONTROL Initiative Costs] = [!UICONTROL Fixed Costs] + [!UICONTROL People] Costs</code> </p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>[!UICONTROL 고정 비용]</strong> 필드에 이 이니셔티브를 완료하는 데 비용이 든다고 생각되는 항목의 대략적인 예상 금액을 수동으로 입력하십시오. 이니셔티브에 대해 예상되는 작업 역할과 관련된 비용은 포함되지 않아야 합니다.</p> <p><span>Tab 키를 사용할 때 한 달에서 다음 달로 이동하여 이니셔티브의 각 달의 금액을 입력합니다.</span> </p> </td> 
     </tr> 
     <tr> 
      <td> 
       <div> 
        <p>FTE를 사용하도록 계획을 설정했는지 또는 시간을 사용하도록 설정했는지에 따라 [!UICONTROL Workfront]에서는 다음 공식을 사용하여 [!UICONTROL 인력 비용]을 계산합니다.</p> 
        <ul> 
         <li> <p>FTE 사용 시: </p> <p><code>[!UICONTROL People Costs] = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>여기서 160은 한 달의 총 작업 시간 수입니다. </p> </li> 
         <li> <p style="font-weight: normal;">시간 사용 시: </p> <p style="font-weight: normal;"><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> <p style="font-weight: normal;">시간 또는 FTE를 사용하도록 계획을 설정하는 방법에 대한 자세한 내용은 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">시나리오 플래너에서 계획 만들기 및 편집</a>을 참조하십시오.</p> </li> 
        </ul> 
        <p>인력 원가는 환율 환경설정에서 선택한 기본 통화로 계산됩니다. 환율에 대한 자세한 내용은 <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">환율 설정</a>을 참조하십시오.</p> 
        <p>이니셔티브에 대한 비용 정보를 업데이트하면 플랜에 대한 [!UICONTROL Costs] 영역도 업데이트됩니다. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"> <p style="font-weight: normal;">이니셔티브에 필요한 작업 역할 및 비용 값을 정의하고 이니셔티브 기간을 수정하면 다음 시나리오 중 하나가 발생할 수 있습니다.</p> 
       <ul> 
        <li> <p style="font-weight: normal;">이니셔티브를 줄이면 [!DNL Workfront]은(는) 필요한 리소스 양과 플랜에서 제거된 시간과 관련된 비용을 제거합니다. 작업 역할은 계획에 남아 있지만 필수 FTE 또는 <span data-mc-edit-date="2021-04-19T13:46:01.5004065-04:00" data-mc-editor="alinawilson" data-mc-comment="drafted, yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-19T13:45:58.7938344-04:00">시간</span>이(가) 없습니다. 제도 및 예산에 사용할 수 있는 자원은 변경되지 않습니다.<br>플랜에 대한 정보를 업데이트하려면 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">[!DNL Scenario Planner]</a>에서 플랜 만들기 및 편집을 참조하십시오. </p> </li> 
        <li> <p style="font-weight: normal;">이니셔티브를 더 길게 만드는 경우 이니셔티브에 새로 추가된 달에 대한 작업 역할과 비용의 양을 지정해야 합니다. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Net Value] 섹션</td> 
      <td><strong>[!DNL Net Value]</strong> 섹션에서 <strong>[!UICONTROL 계획된 이익]</strong> 필드에 대략적인 예상 금액을 수동으로 입력합니다. 이것이 여러분이 이 계획을 달성하는 것의 이점은 다음과 같을 것이라고 믿는 것입니다. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >플랜에 대한 작업 역할 수 및 예산, 편집 중인 이니셔티브 및 그 위에 있는 모든 이니셔티브의 작업 역할 수 및 비용을 이미 정의했으며 그 금액이 플랜에 대해 지정한 금액을 모두 초과하는 경우 [!DNL Workfront]에서 이니셔티브를 완료할 수 있는 충분한 리소스가 부족한 것을 확인할 수 있습니다. [!DNL Workfront]이(가) 이 이니셔티브를 달성하려고 할 때 이를 충돌로 표시하고 빨간색 표시줄로 표시합니다. 충돌하는 이니셔티브를 따르는 모든 이니셔티브가 빨간색 배경에 표시됩니다. 리소스가 부족한 첫 번째 이니셔티브부터 일부 이니셔티브의 요구 사항을 조정해야 할 수 있습니다. 충돌하는 이니셔티브를 조정하는 방법에 대한 자세한 내용은 [이니셔티브 충돌 해결 [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)을 참조하십시오.

1. (선택 사항) 작업 역할의 이름을 마우스로 가리킨 다음 **[!UICONTROL 휴지통 아이콘]** ![](assets/delete.png)을(를) 클릭하여 이니셔티브에서 제거합니다.

1. (조건부) 이니셔티브를 변경한 경우 **[!UICONTROL 적용]**&#x200B;을 클릭합니다.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Add more steps here as you can do more in the Initiative box over time)
   </MadCap:conditionalText>
   -->

1. (조건부) 변경하지 않은 경우 이니셔티브 세부 정보 패널의 오른쪽 상단에 있는 **X** 아이콘을 클릭하여 닫습니다.
1. (선택 사항) 이니셔티브의 우선 순위를 업데이트합니다.

   이니셔티브 우선 순위에 대한 자세한 내용은 [시나리오 플래너에서 이니셔티브 우선 순위 업데이트](../scenario-planner/prioritize-initiatives.md)를 참조하십시오.

   >[!TIP]
   >
   >목록에 먼저 나열된 이니셔티브는 우선 순위가 더 높으며 목록에 더 낮게 나열된 이니셔티브보다 먼저 리소스를 가져옵니다.

1. **[!UICONTROL 플랜 저장]**&#x200B;을 클릭합니다.

   이제 이니셔티브가 플랜에 포함됩니다.

   계획에서 이니셔티브를 삭제하는 방법에 대한 자세한 내용은 [다음에서 이니셔티브 삭제 [!DNL Scenario Planner]](../scenario-planner/delete-initiatives.md)를 참조하십시오.
