---
product-area: projects
navigation-topic: create-tasks
title: 하위 작업 만들기
description: Adobe Workfront에서 작업은 상위-하위 관계를 가질 수 있습니다. 하위 작업을 하위 작업이라고 합니다. 주 작업을 하위 작업으로 만들어 작업 목록에서 하위 작업을 만들 수 있습니다. 하위 작업을 주 작업으로 만들 수도 있습니다.
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: ac24b2486b9fc5a0b8c2944a6ec240140238b908
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# 하위 작업 만들기

<!-- Audited: 01/2025 -->

Adobe Workfront에서 작업은 상위-하위 관계를 가질 수 있습니다. 하위 작업을 하위 작업이라고 합니다. 주 작업을 다른 작업의 하위 작업으로 만들어 작업 목록에 하위 작업을 만들 수 있습니다. 하위 작업을 주 작업으로 만들 수도 있습니다.

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
   <td> <p>표준</p> 
   <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 이상을 추가할 수 있는 권한으로 프로젝트에 참여</p> 
   <p>작업을 만들 때 작업에 대한 관리 권한을 자동으로 받습니다</p> 
    </td> 
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
   <p>New: Standard</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project and the parent task with ability to Add Tasks or higher</p> <p>You automatically receive Manage permissions to the task after you create it.</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## 하위 작업 만들기

작업 목록 또는 작업 하위 작업 섹션에서 하위 작업을 생성할 수 있습니다.

>[!TIP]
>
>프로젝트에 대한 하위 작업을 만드는 것은 템플릿의 템플릿 작업에 템플릿 하위 작업을 만드는 것과 비슷합니다.


### 작업 목록에서 하위 작업 만들기 {#create-subtasks-from-the-task-list}

1. 하위 작업을 만들 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **작업** 섹션을 클릭합니다.
1. (조건부) 하위 작업으로 만들 작업이 상위 작업으로 만들 작업 바로 아래에 아직 없는 경우 작업 목록에서 적절한 위치로 끌어서 놓습니다.
1. 하위 작업을 만들 작업을 선택하고 다음 중 하나를 수행합니다.

   * 선택한 작업을 바로 위에 있는 작업의 하위 작업으로 만들려면 **들여쓰기** 아이콘 ![](assets/indent-icon-nwe-33x29.png)을(를) 클릭하십시오.
   * 표준 영어 QWERTY 키보드를 사용하는 경우 키보드에서 Option + > (Mac) 또는 Alt + > (Windows)를 누릅니다. 다른 언어에서는 Option + , (Mac) 또는 Alt + , (Windows) 명령을 사용하여 들여쓸 수 있습니다.

     >[!TIP]
     >
     >인라인 편집에서 작업을 편집할 때 키보드 단축키가 작동하지 않습니다. 이 경우 들여쓰기 아이콘 ![](assets/indent-icon-nwe-33x29.png)을(를) 사용하여 하위 작업을 만듭니다.

   * 작업을 상위 작업으로 지정할 작업 위로 끌어서 놓습니다.

     >[!NOTE]
     >
     >작업 목록이 작업 번호별로 정렬되고 작업 목록에 적용된 그룹화가 없는 경우에만 작업을 들여쓸 수 있습니다.

### 작업 하위 작업 섹션에서 하위 작업 만들기 {#create-subtasks-from-the-task-subtasks-section}

>[!NOTE]
>
>Workfront 또는 그룹 관리자는 레이아웃 템플릿을 사용하여 사용자 환경에서 하위 작업 섹션을 제거할 수 있습니다.

1. 하위 작업을 만들 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **작업** 섹션을 클릭합니다.
1. 하위 작업을 만들 작업의 이름을 클릭합니다.
1. 사용 가능한 경우 왼쪽 패널의 **하위 작업** 섹션을 클릭합니다.
1. **새 작업을 클릭합니다.**

   작업 만들기에 대한 자세한 내용은 [프로젝트에서 작업 만들기](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)를 참조하십시오.

1. **작업 만들기**&#x200B;를 클릭합니다.

   새 작업은 3단계에서 선택한 작업의 하위 작업으로 만들어집니다. <!--ensure this is accurate-->

## 하위 작업을 주 작업으로 만들기

1. 하위 작업을 주 작업으로 만들 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **작업** 섹션을 클릭합니다.
1. 기본 작업을 수행할 하위 작업을 선택합니다.
1. 하위 작업을 주 작업으로 만들려면 **내어쓰기** 아이콘 ![](assets/outdent-icon-nwe-31x29.png)을(를) 클릭하십시오.

   또는

   표준 영어 QWERTY 키보드에서 Option + &lt;(Mac) 또는 Alt + &lt;(Windows)를 누릅니다. 다른 언어에서는 Option + 명령을 사용할 수 있습니다. (Mac) 또는 Alt + . (Windows) 내어쓰기입니다.

   >[!NOTE]
   >
   >작업 목록이 작업 번호별로 정렬되고 작업 목록에 적용된 그룹화가 없는 경우에만 작업을 내어쓸 수 있습니다.
