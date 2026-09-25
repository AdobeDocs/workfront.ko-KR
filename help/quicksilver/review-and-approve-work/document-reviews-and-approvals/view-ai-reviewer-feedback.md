---
product-area: documents
navigation-topic: approvals
title: AI 검토자 점수 및 피드백 보기
description: 승인 요청을 제출한 후 몇 초 후에 문서 요약 패널에서 AI 검토자의 점수와 피드백을 볼 수 있습니다.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 838e8f3d-0ea6-4844-a261-ef7b0e78a755
TQID: 'https://experienceleague.adobe.com/iPlcSTaPI-zhmWvRvO81RKFYnIzUoJqzM70mNcxrVbs'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%
---
# AI 검토자 점수 및 피드백 보기

검토 및 승인 요청을 제출한 후 몇 초 후에 문서 요약 패널에서 AI 검토자의 점수와 피드백을 볼 수 있습니다.

AI 검토자는 검토 및 승인 워크플로에서 의사 결정자가 되도록 설계되지 않았습니다. 지정된 브랜드 요구 사항에 맞게 에셋을 조정하기 위한 점수 및 권장 사항만 제공합니다.

![AI 검토자 피드백](assets/ai-reviewer-output.png)

## 점수 계산 방법 이해

AI 검토자는 검토 유형에 따라 점수를 다르게 계산합니다.

* 이미지 검토: 이 점수는 통과한 지침과 실패한 지침의 비율을 반영합니다.
* 검토 복사: 이 점수는 주관적 및 객관적 결과의 균형 잡힌 가중치를 사용합니다. 목표 지침(&quot;수정&quot; 아래에 표시됨)은 주관적 지침(&quot;고려&quot; 아래에 표시됨)보다 세 배 더 가중치가 적용됩니다.

객관적인 가이드라인은 복사 검토에 더 많은 비중을 가지므로 브랜드에서 구체적이고 측정 가능한 가이드라인을 작성하는 것이 좋습니다. 자세한 내용은 AI 검토자의 브랜드 만들기 및 관리 문서에서 [브랜드 지침 작성에 대한 모범 사례](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md#best-practices-for-writing-brand-guidelines) 섹션을 참조하십시오.

## 점수 및 피드백 보기

AI 검토자의 점수와 피드백은 문서 요약 패널 또는 문서 세부 정보 페이지의 승인 탭에서 확인할 수 있습니다.

1. Workfront 알림 전자 메일에서 **검토로 이동**&#x200B;을 클릭합니다.

   또는

   문서가 업로드된 문서 영역으로 이동하여 문서 요약 패널을 엽니다.
1. **점수**&#x200B;를 클릭합니다.
   ![문서 점수 보기](assets/view-score.png)

점수 및 피드백 창에서 AI 검토자는 자산이 지정된 지침을 어떻게 충족하지 못하는지 설명합니다.
![AI 검토자 피드백에 주의가 필요합니다](assets/ai-reviewer-needs-attention.png)

## 새 버전 업로드 및 AI 검토자 다시 추가

AI 리뷰어의 피드백을 바탕으로 에셋을 조정해야 하는 경우, 새로운 버전을 업로드하고 새로운 리뷰를 시작할 수 있다.

자세한 내용은 [새 문서 버전 업로드 및 승인 요청](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/upload-new-doc-version.md)을 참조하십시오.
