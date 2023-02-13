---
product-previous: enterprise-scenario-planner
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 계획자에서 계획 시나리오를 생성하고 비교합니다.
description: 회사의 장기 전략을 계획할 때, 처음에 여러분이 가지고 있지 않거나 생각하지 않을 수 있는 많은 정보가 있습니다. 이해 관계자가 수락할 수 있는 최종 전략에 도달하려면 시간과 실험이 필요합니다. "what if" 분석을 수행하여 계획에 대한 여러 시나리오를 만드는 것은 잠재적인 상황을 정확하게 예측하고 평가하고 궁극적으로 가장 적합한 계획을 개발하는 데 도움이 될 수 있습니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: 9a79ef81-6271-4cc9-b701-3ba0aeafb324
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 1%

---

# 에서 계획 시나리오를 만들고 비교합니다. [!DNL Scenario Planner]

회사의 장기 전략을 계획할 때, 처음에 여러분이 가지고 있지 않거나 생각하지 않을 수 있는 많은 정보가 있습니다. 이해 관계자가 수락할 수 있는 최종 전략에 도달하려면 시간과 실험이 필요합니다. &quot;what if&quot; 분석을 수행하여 계획에 대한 여러 시나리오를 만드는 것은 잠재적인 상황을 정확하게 예측하고 평가하고 궁극적으로 가장 적합한 계획을 개발하는 데 도움이 될 수 있습니다.

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
   <td> <p>에 대한 액세스 이상의 편집 [!DNL Scenario Planner]</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>개체 권한</strong> </p> </td> 
   <td> <p>계획에 대한 [!UICONTROL Manage] 권한</p> <p>계획에 대한 추가 액세스 요청에 대한 내용은 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">에서 계획에 대한 액세스 요청 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 시나리오 만들기

시나리오는 계획의 복사본입니다. 필요한 만큼 시나리오를 만들 수 있습니다. 그러나 시나리오를 쉽게 비교할 수 있도록 시나리오 수를 최소한으로 유지하는 것이 좋습니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png)를 클릭한 다음 [!UICONTROL 시나리오].

1. 계획을 만듭니다.

   계획 생성에 대한 자세한 내용은 [에서 계획 생성 및 편집 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   사용자가 생성한 첫 번째 계획은 자동으로 &quot;[!UICONTROL 초기 시나리오].&quot;

1. 기존 시나리오 옆에 있는 아래쪽 방향 화살표를 클릭한 다음 **[!UICONTROL 복사]** 아이콘.

   ![](assets/copy-scenarios-ui-and-highlighted-icon-350x95.png)

   이렇게 하면 복사한 시나리오와 동일한 정보로 새 시나리오가 생성됩니다. 자동으로 &quot; 이름이 지정됩니다.[!UICONTROL 시나리오 2]&quot; 두 번째 시나리오의 경우, &quot;[!UICONTROL 시나리오 3]세 번째라면, 시나리오 이름은 변경할 수 없습니다.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:this might change)
   </MadCap:conditionalText>
   -->

