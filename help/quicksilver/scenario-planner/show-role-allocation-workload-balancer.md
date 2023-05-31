---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 업무 균형자에서 프로젝트 및 이니셔티브에 대한 역할 할당 표시
description: 프로젝트 및 이니셔티브를 연결한 후 리소스 할당을 나란히 관리하여 프로젝트 및 이니셔티브가 제대로 작동하는지 확인할 수 있습니다
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 0%

---

# 에서 프로젝트 및 이니셔티브에 대한 역할 할당 표시 [!UICONTROL 업무 균형자]

>[!IMPORTANT]
>
>조직은 다음에 대한 추가 라이선스를 구입해야 합니다. [!DNL Adobe Workfront Scenario Planner] 프로젝트에 대한 이니셔티브 정보를 볼 수 있습니다. 를 가져오는 방법에 대한 자세한 내용은 [!DNL Workfront Scenario Planner], 참조 [를 사용하기 위해 필요한 액세스 권한 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

프로젝트와 이니셔티브를 연결한 후 리소스 할당을 나란히 관리하여 프로젝트 및 이니셔티브가 일치하는지 확인할 수 있습니다. 이를 통해 이를 과다 할당하거나 과소 활용하는 것을 방지할 수 있습니다.

이 문서에서는 다음을 사용하여 리소스를 조정하는 방법을 설명합니다. [!UICONTROL 역할 할당] 패널 위치 [!UICONTROL 업무 균형자] 프로젝트.

전제 조건을 포함하여 프로젝트와 이니셔티브 간의 리소스 조정에 대한 일반 정보는 다음을 참조하십시오. [프로젝트와 이니셔티브 간 리소스 할당 조정 개요](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## 액세스 요구 사항

다음을 수행해야 합니다.

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
   <td> <p>다음에 대한 추가 라이선스를 구입해야 합니다. [!DNL Adobe Workfront Scenario Planner] 이 문서에 설명된 기능에 액세스합니다.</p> <p>를 가져오는 방법에 대한 자세한 내용은 [!DNL Workfront Scenario Planner], 참조 <a href="../scenario-planner/access-needed-to-use-sp.md">를 사용하기 위해 필요한 액세스 권한 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>액세스 수준 구성*</strong> </td> 
   <td> <p>프로젝트에 대한 [!UICONTROL 보기] 이상 액세스 </p> <p>참고: 여전히 액세스 권한이 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에 추가 제한을 설정하는 경우. 자세한 내용: [!DNL Workfront] 관리자가 액세스 수준을 변경할 수 있습니다. 다음을 참조하십시오. <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>개체 권한</strong> </p> </td> 
   <td> <p>프로젝트에 대한 [!UICONTROL 보기] 이상 권한</p> <p>계획에 대한 추가 액세스 요청에 대한 자세한 내용은 다음을 참조하십시오. <a href="../scenario-planner/request-access-to-plan.md">의 플랜에 대한 [!UICONTROL Request] 액세스 [!DNL Workfront Scenario Planner]</a>.</p> <p>프로젝트에 대한 추가 액세스 요청에 대한 자세한 내용은 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

## 에서 프로젝트 및 이니셔티브에 대한 역할 할당 표시 [!UICONTROL 업무 균형자]

회사가 을(를) 구입한 경우 [!DNL Workfront Scenario Planner] 라이선스, 프로젝트 수준에서 이니셔티브와 이에 연결된 프로젝트 간의 리소스 할당을 조정할 수 있습니다. [!UICONTROL 업무 균형자].

1. (조건부) 다음 문서에 설명된 방법 중 하나를 사용하여 프로젝트와 이니셔티브를 연결합니다.

   * [플랜에 프로젝트 가져오기 [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [에서 이니셔티브를 게시하여 프로젝트 업데이트 또는 만들기 [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md).

   >[!IMPORTANT]
   >
   >이니셔티브의 리소스를 변경하는 경우 이니셔티브의 최신 리소스 정보를 프로젝트에서 업데이트하려면 이니셔티브가 속한 시나리오를 다시 게시해야 합니다.

1. 프로젝트 및 연계된 이니셔티브에 대한 작업 역할 할당을 검토하려는 프로젝트로 이동합니다.
1. 클릭 [!UICONTROL 업무 균형자] 왼쪽 패널에서

   다음을 클릭해야 할 수 있습니다. **[!UICONTROL 예약]**, 그런 다음 **[!UICONTROL 업무 균형자로 전환]**.

1. 다음 중 하나를 수행하십시오.

   * 클릭 **[!UICONTROL 월]** 월별 업무 균형자 를 보려면 타임라인에서 한 달 옆에 있는 드롭다운 메뉴를 누릅니다 ![](assets/drop-down-next-to-month-month-view-wb.png)을 클릭한 다음 을 클릭합니다 **[!UICONTROL 자세히]**.
   * 다음을 클릭합니다. **[!UICONTROL 역할 할당 표시]** 아이콘 ![](assets/show-role-allocation-icon.png) 을 클릭합니다.

   다음 [!UICONTROL 역할 할당] 패널이 표시됩니다.

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >를 볼 수 있지만 [!UICONTROL 역할 할당] 조직에서 구매하지 않은 경우에도 패널 [!DNL Workfront Scenario Planner] 라이선스, 이니셔티브의 작업 역할에 대한 정보를 볼 수 없습니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. 에서 다음 정보를 검토하십시오. **[!UICONTROL 프로젝트 합계]** 역할 할당 패널의 영역:

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
      <td> <p>이니셔티브에 필요한 시간과 프로젝트의 작업과 연결된 계획된 시간 사이의 차이입니다. [!DNL Workfront] 다음 공식을 사용하여 [!UICONTROL 차이]를 계산합니다.</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>이니셔티브에 필요한 시간보다 많은 시간을 리소스를 계획하면 [!UICONTROL 차이]가 음수이고 빨간색으로 표시됩니다. 이는 리소스가 초과 할당되었음을 의미합니다. </p> </td> 
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
   >   * 작업 또는 문제에 [!UICONTROL 기간] / 0.




1. (선택 사항) [!UICONTROL 변량] 열은 리소스가 초과 할당되었음을 보여 줍니다. 다음 중 하나를 조정하십시오.

   * 초과 할당되거나 작업에 더 많은 리소스를 추가하는 작업 역할 하나에 대해 계획된 시간 수를 줄이고 새 리소스에 더 많은 계획된 시간을 분배합니다. 작업 또는 문제를 편집할 때 할당 또는 계획된 시간을 업데이트할 수 있습니다. 자세한 내용은 다음 문서를 참조하십시오.

      * [작업 편집](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [문제 편집](../manage-work/issues/manage-issues/edit-issues.md)

      >[!NOTE]
      >
      >작업 및 문제를 편집하려면 추가 액세스 및 권한이 있어야 합니다.

   * 이니셔티브에 대한 초과 할당을 표시하는 역할에 필요한 시간 수를 늘립니다. 자세한 내용은 [에서 이니셔티브 만들기 및 편집 [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

      >[!NOTE]
      >
      >계획을 편집하려면 추가 액세스 및 권한이 있어야 합니다.


1. (선택 사항) 드롭다운 아이콘을 클릭하여 [!UICONTROL 역할 할당] 패널 또는 타임라인의 [!UICONTROL 업무 균형자].

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   에 표시되는 것과 동일한 유형의 정보 [!UICONTROL 프로젝트 합계] 영역도 매월 표시됩니다.

   >[!TIP]
   >
   >에 나열된 개월 수 [!UICONTROL 역할 할당] 패널은 타임라인의 월이 화면의 화면에 표시됩니다. [!UICONTROL 업무 균형자]. 타임라인에서 앞뒤로 스크롤하여 추가 월을 봅니다.

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->


