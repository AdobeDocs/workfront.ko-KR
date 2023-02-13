---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 프로젝트에 대한 요청 유형 정의
description: 요청 유형별로 Adobe Workfront에 로그인한 문제 또는 요청의 종류를 구성할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 2%

---

# 프로젝트에 대한 요청 유형 정의

요청 유형별로 Adobe Workfront에 로그인한 문제 또는 요청의 종류를 구성할 수 있습니다.

이 조직은 보고 이유 및 프로젝트 라이프타임 동안 발생할 수 있는 예기치 않은 작업의 종류를 사용자가 이해할 수 있도록 돕는 데 유용합니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront 플랜</a>*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Adobe Workfront 라이선스</a>*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하기 전에

* 프로젝트 있음 또는 생성

   프로젝트 만들기에 대한 내용은 [프로젝트 만들기](../../../manage-work/projects/create-projects/create-project.md).

## 요청 유형에 대한 고려 사항

* 구성 시 프로젝트에 기록할 수 있는 문제 또는 요청의 유형을 지정할 수 있습니다 **큐 세부 정보** 프로젝트 영역입니다.
* 프로젝트에 대한 요청 유형을 정의하기 위해 프로젝트를 요청 대기열로 활성화할 필요가 없습니다. 프로젝트에 대해 기록된 모든 문제는 다른 요청 유형으로 레이블이 지정될 수 있습니다.
* 프로젝트에 큐 항목을 추가하는 경우 새 문제 또는 요청을 추가할 때 표시할 각 큐 항목에서 요청 유형 을 정의해야 합니다. 자세한 내용은 [큐 항목 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## 프로젝트에 대한 문제 또는 요청 유형을 정의합니다

1. 클릭 **프로젝트** 를 클릭합니다. ![](assets/main-menu-icon.png)

1. 프로젝트 이름을 클릭하여 엽니다.
1. 왼쪽 패널에서 **큐 세부 정보**.
1. 에서 **큐 속성** 섹션에서 **요청 유형** 프로젝트를 위해

   >[!NOTE]
   >
   >하나 이상의 요청 유형을 선택해야 합니다. 여러 요청 유형을 선택할 수 있습니다.

   다음 유형 중에서 선택합니다.

   * 버그 신고
   * 순서 변경
   * 문제
   * 요청

   >[!TIP]
   >
   >Workfront 관리자가 이러한 옵션 중 일부의 이름을 변경했을 수 있습니다. 자세한 내용은 [요청 유형 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. **저장**&#x200B;을 클릭합니다.

   지정한 요청 유형은 작업 또는 프로젝트에 새 문제를 입력할 때 또는 프로젝트를 요청 큐로 사용할 수 있는 경우 프로젝트에 새 요청을 제출할 때 선택할 수 있습니다.
