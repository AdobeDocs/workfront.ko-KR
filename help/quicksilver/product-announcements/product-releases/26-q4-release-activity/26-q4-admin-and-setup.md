---
title: 2026년 4분기 관리자 개선 사항
description: 2026년 4분기 관리자 개선 사항
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 1dd8ab20d11b2b4471308ac5402b31e20359a04c
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 2026년 4분기 관리자 개선 사항

이 페이지에서는 미리보기 환경에 대한 2026년 4분기 릴리스의 관리자 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2026년 4분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2026년 4분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)를 참조하십시오.

## 그룹 관리자는 비즈니스 프로필을 관리할 수 있습니다.

>[!NOTE]
>
>미리 보기: 2026년 7월 30일>프로덕션 빠른 릴리스: 2026년 8월 13일>모두를 위한 프로덕션: 2026년 10월 15일

이제 그룹 관리자는 시스템 관리자에 액세스하지 않고도 관리하는 그룹의 비즈니스 프로필을 생성, 편집 및 삭제할 수 있습니다. 이를 통해 조직은 그룹 수준에서 비즈니스 프로필 관리를 보다 유연하게 위임할 수 있습니다.

자세한 내용은 [비즈니스 프로필 보기 및 관리](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-business-profiles.md)를 참조하세요.

## 향상된 목록의 보기에 대한 레이아웃 템플릿 지원

>[!NOTE]
>
>미리 보기: 2026년 7월 30일>프로덕션 빠른 릴리스: 2026년 8월 13일>모두를 위한 프로덕션: 2026년 10월 15일

이제 레이아웃 템플릿을 통해 시스템 수준에서 향상된 목록 보기가 지원됩니다. 기존 시스템 보기를 숨기고, 특정 보기를 기본 보기로 지정하고, 사용자 지정 보기를 시스템 보기 목록에 추가할 수 있습니다.

레이아웃 템플릿의 향상된 목록의 예로는 **모든 요청** 및 **고급 할당**&#x200B;이 있습니다. 향상된 목록 보기 옆에 &quot;새 경험&quot; 레이블이 있습니다.

자세한 내용은 [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)을 참조하십시오.

## 외부 조회 필드 벌크 편집

>[!NOTE]
>
>미리 보기: 2026년 7월 30일>프로덕션 빠른 릴리스: 2026년 8월 13일>모두를 위한 프로덕션: 2026년 10월 15일

이제 벌크 편집 대화 상자를 통해 외부 조회 필드를 편집할 수 있습니다. 이전에는 가능하지 않았습니다.

조회 필드가 다른 조회 필드에 종속되는 경우, 첫 번째 필드가 편집되는 모든 객체에 대해 동일하지 않으면 종속성이 있는 필드를 일괄 편집할 수 없습니다.

예를 들어 국가 목록은 지역에 대해 선택한 항목에 따라 다릅니다. 한 프로젝트의 지역이 아시아이고 다른 프로젝트의 지역이 유럽인 경우 두 프로젝트를 모두 일괄 편집하면 지역이 일치하지 않으므로 국가 필드를 사용할 수 없습니다. 두 프로젝트에 대해 지역이 동일하도록 편집한 경우 두 프로젝트에서 사용할 국가를 선택할 수도 있습니다.

외부 조회 필드에 대한 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-external-lookup-fields)를 참조하십시오.

## 사용자 정의 양식 디자이너 미리 보기에서 지원되는 고급 논리

>[!NOTE]
>
>미리 보기: 2026년 7월 30일>프로덕션 빠른 릴리스: 2026년 8월 13일>모두를 위한 프로덕션: 2026년 10월 15일

이제 사용자 정의 양식 디자이너 미리 보기 모드에서 고급 표시 논리, 기본값 논리, 유효성 검사 논리, 서식 논리 및 편집 논리 등의 고급 논리 옵션을 지원합니다. 양식 미리 보기에서 논리 공식을 테스트하고 논리 빌더에서 필요에 따라 조정할 수 있습니다. 테스트 개체(프로젝트, 작업, 문제 등)를 선택할 수도 있습니다. 을 클릭하여 실제 상황별 데이터를 사용하여 양식을 미리 볼 수 있습니다.

이전에는 미리보기 모드에서 기본 디스플레이 및 건너뛰기 논리 옵션만 지원되었습니다.

고급 표시, 기본값, 조건부 서식 설정 및 편집 가능성과 같은 논리 유형은 Workflow Prime 또는 Ultimate 패키지의 조직에서만 사용할 수 있습니다.

자세한 내용은 [사용자 정의 양식 및 필드에 논리 규칙 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md) 및 [양식 구성 및 미리 보기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md)를 참조하십시오.

## 통합 검토 및 승인을 위한 변경 추적

>[!NOTE]
>
>미리 보기: 2026년 7월 30일>프로덕션 빠른 릴리스: 2026년 8월 13일>모두를 위한 프로덕션: 2026년 10월 15일

이제 Workfront의 변경 기록 페이지에서 통합 검토 및 승인 워크플로 활동을 캡처하여 관리자가 검토 및 문서 라이프사이클 이벤트를 위한 완벽한 거버넌스 추적을 수행할 수 있습니다.

이제 승인, 단계 및 참가자 작업이 추적됩니다. 이러한 작업은 다음과 같습니다.

* Frame.io 뷰어에서 승인 결정
* 승인 만들기 또는 삭제
* 문서 업데이트(예: 이름 변경, 이동 또는 삭제)

각 항목에는 날짜 및 시간, 작업, 사용자 이름(또는 &quot;시스템 생성&quot;), 객체 이름 등 추적되는 표준 필드가 포함됩니다. MCP 활동은 LLM(예: Claude)이 업데이트를 수행한 것을 포함하여 캡처됩니다. Frame.io 뷰어 주석은 포함되지 않습니다.

자세한 내용은 [변경 내용 보기 및 관리](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md)를 참조하십시오.
