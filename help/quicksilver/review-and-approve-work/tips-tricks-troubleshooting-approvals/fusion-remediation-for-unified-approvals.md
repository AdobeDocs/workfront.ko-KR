---
product-area: documents
navigation-topic: approvals
title: 통합 검토 및 승인을 위해 Workfront Fusion 시나리오 업데이트
description: 조직에서 Workfront 클라우드 스토리지와 통합 검토 및 승인을 채택함에 따라 레거시 Workfront 증명을 기반으로 구축된 Adobe Fusion 시나리오를 인벤토리, 분류 및 수정합니다.
author: Courtney
feature: Work Management, Digital Content and Documents
role: Admin
source-git-commit: a3ef3b4ea00298e23ebc8b6196c951417e75eebe
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 0%

---

# 통합 검토 및 승인을 위해 Workfront Fusion 시나리오 업데이트

기존 Workfront 증명을 기반으로 구축된 Workfront Fusion 시나리오는 Adobe 클라우드 스토리지 프로젝트에 대해 자동으로 작동하지 않습니다. 증명별 모듈, 웹후크 및 API 엔드포인트는 경우에 따라 직접적인 등가물을 가지며 다른 경우에는 상당한 변경을 가집니다. 이 문서는 이러한 시나리오에 의존하는 팀을 Adobe 클라우드 스토리지 롤아웃으로 가져오기 전에 영향을 받는 시나리오를 인벤터리하고, 분류하고, 수정 경로를 결정하는 데 도움이 됩니다.

기존 Workfront 프로젝트에 범위가 지정된 시나리오는 오늘날과 같이 계속 작동합니다. 이 문서에 설명된 수정 작업은 Adobe 클라우드 스토리지 프로젝트에 대해 실행하려는 시나리오에 적용됩니다.

>[!IMPORTANT]
>
>이제 Adobe Workfront Fusion에서 Workfront 통합 검토 및 승인 커넥터를 사용할 수 있습니다. Adobe 클라우드 스토리지와 Fusion을 사용할 때 보다 간단하고 안정적인 시나리오를 위해서는 이 커넥터를 사용하는 것이 좋습니다.
>
>자세한 내용 및 지침은 Adobe Workfront Fusion 설명서의 [Workfront 통합 검토 및 승인 모듈](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-review-and-approvals-modules)을 참조하십시오.

이 문서를 사용하여 시나리오를 인벤터리하고 분류하여 Adobe 클라우드 스토리지를 고려하여 Fusion 시나리오를 업그레이드하는 최상의 방법을 이해합니다.

조직이 Adobe 클라우드 스토리지의 Workfront으로 이동할 때 변경되는 사항에 대한 높은 수준의 요약을 보려면 [Adobe 클라우드 스토리지의 Workfront으로 이동](/help/quicksilver/review-and-approve-work/workfront-storage.md)을 참조하십시오.


## Adobe 클라우드 스토리지 프로젝트의 Fusion 변경 사항

Workfront Proof을 기반으로 구축된 기존 Fusion 시나리오는 통합 검토 및 승인 데이터 모델의 일부가 아닌 증명별 모듈, 웹후크 트리거 및 API 엔드포인트를 사용합니다. 아래 표는 일반적인 시나리오 유형을 예상 영향과 향후 경로에 매핑합니다.

| 시나리오 유형 | 영향 | 앞으로 경로 |
|---|---|---|
| 증명 생성 및 라우팅 | 중단 | 2026년 3사분기에 통합 승인 API를 사용하여 재구축 |
| 증명 상태 웹후크 | 중단 | 2026년 3사분기의 새로운 승인 이벤트 트리거를 사용하여 재구축 |
| 문서 업로드 트리거 | 부분: 다시 테스트 필요 | 2026년 3분기 마이그레이션 후 감사 및 재테스트 |
| 승인 미리 알림 | 중단 | 승인 템플릿 기한으로 바꾸기 |
| 승인 결정 라우팅 | 중단 | 새 결정 상태 필드를 사용하여 다시 빌드 |
| 사용자 정의 승인 보고 | 부분: 필드 이름이 변경될 수 있음 | 레거시 필드를 새 스키마에 매핑 |


