---
product-area: projects
navigation-topic: create-tasks
title: 하위 작업 만들기
description: Workfront에서 작업은 상위-하위 관계를 가질 수 있습니다. 하위 작업을 하위 작업이라고 합니다. 주 작업을 하위 작업으로 설정하여 작업 목록에서 하위 작업을 만들 수 있습니다. 하위 작업을 주 작업으로 만들 수도 있습니다.
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: fb1f4e609e0cc2b0e9e4d0b36b7ace3fd8937d26
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---

# 하위 작업 만들기

Workfront에서 작업은 상위-하위 관계를 가질 수 있습니다. 하위 작업을 하위 작업이라고 합니다. 주 작업을 하위 작업으로 설정하여 작업 목록에서 하위 작업을 만들 수 있습니다. 하위 작업을 주 작업으로 만들 수도 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. 작업 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">작업에 대한 액세스 권한 부여</a>. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 추가 이상의 기능을 사용하여 프로젝트 및 상위 작업에 권한을 부여합니다</p> <p>작업을 만들면 작업에 대한 관리 권한을 자동으로 받게 됩니다</p> <p> 작업 권한에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">작업 공유 </a>. </p> <p>추가 권한 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 하위 작업 만들기

* [작업 목록에서 하위 작업 만들기](#create-subtasks-from-the-task-list)
* [작업 하위 작업 섹션에서 하위 작업 만들기](#create-subtasks-from-the-task-subtasks-section)

### 작업 목록에서 하위 작업 만들기 {#create-subtasks-from-the-task-list}

1. 하위 작업을 만들 프로젝트로 이동합니다.
1. 을(를) 클릭합니다. **작업** 왼쪽 패널의 섹션에 있습니다.
1. (조건부) 하위 작업을 만들 작업이 상위 작업을 만들 작업 바로 아래에 아직 없으면 작업 목록의 해당 위치로 끕니다.
1. 하위 작업을 만들 작업을 선택하고 다음 중 하나를 수행합니다.

   * 을(를) 클릭합니다. **들여쓰기** 아이콘 ![](assets/indent-icon-nwe-33x29.png) 선택한 작업을 해당 작업 바로 위에 있는 작업의 하위 작업으로 만듭니다.
   * 표준 영어 QWERTY 키보드를 사용하는 경우 키보드에서 Option + > (Mac) 또는 Alt + >(Windows)를 누릅니다. 다른 언어에서는 Option + , (Mac) 또는 Alt + , (Windows) 명령을 사용하여 들여쓸 수 있습니다.

      >[!TIP]
      >
      >인라인 편집에서 작업을 편집할 때는 키보드 단축키가 작동하지 않습니다. 이 경우 들여쓰기 아이콘을 사용합니다 ![](assets/cs1.png) 하위 작업을 만들려면

   * 작업을 상위 작업으로 지정할 작업 위로 끌어서 놓습니다.
   >[!NOTE]
   >
   >작업 목록이 작업 번호로 정렬되고 작업 목록에 적용된 그룹화가 없는 경우에만 작업을 들여쓸 수 있습니다.

### 작업 하위 작업 섹션에서 하위 작업 만들기 {#create-subtasks-from-the-task-subtasks-section}

1. 하위 작업을 만들 프로젝트로 이동합니다.
1. 을(를) 클릭합니다. **작업** 왼쪽 패널의 섹션에 있습니다.
1. 하위 작업을 만들 작업의 이름을 클릭합니다.
1. 을(를) 클릭합니다. **하위 작업** 왼쪽 패널의 섹션에 있습니다.
1. 클릭 **새 작업입니다.**

   다음 문서의 단계에 따라 하위 작업을 계속 만듭니다. [프로젝트에서 작업 만들기](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. 클릭 **작업 저장.**

## 하위 작업을 주 작업으로 만들기

1. 하위 작업을 주 작업으로 만들 프로젝트로 이동합니다.
1. 을(를) 클릭합니다. **작업** 왼쪽 패널의 섹션에 있습니다.
1. 주 작업을 수행할 하위 작업을 선택합니다.
1. 을(를) 클릭합니다. **외설** 아이콘 ![](assets/outdent-icon-nwe-31x29.png) 하위 작업을 주 작업으로 만들기 위해

   또는

   표준 영어 QWERTY 키보드에서 Option + &lt;(Mac) 또는 Alt + &lt;(Windows)를 누릅니다. 다른 언어에서는 Option + 명령을 사용할 수 있습니다. (Mac) 또는 Alt + . (Windows) 을 사용하도록 설정합니다.

   >[!NOTE]
   >
   >작업 목록이 작업 번호별로 정렬되고 작업 목록에 적용된 그룹화가 없는 경우에만 작업을 제외할 수 있습니다.
