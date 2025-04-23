---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 프로젝트에 대한 요청 유형 정의
description: 요청 유형별로 Adobe Workfront에 로그인된 문제 또는 요청의 종류를 구성할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 6311526ddf9143c4a979d8bbac96312a3b0e8151
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 2%

---

# 프로젝트에 대한 요청 유형 정의

요청 유형별로 Adobe Workfront에 로그인된 문제 또는 요청의 종류를 구성할 수 있습니다.

이 조직은 프로젝트 수명 동안 어떤 종류의 예기치 않은 작업이 발생할 수 있는지 사용자가 이해할 수 있도록 이유를 보고하고 도움을 주는 데 유용합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
    <p>새로운 기능: 표준</p>
    <p>또는</p>
    <p>현재: 플랜</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 관리</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

시작하기 전에 다음을 수행해야 합니다.

* 프로젝트 보유 또는 생성

  프로젝트 만들기에 대한 자세한 내용은 [프로젝트 만들기](../../../manage-work/projects/create-projects/create-project.md)를 참조하십시오.

## 요청 유형에 대한 고려 사항

* 프로젝트에 대해 **큐 세부 정보** 영역을 구성할 때 프로젝트에 기록할 수 있는 문제 또는 요청의 유형을 지정할 수 있습니다.
* 프로젝트에 대한 요청 유형을 정의할 수 있도록 프로젝트를 요청 대기열로 활성화하지 않아도 됩니다. 프로젝트에 대해 기록된 모든 문제는 다른 요청 유형으로 레이블 지정할 수 있습니다.
* 프로젝트에 대기열 주제를 추가하는 경우 새 문제 또는 요청을 추가할 때 표시할 요청 유형을 각 대기열 주제에 정의해야 합니다. 자세한 내용은 [대기열 주제 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)를 참조하십시오.

## 프로젝트에 대한 문제 또는 요청 유형 정의

{{step1-to-projects}}

1. 프로젝트 이름을 클릭하여 엽니다.
1. 왼쪽 패널에서 **대기열 세부 정보**&#x200B;를 클릭합니다.
1. **큐 속성** 섹션에서 프로젝트에 사용할 **요청 유형**&#x200B;을 선택합니다.

   >[!NOTE]
   >
   >최소 하나 이상의 요청 유형을 선택해야 합니다. 여러 요청 유형을 선택할 수 있습니다.

   다음 유형 중에서 선택합니다.

   * 버그 신고
   * 순서 변경
   * 문제
   * 요청

   >[!TIP]
   >
   >Workfront 관리자가 이러한 옵션 중 일부의 이름을 변경했을 수 있습니다. 자세한 내용은 [요청 유형 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md)을 참조하십시오.

1. **저장**&#x200B;을 클릭합니다.

   지정한 요청 유형은 작업 또는 프로젝트에 새 문제를 입력할 때 또는 프로젝트가 요청 대기열로 활성화되어 있을 경우 프로젝트에 새 요청을 제출할 때 선택할 수 있습니다.