## 각 시나리오를 편집, 다시 작성 또는 사용 중지로 분류

각 시나리오에 필요한 작업은 수행하는 작업과 통합 검토 및 승인에서 사용할 수 있는 작업에 따라 다릅니다. 다음 분류를 사용합니다.

* **편집**: 기존 증명 관련 작업에 통합 검토 및 승인과 직접적인 동등한 작업이 있으며 새 작업을 사용하도록 시나리오를 업데이트할 수 있습니다.
* **다시 빌드**: 기본 단계가 크게 변경되었거나 시나리오가 사용해야 하는 새 기능이 있으므로 시나리오를 처음부터 다시 빌드해야 합니다.
* **중단**: 기한 미리 알림이 있는 다단계 승인 템플릿과 같은 기본 통합 검토 및 승인 기능은 시나리오가 빌드된 작업을 대체합니다.

특정 비즈니스 논리에 따라 각 시나리오를 검토하여 해당 분류를 결정합니다.

## 교정 접근 방식

다음 접근 방식을 사용하여 Fusion 수정을 계획하고 실행합니다.

1. **지금 인벤토리** 활성 Fusion 시나리오의 전체 목록을 가져와서 증명 생성, 증명 상태, 문서 승인 또는 승인 라우팅을 참조하는 모든 시나리오에 태그를 지정합니다. Adobe 클라우드 스토리지가 활성화될 때까지 기다리지 마십시오.
1. **이전 섹션의 조건을 기준으로 각 시나리오를 편집, 다시 작성 또는 사용 중지로 분류**&#x200B;합니다.
1. 증명 종속 시나리오를 **일시 중지**&#x200B;한 후 해당 시나리오에 종속된 팀을 Adobe 클라우드 저장소 파일럿으로 가져옵니다. 새 모델에 대해 오래된 증명 기반 자동화를 실행하면 자동 오류가 발생하거나 작업이 중복될 수 있습니다.
1. **승인 템플릿을 사용하여 간단한 라우팅 논리를 바꾸십시오.** 기한 자동화를 사용하는 기본 다단계 승인 템플릿은 이전에 Fusion이 필요했던 많은 사용 사례를 처리할 수 있습니다. 자세한 내용은 [자산 및 문서에 대한 승인 템플릿 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)를 참조하십시오.
1. **다시 빌드할 때 Adobe Workfront 통합 검토 및 승인 커넥터를 사용합니다.** 업데이트된 커넥터는 통합 검토 및 승인을 위해 특별히 빌드된 모듈을 노출하고 재빌드를 훨씬 더 간단하고 안정적으로 만듭니다. Workfront API 버전 22에 대해서는 이전에 다시 빌드하지 않는 것이 좋습니다.
1. **프로덕션 환경에서 활성화하기 전에 샌드박스 인스턴스에서 처음부터 끝까지 다시 빌드된 시나리오를 테스트합니다**. 이벤트 구독 페이로드에 특별히 주의하십시오. 필드 이름과 스키마는 기존 증명 이벤트와 다릅니다.

>[!TIP]
>
>많은 조직이 기존 증명 시 발생한 차이를 해결하기 위해 Fusion 시나리오를 축적했습니다. 승인 템플릿, 기한 미리 알림, 다단계 라우팅 등 기본 통합 검토 및 승인 기능을 사용하면 이러한 시나리오 중 일부가 완전히 필요하지 않습니다. 각 시나리오를 분류할 때 기본 피쳐를 대체할 수 있는지 여부를 평가합니다. 시나리오를 폐기하는 것이 시나리오를 재구축하는 것보다 종종 더 깨끗한 장기적 결과입니다.

## 관련 문서

* [Adobe 클라우드 스토리지의 Workfront으로 이동](/help/quicksilver/review-and-approve-work/workfront-storage.md)
* [통합 검토 및 승인 개요](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [통합 검토 및 승인 시작](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [자산 및 문서에 대한 승인 템플릿 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
