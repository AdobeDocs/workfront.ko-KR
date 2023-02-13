---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 주제 그룹 만들기
description: 항목 그룹은 요청 큐와 연결됩니다. 이를 통해 요청의 특성에 따라 여러 카테고리로 요청 큐를 계층화할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 7c5959f4-f33f-4f5e-b031-748dbe1a24a5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# 주제 그룹 만들기

항목 그룹은 요청 큐와 연결됩니다. 이를 통해 요청의 특성에 따라 여러 카테고리로 요청 큐를 계층화할 수 있습니다.

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
   <td role="rowheader"> <p role="rowheader">Adobe Workfront 라이선스*</p> </td> 
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

## 항목 그룹 개요

예를 들어, 마케팅 요청에 대한 요청 큐가 있는 경우, &quot;어머니 날의 캠페인&quot; 주제 그룹과, 두 번째 수준의 &quot;디지털 미디어&quot; 주제 그룹과, 두 번째 수준의 &quot;미디어 인쇄&quot; 주제 그룹이 있을 수 있습니다. 그런 다음 각 주제 그룹 내에 여러 큐 주제를 가질 수 있습니다. 예를 들어 &quot;배너 광고&quot; 및 &quot;블로그&quot;는 &quot;디지털 미디어&quot; 항목 그룹의 큐 항목일 수 있습니다.

요청 큐를 만드는 방법에 대한 자세한 내용은 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!TIP]
>
>* 요청 큐 내에서 최대 10개의 주제 그룹 계층을 만들 수 있습니다.
>* 항목 그룹과 연결할 수 있는 큐 주제 수에는 제한이 없습니다.
>* 항목 그룹은 보고 가능한 개체입니다.
>


## 주제 그룹 만들기

큐 항목을 만들기 전에 주제 그룹을 만드는 것이 좋습니다. 하지만 큐 주제 빌더에서 주제 그룹을 만들 수 있습니다. 큐 항목 만들기에 대한 자세한 내용은 [큐 항목 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

주제 그룹을 생성하려면

1. 도움말 요청 큐로 게시한 프로젝트로 이동합니다.\
   프로젝트를 도움말 요청 큐로 게시하는 방법에 대한 자세한 내용은 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. 클릭 **주제 그룹** 왼쪽 패널에 표시됩니다. 을(를) 클릭하여 **자세히 표시**, 그런 다음 **주제 그룹**.
1. 클릭 **새 주제 그룹**.

   ![](assets/new-topic-group-box-nwe-350x306.png)

1. 다음 정보를 지정합니다.

   * **이름**: 이 요청 큐에 요청을 제출하는 사용자가 이 이름을 볼 수 있습니다.
   * **설명**: 설명은 사용자가 새 요청을 제출하는 프로세스에서 항목 그룹을 선택하면 표시됩니다.
   * **주제 그룹에 추가**: 새 주제 그룹을 기존 주제 그룹에 추가하거나 도움말 요청 대기열로 게시된 프로젝트에 직접 추가할 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.\
   이렇게 하면 요청 큐에서 새 주제 그룹이 만들어집니다. 이제 요청 큐 아래의 첫 번째 드롭다운 메뉴에서 추가 카테고리를 선택할 수 있습니다.\
   요청 제출에 대한 자세한 내용은 [Adobe Workfront 요청 만들기 및 제출](../../../manage-work/requests/create-requests/create-submit-requests.md).
