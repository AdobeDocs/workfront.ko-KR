---
product-area: documents
navigation-topic: approvals
title: 기존 문서 승인에서 통합 승인으로 이동
description: 조직이 통합 승인을 지원하는 Workfront 버전으로 이동할 때 기존 문서 승인 워크플로가 어떻게 되는지 이해합니다.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 4f63b6c4f4c73bedba707aed6b02c9046f9b356c
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 1%
---
# 기존 문서 승인에서 통합 승인으로 이동

Adobe 클라우드 스토리지 프로젝트는 기본적으로 통합 승인을 사용합니다. 이 문서에서는 기존 문서 승인과 비교하여 통합 승인에서 사용할 수 있는 기능에 대해 설명합니다.


>[!NOTE]
>
>통합 승인은 Adobe 클라우드 스토리지에서 생성된 새 오브젝트에 대한 기본값입니다. 기존 Workfront 스토리지 개체는 현재 승인 서비스를 유지합니다.<br>
>자세한 내용은 [Adobe 클라우드 저장소에서 Workfront으로 이동](/help/quicksilver/review-and-approve-work/workfront-storage.md)을 참조하십시오.

## 기존 문서 승인에서 통합 승인으로 변경되는 내용 이해

|  | 레거시 문서 승인 | 통합 승인 |
| --- | --- | --- |
| 승인자 및 검토자 | 개별 사용자만 승인 | 개별 사용자 또는 팀의 승인 또는 검토 |
| 기한 및 알림 | 자동 미리 알림 없음 | 자동화된 미리 알림은 72시간 후, 24시간 후 및 날짜에 |
| 승인 단계 및 경로 | 하나의 승인 단계, 병렬 경로 없음 | [여러 승인 단계 및 병렬 검토 경로](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) |
| 승인 템플릿 | 각 승인이 처음부터 구성됨 | Workfront 설정에서 [재사용 가능한 템플릿](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) 사용 가능 |
| 검토 및 마크업 | 증명 뷰어 | 기존 Workfront 저장소 개체의 [증명 뷰어](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md) 또는 Adobe 클라우드 저장소 개체의 [Frame.io 뷰어](/help/quicksilver/review-and-approve-work/workfront-storage.md#review-and-approval-viewer) |
| AI 지원 검토 | 사용할 수 없음 | [콘텐츠 검토자](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)를 통한 자동 브랜드 준수 확인 |
| 보고 | 이전 보고 | 홈 KPI 위젯 및 [캔버스 대시보드](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) |

### 이미 진행 중인 승인에 나타나는 결과

기존 문서 승인에서 생성된 진행 중 승인은 이전과 마찬가지로 계속 작동합니다. Adobe 클라우드 스토리지 개체에 대한 새로운 승인은 통합 승인을 사용합니다. 기존 Workfront 스토리지 개체에 대한 새 승인은 해당 개체가 이미 사용하고 있는 승인 서비스를 유지합니다.


## 이동 준비

* 최종 사용자와 [통합 검토 및 승인 시작하기](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) 문서를 공유합니다.
* 기존 Workfront Fusion 시나리오를 검토하십시오. 증명이 포함된 레거시 문서 승인을 사용하는 경우 Adobe 클라우드 스토리지로 팀을 가져오기 전에 [통합 검토 및 승인을 위해 Workfront Fusion 시나리오 업데이트](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md)를 참조하십시오.
* 캔버스 대시보드에서 검토 및 승인 대시보드를 설정하여 기존 승인 보고서를 바꿉니다. 자세한 내용은 [검토 및 승인 대시보드 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md)를 참조하십시오.


### 최종 사용자를 위한 도움말 문서

* [통합 검토 및 승인 시작](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [문서 승인에 사용 가능한 기능](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md)
* [통합 검토 및 승인 개요](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Frame.io 뷰어로 검토 및 승인](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)
* [통합 승인 및 증명 함께 사용](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)
* [문서 의사 결정 상태 개요](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)
* [Workfront 콘텐츠 검토자 시작](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)
