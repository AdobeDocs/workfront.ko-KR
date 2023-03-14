---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 요청 큐에 대한 액세스 제공
description: 요청 큐에 대한 액세스 권한을 제공하면 조직 내에서 Adobe Workfront의 요청 영역에서 요청 큐를 볼 수 있는 사용자를 결정합니다.
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: ''
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 요청 큐에 대한 액세스 제공

요청 큐에 대한 액세스 권한을 제공하면 조직 내에서 Adobe Workfront의 요청 영역에서 요청 큐를 볼 수 있는 사용자를 결정합니다.

프로젝트 팀, 프로젝트 그룹 또는 프로젝트 회사에 속해 있는지에 따라 다른 사용자에게 요청 큐에 대한 액세스 권한을 제공할 수 있습니다. 시스템의 모든 사용자에게 요청 큐에 대한 액세스 권한을 제공할 수도 있습니다. 

이 기능은 외부 이해 당사자를 Workfront에 초대하고 사용자의 액세스를 특정 영역으로 제한하려는 조직에서 유용합니다. 이 경우 회사 또는 프로젝트 그룹과 연결된 사용자만 요청 큐를 열어 외부 이해 당사자에게 가시성을 제한합니다. 누구나 액세스할 수 있도록 허용하면 내부 및 외부 이해 관계자가 요청을 볼 수 있습니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p> 프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오

## 전제 조건

요청 영역의 사용자가 요청 큐를 사용할 수 있으려면 먼저 다음 설정을 사용하여 프로젝트를 만들어야 합니다.

* 요청 큐로 지정합니다. 요청 큐 만들기에 대한 자세한 내용은 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* 프로젝트의 상태 를 현재 로 업데이트합니다.

## 요청 큐에 대한 액세스 제공

1. 요청 큐에 대한 액세스를 제공할 프로젝트로 이동합니다.

   >[!NOTE]
   >
   >현재 상태인 프로젝트만 요청 영역에 표시됩니다.

1. 클릭 **큐 세부 정보** 왼쪽 패널에 표시됩니다. 을(를) 클릭하여 **자세히 표시**, 그런 다음 **큐 세부 정보**.
1. 선택 **도움말 요청 큐로 게시** 프로젝트를 요청 큐로 지정합니다.
1. 다음 옵션 중에서 선택합니다.

   * **누구든**: 모든 사용자는 요청 큐를 보고 추가할 수 있습니다.
   * **이 프로젝트에 대한 액세스 권한이 있는 사람**: 프로젝트에 대한 보기 권한이 있는 사용자는 요청을 보고 요청 큐에 추가할 수 있습니다. 
   * **이 프로젝트 회사의 사람**: 프로젝트의 회사와 연결된 사용자는 요청을 보고 추가할 수 있습니다. 프로젝트와 연결된 회사는 이 옵션 옆에 괄호 안에 나열됩니다. 
   * **이 프로젝트 그룹의 사람**: 프로젝트의 그룹과 연결된 사용자는 요청을 보고 추가할 수 있습니다. 프로젝트와 연결된 그룹은 이 옵션 옆에 괄호 안에 나열됩니다.

      여러 부서가 Workfront 계정을 공유하여 고유한 조직 목표를 달성하는 경우 그룹 큐가 유용합니다. 각 부서에는 다른 그룹의 구성원들이 볼 수 없는 고유한 큐가 있을 수 있습니다.

      프로젝트에 대한 권한이 있는 사람에 대한 자세한 내용은 [Adobe Workfront에서 프로젝트 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).\
      프로젝트를 편집할 때 그룹 및 회사를 프로젝트와 연결할 수 있습니다. 프로젝트 편집에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

1. **저장**&#x200B;을 클릭합니다.
