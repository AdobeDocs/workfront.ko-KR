---
product-area: resource-management
navigation-topic: resource-pools
title: 리소스 풀을 프로젝트 및 템플릿과 연결
description: 리소스 풀은 Adobe Workfront에서 리소스를 관리하는 데 도움이 되는 사용자의 컬렉션입니다.
author: Alina
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: 171ccfe5d2bc9825c9cdb195df1a97a32e515646
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# 리소스 풀을 프로젝트 및 템플릿과 연결


<!-- drafted for bulk editing projects: keep this in yellow till this releases to ALL customers - May 1, 2023

Also - take out all the references to Preview and Prod at prod final
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->


<!--
<p>The sections about how to add resource pools to templates, projects are duplicated from the articles listed in those sections (Editing Projects, Creating a Template, etc).</p>
<p>***I decided to keep these steps here, though, because it's hard to parse through those much lunger articles for just updating this one field.)</p>
-->

리소스 풀은 Adobe Workfront에서 리소스를 관리하는 데 도움이 되는 사용자의 컬렉션입니다.

리소스 풀을 만든 후 프로젝트 또는 템플릿과 연결하여 나중에 프로젝트에 대한 리소스 예산을 책정할 수 있습니다.

프로젝트가 시작되기 전에 리소스 풀을 미리 만들어 프로젝트와 연결하고 리소스 예산을 책정하는 것이 좋습니다.

리소스 풀에 대한 자세한 내용은 [리소스 풀 개요](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)를 참조하십시오.

리소스 풀 만들기에 대한 자세한 내용은 [리소스 풀 만들기](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)를 참조하십시오.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>리소스 풀 관리에 대한 액세스 권한을 포함하는 리소스 관리에 대한 액세스 편집</p> <p>프로젝트, 템플릿 및 사용자에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>리소스 풀을 연결할 프로젝트, 템플릿 및 사용자에 대한 권한을 관리합니다.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 리소스 풀을 하나의 프로젝트 또는 템플릿과 연결

리소스 풀을 프로젝트와 연관시키는 것과 동일한 방식으로 리소스 풀을 템플릿에 연관시킬 수 있습니다. 이 문서에서는 리소스 풀을 프로젝트와 연결하는 방법에 대해 설명합니다.

1. 프로젝트로 이동하여 프로젝트 이름 옆에 있는 **자세히** 아이콘 ![](assets/more-icon.png)을(를) 클릭한 다음 **편집**&#x200B;을(를) 클릭합니다.

1. **프로젝트 설정**&#x200B;을 클릭합니다.

1. **리소스 풀** 필드에 리소스 풀 이름을 입력한 다음 표시될 때 목록에서 선택하십시오.\
   여러 리소스 풀을 하나의 프로젝트 또는 템플릿에 연결할 수 있습니다.

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. **저장**&#x200B;을 클릭합니다.

프로젝트를 편집하고 리소스 풀과 연결하는 방법에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md)을 참조하세요.

템플릿을 편집하고 리소스 풀과 연결하는 방법에 대한 자세한 내용은 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)을 참조하십시오.

## 리소스 풀을 여러 프로젝트 또는 템플릿과 일괄 연결

여러 프로젝트 또는 템플릿을 일괄적으로 편집하고 동일한 리소스 풀을 모든 리소스 풀과 동시에 연결할 수 있습니다.

리소스 풀을 프로젝트와 연결하는 것과 동일한 방식으로 리소스 풀을 템플릿에 연결할 수 있습니다.

리소스 풀을 여러 프로젝트와 일괄 연결하려면 다음을 수행합니다.

1. 프로젝트 목록으로 이동합니다.
1. 여러 프로젝트를 선택한 다음 목록 맨 위에 있는 **편집** 아이콘 ![](assets/edit-icon.png)을(를) 클릭합니다.

1. **설정**&#x200B;을 클릭합니다.
1. **리소스 풀** 필드에 리소스 풀 이름을 입력한 다음 표시될 때 목록에서 선택하십시오.\
   여러 리소스 풀을 프로젝트 또는 템플릿과 연결할 수 있습니다.

   >[!NOTE]
   >
   >* 템플릿을 일괄 편집할 때 선택한 모든 템플릿에 공통되는 리소스 풀만 이 필드에 나타납니다. 선택한 템플릿에 공유 리소스 풀이 없는 경우 이 필드는 비어 있습니다. 여기에서 지정하는 리소스 풀은 프로젝트 또는 템플릿의 개별 리소스 풀을 덮어씁니다.
   >
   >* 프로젝트를 일괄 편집할 때 선택한 프로젝트에 다른 리소스 풀이 있는 경우 &quot;여러 값&quot; 표시기가 있습니다. 프로젝트에 대한 리소스 풀을 일괄적으로 추가하면 모든 풀이 선택한 프로젝트에 추가되어 원래 리소스 풀을 덮어씁니다.

   ![add_resource_pools_to_multiple_projects.png](assets/add-resource-pools-to-multiple-projects-350x358.png)

1. **변경 내용 저장**&#x200B;을 클릭합니다.\
   리소스 풀이 프로젝트 또는 템플릿과 연결되면 리소스 플래너 내에서 프로젝트에 대한 사용자 할당의 예산을 책정할 수 있습니다.\
   리소스 플래너에 대한 자세한 내용은 [리소스 플래너 개요](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)를 참조하십시오.

프로젝트를 일괄적으로 편집하는 방법에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md)의 &quot;일괄 프로젝트 편집&quot; 섹션을 참조하십시오.

템플릿을 일괄 편집하는 방법에 대한 자세한 내용은 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)의 &quot;일괄 템플릿 편집&quot; 섹션을 참조하십시오.
