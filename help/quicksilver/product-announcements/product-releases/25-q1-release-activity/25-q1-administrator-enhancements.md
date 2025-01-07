---
title: 2025년 1분기 관리자 개선 사항
description: 2025년 1분기 관리자 개선 사항
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: fa24040d-0403-4799-b690-c3d172797115
source-git-commit: a7a3272cb7bfa22abfee45211e3154b6e21434b8
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# 2025년 1분기 관리자 개선 사항

이 페이지에서는 미리보기 환경에 대한 2025년 1분기 릴리스의 모든 관리자 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2025년 1분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2025년 1분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md)를 참조하십시오.

## 환경 프로모션을 위해 환경 간에 객체 비교

>[!NOTE]
>
>미리보기 릴리스: 2024년 1월 6일, 모든 고객을 위한 프로덕션 릴리스: 25.1 릴리스 포함(2025년 1월)

환경 프로모션 패키지에 포함해야 하는 오브젝트를 더 쉽게 결정할 수 있도록 환경 간에 오브젝트를 비교하는 기능을 추가했습니다. 이제 개체 유형 및 환경을 선택할 수 있습니다. Workfront은 해당 유형의 객체 목록과 대상 환경에 해당 객체가 있는지 여부 및 소스 환경과 대상 환경 간에 차이가 있는지 여부를 생성합니다. 그런 다음 이 목록에서 직접 패키지에 개체를 추가할 수 있습니다.

이전에는 사용자가 환경 간에 개체를 비교하려면 해당 개체를 수동으로 확인해야 했습니다.

자세한 내용은 [환경 간 개체 비교](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-compare.md)를 참조하십시오.

## 환경 프로모션에 사용할 수 있는 추가 오브젝트

>[!NOTE]
>
>미리보기 릴리스: 2024년 1월 6일, 모든 고객을 위한 프로덕션 릴리스: 25.1 릴리스 포함(2025년 1월)

환경 프로모션 기능의 기능을 확장하기 위해 더 많은 개체를 추가했습니다. 이제 환경 프로모션 패키지에 다음 오브젝트를 추가할 수 있습니다.

* 위치
* 요율 카드
* 할당

이전에는 이러한 개체를 환경 프로모션에 사용할 수 없었습니다.

환경 프로모션에 사용할 수 있는 개체에 대한 자세한 내용은 환경 프로모션 개요 문서에서 [환경 프로모션에 대해 지원되는 개체](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion)를 참조하십시오.

## 기록된 시간이 있을 때 작업 이동 방지

>[!NOTE]
>
>미리보기 릴리스: 2024년 12월 19일, 모든 고객을 위한 프로덕션 릴리스: 25.1 릴리스 포함(2025년 1월)

시간이 기록된 작업 또는 문제를 이동하면 경우에 따라 준수 또는 감사 문제가 발생할 수 있으므로 작업 및 문제에 기록된 시간이 있는 경우 사용자가 작업 및 문제를 이동할 수 없도록 하는 기본 설정을 설정의 작업 및 문제 기본 설정 영역에 추가했습니다. 이 기능이 향상되기 전에는 사용자가 작업 및 문제에 로그온한 시간이 있더라도 해당 작업과 문제를 다른 프로젝트로 이동할 수 있었습니다.

자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)을 참조하십시오.

## 단일 할당 작업에 프로젝트 또는 사용자 일정을 사용하는 환경 설정

>[!NOTE]
>
>미리보기 릴리스: 2024년 11월 21일, 빠른 릴리스를 위한 프로덕션: 24.12 릴리스(2024년 12월 12일), 분기별 릴리스의 프로덕션: 25.1 릴리스(2025년 1월)

이제 시스템 또는 그룹 관리자로서, 작업에 한 명의 사용자를 할당하고 프로젝트와 사용자를 모두 예약과 연결할 때 Workfront이 프로젝트의 일정을 계산할지 또는 사용자의 일정을 사용할지 여부를 나타내는 새로운 환경 설정이 제공됩니다. 이 개선 이전에는 여러 사용자 할당에 대해 이 설정이 있었습니다. 이제 이 설정을 단일 사용자가 작업에 할당할 수 있습니다.

자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

## 비즈니스 규칙이 이제 하이퍼링크를 지원합니다.

>[!NOTE]
>
>미리보기 릴리스: 2024년 11월 21일, 빠른 릴리스를 위한 프로덕션: 24.12 릴리스(2024년 12월 12일), 분기별 릴리스의 프로덕션: 25.1 릴리스(2025년 1월)

이제 비즈니스 규칙의 사용자 지정 오류 메시지에 하이퍼링크를 포함하여 규칙의 제한 사항 내에서 작업을 수정하는 방법을 사용자에게 안내할 수 있습니다. 정적 URL은 설명서 또는 사용자에게 유용한 다른 페이지에 연결할 수 있습니다.

자세한 내용은 [비즈니스 규칙 만들기 및 편집](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md)을 참조하세요.

## 이제 기본 자동 완성 필드에 대한 필터링을 사용할 수 있습니다

>[!NOTE]
>
>미리보기 릴리스: 2024년 11월 21일, 빠른 릴리스를 위한 프로덕션: 24.12 릴리스(2024년 12월 12일), 분기별 릴리스의 프로덕션: 25.1 릴리스(2025년 1월)

이제 사용자 정의 양식에 기본 필드 참조를 추가하고 이 필드가 자동 완성 필드(예: Portfolio, 회사 또는 소유자)를 참조하는 경우 필터 옵션을 사용할 수 있습니다. 필터를 사용하면 사용자가 필드를 사용할 때 선택할 수 있는 개체를 제한할 수 있습니다. 이 사용자 지정 필터는 사용자 지정 자동 완성 필드의 필터와 동일하게 작동하며 텍스트 모드를 사용하여 필터를 정의합니다.

자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

## 사용자 정의 필드에 &quot;이동&quot; 아이콘이 추가됨

>[!NOTE]
>
>미리보기 릴리스: 2024년 10월 29일, 빠른 릴리스를 위한 프로덕션: 24.11 릴리스(2024년 11월 14일), 분기별 릴리스의 프로덕션: 25.1 릴리스(2025년 1월)

사용자 정의 양식에 필드가 많은 섹션이 포함된 경우 끌어다 놓아 한 섹션에서 다른 섹션으로 필드를 이동하는 데 어려움이 있을 수 있습니다. 각 필드에 &quot;이동&quot; 아이콘이 추가되어 필드가 배치될 섹션을 선택할 수 있습니다.

자세한 내용은 [양식 구성 및 미리 보기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md)를 참조하세요.
