---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 플래너에서 이니셔티브 생성 및 편집
description: Adobe Workfront 시나리오 계획자를 사용할 때 생성했거나 사용자와 공유된 계획에서 이니셔티브를 생성할 수 있습니다. 이니셔티브를 작성하면 계획 완료에 기여하는 조직의 수가 얼마나 작은지를 표시할 수 있습니다. 예를 들어, 조직에서 다음 3년 동안 새로운 시장으로 확장하기 위한 계획을 가지고 있는 경우, 이 계획 내에서 각 부서에 대한 이니셔티브를 생성하여 이 계획을 달성하기 위한 인력 및 예산에 대한 각 부서의 필요성을 예측할 수 있습니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: a811bad0-d3c0-4cba-8b78-d9a14ffc8482
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '1635'
ht-degree: 0%

---

# 에서 이니셔티브 만들기 및 편집 [!DNL Scenario Planner]

를 사용할 때 [!UICONTROL Adobe Workfront 시나리오 플래너]를 생성할 계획이나 사용자와 공유된 계획에서 이니셔티브를 생성할 수 있습니다. 이니셔티브를 작성하면 계획 완료에 기여하는 조직의 수가 얼마나 작은지를 표시할 수 있습니다. 예를 들어, 조직에서 다음 3년 동안 새로운 시장으로 확장하기 위한 계획을 가지고 있는 경우, 이 계획 내에서 각 부서에 대한 이니셔티브를 생성하여 이 계획을 달성하기 위한 인력 및 예산에 대한 각 부서의 필요성을 예측할 수 있습니다.

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
   <td> <p>에 대한 추가 라이센스를 구입해야 합니다. [!DNL Adobe Workfront Scenario Planner] 을 눌러 이 문서에 설명된 기능에 액세스합니다. </p> <p>를 가져오는 방법에 대한 자세한 내용은 [!DNL Workfront Scenario Planner]를 참조하십시오. <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">을 사용하는 데 필요한 액세스 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>액세스 수준 구성* </td> 
   <td> <p>[!UICONTROL Edit] 액세스 이상의 [!DNL Scenario Planner]</p> <p>여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 변경할 수 있습니다. <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>개체 권한 </p> </td> 
   <td> <p>계획에 대한 [!UICONTROL Manage] 권한</p> <p>계획에 대한 추가 액세스 요청에 대한 내용은 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">에서 계획에 대한 액세스 요청 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*어떤 플랜, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 전제 조건

