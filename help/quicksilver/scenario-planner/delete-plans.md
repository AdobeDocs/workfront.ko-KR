---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 플래너에서 계획 삭제
description: 생성한 계획을 삭제할 수 있습니다. 공유된 플랜은 삭제할 수 없습니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# [!DNL Scenario Planner]에서 플랜 삭제

생성한 계획을 삭제할 수 있습니다. 공유된 플랜은 삭제할 수 없습니다.

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

## 플랜 삭제

>[!IMPORTANT]
>
>삭제된 계획은 복구할 수 없습니다.

계획을 삭제하거나 계획의 시나리오 하나를 삭제할 수 있습니다.

* [계획 삭제](#delete-plans)
* [시나리오 삭제](#delete-scenarios)

### 플랜 삭제

>[!IMPORTANT]
>
>계획을 삭제할 때는 다음 사항을 고려하십시오.
>
>* 해당 계획과 관련된 모든 정보도 삭제됩니다. 여기에는 작업 역할 및 비용에 대한 정보를 포함하여 플랜과 관련된 모든 시나리오 및 이니셔티브가 포함됩니다. 이 정보는 복구할 수 없습니다.
>* 플랜에 게시된 시나리오가 포함된 경우 삭제된 이니셔티브에 연결된 프로젝트가 보존되고 [!DNL Scenario Planner] 영역은 [!UICONTROL 프로젝트 세부 정보] 섹션에 남아 있습니다.
>
>  프로젝트에 이니셔티브를 게시하는 방법에 대한 자세한 내용은 [이니셔티브를 게시하여 프로젝트 업데이트 또는 만들기 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)를 참조하십시오.

계획을 삭제하려면

{{step1-to-scenario-planner}}

계획 목록이 표시됩니다.

1. 계획명을 눌러 계획을 엽니다.
1. 플랜 이름 오른쪽에 있는 **[!UICONTROL 추가 메뉴]** ![](assets/more-menu.png)를 클릭한 다음 **[!UICONTROL 삭제]** > **[!UICONTROL 예, 삭제]**&#x200B;를 클릭합니다.

   플랜이 삭제되고 플랜 목록으로 돌아갑니다.

### 시나리오 삭제 {#delete-scenarios}

>[!IMPORTANT]
>
>시나리오를 삭제할 때는 다음 사항을 고려하십시오.
>
>* 시나리오를 삭제하면 시나리오에서 모든 이니셔티브와 해당 정보가 삭제됩니다. 이니셔티브가 다른 시나리오에 복사되는 경우 이니셔티브는 다른 시나리오에 유지됩니다.
>* 시나리오를 삭제할 때 후속 시나리오는 삭제된 시나리오의 수를 사용하며 계산 순서는 유지됩니다. 예를 들어 시나리오 4를 삭제하면 시나리오 5가 시나리오 4가 됩니다.
>* 시나리오의 일부 이니셔티브가 게시되면 이니셔티브에 연결된 프로젝트가 보존되고 시나리오 플래너 영역은 연결된 프로젝트에 유지됩니다
>* 게시된 이니셔티브가 다른 시나리오에 있는 경우 프로젝트에 대한 링크를 포함하여 해당 시나리오에 유지됩니다. 다른 시나리오에서 이러한 이니셔티브를 게시하면 연결된 프로젝트가 해당 시나리오에서 새로운 정보로 업데이트됩니다.
>
>  프로젝트에 이니셔티브를 게시하는 방법에 대한 자세한 내용은 [이니셔티브를 게시하여 프로젝트 업데이트 또는 만들기 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)를 참조하십시오.

시나리오를 삭제하려면 다음을 수행하십시오.

1. 시나리오를 삭제할 계획으로 이동합니다.

   기본적으로 초기 시나리오가 표시됩니다.

1. **[!UICONTROL 시나리오 비교]**&#x200B;를 클릭합니다.
1. 시나리오 카드의 오른쪽 상단 모서리에서 **[!UICONTROL 자세히]** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 다음 **[!UICONTROL 삭제]**&#x200B;를 클릭합니다.

   시나리오가 삭제됩니다.

1. 변경 내용을 저장하려면 **[!UICONTROL 계획 저장]**&#x200B;을 클릭하세요.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete initiatives</h2>
<p>(NOTE: moved this section to its own article about deleting initiatives) </p> <note type="important">
<p>Consider the following when deleting initiatives:</p>
<ul>
<li>Deleting an initiative deletes the job roles and cost information from the initiative.</li>
<li><span>When you delete an initiative that is published to a project, the initiative is removed from the scenario but the Scenario Planner area remains in the Project Details section.</span> </li>
<li> <p>If the initiative you delete is the only published initiative on the scenario, the indicator that the plan has been published is also removed. </p> <p>For information about publishing initiatives to projects, see <a href="../scenario-planner/publish-scenarios-update-projects.md" class="MCXref xref">Update or create projects by publishing initiatives in the Scenario Planner</a>.</p> </li>
</ul>
</note>
<p>To delete an initiative:</p>
<ol>
<li value="1"> <p> <p>Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png">, then click Scenarios.</p> </p> <p>A list of plans displays. </p> </li>
<li value="2">Click the name of a plan to open it, then locate the initiative you want to delete.</li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/more-menu.png"> to the right of the initiative name, then click <strong>Delete</strong> > <strong>Yes, delete it</strong>. </p> <p>The initiative is deleted. </p> </li>
<li value="4">Click <strong>Save Plan</strong> to save your changes. </li>
</ol>
</div>
-->


