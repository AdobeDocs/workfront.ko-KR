---
product-area: documents
navigation-topic: approvals
title: AI 검토자 만들기
description: Workfront에 브랜드를 하나 이상 설정한 후에는 여러 AI 검토자를 만들어 승인 템플릿과 개별 검토 및 승인 요청에 할당할 수 있습니다.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
exl-id: 4673049e-119e-4315-95f0-f10d8b286856
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/sfM3OtA-DVqywr3Up8VGjcycLRs5WtF22dcpXzRlnvQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 290
ht-degree: 8%

---

# AI 검토자 만들기

>[!NOTE]
>
>이 기능은 현재 베타 버전입니다.

Workfront에 브랜드를 하나 이상 설정한 후에는 여러 AI 검토자를 만들어 승인 템플릿과 개별 검토 및 승인 요청에 할당할 수 있습니다.


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
   <td> <p>표준</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 관리자여야 합니다.</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

시작하기 전에 Workfront에서 이미지 브랜드 지침을 설정해야 합니다. 자세한 내용은 [콘텐츠 검토자를 위한 브랜드 만들기 및 관리](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)를 참조하십시오.

## AI 검토자 추가

>[!NOTE]
>
>AI 검토자는 검토 및 승인 워크플로에서 의사 결정자가 되도록 설계되지 않았습니다. 지정된 브랜드 요구 사항에 맞게 에셋을 조정하기 위한 점수 및 권장 사항만 제공합니다.

콘텐츠 검토자를 추가하려면 다음 작업을 수행하십시오.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **검토 및 승인** > **AI 검토자**(으)로 이동합니다.
1. **새로 추가**&#x200B;를 클릭합니다.
1. 검토자 이름을 지정합니다.
1. **브랜드**&#x200B;를 선택하십시오.
1. **지침 유형** 드롭다운 메뉴에서 다음 중 하나를 선택합니다.
   * **이미지**: AI 검토자는 Workfront에서 설정한 이미지 브랜드 지침에 따라 자산을 검토합니다.
   * **브랜드 음성**: AI 검토자는 Workfront에서 설정한 브랜드 음성 지침에 따라 자산을 검토합니다.
1. Click **Create**.

   AI 검토자가 생성되면 사용자는 승인 템플릿 또는 개별 승인에 AI 검토자를 추가할 수 있습니다.

   자세한 내용은 다음 문서를 참조하십시오.

   * [문서에 대한 승인 워크플로 템플릿 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
   * [문서 승인 워크플로 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)
