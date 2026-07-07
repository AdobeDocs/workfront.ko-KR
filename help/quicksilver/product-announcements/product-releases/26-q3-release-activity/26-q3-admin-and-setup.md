---
title: 2026년 3분기 관리자 개선 사항
description: 2026년 3분기 관리자 개선 사항
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 9cdb31404a92171c8972520eb54a9b5b0c729514
workflow-type: tm+mt
source-wordcount: '1328'
ht-degree: 4%

---

# 2026년 3분기 관리자 개선 사항

이 페이지에서는 미리보기 환경에 대한 2026년 3분기 릴리스의 관리자 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2026년 3분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2026년 3분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)를 참조하십시오.

<!--

## Change tracking for unified review and approval

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

The Change History page in Workfront now captures activity across unified review and approval workflows, giving administrators a complete governance trail for review and document lifecycle events.

Approval, stage, and participant actions are now tracked. These actions may include:

* Making an approval decision in the Frame.io viewer
* Creating or deleting an approval
* Updating a document such as renaming, moving, or deleting it

Each entry includes the standard tracked fields: date and time, operation, user name (or "system generated"), and object name. Frame.io viewer comments are not included.

This phase of change tracking does not include MCP events. Those will be part of a future release.

For more information, see [View and manage change history](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

-->

## 타이프 어헤드 필드 유형을 바꾸는 내부 조회 필드

>[!NOTE]
>
>미리 보기: 2026년 7월 7일프로덕션 빠른 릴리스: 2026년 7월 15일모두를 위한 프로덕션: 2026년 7월 16일

사용자 정의 양식의 새 **내부 조회** 필드 유형에서 동적 필터링을 제공합니다. 타이프 어헤드 필드 유형과 유사하며 이름의 일부를 입력하여 기존 Workfront 개체를 검색하고 선택할 수 있습니다. 내부 조회의 필터는 폼의 다른 필드에 있는 값을 참조할 수 있지만, Typeahead에서는 가능하지 않습니다.

다중 선택은 내부 조회에서 지원되며 이 필드 유형은 대용량 데이터 세트에 대한 향상된 성능도 제공합니다. 내부 조회에서 지원되는 기본 Workfront 개체는 프로젝트, 회사, 그룹, 작업 역할, Portfolio, 프로그램, 팀, 템플릿, 사용자, 작업, 문제, 문서 및 위치입니다.

내부 조회 필드 유형이 자동 완성 필드 유형을 대체하고 있습니다. 오른쪽의 필드 옵션에서 버튼을 클릭하여 기존 자동 완성 필드를 내부 조회로 빠르게 변환할 수 있습니다. 변환할 때 내역 데이터는 필드에 남아 있으며 보고서에서 동일한 방식으로 사용됩니다.

>[!IMPORTANT]
>
>Workfront Fusion 시나리오 또는 API 기반 자동화와 같은 외부 통합은 기존 필드 구조를 참조하고 전환 후 업데이트가 필요할 수 있습니다. 타이프 어헤드 필드를 내부 조회 필드로 전환하기 전에 모든 통합을 확인해야 합니다.

자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

## 네이티브 참조 필드에서 지원되는 기본값 논리

>[!NOTE]
>
>미리 보기: 2026년 7월 7일프로덕션 빠른 릴리스: 2026년 7월 15일모두를 위한 프로덕션: 2026년 7월 16일
>
>이 기능은 Workflow Prime 또는 Ultimate 패키지의 조직에서만 사용할 수 있습니다.

이제 사용자 정의 양식의 기본 참조 필드를 사용하여 기본값 논리를 추가할 수 있습니다.

기본 참조 필드에 대한 이 논리 유형은 Workfront API가 아닌 사용자 인터페이스에서만 사용할 수 있습니다.

자세한 내용은 문서 [사용자 정의 양식 및 필드에 논리 규칙 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md)에서 [사용자 정의 양식에 기본값 논리 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md#add-default-value-logic-to-a-custom-form)를 참조하십시오.

## 사용자 정의 양식의 기본 필드 필터링 업데이트

>[!NOTE]
>
>미리 보기: 2026년 7월 7일프로덕션 빠른 릴리스: 2026년 7월 15일모두를 위한 프로덕션: 2026년 7월 16일

이제 기본 필드에 존재하는 시스템 필터가 사용자 정의 양식의 필드에 적용되어 관리자가 볼 수 있습니다.

시스템 필터가 적용된 기본 참조 필드를 추가할 때 사용자 정의 양식의 필드에 동일한 필터를 적용하고 필요한 경우 텍스트 모드 상자에서 필터를 수정할 수 있습니다.

사용자 정의 필터를 필드에 추가하면 해당 필드에 대한 시스템 필터가 무시됩니다. 사용자 지정 필터를 입력하지 않으면 기본적으로 시스템 필터가 적용됩니다.

또한 이제 기본 참조 필드에서 동적 필터링을 사용할 수 있습니다. 동적 필터를 사용하면 다른 필드의 값을 기준으로 항목 목록의 범위를 좁힐 수 있습니다.

예를 들어 프로젝트 필드 필터에서 `?portfolioID={portfolio}.{ID}`을(를) 사용하고 Portfolio 네이티브 필드가 사용자 지정 양식에 있는 경우 프로젝트 필드에는 선택한 포트폴리오에 있는 프로젝트만 표시됩니다. Portfolio 필드를 비워 두면 프로젝트 필드에서 모든 프로젝트를 사용할 수 있습니다.

자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

## 실수로 이름이 바뀌지 않도록 필드 이름 보호

>[!NOTE]
>
>미리 보기: 2026년 7월 7일프로덕션 빠른 릴리스: 2026년 7월 15일모두를 위한 프로덕션: 2026년 7월 16일

통합 및 데이터 무결성을 보호하기 위해 사용자 지정 양식의 필드 설정 패널에서 필드 이름을 편집하는 방법을 업데이트했습니다.

이제 필드 설정 패널의 필드 이름이 기본적으로 읽기 전용입니다. 필드 이름을 편집할 수는 있지만 이름을 바꾸려면 명시적인 확인 단계가 필요합니다. 이전에 **Name**(으)로 호출된 필드도 기술적 중요성을 더 잘 반영하도록 **API 이름**(으)로 업데이트되었습니다. **레이블** 필드는 편집 가능한 상태로 유지됩니다.

자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#notes-on-field-names-and-labels)를 참조하십시오.

## Workfront 개체에 대한 변경 내역 보기

>[!NOTE]
>
>미리 보기: 2026년 6월 11일프로덕션 빠른 릴리스: 2026년 6월 11일모두를 위한 프로덕션: 2026년 7월 16일

하나의 중앙 목록에서 발생한 변경 사항을 더 쉽게 확인할 수 있도록 변경 기록 목록을 만들었습니다. 이 목록에는 객체, 작업 및 변경 소스(예: 사용자 또는 Workfront 시스템)와 같은 정보가 표시됩니다.

이전에는 감사 로그를 사용할 수 있었지만 개체를 다루지는 않았습니다.

자세한 내용은 [변경 내용 보기 및 관리](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md)를 참조하세요.

## 레거시 스토리지 포트폴리오를 Adobe 클라우드 스토리지로 변환하는 새로운 시스템 환경 설정

>[!NOTE]
>
>미리 보기: 2026년 6월 11일모두를 위한 프로덕션: 2026년 6월 11일

Workfront 관리자는 이제 시스템 환경 설정에서 직접 레거시 스토리지 포트폴리오를 Adobe 클라우드 스토리지로 변환할 수 있습니다. 포트폴리오를 변환하려면 새 엔터프라이즈 스토리지로 변환할 포트폴리오 선택 필드에서 해당 포트폴리오를 선택하고 페이지를 저장합니다.

포트폴리오를 Adobe 클라우드 스토리지로 변환할 때:

* 이전 Workfront 스토리지를 사용하는 프로젝트를 더 이상 이 포트폴리오로 이동할 수 없습니다.
* 이 포트폴리오에서 새로 생성된 모든 프로젝트가 Adobe 클라우드 스토리지를 사용합니다.
* Frame.io는 Adobe 클라우드 스토리지를 사용하는 문서의 뷰어입니다
* 기존 Workfront 스토리지를 사용하는 하위 객체는 기존 스토리지에 남음

이전에는 기존 스토리지 포트폴리오에 Adobe 클라우드 스토리지 프로젝트를 추가하면 포트폴리오가 Adobe 클라우드 스토리지로 자동 변환되었습니다.

자세한 내용은 [시스템 환경 설정 구성](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)을 참조하십시오.

## 서식이 있는 텍스트 필드 유형을 리치 텍스트로 교체

>[!NOTE]
>
>미리 보기: 2026년 5월 28일프로덕션 빠른 릴리스: 2026년 6월 11일모두를 위한 프로덕션: 2026년 7월 16일

사용자 정의 양식의 새 **서식 있는 텍스트** 필드 형식은 굵게, 기울임꼴, 밑줄, 글머리 기호, 번호 매기기, 하이퍼링크 및 블록 인용과 같은 기존 옵션 외에도 위 첨자 및 아래 첨자, 제목 및 표와 같은 서식 지정 옵션이 있는 강력한 텍스트 편집기입니다. 문자 길이는 15,000자로 제한됩니다.

서식 있는 텍스트 필드 유형이 텍스트를 서식 있는 필드 유형으로 바꿉니다. 오른쪽의 필드 옵션에서 버튼을 클릭하여 서식 필드가 있는 기존 텍스트를 서식 있는 텍스트로 빠르게 변환할 수 있습니다. 변환할 때 내역 데이터는 필드에 남아 있으며 보고서에서 동일한 방식으로 사용됩니다.

>[!IMPORTANT]
>
>Workfront Fusion 시나리오 또는 API 기반 자동화와 같은 외부 통합은 기존 필드 구조를 참조하고 전환 후 업데이트가 필요할 수 있습니다. 필드를 리치 텍스트로 변환하기 전에 모든 통합을 확인해야 합니다.

자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

## 사용자 정의 양식에서 지원되는 기본 재무 필드

>[!NOTE]
>
>미리 보기: 2026년 5월 28일프로덕션 빠른 릴리스: 2026년 6월 11일모두를 위한 프로덕션: 2026년 7월 16일

이제 사용자 정의 양식에 Workfront 기본 재무 필드를 포함할 수 있습니다. 이전에는 재무 필드가 지원되지 않았습니다.

참조할 수 있는 재무 필드는 양식 유형에 따라 다릅니다.

자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields)를 참조하십시오.

## 첨부 액세스 권한을 통해 사용자 정의 양식을 시스템 전체에 공유 가능

>[!NOTE]
>
>미리 보기: 2026년 5월 28일프로덕션 빠른 릴리스: 2026년 6월 11일모두를 위한 프로덕션: 2026년 7월 16일

새 공유 옵션 &quot;시스템의 모든 사용자가 보고 첨부할 수 있습니다&quot;가 사용자 정의 양식에 추가되었습니다. 이 옵션을 선택하면 시스템 전체에서 모든 사용자가 양식을 다른 오브젝트에 첨부할 수 있습니다.

시스템 전체에서 공유하면 새 그룹이 추가될 때 그룹 또는 에이전시에서 양식을 수동으로 공유하고 권한을 업데이트할 필요가 없습니다.

자세한 내용은 [사용자 정의 양식 공유](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)를 참조하십시오.

## 일괄 편집에서 필수 필드를 적용하는 새로운 시스템 환경 설정

>[!NOTE]
>
>미리 보기: 2026년 5월 28일프로덕션 빠른 릴리스: 2026년 6월 11일모두를 위한 프로덕션: 2026년 7월 16일

현재 오브젝트를 벌크 편집할 때 필수 필드는 사용자가 필드를 수정할 때만 적용됩니다. 필드가 수정되지 않으면 선택 사항으로 처리되고 확인되지 않습니다.

이제 새 시스템 기본 설정을 사용하여 필수 필드를 일괄 편집할 수 있습니다. 모든 필수 필드에 값이 없으면 대량 편집 개체가 저장되지 않도록 하려면 설정 > 시스템 > 환경 설정 페이지에서 **항상 대량 편집에 필수 필드 적용** 옵션을 선택하십시오.

자세한 내용은 [시스템 환경 설정 구성](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)을 참조하십시오.