계획을 생성해야 합니다. 그렇지 않으면 다른 사용자가 계획을 공유해야 해당 계획 내에서 이니셔티브를 생성할 수 있습니다. 계획 생성에 대한 자세한 내용은 [에서 계획 생성 및 편집 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

이니셔티브에 대한 자세한 내용은 [의 이니셔티브 개요 [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md).

## 이니셔티브 만들기

다음과 같은 방법으로 이니셔티브를 생성할 수 있습니다.

* 처음부터
* 프로젝트로 가져오기

   계획에서 프로젝트로 가져오는 방법에 대한 자세한 내용은 [계획 로 프로젝트 가져오기 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* 기존 이니셔티브를 복사하여

   이니셔티브 복사에 대한 자세한 내용은 [에서 이니셔티브 복사 [!DNL Scenario Planner]](../scenario-planner/copy-initiatives.md).

처음부터 이니셔티브를 생성하려면

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png)를 클릭한 다음 [!UICONTROL 시나리오].

1. 이니셔티브를 생성할 계획명을 누릅니다.
1. 을(를) 클릭합니다. **+ 아이콘** 의 왼쪽에 **[!UICONTROL 새로운 이니셔티브]**

   또는

   을(를) 클릭합니다. **[!UICONTROL 새로운 이니셔티브]** 드롭다운 메뉴를 선택하고 **[!UICONTROL 새로운 이니셔티브]** 또는 **[!UICONTROL 프로젝트 가져오기].**

1. 이니셔티브의 이름을 **[!UICONTROL 제목 없는 이니셔티브]** 필드를 클릭한 다음 Enter 키를 누르거나 페이지의 다른 위치를 클릭합니다.

   이니셔티브가 계획의 타임라인에 파란색 막대로 표시됩니다. 기본적으로 이니셔티브 기간은 1개월이며 항상 계획의 첫 번째 달에 시작됩니다.

1. (선택 사항) 왼쪽 패널과 타임라인 사이에 분리 막대를 드래그하여 왼쪽 패널의 크기를 조정합니다.

1. (선택 사항) 이니셔티브 막대의 끝을 드래그하여 기간을 1개월 이상으로 연장하고 이니셔티브 종료 월을 원하는 위치에 놓습니다.
1. (선택 사항 및 조건부) 이니셔티브 기간이 계획의 기간보다 짧은 경우, 이니셔티브 막대를 계획의 타임라인에서 다른 위치로 드래그하여 놓으면 다른 시간대로 이동합니다.

   ![](assets/move-initiative-back-and-forth-on-the-timeline-350x71.png)

   >[!IMPORTANT]
   >
   >기간은 월 단위만 선택할 수 있습니다. 처음부터 생성하는 이니셔티브의 기간은 계획 기간을 초과할 수 없습니다.

1. (선택 사항) **[!UICONTROL 월]** 드롭다운 메뉴에서 다음 옵션 중 하나를 선택하여 계획의 타임라인을 변경합니다.

   | 드롭다운 메뉴 옵션 | 설명 |
   |---|---|
   | [!UICONTROL 월] | 월별로 타임라인을 표시합니다. 1년 계획의 기본 옵션입니다. |
   | [!UICONTROL 분기] | 분기별로 타임라인을 표시합니다. 이 옵션은 [!UICONTROL 기간] 그 계획은 3~5년입니다. 3년 계획의 기본 옵션입니다. |
   | [!UICONTROL 년] | 연도별 타임라인을 표시합니다. 이 옵션은 [!UICONTROL 기간] 그 계획은 5년이다. 5년 계획의 기본 옵션입니다. |


1. (선택 사항) 이니셔티브의 전체 기간을 보려면 왼쪽에서 오른쪽으로 스크롤합니다.
1. (선택 사항) **[!UICONTROL 오늘]** 현재 날짜로 돌아올 지표 라인.

   ![](assets/today-indicator-350x160.png)

   >[!TIP]
   >
   >계획이 미래 또는 과거에 있고 현재 날짜를 포함하지 않는 경우 오늘 지표가 표시되지 않습니다.

1. 이니셔티브 막대를 클릭합니다. 이니셔티브 세부 정보 패널이 오른쪽에 열립니다.

   ![](assets/initiative-details-panel-multiple-months-350x626.png)

   다음 정보를 지정하거나 검토하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">이니셔티브 기간</td> 
      <td>이니셔티브의 기간(개월)입니다. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">시작 및 종료 날짜</td> 
      <td>이니셔티브 시작 및 종료 날짜입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">필수 작업 역할 섹션 </td> 
      <td> <p>을(를) 클릭합니다. <strong>[!UICONTROL 작업 역할 입력 시작]</strong> 필드를 선택하고 목록에서 역할을 선택하거나 이름을 입력합니다<span>비활성</span> 직무 역할입니다. </p> <p><span>FTE를 사용하도록 계획을 설정했는지 또는 시간에 따라</span> FTE에서 이 이니셔티브에 필요한 작업 역할 수 추가 <span><span>또는 시간</span></span><span> 이니셔티브의 매월</span>. <span>이니셔티브의 처음 3개월이 기본적으로 표시됩니다.</span></p> <p><span>이니셔티브에 대한 작업 역할 정보를 갱신하면 계획에 대한 필수 작업 역할 정보도 갱신됩니다.</span> </p> <p>FTE 또는 시간 사용 계획 설정에 대한 자세한 내용은 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">에서 계획 생성 및 편집 [!DNL Scenario Planner]</a>. </p>
      <p><b>중요 사항</b></p>  
      <p>의 모든 계산에 대해 [!DNL Scenario Planner], [!DNL Workfront] 는 다음 값을 사용합니다. 1 FTE = 8시간 </p>

   <p><b>팁</b></p>

   <ul> 
       <li> <p><span>다음 달로 이동하려면 [!UICONTROL Tab] 키를 사용합니다.</span> </p> </li> 
      <li> <p> 모두 <span>활성</span> 이 필드를 클릭하면 시스템의 작업 역할이 나열됩니다. </p> </li> 
       <li> <p>계획의 사용 가능한 작업 역할에 이미 추가된 작업 역할이 먼저 표시됩니다. 계획에 사용 가능한 작업 역할 추가에 대한 자세한 내용은 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">시나리오 계획자에서 계획 생성 및 편집</a>. </p> </li> 
       <li> <p>[!DNL Workfront] 한 달에 160시간 정도의 시간으로 간주합니다. </p> <p>시나리오 플래너의 모든 계산에 대해 Workfront은 다음 값을 사용합니다. 1 FTE = 8시간 </p></li> 
      </ul> </p> <p>FTE에 대해 1 FTE 또는 소수점 이하 숫자를 입력할 수 있습니다 <span>또는</span> <span>시간</span>. 예를 들어 0.5 컨설턴트 작업 역할은 컨설턴트가 FTE의 절반인 4시간(일반적으로 8시간이 FTE인 경우 1시간)을 이 이니셔티브 작업에 투입한다는 것을 의미합니다. </p>  </td> 
     </tr> 
     <tr> 
      <td rowspan="3" role="rowheader">비용 섹션</td> 
      <td> <p>이니셔티브의 총 비용이 [!UICONTROL Cost] 섹션의 오른쪽에 표시됩니다. [!DNL Workfront] 다음 공식을 사용하여 이니셔티브 비용을 계산합니다.</p> <p><code>[!UICONTROL Initiative Costs] = [!UICONTROL Fixed Costs] + [!UICONTROL People] Costs</code> </p> </td> 
     </tr> 
     <tr> 
      <td> <p>에서 <strong>[!UICONTROL 고정 비용]</strong> 필드에서 이 이니셔티브를 완료하는 데 소요되는 비용의 대략적인 예상 금액을 수동으로 입력합니다. 여기에는 이니셔티브에 대해 예상되는 작업 역할과 연관된 비용이 포함되지 않아야 합니다.</p> <p><span>Tab 키를 사용할 때 한 달에서 다음 달로 이동하여 이니셔티브의 각 달에 대한 금액을 입력합니다.</span> </p> </td> 
     </tr> 
     <tr> 
      <td> 
       <div> 
        <p>[!UICONTROL Workfront]은 FTE를 사용하도록 계획이 설정되어 있는지 아니면 시간을 사용하도록 설정되어 있는지에 따라 다음 공식을 사용하여 [!UICONTROL People Cost]를 계산합니다.</p> 
        <ul> 
         <li> <p>FTE 사용 시: </p> <p><code>[!UICONTROL People Costs] = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>여기서 160은 한 달에 발생한 총 근무 시간 수입니다. </p> </li> 
         <li> <p style="font-weight: normal;">시간 사용 시: </p> <p style="font-weight: normal;"><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> <p style="font-weight: normal;">시간 또는 FTE를 사용하도록 계획을 설정하는 방법에 대한 자세한 내용은 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">시나리오 계획자에서 계획 생성 및 편집</a>.</p> </li> 
        </ul> 
        <p>인력 원가는 환율 기본 설정에서 선택한 기본 통화로 계산됩니다. 환율에 대한 자세한 내용은 <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">환율 설정</a>.</p> 
        <p>이니셔티브에 대한 비용 정보를 업데이트하면 계획에 대한 [!UICONTROL 비용] 영역도 업데이트됩니다. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"> <p style="font-weight: normal;">이니셔티브에 필요한 작업 역할 및 비용 값을 정의하고 이니셔티브 기간을 수정한 후 다음과 같은 시나리오가 발생할 수 있습니다.</p> 
       <ul> 
        <li> <p style="font-weight: normal;">이 계획을 앞당긴다면, [!DNL Workfront] 계획에서 제거된 시간과 관련된 필수 자원 및 비용을 제거합니다. 작업 역할은 계획에 남아 있지만 필수 FTE 또는 <span data-mc-edit-date="2021-04-19T13:46:01.5004065-04:00" data-mc-editor="alinawilson" data-mc-comment="drafted, yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-19T13:45:58.7938344-04:00">시간</span>. 계획 및 예산에 대한 가용 자원은 변경되지 않은 상태로 유지됩니다.<br>계획에 대한 정보를 갱신하려면 다음을 참조하십시오. <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">에서 계획 생성 및 편집 [!DNL Scenario Planner]</a>. </p> </li> 
        <li> <p style="font-weight: normal;">이니셔티브를 더 길게 하는 경우 이니셔티브에 새로 추가된 달에 대한 직무 역할과 비용의 양을 지정해야 합니다. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Net Value] 섹션</td> 
      <td>에서 <strong>[!DNL Net Value]</strong> 섹션에서, <strong>[!UICONTROL Planning Benefits]</strong> 필드. 이 계획을 달성함으로써 얻을 수 있는 이점은 다음과 같습니다. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >계획에 대한 Job 역할 수 및 예산, 편집 중인 Job 역할 수 및 이니셔티브 비용 및 그 위의 모든 이니셔티브 중 하나를 이미 정의한 경우, 모두 계획에 대해 지정한 금액을 초과하는 경우, [!DNL Workfront] 이니셔티브를 마칠 충분한 리소스가 없다는 것을 알 수 있습니다. [!DNL Workfront] 이 이니셔티브를 달성하려고 할 때 이것을 분쟁으로 표시하고 빨간색 막대로 표시합니다. 혼조된 이니셔티브를 따르는 모든 이니셔티브는 적색 배경으로 표시됩니다. 자원이 부족한 첫 번째 태그로 시작하여 이니셔티브의 필요성의 일부를 조정해야 할 수도 있습니다. 충돌하는 이니셔티브를 조정하는 방법에 대한 자세한 내용은 [에서 이니셔티브 충돌 해결 [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. (선택 사항) 작업 롤의 이름을 마우스로 가리킨 다음, **[!UICONTROL 휴지통 아이콘]** ![](assets/delete.png) 솔루션에서 제거할 수 있습니다.

1. (조건부) 이니셔티브를 변경한 경우 **[!UICONTROL 적용]**.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Add more steps here as you can do more in the Initiative box over time)
   </MadCap:conditionalText>
   -->

1. (조건부) 변경하지 않은 경우 **X** [이니셔티브 세부 정보] 패널의 오른쪽 위에 있는 아이콘을 클릭하여 닫습니다.
1. (선택 사항) 이니셔티브의 우선순위를 업데이트합니다.

   이니셔티브 우선 순위에 대한 자세한 내용은 [시나리오 플래너에서 이니셔티브 우선순위 업데이트](../scenario-planner/prioritize-initiatives.md).

   >[!TIP]
   >
   >목록에서 먼저 나열된 이니셔티브는 우선순위가 더 높고 목록에서 아래에 나열된 이니셔티브 전에 리소스를 가져옵니다.

1. 클릭 **[!UICONTROL 계획 저장]**.

   그 계획은 이제 너의 계획에 포함되어 있다.

   계획에서 이니셔티브 삭제에 대한 자세한 내용은 [에서 이니셔티브 삭제 [!DNL Scenario Planner]](../scenario-planner/delete-initiatives.md).
