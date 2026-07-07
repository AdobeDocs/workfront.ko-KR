---
title: 2026년 3분기 관리자 개선 사항
description: 2026년 3분기 관리자 개선 사항
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: d83d823426b42202e83cb4db64f85d27d4dca0bb
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 7%

---

# 2026년 3분기 관리자 개선 사항

이 페이지에서는 미리보기 환경에 대한 2026년 3분기 릴리스의 관리자 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2026년 3분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2026년 3분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)를 참조하십시오.

## 통합 검토 및 승인을 위한 변경 추적

>[!NOTE]
>
>미리 보기: 2026년 7월 7일프로덕션 빠른 릴리스: 2026년 7월 15일모두를 위한 프로덕션: 2026년 7월 16일

이제 Workfront의 변경 기록 페이지에서 통합 검토 및 승인 워크플로 활동을 캡처하여 관리자가 검토 및 문서 라이프사이클 이벤트를 위한 완벽한 거버넌스 추적을 수행할 수 있습니다.

이제 승인, 단계 및 참가자 작업이 추적됩니다. 이러한 작업은 다음과 같습니다.

* Frame.io 뷰어에서 승인 결정
* 승인 만들기 또는 삭제
* 문서 업데이트(예: 이름 변경, 이동 또는 삭제)

각 항목에는 날짜 및 시간, 작업, 사용자 이름(또는 &quot;시스템 생성&quot;), 객체 이름 등 추적되는 표준 필드가 포함됩니다. Frame.io 뷰어 주석은 포함되지 않습니다.

이 변경 추적 단계는 MCP 이벤트를 포함하지 않습니다. 향후 릴리스의 일부가 될 예정입니다.

자세한 내용은 [변경 내용 보기 및 관리](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md)를 참조하십시오.

<!--

## Internal lookup field replacing Typeahead field type

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

The new **Internal lookup** field type in custom forms provides dynamic filtering. It is similar to the Typeahead field type and allows users to search and select existing Workfront objects by typing part of the name. The filter on the internal lookup can reference the value in another field on the form, which is not possible with Typeaheads.

Multi-select is supported on internal lookups, and this field type also provides improved performance for large datasets. The following native Workfront objects are supported in internal lookups: Project, Company, Group, Job Role, Portfolio, Program, Team, Template, User, Task, Issue, Document, and Location.

The Internal lookup field type is replacing the Typeahead field type. You can quickly convert existing Typeahead fields to Internal lookups by clicking the button in the field options on the right. When you convert, historical data remains on the field and it is used the same way in reports.

>[!IMPORTANT]
>
>External integrations such as Workfront Fusion scenarios or API-based automations may reference legacy field structures and require updates after the conversion. You should verify any integrations before converting Typeahead fields to Internal lookup fields.

For more information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

-->

<!--

## Default value logic supported on native reference fields

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026
>
>This feature is only available for organizations on the Workflow Prime or Ultimate packages.

In custom forms, native reference fields now allow you to add default value logic.

This logic type on native reference fields is available only in the user interface and not in the Workfront API.

For information, see [Add default value logic to a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md#add-default-value-logic-to-a-custom-form) in the article [Add logic rules to custom forms and fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

-->

<!--

## Updates to native field filtering in custom forms

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

System filters that exist on native fields are now applied to the fields in custom forms and are visible to administrators.

When you add a native reference field that has a system filter applied, you can apply the same filter to the field in the custom form and modify the filter if needed in the Text Mode box.

Adding your own custom filter to the field overrides the system filter for the field. If you do not enter a custom filter, the system filter is applied by default.

Also, dynamic filtering is now available on native reference fields. A dynamic filter allows you to narrow the list of items based on the value of another field.

For example, when you use `?portfolioID={portfolio}.{ID}` in a Project field filter and a Portfolio native field is on the custom form, the Project field shows only projects that are in the selected portfolio. If the Portfolio field is left blank, then all projects are available in the Project field.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

-->

<!--

## Protect field names from accidental renaming

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

To protect integrations and data integrity, we've updated how field names can be edited in the field settings panel of a custom form.

Field names in the field settings panel are now read-only by default. You can still edit the field name, but renaming requires an explicit confirmation step. The field previously called **Name** has also been updated to **API Name** to better reflect its technical significance. The **Label** field remains editable.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#notes-on-field-names-and-labels).

-->

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
