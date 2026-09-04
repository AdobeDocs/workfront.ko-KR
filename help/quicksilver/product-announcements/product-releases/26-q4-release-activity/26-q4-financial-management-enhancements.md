---
title: 2026년 4분기 재무 관리 개선 사항
description: 2026년 4분기 재무 관리 개선 사항
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 4ca5bba5090d9e3a72c8964bdf6cca1085c314db
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 2026년 4분기 재무 관리 개선 사항

이 페이지에서는 미리보기 환경에 대한 2026년 4분기 릴리스의 Financial Management 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2026년 4분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2026년 4분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)를 참조하십시오.

## 회사 청구 요금 개선

>[!NOTE]
>
>미리 보기: 2026년 9월 3일
>프로덕션 빠른 릴리스: 2026년 9월 17일
>모두를 위한 프로덕션: 2026년 10월 15일

회사 청구 요금 기능이 여러 번 업데이트되었습니다.

### 모든 Workfront 및 워크플로 패키지의 고객

* Workfront의 다른 영역과 일관된 보다 현대적인 디자인으로 회사 청구 요금을 추가 및 편집하기 위한 대화 상자를 업데이트했습니다.
* &quot;회사 수준의 청구 요금이 프로젝트 수준의 청구 요금을 재정의할 수 있도록 허용&quot; 설정은 회사가 프로젝트에 추가되면 요금 재정의를 올바르게 추가하며, 계획된 수익 계산에서는 회사 수준의 청구 요금을 사용합니다.
* 프로젝트 수준에서 일반 재무 편집 및 청구 요금 편집 액세스 권한이 없는 사용자는 더 이상 해당 프로젝트에 회사를 추가할 수 없습니다.

### Workflow Ultimate 패키지의 고객만 해당

이제 요금 속성을 회사 수준의 청구 요금에 적용할 수 있습니다. 유효 일자는 회사 비율에도 적용할 수 있습니다.

주: 회사 레벨 환율이 환율 계층에 추가되지 않았습니다.

자세한 내용은 [회사 수준의 작업 역할 청구 요금 무시](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md) 및 [회사 수준의 청구 요율로 프로젝트 수준의 청구 요금 무시](/help/quicksilver/manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md)를 참조하십시오.

## 이제 속성 계층은 자동으로 연결된 상태로 유지됩니다.

>[!NOTE]
>
>미리 보기: 2026년 9월 3일
>프로덕션 빠른 릴리스: 2026년 9월 17일
>모두를 위한 프로덕션: 2026년 10월 15일
>이 기능은 Workflow Ultimate 패키지의 조직에서만 사용할 수 있습니다.

고급 할당과 같은 Workfront의 다양한 영역에서 비율 속성을 필터로 사용하는 경우 이제 추가 유효성 검사가 상위-하위 필터링에 적용됩니다.

이전에는 한 속성을 상위에 연결하고 해당 상위를 조부모에 연결한 경우 원래 속성도 조부모에 속하는 것으로 자동으로 인식되지 않았습니다. 이제 최하위 레벨 속성을 선택하면 그 위에 있는 모든 레벨이 자동으로 할당됩니다.

특성에 대한 자세한 내용은 [비율 특성 정의](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)를 참조하십시오.
