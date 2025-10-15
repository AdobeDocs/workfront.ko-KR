---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 작업 목록에 프로젝트 및 이니셔티브에 대한 역할 할당 표시
description: 프로젝트와 이니셔티브를 연결한 후 리소스 할당을 나란히 관리하여 프로젝트 및 이니셔티브가 일치하는지 확인할 수 있습니다. 이를 통해 이를 과다 할당하거나 과소 활용하는 것을 방지할 수 있습니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: 77152e46-0b7b-4937-9d16-1a20c2a7fdf1
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# 작업 목록에 프로젝트 및 이니셔티브에 대한 역할 할당 표시

<!--Audited: 07/2024-->

프로젝트와 이니셔티브를 연결한 후 리소스 할당을 나란히 관리하여 프로젝트 및 이니셔티브가 일치하는지 확인할 수 있습니다. 이를 통해 이를 과다 할당하거나 과소 활용하는 것을 방지할 수 있습니다.

이 문서에서는 프로젝트의 작업 목록에 있는 [!UICONTROL 역할 할당] 패널을 사용하여 리소스를 조정하는 방법에 대해 설명합니다.

필수 구성 요소를 포함하여 프로젝트와 이니셔티브 간의 리소스 조정에 대한 일반적인 정보는 [프로젝트와 이니셔티브 간의 리소스 할당 조정에 대한 개요](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 패키지</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>메모</b></p>
<p>다른 Workfront 패키지가 있는 경우 Workfront 담당자에게 문의하십시오.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 라이센스</p> </td> 
   <td> <p>[!UICONTROL Light] 이상</p> 
   <p>[!UICONTROL Review] 이상</p> </td> 
  </tr> 
    <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 보기 이상의 액세스 권한.</p></td> 
  </tr> 
  <tr> 
   <td> <p>개체 권한 </p> </td> 
   <td> <p> 프로젝트에 대한 보기 이상의 권한.</p></td> 
  </tr> 
 </tbody> 
</table>

시나리오 플래너에 액세스하는 방법에 대한 자세한 내용은 [을(를) 사용하는 데 필요한 액세스 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md)를 참조하십시오.

Workfront 액세스 요구 사항에 대한 자세한 내용은 [Workfront 설명서에 대한 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>View or higher access to Projects.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p> View or higher permission to a project.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 작업 목록에 프로젝트 및 이니셔티브에 대한 역할 할당 표시

회사에서 [!DNL Workfront Scenario Planner] 라이선스를 구입한 경우 프로젝트의 [!UICONTROL 작업] 섹션에서 이니셔티브와 연결된 프로젝트 간의 리소스 할당을 조정할 수 있습니다.

1. (조건부) 이 문서의 [작업 목록에서 프로젝트 및 이니셔티브에 대한 역할 할당 표시](#show-role-allocation-for-projects-and-initiatives-in-the-task-list) 섹션에 설명된 방법 중 하나를 사용하여 프로젝트를 이니셔티브와 연결해야 합니다.

   >[!IMPORTANT]
   >
   >이니셔티브의 리소스를 변경하는 경우 이니셔티브의 최신 리소스 정보를 프로젝트에서 업데이트하려면 이니셔티브가 속한 시나리오를 다시 게시해야 합니다.

1. 프로젝트 및 연계된 이니셔티브에 대한 작업 역할 할당을 검토하려는 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **[!UICONTROL 작업]**&#x200B;을 클릭합니다.
1. 도구 모음의 오른쪽 상단에 있는 **[!UICONTROL 역할 할당 표시]** 아이콘 ![역할 할당 표시](assets/show-role-allocation-icon.png)를 클릭합니다.

   [!UICONTROL 역할 할당] 패널이 표시됩니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. **[!UICONTROL 역할 할당]** 패널의 [!UICONTROL 프로젝트 합계] 영역에서 다음 정보를 검토하십시오.

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
   >   * 작업 또는 문제의 기간이 0인 경우.
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


