---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 프로젝트에 대한 요청 유형 정의
description: 요청 유형별로 Adobe Workfront에 로그인된 문제 또는 요청의 종류를 구성할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/fOdoie2wI-EHoKmQTHy0cDaVipi6XYE1JgMHdX6-Tbo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 354
ht-degree: 7%

---

# 프로젝트에 대한 요청 유형 정의

<!-- Audited: 6/2025 -->

요청 유형별로 Adobe Workfront에 로그인된 문제 또는 요청의 종류를 구성할 수 있습니다. 이는 이유를 보고하고 사용자가 프로젝트 수명 동안 발생할 수 있는 예상치 못한 작업 종류를 이해하는 데 유용합니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
    <p>표준</p>
    <p>플랜</p></td>  
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

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

시작하기 전에 다음을 수행해야 합니다.

* 프로젝트를 보유하거나 만듭니다.

  프로젝트 만들기에 대한 자세한 내용은 [프로젝트 만들기](../../../manage-work/projects/create-projects/create-project.md)를 참조하십시오.

## 요청 유형에 대한 고려 사항

* 프로젝트에 대한 대기열 세부 정보 영역을 구성할 때 프로젝트에 기록할 수 있는 문제 또는 요청의 유형을 지정할 수 있습니다.
* 프로젝트에 대한 요청 유형을 정의할 수 있도록 프로젝트를 요청 대기열로 활성화하지 않아도 됩니다. 프로젝트에 대해 기록된 모든 문제는 다른 요청 유형으로 레이블 지정할 수 있습니다.
* 프로젝트에 대기열 주제를 추가하는 경우 새 문제 또는 요청을 추가할 때 표시할 요청 유형을 각 대기열 주제에 정의해야 합니다. 자세한 내용은 [대기열 주제 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)를 참조하십시오.

## 프로젝트에 대한 문제 또는 요청 유형 정의

{{step1-to-projects}}

1. **프로젝트** 페이지에서 프로젝트를 선택하십시오.
1. 왼쪽 패널에서 **대기열 세부 정보**&#x200B;를 클릭합니다.
1. **큐 속성** 섹션에서 프로젝트에 사용할 **요청 유형**&#x200B;을 선택합니다.
   * 버그 신고
   * 순서 변경
   * 문제
   * 요청

   >[!NOTE]
   >
   >* 최소 하나 이상의 요청 유형을 선택해야 합니다. 여러 유형을 선택할 수 있습니다.
   >* Workfront 관리자가 이러한 옵션 중 일부의 이름을 변경했을 수 있습니다. 자세한 내용은 [요청 유형 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md)을 참조하십시오.

1. **저장**&#x200B;을 클릭합니다. 작업 또는 프로젝트에 새 문제를 입력하거나 새 요청을 프로젝트에 제출할 때(프로젝트가 요청 대기열로 활성화된 경우) 지정한 요청 유형을 선택할 수 있습니다.
