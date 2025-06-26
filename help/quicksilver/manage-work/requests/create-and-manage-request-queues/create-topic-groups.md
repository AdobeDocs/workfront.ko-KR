---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 주제 그룹 만들기
description: 주제 그룹은 요청 대기열과 연관됩니다. 요청 특성에 따라 요청 대기열을 여러 카테고리에 계층화할 수 있습니다.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 7c5959f4-f33f-4f5e-b031-748dbe1a24a5
source-git-commit: 0da05d048d0dab1c2f06870e589c1349c48ccc58
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# 주제 그룹 만들기

<!-- Audited: 2/2024 -->

주제 그룹은 요청 대기열과 연관됩니다. 주제 그룹을 사용하여 요청의 특성에 따라 요청 대기열을 여러 카테고리에 계층화할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront 라이선스</p> </td> 
   <td>   
      <p>새로운 기능: 표준</p>
      <p>또는</p> 
      <p>현재: 플랜</p>
 </td> 
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

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 주제 그룹 개요

예를 들어 마케팅 요청에 대한 요청 대기열이 있는 경우 &quot;어머니날 캠페인&quot;이라는 주제 그룹과 &quot;디지털 미디어&quot;라는 두 번째 수준 주제 그룹 및 &quot;인쇄 미디어&quot;라는 추가 두 번째 수준 주제 그룹이 있을 수 있습니다. 그런 다음 각 주제 그룹 내에 여러 개의 대기열 주제를 가질 수 있습니다. 예를 들어 &quot;배너 광고&quot; 및 &quot;블로그&quot;는 &quot;디지털 미디어&quot; 주제 그룹의 대기열 주제일 수 있습니다.

요청 대기열을 만드는 방법에 대한 자세한 내용은 [요청 대기열 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)를 참조하십시오.

주제 그룹으로 작업할 때 다음 사항을 고려하십시오.

* 요청 대기열 내에 최대 10개의 주제 그룹 계층을 만들 수 있습니다.
* 주제 그룹과 연결할 수 있는 대기열 주제 수에는 제한이 없습니다.
* 주제 그룹은 보고 가능한 객체입니다.
* 한 프로젝트에서 다른 프로젝트로 주제 그룹을 이동할 수 없습니다.

## 주제 그룹 만들기

대기열 주제를 생성하기 전에 주제 그룹을 생성하는 것이 좋습니다. 그러나 대기열 주제 빌더에서 주제 그룹을 생성할 수 있습니다. 대기열 주제 만들기에 대한 자세한 내용은 [대기열 주제 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)를 참조하십시오.

주제 그룹을 생성하려면

1. 도움말 요청 대기열로 게시한 프로젝트로 이동합니다.\
   프로젝트를 도움말 요청 대기열로 게시하는 방법에 대한 자세한 내용은 [요청 대기열 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)를 참조하십시오.

1. 왼쪽 패널에서 **주제 그룹**&#x200B;을 클릭합니다.
1. **새 주제 그룹**&#x200B;을 클릭합니다.

   <!--   ![](assets/new-topic-group-box-nwe-350x306.png) -->

1. 다음 정보를 지정합니다.

   * **이름**: 이 요청 대기열에 요청을 제출하는 사용자에게 이 이름이 표시됩니다.
   * **설명**: 사용자가 새 요청을 제출하는 과정에서 주제 그룹을 선택할 때 설명이 표시됩니다.
   * **주제 그룹에 추가**: 새 주제 그룹을 기존 주제 그룹에 추가하거나 도움말 요청 대기열로 게시된 프로젝트에 직접 추가할 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.\
   이렇게 하면 요청 대기열에 새 주제 그룹이 만들어집니다. 이제 요청 대기열 아래의 첫 번째 드롭다운 메뉴에서 추가 범주를 선택할 수 있습니다.\
   요청 제출에 대한 자세한 내용은 [Adobe Workfront 요청 만들기 및 제출](../../../manage-work/requests/create-requests/create-submit-requests.md)을 참조하십시오.
1. 기존 주제 그룹을 편집하려면 주제 그룹 목록에서 주제 그룹을 선택한 다음 열리는 창에서 세부 정보를 편집합니다. 변경 내용을 저장하려면 **저장**&#x200B;을 클릭하세요.
