---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: Portfolio에 프로젝트 추가
description: 프로젝트를 시작할 때 포트폴리오에 프로젝트를 추가하는 것이 좋습니다. 그러나 라이프타임 동안 언제든지 포트폴리오에 추가할 수 있습니다.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 97f36c18-3ac8-45ac-b5bc-dfe8b1363faf
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: fee6b71eeb0ca79703a2a9e29a14040b91cb7387
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 2%

---

# 포트폴리오에 프로젝트 추가

<!--Audited: 08/2025-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

프로젝트를 시작할 때 포트폴리오에 프로젝트를 추가하는 것이 좋습니다. 그러나 라이프타임 동안 언제든지 포트폴리오에 추가할 수 있습니다.

포트폴리오에 프로젝트를 추가할 때 다음 사항을 고려하십시오.

* 한 개의 포트폴리오만 프로젝트와 연결할 수 있습니다.
* 프로젝트는 삭제되거나 다른 포트폴리오와 연결될 때까지 포트폴리오에 남아 있습니다.
* 포트폴리오에는 프로젝트를 무제한으로 포함할 수 있습니다.

>[!CAUTION]
>
>   상속된 권한은 많은 하위 오브젝트에서 사용되는 경우 올바르게 적용되지 않을 수 있습니다.
>   
>   상속된 권한 문제를 방지하기 위해 다음 방법을 권장합니다.
>
>   * 단일 상위(포트폴리오 또는 프로그램) 아래에 있는 하위 개체(프로젝트) 수를 제한합니다. 포트폴리오 또는 프로그램당 10,000개 이하의 프로젝트를 권장합니다.
>   * 하위 수준 개체에 권한을 적용하여 상속 깊이를 줄입니다.
>
>     예를 들어, 포트폴리오에서 상속된 권한을 프로그램에 적용한 다음 프로젝트에 의존하지 않고 프로젝트 수준에서 직접 권한을 적용합니다.
>   * 더 적은 수의 프로젝트를 포함하도록 프로그램을 분할하므로 권한 복잡성이 줄어듭니다.


## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 패키지</td> 
   <td> <p>Any</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>표준</p> 
   <p>[!UICONTROL 계획] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>[!UICONTROL Edit] 액세스 포트폴리오</p> <p>프로젝트에 대한 [!UICONTROL 편집] 액세스 권한</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>포트폴리오에 대한 [!UICONTROL 관리] 권한</p> <p>[!UICONTROL Manage] permissions to the projects</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>[!UICONTROL Edit] access Portfolios</p> <p>[!UICONTROL Edit] access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>[!UICONTROL Manage] permissions to the projects</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## Add a project to a portfolio

1. Go to a portfolio, then click **[!UICONTROL Projects]** in the left panel.

   ![Portfolio with projects](assets/qs-portfolio-with-projects-350x90.png)

1. Click **[!UICONTROL New Project]** and select a method for adding a project.

   >[!TIP]
   >
   >You cannot add a project when you view the list of projects in the [!UICONTROL Milestone] view.

   다음 옵션 중에서 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Existing Project]</td> 
      <td> <p>Add a project that has already been created.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL New Project]</td> 
      <td> <p>Add a new project. </p> <p>For more information about creating a new project, see <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Create a project</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Import a Project from [!DNL MS Project]] </td> 
      <td> <p>Add a project that you previously exported from [!DNL MS Project] and have saved on your computer. </p> <p>For more information about creating a new project by importing it from [!DNL Microsoft Project], see <a href="../../../manage-work/projects/create-projects/import-project-from-ms-project.md" class="MCXref xref">Import a project from [!DNL Microsoft Project]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request Project]</td> 
      <td> <p>Request that a project is approved.</p> <p>For information about requesting projects, see <a href="../../../manage-work/projects/create-projects/request-project.md">Requesting a Project</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL New from Template]</td> 
      <td> <p>Add a new project using an existing template. </p> <p>For more information about creating a project from a template, see <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Create a project using a template</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![새 프로젝트 드롭다운](assets/new-project-dropdown-expanded-from-portfolio-nwe-350x376.png)

1. (Conditional) If you selected to add an existing project, the **Add Projects** box opens. <!--check this after UI changes-->

   ![Add existing project](assets/add-existing-projects-to-portfolios-box.png) <!--check this after UI changes-->

1. **[!UICONTROL 이 Portfolio에 프로젝트 추가]** 필드에 프로젝트 이름을 입력한 다음 목록에 나타나면 클릭합니다.  <!--check this after UI changes-->

   두 개 이상의 프로젝트를 추가할 수 있습니다.

1. (선택 사항) 포트폴리오에 추가하지 않으려면 프로젝트 이름 오른쪽에 있는 **X** 아이콘을 클릭하여 목록에서 제거합니다.

   <!--replace last step with this, for unshim: 1. (Optional) Click the **Delete** icon ![Delete icon](assets/delete-icon.png) next to the name of a project if you decide not to add it to the portfolio.-->

1. **[!UICONTROL 프로젝트 추가]**&#x200B;를 클릭합니다. <!--check this after UI changes-->

   선택한 프로젝트가 이제 포트폴리오와 연결됩니다.