1. 다음 방법 중 하나로 새 시나리오를 업데이트합니다.

   * 이니셔티브 생성, 업데이트 또는 삭제

      >[!TIP]
      >
      >시나리오에서 이니셔티브를 삭제하면 선택한 시나리오에서만 제거되고 모든 시나리오에서 제거되지는 않습니다.

      이니셔티브 만들기에 대한 내용은 [에서 이니셔티브 만들기 및 편집 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   * 이니셔티브의 우선순위 업데이트
   * 사람 또는 예산 정보 조정
   * 시나리오에서 이니셔티브 충돌 검토 및 조정

      충돌 해결에 대한 자세한 내용은 [에서 이니셔티브 충돌 해결 [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. 클릭 **[!UICONTROL 계획 저장]** 변경 사항을 저장하려면 을 클릭합니다.

## 시나리오 비교

시나리오를 만든 후 이를 비교하여 조직에 가장 적합한 시나리오를 찾을 수 있습니다.

1. 시나리오를 비교할 계획으로 이동합니다.
1. 클릭 **[!UICONTROL 시나리오 비교]**. 시나리오 비교 페이지가 표시됩니다.

   계획에 대한 모든 기존 시나리오는 나란히 카드 형식으로 표시됩니다. 초기 시나리오가 항상 먼저 나열되며 정적입니다.

   ![](assets/scenario-cards-overlapping-350x166.png)

1. (선택 사항) 오른쪽으로 스크롤하여 모든 시나리오 카드를 볼 수 있습니다.

   시나리오 카드에 다음 정보가 표시됩니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>시나리오 이름</td> 
      <td> <p>Workfront에 의해 자동으로 생성된 이름은 편집할 수 없습니다. 예를 들어 "[!UICONTROL Initial Scenario]", "[!UICONTROL Scenario 2]" 등이 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td>시나리오 설명</td> 
      <td>시나리오에 대한 세부 사항을 설명할 수 있는 수동 항목입니다. </td> 
     </tr> 
     <tr> 
      <td>사용 가능한 작업 역할</td> 
      <td>계획 기간 동안 계획의 예산에서 사용할 수 있는 Job 역할 수. </td> 
     </tr> 
     <tr> 
      <td>필수 작업 역할</td> 
      <td>이니셔티브에 따라 필요한 작업 역할 수입니다. </td> 
     </tr> 
     <tr> 
      <td>예산</td> 
      <td>이 시나리오에서 계획에 대해 정의된 총 예산. 계획에 대한 예산 정보는 <a href="../scenario-planner/plans-overview.md" class="MCXref xref">의 계획 개요 [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>비용</td> 
      <td>시나리오의 이니셔티브와 관련된 비용입니다. 비용에 대한 자세한 내용은 <a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">의 이니셔티브 개요 [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>활용성</td> 
      <td>이 시나리오에서 계획에 대한 [!UICONTROL Budget Utilization] 백분율입니다. [!UICONTROL Budget Utilization] 백분율에 대한 내용은 <a href="../scenario-planner/plans-overview.md" class="MCXref xref">의 계획 개요 [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>순 가치</td> 
      <td>이 시나리오에서 계획의 [!UICONTROL Net Value]. 계획의 [!UICONTROL Net Value]에 대한 자세한 내용은 다음을 참조하십시오 <a href="../scenario-planner/plans-overview.md" class="MCXref xref">의 계획 개요 [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>이니셔티브</td> 
      <td>이 시나리오에서 계획에 대한 이니셔티브 수입니다.</td> 
     </tr> 
     <tr> 
      <td>충돌</td> 
      <td>이 시나리오에 대한 계획에서 모든 유형의 충돌을 표시하는 이니셔티브 수입니다. 이니셔티브 충돌에 대한 자세한 내용은 <a href="../scenario-planner/resolve-conflicts-in-sp.md" class="MCXref xref">에서 이니셔티브 충돌 해결 [!DNL Scenario Planner]</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >초기 시나리오와 추가 시나리오 간에 정보가 다르면 초기 시나리오와 비교하여 해당 값의 증가 또는 감소를 나타내도록 변경된 값 옆에 위쪽 또는 아래쪽 화살표가 표시됩니다.
   >
   >
   >![](assets/arrows-on-scenario-cards-highlighted-350x70.png)
   >
   >예를 들어 예산, Job 역할 수, 이니셔티브 수가 한 시나리오에서 다른 시나리오로 변경될 수 있습니다.

1. 시나리오 이름을 클릭하여 액세스하고 변경합니다.

   자세한 내용은 [시나리오 만들기](#create-scenarios) 섹션에 자세히 설명되어 있습니다.

1. 클릭 **[!UICONTROL 설명 추가]** 시나리오에 대한 설명을 추가하려면

   또는

   설명 필드를 클릭하여 업데이트한 다음 화면의 아무 곳이나 클릭하여 변경 내용을 저장합니다.

1. (선택 사항) **[!UICONTROL 자세히]** 메뉴 ![](assets/more-icon.png) to **[!UICONTROL 복사]** 또는 **[!UICONTROL 삭제]** 시나리오를 참조하십시오.

   ![](assets/copy-or-delete-scenario-links-from-card-350x109.png)

   시나리오를 복사하면 카드 페이지에 자동으로 표시되며, 이 패턴에 따라 이름이 변경됩니다. &quot;[!UICONTROL 시나리오] `<next number in order>`.&quot;

1. (조건부) **[!UICONTROL 삭제]**&#x200B;를 클릭합니다. **[!UICONTROL 예, 삭제합니다]** 확인합니다.

   삭제된 시나리오를 복구할 수 없습니다.

   시나리오 삭제에 대한 자세한 내용은 [에서 계획 삭제 [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

1. 클릭 **[!UICONTROL 계획 저장]** 시나리오 및 계획을 저장합니다.
