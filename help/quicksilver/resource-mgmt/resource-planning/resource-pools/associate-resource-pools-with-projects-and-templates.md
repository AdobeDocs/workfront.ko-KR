---
product-area: resource-management
navigation-topic: resource-pools
title: 프로젝트 및 템플릿에 리소스 풀 연결
description: 리소스 풀은 Adobe Workfront에서 리소스를 관리하는 데 도움이 되는 사용자의 컬렉션입니다.
author: Alina
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: 6580fec18982215dbc2535d5f2ab159fc32ac3f5
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# 프로젝트 및 템플릿에 리소스 풀 연결


<!-- drafted for bulk editing projects: make this live when we release edit projects in bulk and replace the screen shot below (marked) and make the shot in yellow showing adding resource pools to multiple projects:
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The sections about how to add resource pools to templates, projects are duplicated from the articles listed in those sections (Editing Projects, Creating a Template, etc).</p>
<p>***I decided to keep these steps here, though, because it's hard to parse through those much lunger articles for just updating this one field.)</p>
</div>
-->

리소스 풀은 Adobe Workfront에서 리소스를 관리하는 데 도움이 되는 사용자의 컬렉션입니다.

리소스 풀을 생성한 후에는 프로젝트 또는 템플릿과 연결할 수 있으므로 나중에 프로젝트에 대한 리소스를 예약할 수 있습니다.

리소스 풀을 미리 만들고, 프로젝트에 연결하고, 프로젝트를 시작하기 전에 리소스를 편성하는 것이 좋습니다.

리소스 풀에 대한 자세한 내용은 [리소스 풀 개요](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

리소스 풀 만들기에 대한 내용은 [리소스 풀 만들기](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

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
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>리소스 풀 관리에 대한 액세스를 포함하는 리소스 관리에 대한 액세스 편집</p> <p>프로젝트, 템플릿 및 사용자에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트, 템플릿 및 리소스 풀을</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 하나의 프로젝트 또는 템플릿과 리소스 풀을 연결합니다

리소스 풀을 프로젝트와 연결하는 것과 같은 방식으로 템플릿과 리소스 풀을 연결할 수 있습니다. 이 문서에서는 리소스 풀을 프로젝트와 연결하는 방법을 설명합니다.

1. 프로젝트로 이동하여 **자세히** 아이콘 ![](assets/more-icon.png)프로젝트 이름 옆의 **편집**.

1. 클릭 **프로젝트 설정**.

1. 에 리소스 풀 이름을 입력합니다. **리소스 풀** 필드를 선택한 다음 목록이 나타나면 목록에서 선택합니다.\
   여러 리소스 풀을 하나의 프로젝트 또는 템플릿과 연결할 수 있습니다.

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. **저장**&#x200B;을 클릭합니다.

프로젝트를 편집하고 리소스 풀과 연결하는 방법에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

템플릿을 편집하고 리소스 풀에 연결하는 방법에 대한 자세한 내용은 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## 리소스 풀을 여러 프로젝트 또는 템플릿과 일괄적으로 연결

여러 프로젝트나 템플릿을 일괄적으로 편집하고 동일한 리소스 풀을 모두 동시에 연결할 수 있습니다.

리소스 풀을 프로젝트와 연결하는 것과 같은 방식으로 리소스 풀을 템플릿과 연결할 수 있습니다.

자원 풀을 여러 프로젝트에 일괄적으로 연결하려면

1. 프로젝트 목록으로 이동합니다.
1. 여러 프로젝트를 선택한 다음 **편집** 아이콘 ![](assets/edit-icon.png) 를 클릭합니다.

1. 클릭 **설정**.
1. 에 리소스 풀 이름을 입력합니다. **리소스 풀** 필드를 선택한 다음 목록이 나타나면 목록에서 선택합니다.\
   여러 리소스 풀을 프로젝트 또는 템플릿과 연결할 수 있습니다.

   >[!NOTE]
   >
   >프로젝트 또는 템플릿을 일괄적으로 편집할 때 선택한 모든 프로젝트 또는 템플릿에 공통인 리소스 풀만 이 필드에 표시됩니다. 선택한 프로젝트에 공유 리소스 풀이 없으면 이 필드는 비어 있습니다. 여기서 지정하는 리소스 풀은 프로젝트 또는 템플릿의 개별 리소스 풀을 덮어씁니다.

<!--drafted note for bulk editing projects - update the screen shot below for Edit Projects with the new UI in bulk and add the preview tags to the picture for Preview-->

![add_resource_pools_to_multiple_projects.png](assets/add-resource-pools-to-multiple-projects-350x358.png)

1. 클릭 **변경 내용 저장**.\
   자원 풀이 프로젝트 또는 템플리트와 연관되어 있으면 자원 계획자 내의 프로젝트에 대한 사용자 할당을 예산을 책정할 수 있습니다.\
   리소스 계획자에 대한 자세한 내용은 [리소스 플래너 개요](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

프로젝트를 일괄적으로 편집하는 방법에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

템플릿을 일괄적으로 편집하는 방법에 대한 자세한 내용은 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
