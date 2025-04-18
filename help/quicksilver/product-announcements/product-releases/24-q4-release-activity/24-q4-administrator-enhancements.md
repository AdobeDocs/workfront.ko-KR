---
title: 2024년 4분기 관리자 개선 사항
description: 2024년 4분기 관리자 개선 사항
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4f4694dd-a6cb-46b7-b2cf-fe24ed9419f5
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# 2024년 4분기 관리자 개선 사항

이 페이지에서는 미리보기 환경에 대한 2024년 4분기 릴리스의 모든 관리자 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2024년 4분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2024년 4분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-release-overview.md)를 참조하십시오.

## 이제 환경 프로모션에서 액세스 수준을 사용할 수 있습니다.

>[!NOTE]
>
>미리보기 릴리스: 2024년 10월 17일, 모든 고객을 위한 프로덕션 릴리스: 24.10 릴리스 포함(2024년 10월 17일)

환경 프로모션 기능의 기능을 확장하기 위해 액세스 수준을 포함하는 기능이 추가되었습니다. 이제 샌드박스 환경에서 액세스 수준을 구성한 다음 해당 액세스 수준을 프로덕션 환경으로 승격할 수 있습니다.

이전에는 환경 프로모션에 액세스 수준을 사용할 수 없었습니다.

환경 프로모션에 사용할 수 있는 개체에 대한 자세한 내용은 환경 프로모션 개요 문서에서 [환경 프로모션에 대해 지원되는 개체](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion)를 참조하십시오.

## 사용자 정의 양식의 카운터는 필드 수를 보여 줍니다

>[!NOTE]
>
>미리보기 릴리스: 2024년 10월 1일, 모든 고객을 위한 프로덕션 릴리스: 24.10 릴리스 포함(2024년 10월 17일)

사용자 정의 양식은 500개의 필드로 제한됩니다. 긴 형식에서는 형식에 몇 개의 필드가 있으며 한도에 도달하는지 여부를 알기 어려울 수 있습니다.

왼쪽 하단의 사용자 정의 양식에 카운터가 추가되었습니다. 카운터는 폼에 사용되는 필드 수를 표시하며 폼 디자이너 내에서 스크롤할 때 항상 표시됩니다.

자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

## 이제 레이아웃 템플릿에서 &quot;모두 선택&quot; 옵션을 사용할 수 있습니다

>[!NOTE]
>
>미리보기 릴리스: 2024년 8월 29일, 모든 고객을 위한 프로덕션 릴리스: 2024년 8월 29일

레이아웃 템플릿을 사용하여 필드를 보다 쉽게 표시하거나 숨길 수 있도록 레이아웃 템플릿에서 세부 정보 보기의 개요 및 재무 영역에 **모두 선택** 확인란이 추가되었습니다. 이 옵션은 **사용자에게 표시되는 항목 사용자 지정**&#x200B;에서 프로젝트, 작업, 문제, Portfolio 또는 프로그램을 선택한 경우 사용할 수 있습니다. 일부 객체에는 재무 영역이 표시되지 않으며 각 영역의 필드는 객체에 따라 다릅니다.

자세한 내용은 [레이아웃 템플릿을 사용하여 세부 정보 보기 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)을 참조하십시오.

## 환경 프로모션 패키지 롤백

>[!NOTE]
>
>미리보기 릴리스: 2024년 8월 29일, 빠른 릴리스를 위한 프로덕션: 24.9 릴리스 포함(2024년 9월 12일), 분기별 릴리스의 프로덕션: 24.10 릴리스 포함(2024년 10월 17일)

환경 프로모션을 보다 유연하고 쉽게 사용할 수 있도록 롤백 기능을 활성화했습니다. 이제 24시간 내에 패키지를 롤백하여 환경 프로모션 패키지의 영향을 받은 이전 구성을 보다 쉽게 복원할 수 있습니다.

이전에는 구성을 수동으로 또는 다른 환경 프로모션 패키지를 통해 복원했습니다.

환경 홍보 패키지 롤백에 대한 자세한 내용은 [환경 홍보 패키지 롤백](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-rollback.md)을 참조하십시오.

[이 기능에 대한 비디오 데모를 봅니다.](https://video.tv.adobe.com/v/3434025/){target=_blank}

## 사용자 정의 양식 디자이너의 레이아웃 단추를 사용하면 2개 또는 3개의 열을 사용할 수 있습니다.

>[!NOTE]
>
>~~미리 보기 릴리스: 2024년 8월 12일~~; 빠른 릴리스를 위한 프로덕션: 해당 사항 없음; 분기별 릴리스를 위한 프로덕션: 해당 사항 없음
>
>_이 기능은 미리 보기에서 제거되었으며 향후 릴리스와 함께 릴리스되지 않습니다._

사용자 정의 양식 디자이너의 &quot;레이아웃&quot; 버튼을 사용하면 2열 또는 3열 작업 영역 중에서 선택할 수 있습니다. 원래 양식 디자이너는 세 개의 열을 사용하며 필드 설정은 맨 오른쪽 열에 표시됩니다. 두 개의 열을 선택하면 맨 왼쪽 열의 필드 라이브러리 옆에 필드 설정이 표시됩니다.

자세한 내용은 [사용자 정의 양식 개요](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md)를 참조하십시오.
