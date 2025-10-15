---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 요청 대기열에 대한 액세스 권한 제공
description: 요청 대기열에 대한 액세스 권한을 제공하면 조직에서 Adobe Workfront의 요청 영역에서 요청 대기열을 볼 수 있는 사용자를 결정합니다.
author: Becky
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: 9cdf3d78e1d19f3d581f8d527919a608c5cc0ddc
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 1%

---

# 요청 대기열에 대한 액세스 권한 제공

<!-- Audited: 6/2025 -->

요청 대기열에 대한 액세스 권한을 제공하면 조직에서 Adobe Workfront의 요청 영역에서 요청 대기열을 볼 수 있는 사용자를 결정합니다.

프로젝트 팀, 프로젝트 그룹 또는 프로젝트 회사의 구성원인지 여부에 따라 요청 대기열에 대한 다양한 액세스 권한을 제공할 수 있습니다. 시스템의 모든 사용자에게 요청 대기열 액세스 권한을 제공할 수도 있습니다.

이 기능은 외부 이해 당사자를 Workfront에 초대하고 특정 영역에 대한 사용자 액세스를 제한하려는 조직에서 유용합니다. 이 경우 프로젝트 회사 또는 그룹과 관련된 사용자에게만 열리는 요청 대기열은 외부 관련자에 대한 가시성을 제한합니다. 누구에게든 액세스 권한을 부여하면 요청이 내부 및 외부 관련자 모두에게 표시됩니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>표준 </p>
   <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p> 프로젝트에 대한 권한 관리</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

요청 영역에서 사용자가 요청 대기열을 사용할 수 있으려면 먼저 다음 설정으로 프로젝트를 만들어야 합니다.

* 요청 대기열로 지정합니다. 자세한 내용은 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)를 참조하세요.
* 프로젝트의 상태를 현재로 업데이트합니다.

## 요청 대기열에 대한 액세스 권한 제공

1. 요청 대기열에 대한 액세스 권한을 제공하려는 프로젝트로 이동합니다.

   >[!NOTE]
   >
   >현재 상태의 프로젝트만 요청 영역에 표시됩니다.

1. 왼쪽 패널에서 **큐 세부 정보**&#x200B;를 클릭합니다.
1. **도움말 요청 대기열로 게시**&#x200B;를 선택하여 프로젝트를 요청 대기열로 지정합니다.
1. 표시되는 다음 옵션 중에서 선택합니다.

   * **모든 사용자**: 모든 사용자는 요청을 보고 요청 큐에 추가할 수 있습니다.
   * **이 프로젝트에 대한 보기 액세스 권한이 있는 사용자**: 프로젝트에 대한 보기 권한이 있는 사용자는 요청을 보고 요청 큐에 추가할 수 있습니다.
   * **이 프로젝트의 회사에 있는 직원**: 프로젝트의 회사와 연결된 사용자가 요청을 보고 추가할 수 있습니다. 이 옵션 옆에 프로젝트와 연계된 회사가 괄호 안에 나열되어 있습니다.
   * **이 프로젝트의 그룹에 있는 사용자**: 프로젝트의 그룹에 연결된 사용자가 요청을 보고 추가할 수 있습니다. 프로젝트와 연관된 그룹은 이 옵션 옆에 있는 괄호로 표시됩니다.

     그룹 큐는 여러 부서가 고유한 조직 목표를 달성하기 위해 Workfront 계정을 공유할 때 유용합니다. 각 부서에는 다른 그룹의 구성원이 볼 수 없는 고유한 대기열이 있을 수 있습니다.

     프로젝트에 대한 권한이 있는 사용자에 대한 자세한 내용은 [Adobe Workfront에서 프로젝트 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)를 참조하십시오.

     프로젝트를 편집할 때 그룹 및 회사를 프로젝트와 연결할 수 있습니다. 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md)을 참조하세요.

1. **저장**&#x200B;을 클릭합니다.
