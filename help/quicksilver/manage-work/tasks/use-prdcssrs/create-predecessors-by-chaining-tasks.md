---
product-area: projects
navigation-topic: use-predecessors
title: 작업을 연결하여 전임 작업 관계 만들기
description: Adobe Workfront에서 여러 가지 방법으로 전임 작업 관계를 만들 수 있습니다. 한 가지 방법은 작업을 연결하는 것입니다.
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# 작업을 연결하여 전임 작업 관계 만들기

Adobe Workfront에서 여러 가지 방법으로 전임 작업 관계를 만들 수 있습니다. 한 가지 방법은 작업을 연결하는 것입니다.

전임 작업에 대한 자세한 내용은 [작업 전임 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)를 참조하십시오.

작업을 연결하면 시스템에서 각 작업에 수동으로 관계를 만들지 않고 선택한 작업에 대해 자동으로 전임 작업 관계를 만들 수 있습니다. 작업 간에 다른 전임 작업 관계 유형을 계속 사용할 수 있습니다.

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
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 및 프로젝트에 대한 권한 관리</p></td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Standard </p>
    <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 선행 작업 관계를 만드는 체인 작업

1. 연결할 작업이 포함된 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **작업**&#x200B;을 클릭합니다.
1. (조건부) 작업 목록의 오른쪽 상단 모서리에서 **자동 저장**&#x200B;을 선택한 다음 연결할 작업을 선택합니다.

   ![](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >작업 변경 사항을 수동으로 저장하거나 타임라인 계획 수립 모드를 사용하여 작업을 저장하는 경우에는 작업 목록에서 작업을 연결할 수 없습니다.

1. 선택한 작업을 마우스 오른쪽 단추로 클릭한 다음 **체인**&#x200B;을 클릭합니다.
1. 다음 종속성 유형 중에서 선택합니다.

   * **마침-시작**
   * **마침**
   * **시작**
   * **시작-완료**

   전임 작업 종속성 유형에 대한 자세한 내용은 [작업 종속성 유형 개요](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)를 참조하십시오.

1. (선택 사항) 일부 작업이 이전에 연결된 경우 **체인 해제**&#x200B;를 클릭합니다.

   >[!CAUTION]
   >
   >작업을 일괄 편집할 때 [체인 해제] 옵션을 사용하면 순차적 전임 작업만 제거됩니다.

   선택한 작업이 이제 전임 작업 관계에 의해 연결됩니다.
