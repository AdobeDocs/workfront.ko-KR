---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 플래너에서 이니셔티브 삭제
description: 자신이 생성한 계획이나 다른 사람이 나와 공유한 계획에서 이니셔티브를 삭제할 수 있습니다. 삭제한 이니셔티브는 복구할 수 없습니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 1%

---

# [!DNL Scenario Planner]에서 이니셔티브 삭제

자신이 생성한 계획이나 다른 사람이 나와 공유한 계획에서 이니셔티브를 삭제할 수 있습니다. 삭제한 이니셔티브는 복구할 수 없습니다.

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
   <td> <p>다음에 대한 [!UICONTROL 편집] 액세스 권한: [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>개체 권한 </p> </td> 
   <td> <p>플랜에 대한 [!UICONTROL 관리] 권한</p> </td> 
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
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements to Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## 이니셔티브 삭제

이니셔티브를 삭제할 때는 다음 사항을 고려하십시오.

* 이니셔티브를 삭제하면 필요한 작업 역할의 양과 이니셔티브와 관련된 비용 정보가 계획에서 제거됩니다.
* 프로젝트를 가져와서 만든 이니셔티브를 삭제해도 이니셔티브와 연결된 프로젝트는 삭제되지 않습니다.
* 프로젝트에 게시된 이니셔티브를 한 번 이상 삭제하면 다음과 같은 결과가 발생합니다.

   * 이니셔티브가 시나리오에서 삭제되었지만 [!DNL Scenario Planner] 영역은 [!UICONTROL 프로젝트 세부 정보] 섹션에 남아 있습니다.
   * 삭제한 이니셔티브가 시나리오에 게시된 유일한 이니셔티브인 경우 플랜이 게시되었다는 표시기도 제거됩니다.

     프로젝트에 이니셔티브를 게시하는 방법에 대한 자세한 내용은 [이니셔티브를 게시하여 프로젝트 업데이트 또는 만들기 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)를 참조하십시오.

     프로젝트를 가져와서 이니셔티브를 만드는 방법에 대한 자세한 내용은 [의 플랜에 프로젝트 가져오기 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) 를 참조하십시오.

한 번에 하나의 이니셔티브를 삭제하거나 여러 이니셔티브를 일괄적으로 삭제할 수 있습니다.

* [이니셔티브 하나 삭제](#delete-one-initiative)
* [일괄 이니셔티브 삭제](#delete-initiatives-in-bulk)

### 1개의 이니셔티브 삭제 {#delete-one-initiative}

{{step1-to-scenario-planner}}

계획 목록이 표시됩니다.

1. 계획명을 눌러 계획을 연 다음 삭제할 이니셔티브를 찾습니다.
1. 다음 중 하나를 수행하십시오.

   * 이니셔티브 이름의 오른쪽에 있는 **[!UICONTROL 추가 메뉴]** ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **[!UICONTROL 삭제]** > **[!UICONTROL 예, 삭제]**&#x200B;를 클릭합니다.

   * 이니셔티브 왼쪽에 있는 상자를 선택한 다음, 플랜 하단에 나타나는 부동 메뉴에서 **[!UICONTROL 삭제]**&#x200B;를 클릭한 다음, **[!UICONTROL 예, 삭제]**&#x200B;를 클릭합니다.

   이니셔티브와 해당 작업 역할 및 비용 정보가 플랜에서 삭제됩니다.

1. 변경 내용을 저장하려면 **[!UICONTROL 계획 저장]**&#x200B;을 클릭하세요.

### 일괄 이니셔티브 삭제 {#delete-initiatives-in-bulk}

{{step1-to-scenario-planner}}

계획 목록이 표시됩니다.

1. 계획명을 눌러 계획을 연 다음 삭제할 이니셔티브를 찾습니다.
1. 삭제할 이니셔티브의 왼쪽에 있는 상자를 선택한 다음, 플랜 하단에 나타나는 메뉴에서 **[!UICONTROL 삭제]**&#x200B;를 클릭한 다음, **[!UICONTROL 예, 삭제]**&#x200B;를 클릭합니다.

   ![이니셔티브 메뉴 관리](assets/bottom-manage-initiative-menu-350x45.png)

   이니셔티브와 해당 작업 역할 및 비용 정보가 계획에서 삭제됩니다.

1. 변경 내용을 저장하려면 **[!UICONTROL 계획 저장]**&#x200B;을 클릭하세요.
