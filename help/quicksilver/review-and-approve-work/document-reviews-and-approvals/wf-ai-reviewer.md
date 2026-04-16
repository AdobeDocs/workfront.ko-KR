---
product-area: documents
navigation-topic: approvals
title: Workfront 콘텐츠 검토자 시작
description: Workfront 콘텐츠 검토자 AI Collaborator를 사용하여 검토 및 승인 워크플로우 동안 브랜드 지침에 따라 콘텐츠를 평가할 수 있습니다.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 99048cf2b9320b7f00e1de3bae3f48bc145af5f0
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 1%

---

# Workfront 콘텐츠 검토자 시작

콘텐츠 검토자는 프로젝트, 작업 및 문서에 추가할 수 있는 AI 에이전트의 한 유형인 AI 공동 작업자입니다. 설정 영역에서 AI 공동 작업자를 구성하고 사용자와 동일하게 할당할 수 있습니다.

Workfront에서 컨텐츠 검토자는 검토 및 승인 프로세스 전반에 걸쳐 컨텐츠 속도를 높이고 브랜드 준수를 개선하는 데 도움이 됩니다. 콘텐츠 검토자를 승인 템플릿에 추가하거나 개별 검토 및 승인 요청에 포함할 수 있습니다.

## 액세스 요구 사항

Workfront에서 컨텐츠 검토자를 설정하려면 시스템 관리자여야 합니다.

모든 사용자는 검토 및 승인 요청에 콘텐츠 검토자를 추가할 수 있습니다.

## 요구 사항

* Workfront 인스턴스에는 통합 승인이 활성화되어 있어야 합니다.
* 조직에 GenStudio Foundation이 있어야 합니다.
   * Workfront의 컨텐츠 검토자는 자산 검토 및 승인 워크플로에 GenStudio Foundation에서 사용할 수 있는 기능을 제공합니다. 작업을 완료하기 위해 GenStudio Foundation에 직접 액세스할 필요는 없습니다. 콘텐츠 검토자를 통해 GenStudio Foundation 기능에 대한 액세스는 Workfront 계약 조건에 해당됩니다.
* Adobe은 파일에 서명된 Adobe Gen AI 계약이 있어야 합니다.
계약 서명에 대한 자세한 내용은 [Adobe Gen AI 계약 서명](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)을 참조하십시오.


## 지원되는 파일 유형 {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="지원되지 않는 파일 유형"
>abstract="이 콘텐츠 검토자는 선택한 파일 형식을 지원하지 않습니다. 지원되는 파일 유형을 업로드하거나 콘텐츠 검토자를 제거하여 요청을 제출합니다."

콘텐츠 검토자는 다음 파일 유형을 검토할 수 있습니다.

* PNG(.png)
* JPEG (.jpeg, .jpg)
* WEBP (.webp)
* 비 애니메이션 GIF(.gif)
* PDF (.pdf)
* PPT(.ppt, .pptx)
* DOC(.doc, .docx)

지원되지 않는 파일 유형을 업로드하는 경우, 승인 워크플로를 만들 때 콘텐츠 검토자 옵션을 사용할 수 없습니다.

## 브랜드 지침 설정

Workfront 콘텐츠 검토자는 콘텐츠를 검토할 때 브랜드 지침을 사용합니다. Workfront 관리자는 Workfront 설정 영역에서 브랜드 지침을 설정할 수 있습니다. GenStudio Foundation에서 만든 브랜드는 Workfront에서도 사용할 수 있습니다.

브랜드 지침을 설정하려면 시스템 관리자가 다음을 수행해야 합니다.

1. [브랜드 권한에 대한 액세스 권한 부여](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)
1. [콘텐츠 검토자를 위한 브랜드를 만들고 관리하기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).


## 콘텐츠 검토자 만들기

하나 이상의 브랜드가 설정되면 Workfront 관리자는 설정 영역에서 콘텐츠 검토자 생성을 시작할 수 있습니다. 다양한 지침에 초점을 맞춘 여러 콘텐츠 검토자를 만들 수 있습니다.

* **이미지**: 이 콘텐츠 검토자는 Workfront에서 설정한 이미지 브랜드 지침에 따라 자산을 검토합니다. [!BADGE Beta]{type=Positive tooltip="이 기능은 현재 베타 버전입니다."}
   * 시스템 관리자는 이 기능을 사용하려면 Beta 계약서에 서명해야 합니다.
* **브랜드 음성**: 콘텐츠 검토자는 Workfront에서 설정한 브랜드 음성 지침에 따라 자산을 검토합니다.

그런 다음 콘텐츠 검토자를 승인 템플릿과 개별 검토 및 승인 요청에 할당할 수 있습니다.

자세한 내용은 [AI 공동 작업자 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md)을 참조하십시오.

## 검토 및 승인 요청에 콘텐츠 검토자 추가

사용자는 기존 승인 템플릿 또는 개별 검토 및 승인 요청에 콘텐츠 검토자를 추가할 수 있습니다.

### 승인 템플릿

조직에서 검토 및 승인 요청에 동일한 인력을 추가하는 경우가 많은 경우 Standard 라이선스 사용자는 Workfront 설정 영역에서 승인 템플릿을 만들 수 있습니다.

사용자는 템플릿을 사용하여 요청을 만들 때 승인 템플릿에 콘텐츠 검토자를 추가하여 브랜드 준수 여부를 자동으로 확인할 수 있습니다.

승인 템플릿이 생성되면 프로젝트, 작업 또는 문제의 문서 영역에 있는 자산에 적용할 수 있습니다.

자세한 내용은 [문서에 대한 승인 워크플로 템플릿 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)를 참조하십시오.

AI 검토자를 표시하는 ![템플릿 목록](assets/ai-review-templates.png)

### 개별 검토 및 승인 요청

사용자가 개별 검토 및 승인 요청을 만들 때 다른 참가자와 함께 콘텐츠 검토자를 추가하거나 콘텐츠 검토자로만 단일 요청을 만들어 브랜드 준수 여부를 확인할 수 있습니다.

자세한 내용은 [문서 승인 워크플로 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)를 참조하십시오.


![콘텐츠 검토자가 개별 승인 요청에 추가됨](assets/new-stage.png)

## 콘텐츠 검토자 점수 및 피드백 보기

콘텐츠 검토자의 검토 및 승인 요청이 제출된 후 몇 초 후에 콘텐츠 검토자의 점수 및 피드백을 문서 요약 패널에서 사용할 수 있습니다(다른 참가자가 아직 검토 및 결정을 진행 중인 경우에도).

승인 소유자는 에셋에 대한 검토가 완료되었음을 알리는 이메일도 받게 됩니다. 이메일에서 **검토로 이동**&#x200B;을 클릭하고 Workfront에서 점수와 피드백을 확인합니다.

콘텐츠 검토자는 검토 및 승인 워크플로에서 의사 결정자가 되도록 설계되지 않았습니다. 지정된 브랜드 요구 사항에 맞게 에셋을 조정하기 위한 점수 및 권장 사항만 제공합니다.

자산이 브랜드 지침을 충족하지 않는 경우, 크리에이티브는 새 버전을 업로드할 수 있고 승인 소유자는 콘텐츠 검토자와 함께 두 번째 검토 및 승인 요청을 만들 수 있습니다.

점수 및 피드백 보기에 대한 자세한 내용은 [콘텐츠 검토자 점수 및 피드백 보기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md)를 참조하십시오.

