---
title: 2026년 3분기 관리자 개선 사항
description: 2026년 3분기 관리자 개선 사항
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 3d8439efd8a92042098fbf995aacf2fe3add43f2
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# 2026년 3분기 관리자 개선 사항

이 페이지에서는 미리보기 환경에 대한 2026년 3분기 릴리스의 관리자 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2026년 3분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2026년 3분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)를 참조하십시오.

## 서식 있는 텍스트가 서식 있는 필드 유형으로 텍스트 바꾸기

>[!NOTE]
>
>미리 보기: 2026년 5월 28일>프로덕션 빠른 릴리스: 2026년 6월 11일>모두를 위한 프로덕션: 2026년 7월 16일

사용자 정의 양식의 새 **서식 있는 텍스트** 필드 형식은 굵게, 기울임꼴, 밑줄, 글머리 기호, 번호 매기기, 하이퍼링크 및 블록 인용과 같은 기존 옵션 외에도 위 첨자 및 아래 첨자, 제목 및 표와 같은 서식 지정 옵션이 있는 강력한 텍스트 편집기입니다. 문자 길이는 15,000자로 제한됩니다.

서식 있는 텍스트 필드 유형이 텍스트를 서식 있는 필드 유형으로 바꿉니다. 오른쪽의 필드 옵션에서 버튼을 클릭하여 서식 필드가 있는 기존 텍스트를 서식 있는 텍스트로 빠르게 변환할 수 있습니다. 변환할 때 내역 데이터는 필드에 남아 있으며 보고서에서 동일한 방식으로 사용됩니다.

>[!IMPORTANT]
>
>Workfront Fusion 시나리오 또는 API 기반 자동화와 같은 외부 통합은 기존 필드 구조를 참조하고 전환 후 업데이트가 필요할 수 있습니다. 필드를 리치 텍스트로 변환하기 전에 모든 통합을 확인해야 합니다.

자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

## 사용자 정의 양식에서 지원되는 기본 재무 필드

>[!NOTE]
>
>미리 보기: 2026년 5월 28일>프로덕션 빠른 릴리스: 2026년 6월 11일>모두를 위한 프로덕션: 2026년 7월 16일

이제 사용자 정의 양식에 Workfront 기본 재무 필드를 포함할 수 있습니다. 이전에는 재무 필드가 지원되지 않았습니다.

참조할 수 있는 재무 필드는 양식 유형에 따라 다릅니다.

자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields)를 참조하십시오.

## 사용자 정의 양식을 연결할 수 있는 액세스 권한으로 시스템 전체에 공유할 수 있습니다.

>[!NOTE]
>
>미리 보기: 2026년 5월 28일>프로덕션 빠른 릴리스: 2026년 6월 11일>모두를 위한 프로덕션: 2026년 7월 16일

새 공유 옵션 &quot;시스템의 모든 사용자가 보고 첨부할 수 있습니다&quot;가 사용자 정의 양식에 추가되었습니다. 이 옵션을 선택하면 시스템 전체에서 모든 사용자가 양식을 다른 오브젝트에 첨부할 수 있습니다.

시스템 전체에서 공유하면 새 그룹이 추가될 때 그룹 또는 에이전시에서 양식을 수동으로 공유하고 권한을 업데이트할 필요가 없습니다.

자세한 내용은 [사용자 정의 양식 공유](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)를 참조하십시오.

## 일괄 편집에서 필수 필드를 적용하는 새로운 시스템 환경 설정

>[!NOTE]
>
>미리 보기: 2026년 5월 28일>프로덕션 빠른 릴리스: 2026년 6월 11일>모두를 위한 프로덕션: 2026년 7월 16일

현재 오브젝트를 벌크 편집할 때 필수 필드는 사용자가 필드를 수정할 때만 적용됩니다. 필드가 수정되지 않으면 선택 사항으로 처리되고 확인되지 않습니다.

이제 새 시스템 기본 설정을 사용하여 필수 필드를 일괄 편집할 수 있습니다. 모든 필수 필드에 값이 없으면 대량 편집 개체가 저장되지 않도록 하려면 설정 > 시스템 > 환경 설정 페이지에서 **항상 대량 편집에 필수 필드 적용** 옵션을 선택하십시오.

자세한 내용은 [시스템 환경 설정 구성](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)을 참조하십시오.
