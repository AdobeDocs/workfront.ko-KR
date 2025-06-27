---
product-area: documents
navigation-topic: approvals
title: Workfront AI 검토자 시작
description: Workfront AI 검토자
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
source-git-commit: da980cee8710570f52c724053d1e0f359c6a9fe1
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 3%

---

# Workfront AI 검토자 시작

Workfront AI 검토자를 사용하면 검토 및 승인 작업 과정에서 콘텐츠 속도를 높이고 브랜드 준수를 최적화할 수 있습니다. Workfront에서 승인 템플릿 또는 개별 검토 및 승인 요청에 AI 검토자를 추가할 수 있습니다.

## 액세스 요구 사항

Workfront에서 AI 검토자를 설정하려면 시스템 관리자여야 합니다.

모든 사용자는 검토 및 승인 요청에 AI 검토자를 추가할 수 있습니다.


## 전제 조건

* 조직이 Adobe IMS(Identity Management System)로 마이그레이션되었어야 합니다.
* Workfront 인스턴스에는 통합 승인이 활성화되어 있어야 합니다.
* Adobe은 파일에 서명된 Adobe Gen AI 계약이 있어야 합니다.
계약 서명에 대한 자세한 내용은 [Adobe Gen AI 계약 서명](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)을 참조하십시오.


## 지원되는 파일 유형 {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="지원되지 않는 파일 유형"
>abstract="이 AI 검토자는 선택한 파일 유형을 지원하지 않습니다. 지원되는 파일 유형을 업로드하거나 AI 검토자를 제거하여 요청을 제출하십시오."

AI 검토자는 다음 파일 유형을 검토할 수 있습니다.

* PNG(.png)
* JPEG (.jpeg, .jpg)
* WEBP (.webp)
* 비 애니메이션 GIF(.gif)

## 브랜드 지침 설정

Workfront AI 검토자는 콘텐츠를 검토할 때 Genstudio Foundations에 설정된 브랜드 지침을 사용합니다.

브랜드 지침에 대한 자세한 내용은 다음을 참조하십시오.

* [GenStudio for Performance Marketing 브랜드](https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/guidelines/brands)
* [지침 추가](https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/guidelines/add-guidelines)


## AI 검토자 만들기

GenStudio Foundations에 브랜드가 하나 이상 설정되면 Workfront 관리자는 설정 영역에서 AI 검토자 생성을 시작할 수 있습니다. 그런 다음 해당 AI 검토자를 승인 템플릿과 개별 검토 및 승인 요청에 할당할 수 있습니다.

자세한 내용은 [AI 검토자 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/set-up-ai-reviewer.md)를 참조하십시오.

## 검토 및 승인 요청에 AI 검토자 추가

사용자는 기존 승인 템플릿 또는 개별 검토 및 승인 요청에 AI 검토자를 추가할 수 있습니다.

### 승인 템플릿

조직에서 검토 및 승인 요청에 동일한 인력을 추가하는 경우가 많은 경우 Standard 라이선스 사용자는 Workfront 설정 영역에서 승인 템플릿을 만들 수 있습니다.

사용자는 템플릿을 사용하여 요청을 만들 때 승인 템플릿에 AI 검토자를 추가하여 브랜드 준수 여부를 자동으로 확인할 수 있습니다.

승인 템플릿이 생성되면 프로젝트, 작업 또는 문제의 문서 영역에 있는 자산에 적용할 수 있습니다.

자세한 내용은 [자산 및 문서에 대한 승인 템플릿 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)를 참조하세요.

![AI 검토자를 표시하는 템플릿 목록](assets/ai-review-templates.png)

### 개별 검토 및 승인 요청

사용자가 개별 검토 및 승인 요청을 만들 때 다른 참여자와 함께 AI 검토자를 추가하거나 AI 검토자만 사용하여 단일 요청을 만들어 브랜드 준수 여부를 확인할 수 있습니다.

자세한 내용은 [문서 검토 또는 승인 요청 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)를 참조하십시오.


![AI 검토자가 개별 승인 요청에 추가됨](assets/ad-ai-reviewer-to-request.png)

## AI 검토자 점수 및 피드백 보기

AI 검토자의 검토 및 승인 요청이 제출된 후 몇 초 후에 문서 요약 패널에서 AI 검토자의 점수 및 피드백을 사용할 수 있습니다(다른 참가자가 아직 검토하고 결정을 내리는 경우에도).

승인 소유자는 에셋에 대한 검토가 완료되었음을 알리는 이메일도 받게 됩니다. 이메일에서 **검토로 이동**&#x200B;을 클릭하고 Workfront에서 점수와 피드백을 확인합니다.

AI 검토자는 검토 및 승인 워크플로에서 의사 결정자가 되도록 설계되지 않았습니다. 지정된 브랜드 요구 사항에 맞게 에셋을 조정하기 위한 점수 및 권장 사항만 제공합니다.

이미지가 브랜드 가이드라인을 오랫동안 충족하지 않는 경우 크리에이티브는 새 버전을 업로드하고 승인 소유자는 AI 검토자와 함께 두 번째 검토 및 승인 요청을 만들 수 있으므로 버전 간에 전환하고 피드백을 비교할 수 있습니다.

점수 및 피드백 보기에 대한 자세한 내용은 [AI 검토자 점수 및 피드백 보기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md)를 참조하십시오.


![AI 검토자 피드백](assets/ai-reviewer-feedback.png)


