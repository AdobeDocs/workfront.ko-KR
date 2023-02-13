---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 계획자에서 계획 삭제
description: 생성한 계획을 삭제할 수 있습니다. 공유된 계획은 삭제할 수 없습니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 1%

---

# 에서 계획 삭제 [!DNL Scenario Planner]

생성한 계획을 삭제할 수 있습니다. 공유된 계획은 삭제할 수 없습니다.

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
   <td> <p>[!UICONTROL Edit] 액세스 이상의 [!DNL Scenario Planner]</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>개체 권한</strong> </p> </td> 
   <td> <p>계획에 대한 [!UICONTROL Manage] 권한</p> <p>계획에 대한 추가 액세스 요청에 대한 내용은 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">에서 계획에 대한 액세스 요청 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 플랜 삭제

>[!IMPORTANT]
>
>삭제된 계획은 복구할 수 없습니다.

계획을 삭제하거나 계획에서 하나의 시나리오를 삭제할 수 있습니다.

* [플랜 삭제](#delete-plans)
* [시나리오 삭제](#delete-scenarios)

### 플랜 삭제

>[!IMPORTANT]
>
>계획을 삭제할 때 다음 사항을 고려하십시오.
>
>* 플랜과 관련된 모든 정보도 삭제됩니다. 여기에는 Job 역할 및 비용에 대한 정보를 포함하여 계획과 연관된 모든 시나리오 및 이니셔티브가 포함됩니다. 이 정보는 복구할 수 없습니다.
>* 계획에 게시된 시나리오가 포함되어 있으면 삭제된 이니셔티브에 연결된 프로젝트가 유지되고 [!DNL Scenario Planner] 영역은 [!UICONTROL 프로젝트 세부 사항] 섹션을 참조하십시오.
>
>  프로젝트에 이니셔티브 게시에 대한 자세한 내용은 [에서 이니셔티브를 게시하여 프로젝트를 업데이트하거나 만들 수 있습니다 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

계획을 삭제하려면

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png)를 클릭한 다음 [!UICONTROL 시나리오].

   계획 목록이 표시됩니다.

1. 계획 이름을 눌러 엽니다.
1. 을(를) 클릭합니다. **[!UICONTROL 추가 메뉴]** ![](assets/more-menu.png) 계획 이름의 오른쪽에 있는 다음 **[!UICONTROL 삭제]** > **[!UICONTROL 예, 삭제합니다]**.

   계획이 삭제되고 계획 목록으로 돌아갑니다.

### 시나리오 삭제 {#delete-scenarios}

>[!IMPORTANT]
>
>시나리오를 삭제할 때 다음 사항을 고려하십시오.
>
>* 시나리오를 삭제하면 시나리오에서 모든 이니셔티브 및 해당 정보가 삭제됩니다. 다른 시나리오에 복사된 경우 이니셔티브는 다른 시나리오에 유지됩니다.
>* 시나리오를 삭제할 때 이후 시나리오는 삭제된 시나리오의 수를 가져오며 계산 순서가 유지됩니다. 예를 들어 시나리오 4를 삭제하면 시나리오 5가 시나리오 4가 됩니다.
>* 시나리오의 일부 이니셔티브가 게시되면 이니셔티브에 연결된 프로젝트가 유지되고 시나리오 계획자 영역은 연결된 프로젝트에 남아 있습니다
>* 게시된 이니셔티브가 다른 시나리오에 있으면, 프로젝트에 대한 링크를 포함하여 해당 시나리오에 유지됩니다. 다른 시나리오에서 이러한 이니셔티브를 게시하면 연결된 프로젝트가 해당 시나리오의 새로운 정보로 업데이트됩니다.
>
>  프로젝트에 이니셔티브 게시에 대한 자세한 내용은 [에서 이니셔티브를 게시하여 프로젝트를 업데이트하거나 만들 수 있습니다 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

시나리오를 삭제하려면

1. 시나리오를 삭제할 계획으로 이동합니다.

   기본적으로 초기 시나리오가 표시됩니다.

1. 클릭 **[!UICONTROL 시나리오 비교]**.
1. 시나리오 카드의 오른쪽 상단에서 **[!UICONTROL 자세히]** 메뉴 ![](assets/more-menu.png)를 클릭한 다음 **[!UICONTROL 삭제]**.

   시나리오가 삭제됩니다.

1. 클릭 **[!UICONTROL 계획 저장]** 변경 사항을 저장하려면 을 클릭합니다.

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


