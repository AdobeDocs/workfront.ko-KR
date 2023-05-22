---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 요청 대기열에 대한 액세스 권한 제공
description: 요청 대기열에 대한 액세스 권한을 제공하면 조직에서 Adobe Workfront의 요청 영역에서 요청 대기열을 볼 수 있는 사용자를 결정합니다.
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 요청 대기열에 대한 액세스 권한 제공

요청 대기열에 대한 액세스 권한을 제공하면 조직에서 Adobe Workfront의 요청 영역에서 요청 대기열을 볼 수 있는 사용자를 결정합니다.

요청 대기열이 프로젝트 팀, 프로젝트 그룹 또는 프로젝트 회사의 일부인지 여부에 따라 다른 사용자에게 요청 대기열에 대한 액세스 권한을 제공할 수 있습니다. 시스템의 모든 사용자에게 요청 대기열에 대한 액세스 권한을 제공할 수도 있습니다. 

이 기능은 외부 관련자를 Workfront에 초대하고 특정 영역에 대한 사용자 액세스를 제한하려는 조직에서 유용합니다. 이 경우 회사 또는 프로젝트 그룹과 연결된 사용자에게만 열려 있는 요청 대기열이 외부 관련자에 대한 가시성을 제한합니다. 누구에게든 액세스 권한을 부여하면 요청이 내부 및 외부 관련자 모두에게 표시됩니다.

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
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p> 프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오

## 전제 조건

요청 영역에서 사용자가 요청 대기열을 사용할 수 있으려면 먼저 다음 설정으로 프로젝트를 만들어야 합니다.

* 요청 대기열로 지정합니다. 요청 대기열 만들기에 대한 자세한 내용은 [요청 대기열 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* 프로젝트의 상태를 현재로 업데이트합니다.

## 요청 대기열에 대한 액세스 권한 제공

1. 요청 대기열에 대한 액세스 권한을 제공하려는 프로젝트로 이동합니다.

   >[!NOTE]
   >
   >현재 상태의 프로젝트만 요청 영역에 표시됩니다.

1. 클릭 **대기열 세부 정보** 왼쪽 패널에서 다음을 클릭해야 할 수 있습니다. **더 보기**, 그런 다음 **대기열 세부 정보**.
1. 선택 **도움말 요청 대기열로 게시** 프로젝트를 요청 대기열로 지정합니다.
1. 다음 옵션 중에서 선택합니다.

   * **모든 사용자**: 모든 사용자는 요청을 보고 요청 대기열에 추가할 수 있습니다.
   * **이 프로젝트에 대한 보기 액세스 권한이 있는 직원**: 프로젝트에 대한 보기 권한이 있는 사용자는 요청을 보고 요청 대기열에 추가할 수 있습니다. 
   * **이 프로젝트 회사의 직원**: 프로젝트의 회사와 연결된 사용자가 요청을 보고 추가할 수 있습니다. 이 옵션 옆에 프로젝트와 연계된 회사가 괄호 안에 나열되어 있습니다. 
   * **이 프로젝트의 그룹에 있는 직원들**:프로젝트의 그룹에 연결된 사용자가 요청을 보고 추가할 수 있습니다. 프로젝트와 연관된 그룹은 이 옵션 옆에 있는 괄호로 표시됩니다.

      그룹 큐는 여러 부서가 고유한 조직 목표를 달성하기 위해 Workfront 계정을 공유할 때 유용합니다. 각 부서에는 다른 그룹의 구성원이 볼 수 없는 고유한 대기열이 있을 수 있습니다.

      프로젝트에 대한 권한이 있는 사람에 대한 자세한 내용은 [Adobe Workfront에서 프로젝트 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).\
      프로젝트를 편집할 때 그룹 및 회사를 프로젝트와 연결할 수 있습니다. 프로젝트 편집에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

1. **저장**&#x200B;을 클릭합니다.
