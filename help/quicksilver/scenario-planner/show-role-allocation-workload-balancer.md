---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 업무 균형자에서 프로젝트 및 이니셔티브에 대한 역할 할당 표시
description: 프로젝트 및 이니셔티브를 연결한 후 리소스 할당을 나란히 관리하여 프로젝트 및 이니셔티브가 제대로 작동하는지 확인할 수 있습니다
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 0%

---

# [!UICONTROL 업무 균형자]에서 프로젝트 및 이니셔티브에 대한 역할 할당 표시

<!--Audited: 07/2024-->

프로젝트와 이니셔티브를 연결한 후 리소스 할당을 나란히 관리하여 프로젝트 및 이니셔티브가 일치하는지 확인할 수 있습니다. 이를 통해 이를 과다 할당하거나 과소 활용하는 것을 방지할 수 있습니다.

이 문서에서는 프로젝트의 [!UICONTROL 업무 균형자]에서 [!UICONTROL 역할 할당] 패널을 사용하여 리소스를 조정하는 방법에 대해 설명합니다.

필수 구성 요소를 포함하여 프로젝트와 이니셔티브 간의 리소스 조정에 대한 일반적인 정보는 [프로젝트와 이니셔티브 간의 리소스 할당 조정에 대한 개요](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 플랜*</p> </td> 
   <td> <p>현재: [!UICONTROL Business] 이상</p>
   <p>새로운 기능: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 라이센스*</p> </td> 
   <td> <p>새로운 기능: 밝게 또는 높음</p> 
   <p>현재: [!UICONTROL Review] 이상</p> </td> 
  </tr> 
  <tr> 
   <td>제품* </td> 
   <td> 
   <p>현재 Workfront 플랜의 경우: </p>
   <p>이 문서에 설명된 기능에 액세스하려면 [!DNL Adobe Workfront Scenario Planner]에 대한 추가 라이선스를 구입해야 합니다.</p> <p>[!DNL Workfront Scenario Planner]에 대한 액세스 및 사용 권한에 대한 자세한 내용은 [!DNL Scenario Planner]</a>을(를) 사용하는 데 필요한 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">액세스를 참조하십시오. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>액세스 수준 </td> 
   <td> <p>[!UICONTROL Projects]에 대한 [!UICONTROL 보기] 이상 액세스</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>개체 권한 </p> </td> 
   <td> <p>프로젝트에 대한 [!UICONTROL 보기] 권한</p> </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서에 대한 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## [!UICONTROL 업무 균형자]에서 프로젝트 및 이니셔티브에 대한 역할 할당 표시

회사에서 [!DNL Workfront Scenario Planner] 라이선스를 구입한 경우 프로젝트 수준 [!UICONTROL 업무 균형자]에서 이니셔티브와 이에 연결된 프로젝트 간의 리소스 할당을 조정할 수 있습니다.

1. (조건부) 다음 문서에 설명된 방법 중 하나를 사용하여 프로젝트와 이니셔티브를 연결합니다.

   * [프로젝트를  [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md)의 플랜으로 가져옵니다.
   * [ [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md)에서 이니셔티브를 게시하여 프로젝트를 업데이트하거나 만듭니다.

   >[!IMPORTANT]
   >
   >이니셔티브의 리소스를 변경하는 경우 이니셔티브의 최신 리소스 정보를 프로젝트에서 업데이트하려면 이니셔티브가 속한 시나리오를 다시 게시해야 합니다.

1. 프로젝트 및 연계된 이니셔티브에 대한 작업 역할 할당을 검토하려는 프로젝트로 이동합니다.
1. 왼쪽 패널에서 [!UICONTROL 업무 균형자]를 클릭합니다.

   **[!UICONTROL 예약]**&#x200B;을 클릭한 다음 **[!UICONTROL 업무 균형자로 전환]**&#x200B;을 클릭해야 할 수 있습니다.

1. 다음 중 하나를 수행하십시오.

   * 월별 업무 균형자를 보려면 **[!UICONTROL 월]**&#x200B;을(를) 클릭하고 타임라인에서 한 달 옆에 있는 드롭다운 메뉴를 클릭한 다음 ![](assets/drop-down-next-to-month-month-view-wb.png)자세히&#x200B;]**를 클릭합니다.**[!UICONTROL 
   * 도구 모음의 오른쪽 상단에 있는 **[!UICONTROL 역할 할당 표시]** 아이콘 ![](assets/show-role-allocation-icon.png)을(를) 클릭합니다.

   [!UICONTROL 역할 할당] 패널이 표시됩니다.

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >조직에서 [!DNL Workfront Scenario Planner] 라이선스를 구매하지 않았더라도 [!UICONTROL 역할 할당] 패널을 볼 수 있지만 이니셔티브의 작업 역할에 대한 정보는 볼 수 없습니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. 역할 할당 패널의 **[!UICONTROL 프로젝트 합계]** 영역에서 다음 정보를 검토하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 작업 역할]</td> 
      <td> <p>다음 중 하나와 연관된 작업 역할의 이름:</p> 
       <ul> 
        <li> <p>프로젝트의 작업</p> </li> 
        <li> <p>프로젝트의 문제</p> </li> 
        <li> <p>프로젝트에 연결된 이니셔티브</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 이니셔티브 시간]</td> 
      <td>이니셔티브의 총 기간 동안 이니셔티브의 각 작업 역할과 연관된 필수 시간 수입니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 계획된 시간]</td> 
      <td>총 프로젝트 기간 동안 프로젝트의 작업 또는 문제에서 각 작업 역할과 연관된 계획된 시간 수입니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Variance]</td> 
      <td> <p>이니셔티브에 필요한 시간과 프로젝트의 작업과 연결된 계획된 시간 사이의 차이입니다. [!DNL Workfront]은(는) 다음 공식을 사용하여 [!UICONTROL Variance]를 계산합니다.</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>이니셔티브에 필요한 시간보다 많은 시간을 리소스를 계획하면 [!UICONTROL 차이]가 음수이고 빨간색으로 표시됩니다. 이는 리소스가 초과 할당되었음을 의미합니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >프로젝트의 계획된 시간은 다음 시나리오에 표시되지 않습니다.
   >
   >   
   >   
   >   * 작업 또는 문제가 작업 역할 또는 작업 역할과 연관된 사용자에게 할당되지 않은 경우.
   >   * 작업 또는 문제에 [!UICONTROL 기간]이 0인 경우.
   >   
   >

