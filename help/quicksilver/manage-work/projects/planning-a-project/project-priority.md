---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 프로젝트 우선 순위 이해 및 업데이트
description: 프로젝트에 우선 순위를 사용하는 여러 가지 방법이 있으며 서로 통신하지 않습니다. 사용자의 요구 사항과 일치하는 프로젝트의 우선 순위 중 하나를 선택하고 프로젝트의 중요도를 분류할 때 참조하는 것이 좋습니다.
author: Alina
feature: Work Management
exl-id: b1e0b6c5-f2a7-455b-836b-6c0ead85e3ad
source-git-commit: 00e693fc8b35a59f6ed212bc30da7f85cc78c845
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 1%

---

# 프로젝트 우선 순위 이해 및 업데이트

프로젝트에 우선 순위를 사용하는 여러 가지 방법이 있으며 서로 통신하지 않습니다. 사용자의 요구 사항과 일치하는 프로젝트의 우선 순위 중 하나를 선택하고 프로젝트의 중요도를 분류할 때 참조하는 것이 좋습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>표준</p> 
   <p>플랜</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 관리</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Adobe Workfront의 프로젝트 우선 순위 유형

다음은 Adobe Workfront에서 프로젝트의 등급을 매기는 데 사용할 수 있는 우선 순위 유형입니다.

* **프로젝트 우선 순위 필드**: 프로젝트에 우선 순위를 수동으로 할당할 수 있습니다. 이 문서에서는 프로젝트에 수동으로 우선 순위를 할당하는 방법을 설명합니다.

  자세한 내용은 이 문서의 [프로젝트 우선 순위에 대한 고려 사항](#considerations-about-project-priority) 섹션을 참조하십시오.

* **Portfolio Optimizer에서 프로젝트의 우선 순위**(프로젝트가 포트폴리오와 연결된 경우):

  Portfolio Optimizer에서 프로젝트의 우선 순위에 대한 자세한 내용은 [Portfolio Optimizer에서 프로젝트 우선 순위 지정](../../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md) 문서를 참조하십시오.

* **리소스 플래너에서 프로젝트의 우선 순위**: 리소스 플래너에서 프로젝트의 우선 순위를 수동으로 지정하여 리소스를 먼저 받아야 하는 프로젝트를 표시할 수 있습니다.

  리소스 플래너에서 프로젝트 우선 순위에 대한 자세한 내용은 [리소스 플래너 탐색 개요](../../../resource-mgmt/resource-planning/resource-planner-navigation.md) 문서의 &quot;프로젝트 계획 우선 순위&quot; 섹션을 참조하십시오.

## 프로젝트 우선 순위에 대한 고려 사항 {#considerations-about-project-priority}

Workfront에서 우선 순위를 프로젝트와 연결할 수 있습니다. 프로젝트의 우선 순위를 표시하면 해당 프로젝트가 얼마나 중요한지가 시스템의 모든 사용자에게 표시됩니다.

프로젝트의 우선 순위를 선택할 때는 다음 사항을 고려하십시오.

* Workfront 관리자는 Workfront에서 사용할 수 있는 우선 순위를 정의합니다. 이를 설정한 후에는 우선순위 필드의 프로젝트와 연결할 수 있습니다.

  Workfront에서 우선 순위를 만드는 방법에 대한 자세한 내용은 [우선 순위 만들기 및 사용자 지정](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md) 문서를 참조하십시오.

* 프로젝트의 우선순위 필드를 업데이트할 때 이 우선순위는 Portfolio Optimizer 또는 리소스 플래너로 전송되지 않습니다. 프로젝트의 우선 순위 필드는 단순히 다른 사용자에게 중요도를 표시하기 위해 프로젝트에 배치하는 수동 플래그입니다.
* 프로젝트의 우선 순위 값은 주로 보고 목적으로 사용됩니다.

  예를 들어 프로젝트 필터에서 이 필드를 사용할 때 우선순위 값이 &quot;긴급&quot;인 모든 프로젝트를 검색할 수 있습니다.
* 작업과 문제에는 우선 순위도 있지만 작업, 문제 및 프로젝트 우선 순위는 서로 독립적으로 작동하며 자동으로 서로 영향을 주지 않습니다. 우선순위가 높은 프로젝트나 우선순위가 낮은 프로젝트에서 우선순위가 높은 작업이 있을 수 있습니다.
* Workfront의 다음 영역에서 프로젝트 우선 순위를 업데이트할 수 있습니다.

   * **프로젝트 편집** 대화 상자에서
   * 프로젝트의 **프로젝트 세부 정보** 탭에서.
   * 프로젝트 목록 또는 보고서에서.

## 프로젝트 우선 순위 필드 업데이트

1. 우선 순위를 업데이트할 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **프로젝트 세부 정보**&#x200B;를 클릭합니다.
1. 프로젝트 세부 정보 영역의 오른쪽 상단에 있는 **편집** 아이콘 ![편집 아이콘](assets/qs-edit-icon.png)을 클릭한 다음 **개요**&#x200B;를 클릭합니다.

1. **우선 순위** 필드에서 다음 옵션 중 하나를 선택합니다.

   * 없음
   * 낮음
   * 일반

     기본 우선 순위입니다.

   * 높음
   * 긴급

   ![프로젝트의 우선 순위 목록](assets/project-priority-picker-list.png)

1. **변경 내용 저장**&#x200B;을 클릭합니다.

   다른 사용자와 통신하고 각 수준의 우선 순위가 프로젝트에 어떤 의미를 갖는지 이해해야 합니다.
