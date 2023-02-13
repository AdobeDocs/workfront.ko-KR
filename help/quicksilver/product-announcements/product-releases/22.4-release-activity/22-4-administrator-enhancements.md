---
title: 22.4 관리자 개선 사항
description: 22.4 관리자 개선 사항
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
source-git-commit: 80fa784e15c3b4a927ee8ba2d18a80a2d84f4a91
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# 22.4 관리자 개선 사항

이 페이지에서는 미리 보기 환경에 대한 22.4 릴리스로 향상된 모든 관리자 기능을 설명합니다. 이러한 개선 사항은 2022년 10월 3일이 있는 주에 제공될 예정입니다.

22.4 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [22.4 릴리스 개요](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## 승인 프로세스에서 잠금 해제된 상태 사용

>[!NOTE]
>
>이 기능은 22.3 릴리스 기간 동안 미리 보기 환경에서 처음 도입되었습니다. 프로덕션 릴리스는 2022년 9월 15일입니다.

시스템의 승인 프로세스 및 상태를 보다 세밀하게 제어할 수 있도록 잠금 해제된 시스템 상태에 따라 승인 프로세스를 만들 수 있도록 했습니다. 또한 승인 프로세스에서 이미 사용되고 있는 모든 상태의 잠금을 해제할 수도 있습니다. 이전에는 승인 프로세스에서 사용된 시스템 상태를 잠가야 했습니다. 따라서 그룹 관리자가 특정 요구에 맞게 그룹의 상태 목록을 간소화할 수 없었습니다.

## 이제 레이아웃 템플릿을 통해 기본 메뉴의 블루프린트 아이콘을 제어합니다

시스템 관리자는 이제 레이아웃 템플릿 구성을 통해 기본 메뉴에서 Blueprint 아이콘을 추가하거나 제거할 수 있습니다. 이렇게 하면 Blueprint 카탈로그를 찾을 수 있는 사용자를 더 잘 제어할 수 있습니다.

다음과 같은 경우 기본 메뉴에 Blueprint 아이콘이 표시됩니다.

* 사용자에게 할당된 레이아웃 템플릿이 없습니다

* 사용자의 레이아웃 템플릿에는 활성 항목 목록에 블루프린트 옵션이 있습니다

* 사용자의 레이아웃 템플릿에 사용 가능한 항목 목록의 블루프린트 옵션이 있고 기본 메뉴에 아이콘이 표시되지 않습니다.

기존 레이아웃 템플릿에는 블루프린트 아이콘이 자동으로 포함되며, 관리자는 레이아웃 템플릿에서 아이콘을 제거하여 블루프린트 카탈로그의 가시성을 제한할 수 있습니다. 22.4 릴리스 후에 생성된 새 레이아웃 템플릿에는 활성 항목 목록의 블루프린트 아이콘이 포함됩니다.

자세한 내용은 [블루프린트에 대한 액세스 구성](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md).

[이 기능에 대한 비디오 데모 보기](https://video.tv.adobe.com/v/3412382/){target=_blank}

## 문제 헤더 사용자 지정

이제 Workfront 또는 그룹 관리자는 레이아웃 템플릿을 사용할 때 문제 헤더에 표시되는 필드를 사용자 지정할 수 있습니다.

이 업데이트에는 다음과 같은 개선 사항이 포함됩니다.

* 문제 헤더에서 기존 필드를 제거하거나 다시 배열합니다.

* 편집할 수 없는 새 문제 개요 필드를 추가합니다. 편집할 수 있는 사용자 지정 필드나 필드는 추가할 수 없습니다. 현재 문제 헤더에 있는 편집 가능한 필드(예: 상태 또는 완료 퍼센트)를 표시할 수도 있습니다.

* 문제 헤더에는 최대 5개의 필드가 포함될 수 있습니다.

* 이제 &quot;해결된 사람&quot; 필드를 문제 헤더에 추가할 수 있습니다. 해결 객체가 문제와 연관되어 있으면 문제와 연관된 객체 유형에 따라 &quot;해결 방법&quot; 필드가 &quot;문제 해결&quot;, &quot;태스크 해결&quot; 또는 &quot;프로젝트 해결&quot;으로 변경됩니다.

이 릴리스 이전에는 프로젝트 및 작업 헤더만 사용자 지정할 수 있었습니다.



자세한 내용은 [레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[이 기능에 대한 비디오 데모 보기](https://video.tv.adobe.com/v/3412383/){target=_blank}

## 작업 헤더 사용자 지정

이제 Workfront 또는 그룹 관리자는 레이아웃 템플릿을 사용할 때 작업 헤더에 표시되는 필드를 사용자 지정할 수 있습니다.

이 업데이트에는 다음과 같은 개선 사항이 포함됩니다.

* 작업 헤더에서 기존 필드를 제거하거나 다시 배열합니다.

* 편집할 수 없는 새 작업 개요 필드를 추가합니다. 편집할 수 있는 사용자 지정 필드나 필드는 추가할 수 없습니다. 현재 작업 헤더에 있는 편집 가능한 필드(예: 상태 또는 완료 퍼센트)를 표시할 수도 있습니다.

* 작업 헤더에는 최대 5개의 필드가 포함될 수 있습니다.

이 릴리스 이전에는 프로젝트 헤더만 사용자 지정할 수 있었습니다.

자세한 내용은 [레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[이 기능에 대한 비디오 데모를 봅니다.](https://video.tv.adobe.com/v/3412384/){target=_blank}

## 보드의 최신 기능에 대한 초기 기능 옵트인

초기 기능 옵트인을 위한 새로운 보드 기능을 열게 되어 기쁘게 생각합니다. 이 선택적 도구는 모든 조직에서 사용할 수 있습니다.

Workfront 관리자만 초기 기능에 옵트인할 수 있습니다. 관리자가 초기 기능에 옵트인하면 조직의 모든 사용자가 옵트인되고 프로덕션 Workfront 환경에서 추가 기능이 활성화됩니다.

자세한 내용은 [Adobe Workfront 보드에 대한 초기 기능 옵트인](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

[이 기능에 대한 비디오 데모를 봅니다.](https://video.tv.adobe.com/v/3412386/){target=_blank}

## 사용자 지정 양식 필드 계산 편집기에 오류 정보가 표시됩니다

>[!NOTE]
>
>이 기능은 22.3 릴리스 기간 동안 미리 보기 환경에서 처음 도입되었습니다. 22.4 릴리스와 함께 프로덕션에 릴리스됩니다.

이제 계산에 직접 표시되는 유용한 오류 정보를 사용하면 사용자 지정 필드에 대한 계산을 더 쉽게 편집할 수 있습니다. 사용자 지정 양식에 계산된 필드를 만드는 동안 오류가 분홍색으로 강조 표시됩니다. 강조 표시된 부분을 마우스로 가리키면 문제가 무엇인지 설명하는 도구 설명이 표시됩니다.

자세한 내용은 [사용자 지정 양식에 계산된 데이터 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

[이 기능에 대한 비디오 데모를 봅니다.](https://video.tv.adobe.com/v/3412387/){target=_blank}

## Adobe 통합 경험으로 마이그레이션

참고: 이 마이그레이션은 2023년 Q1-Q2로 연기되었습니다. 영향을 받는 모든 고객은 해당 시간에 알림을 받게 됩니다.

조직이 Adobe Admin Console으로 온보딩된 경우 Workfront 인스턴스가 22.4 릴리스를 통해 Adobe 통합 경험으로 마이그레이션됩니다.

Adobe 통합 경험에는 다음이 포함됩니다.

* Adobe Experience Cloud을 통한 모든 Adobe 애플리케이션에 대한 단일 로그인

* Workfront 조직 및 환경 간을 이동하기 위한 &quot;조직 전환기&quot;

* Workfront 페이지, Adobe Experience Cloud 환경 설정 및 Workfront 프로필 옵션이 있는 탐색

자세한 내용은 [Workfront용 통합 경험 Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

[이 기능에 대한 비디오 데모를 봅니다.](https://video.tv.adobe.com/v/3412388/){target=_blank}