1. (선택 사항) [!UICONTROL Variance] 열에 리소스가 초과 할당된 것으로 표시되면 다음 중 하나를 조정하십시오.

   * 초과 할당되거나 작업에 더 많은 리소스를 추가하는 작업 역할 하나에 대해 계획된 시간 수를 줄이고 새 리소스에 더 많은 계획된 시간을 분배합니다. 작업 또는 문제를 편집할 때 할당 또는 계획된 시간을 업데이트할 수 있습니다. 자세한 내용은 다음 문서를 참조하십시오.

      * [작업 편집](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [문제 편집](../manage-work/issues/manage-issues/edit-issues.md)

     >[!NOTE]
     >
     >작업 및 문제를 편집하려면 추가 액세스 및 권한이 있어야 합니다.

   * 이니셔티브에 대한 초과 할당을 표시하는 역할에 필요한 시간 수를 늘립니다. 자세한 내용은 [이니셔티브 만들기 및 편집 [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md)을 참조하세요.

     >[!NOTE]
     >
     >계획을 편집하려면 추가 액세스 및 권한이 있어야 합니다.

1. (선택 사항) 드롭다운 아이콘을 클릭하여 [!UICONTROL 역할 할당] 패널 또는 [!UICONTROL 업무 균형자]의 타임라인에서 월 중 하나를 확장합니다.

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   [!UICONTROL 프로젝트 총계] 영역에 표시되는 같은 유형의 정보도 각 달에 표시됩니다.

   >[!TIP]
   >
   >[!UICONTROL 역할 할당] 패널에 나열된 월은 [!UICONTROL 업무 균형자]의 화면에 표시되는 타임라인의 월입니다. 타임라인에서 앞뒤로 스크롤하여 추가 월을 봅니다.

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->


