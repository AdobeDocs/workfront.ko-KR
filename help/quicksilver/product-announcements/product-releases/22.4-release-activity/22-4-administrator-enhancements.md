---
title: 22.4 관리자 개선 사항
description: 22.4 관리자 개선 사항
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 0%

---

# 22.4 관리자 개선 사항

이 페이지에서는 미리보기 환경에 대한 22.4 릴리스의 모든 관리자 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2022년 10월 3일이 있는 주에 사용할 수 있습니다.

22.4 릴리스에서 사용할 수 있는 모든 변경 사항 목록을 보려면 [22.4 릴리스 개요](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md)를 참조하십시오.

## 승인 프로세스에서 잠금 해제된 상태 사용

>[!NOTE]
>
>이 기능은 22.3 릴리스 기간 동안 미리보기 환경에 처음 도입되었습니다. 프로덕션 환경에 2022년 9월 15일 릴리스됩니다.

시스템의 승인 프로세스 및 상태를 보다 세밀하게 제어할 수 있도록 잠금 해제된 시스템 상태를 기반으로 승인 프로세스를 만들 수 있도록 했습니다. 또한 이제 승인 프로세스에서 이미 사용된 모든 상태를 잠금 해제할 수 있습니다. 이전에는 승인 프로세스에 사용되는 시스템 상태를 잠가야 했습니다. 따라서 그룹 관리자는 그룹 상태를 제거하거나 이름을 변경하지 않고도 모든 그룹에서 사용할 수 있으므로 그룹 관리자가 특정 요구 사항에 맞게 그룹 상태 목록을 간소화할 수 없었습니다.

## 메인 메뉴의 블루프린트 아이콘이 레이아웃 템플릿을 통해 제어됨

이제 시스템 관리자는 레이아웃 템플릿 구성을 통해 기본 메뉴의 블루프린트 아이콘을 추가하거나 제거할 수 있습니다. 이렇게 하면 블루프린트 카탈로그를 검색할 수 있는 사용자를 보다 세밀하게 제어할 수 있습니다.

다음과 같은 경우 기본 메뉴에 블루프린트 아이콘이 표시됩니다.

* 사용자에게 할당된 레이아웃 템플릿이 없습니다.

* 사용자의 레이아웃 템플릿에는 활성 항목 목록에 블루프린트 옵션이 있습니다.

* 사용자의 레이아웃 템플릿에는 사용 가능한 항목 목록에 있는 블루프린트 옵션이 있으며 아이콘이 메인 메뉴에 나타나지 않습니다.

기존 레이아웃 템플릿에는 자동으로 블루프린트 아이콘이 포함되며, 관리자는 레이아웃 템플릿에서 아이콘을 제거하여 블루프린트 카탈로그의 가시성을 제한할 수 있습니다. 22.4 릴리스 이후에 생성된 새 레이아웃 템플릿에는 활성 항목 목록에 블루프린트 아이콘이 포함됩니다.

자세한 내용은 [블루프린트에 대한 액세스 구성](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md)을 참조하십시오.

[이 기능의 비디오 데모 보기](https://video.tv.adobe.com/v/3412382/){target=_blank}

## 문제 헤더 사용자 정의

이제 Workfront 또는 그룹 관리자는 레이아웃 템플릿을 사용할 때 문제의 헤더에 표시되는 필드를 사용자 정의할 수 있습니다.

이 업데이트에는 다음과 같은 개선 사항이 포함됩니다.

* 문제 헤더에서 기존 필드를 제거하거나 다시 정렬합니다.

* 편집할 수 없는 새 문제 개요 필드를 추가합니다. 사용자 정의 필드 또는 편집할 수 있는 필드를 추가할 수 없습니다. 현재 문제 헤더에 있는 편집 가능한 필드(예: 상태 또는 완료율)를 표시할 수도 있습니다.

* 문제 헤더에는 최대 5개의 필드가 포함될 수 있습니다.

* 이제 &quot;해결자&quot; 필드를 문제 헤더에 추가할 수 있습니다. 해결 중인 오브젝트가 문제와 연결되면 &quot;해결한 사람&quot; 필드가 문제와 연결된 오브젝트 유형에 따라 &quot;해결 중 문제&quot;, &quot;해결 중 작업&quot; 또는 &quot;해결 중 프로젝트&quot;로 변경됩니다.

이 릴리스 이전에는 프로젝트 및 작업 헤더만 사용자 지정할 수 있었습니다.



자세한 내용은 [레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)을 참조하십시오.

[이 기능의 비디오 데모 보기](https://video.tv.adobe.com/v/3412383/){target=_blank}

## 작업 헤더 사용자 정의

이제 Workfront 또는 그룹 관리자는 레이아웃 템플릿을 사용할 때 작업 헤더에 표시되는 필드를 사용자 정의할 수 있습니다.

이 업데이트에는 다음과 같은 개선 사항이 포함됩니다.

* 작업 헤더에서 기존 필드를 제거하거나 다시 정렬합니다.

* 편집할 수 없는 새 작업 개요 필드를 추가합니다. 사용자 정의 필드 또는 편집할 수 있는 필드를 추가할 수 없습니다. 작업 헤더에 현재 있는 편집 가능한 필드(예: 상태 또는 완료율)를 표시할 수도 있습니다.

* 작업 헤더에는 최대 5개의 필드가 포함될 수 있습니다.

이 릴리스 이전에는 프로젝트 헤더만 사용자 지정할 수 있었습니다.

자세한 내용은 [레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)을 참조하십시오.

[이 기능에 대한 비디오 데모를 봅니다.](https://video.tv.adobe.com/v/3412384/){target=_blank}

## 보드의 최신 기능에 대한 초기 기능 옵트인

초기 기능 옵트인을 위해 새 보드 기능을 열게 되어 기쁩니다. 이 선택적 도구는 모든 조직에서 사용할 수 있습니다.

Workfront 관리자만 초기 기능을 선택할 수 있습니다. 관리자가 초기 기능을 선택하면 조직의 모든 사용자가 옵트인되고 프로덕션 Workfront 환경에서 추가 기능이 활성화됩니다.

자세한 내용은 [Adobe Workfront 보드에 대한 초기 기능 옵트인](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md)을 참조하십시오.

[이 기능에 대한 비디오 데모를 봅니다.](https://video.tv.adobe.com/v/3412386/){target=_blank}

## 사용자 정의 양식 필드 계산 편집기에 오류 정보 표시

>[!NOTE]
>
>이 기능은 22.3 릴리스 기간 동안 미리보기 환경에 처음 도입되었습니다. 프로덕션 환경에는 22.4 릴리스와 함께 릴리스됩니다.

이제 계산에 직접 표시된 유용한 오류 정보를 사용하여 사용자 정의 필드에 대한 계산을 보다 쉽게 편집할 수 있습니다. 사용자 정의 양식에서 계산된 필드를 만드는 동안 오류가 분홍색으로 강조 표시됩니다. 강조 표시된 부분을 마우스로 가리키면 문제가 무엇인지 설명하는 도구 설명이 표시됩니다.

자세한 내용은 [사용자 정의 양식에 계산된 데이터 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)를 참조하십시오.

[이 기능에 대한 비디오 데모를 봅니다.](https://video.tv.adobe.com/v/3412387/){target=_blank}

## Adobe 통합 경험으로 마이그레이션

참고: 이 마이그레이션은 2023년 1분기~2분기로 연기되었습니다. 영향을 받는 모든 고객은 해당 시점에 통지됩니다.

조직이 Adobe Admin Console에 온보딩된 경우 Workfront 인스턴스는 22.4 릴리스가 포함된 Adobe 통합 경험으로 마이그레이션됩니다.

통합 경험 Adobe은 다음을 포함합니다.

* Adobe Experience Cloud을 통한 모든 Adobe 애플리케이션에 대한 단일 로그인

* Workfront 조직과 환경 사이를 이동하는 &quot;조직 전환기&quot;

* Workfront 페이지, Adobe Experience Cloud 환경 설정 및 Workfront 프로필에 대한 옵션을 사용하여 탐색

자세한 내용은 [Workfront용 통합 경험 Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)를 참조하십시오.

[이 기능에 대한 비디오 데모를 봅니다.](https://video.tv.adobe.com/v/3412388/){target=_blank}
