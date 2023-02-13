---
title: 22.3 관리자 개선 사항
description: 22.3 관리자 개선 사항
author: Luke
draft: false
feature: Product Announcements
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 0%

---

# 22.3 관리자 개선 사항

이 페이지에서는 미리 보기 환경에 대한 22.3 릴리스로 향상된 모든 관리자 기능을 설명합니다. 이러한 개선 사항은 2022년 7월 11일이 있는 주에 제공됩니다. 22.3 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [22.3 릴리스 개요](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## JumpSeat와 Adobe Workfront 통합

이제 JumpSeat를 Workfront과 통합하여 사용자를 위한 맞춤형 제품 내 지침을 만들 수 있습니다. 통합을 사용하려면 Adobe Workfront 엔터프라이즈 라이센스와 활성 JumpSeat 구독이 있어야 합니다.

자세한 내용은 [JumpSeat 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## 증명 기본 설정이 Workfront으로 이동되었습니다.

이제 Workfront 설정 영역 내에서 다음 증명 설정을 편집할 수 있습니다.

* 증명 기본 설정

* 증명 결정 설정

자세한 내용은 [기본 증명 설정 구성](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).

## 승인 프로세스에서 잠금 해제된 상태 사용

**참고:** 22.3 프로덕션 릴리스에서 제거되었습니다. 이 기능은 2022년 9월 15일에 프로덕션에 릴리스될 예정입니다.

시스템의 승인 프로세스 및 상태를 보다 세밀하게 제어할 수 있도록 잠금 해제된 시스템 상태에 따라 승인 프로세스를 만들 수 있도록 했습니다. 또한 승인 프로세스에서 이미 사용되고 있는 모든 상태의 잠금을 해제할 수도 있습니다.

이전에는 승인 프로세스에서 사용된 시스템 상태를 잠가야 했습니다. 따라서 그룹 관리자가 특정 요구에 맞게 그룹의 상태 목록을 간소화할 수 없었습니다.

자세한 내용은 다음 문서를 참조하십시오.

* [작업 항목에 대한 승인 프로세스 생성](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [상태 만들기 또는 편집](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [잠금 및 잠금 해제된 시스템 수준 상태](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## 사용자 지정 양식에 PDF 파일 추가

Adobe는 이미지 및 비디오와 같이 추가할 수 있는 새로운 자산 위젯을 통해 사용자 지정 양식을 보다 시각적이고 유용한 정보를 계속 제공합니다. 이제 PDF 파일에 대한 링크를 사용자 지정 양식에 추가할 수 있습니다. 양식이 개체에 연결되면 개체를 사용하여 작업하는 사용자는 양식 내에서 PDF을 보고 상호 작용할 수 있습니다.

자세한 내용은 [사용자 지정 양식에서 이미지 또는 기타 자산 위젯을 추가하거나 편집합니다](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## 사용자 지정 양식 필드 계산 편집기에 오류 정보가 표시됩니다

>[!NOTE]
>
>이 기능은 일시적으로 사용할 수 없습니다. 이 페이지는 기능을 사용할 수 있으면 업데이트됩니다.

이제 계산에 직접 표시되는 유용한 오류 정보를 사용하면 사용자 지정 필드에 대한 계산을 더 쉽게 편집할 수 있습니다. 사용자 지정 양식에 계산된 필드를 만드는 동안 오류가 분홍색으로 강조 표시됩니다. 강조 표시된 부분을 마우스로 가리키면 문제가 무엇인지 설명하는 도구 설명이 표시됩니다.

자세한 내용은 [사용자 지정 양식에 계산된 데이터 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## 프로젝트 헤더 사용자 지정

이제 Workfront 또는 그룹 관리자는 레이아웃 템플릿을 사용할 때 프로젝트 헤더에 표시되는 필드를 사용자 지정할 수 있습니다.

이 업데이트에는 다음과 같은 개선 사항이 포함됩니다.

* 프로젝트 헤더에서 기존 필드를 제거합니다.

* 편집할 수 없는 새 프로젝트 개요 필드를 추가합니다. 편집할 수 있는 사용자 지정 필드나 필드는 추가할 수 없습니다. 현재 프로젝트 헤더에 있는 편집 가능한 필드는 헤더에 남아 있을 수 있습니다.

* 개체 헤더에는 최대 5개의 필드가 포함될 수 있습니다.


이 릴리스 이전에는 개체 헤더의 필드를 사용자 지정할 수 없었습니다.

자세한 내용은 [레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## 빈 프로젝트 만들기 컨트롤

이제 시스템 또는 그룹 관리자가 템플릿을 사용하지 않고 사용자가 빈 프로젝트를 만들 수 있는지 여부를 제어할 수 있습니다. 다음 영역에서 빈 프로젝트 만들기를 비활성화할 수 있는 설정 의 프로젝트 환경 설정 영역에 새 설정이 도입되었습니다.

* 프로젝트 목록의 새 프로젝트 옵션에서

* 문제 페이지에서 프로젝트로 문제를 변환할 때


새 설정은 &quot;템플릿을 사용하지 않고 사용자가 프로젝트를 만들 수 있도록 허용&quot;이며, 기본적으로 활성화되어 있습니다.

**참고:** 사용자는 여전히 작업을 빈 프로젝트로 변환할 수 있습니다.

자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## 그룹 페이지에서 그룹 비활성화

최근에 그룹을 비활성화하고 다시 활성화하는 기능을 추가했습니다. 해당 작업을 보다 빠르고 쉽게 수행할 수 있도록 그룹의 페이지에 추가했습니다. 이제 그룹 이름을 클릭하여 해당 페이지로 이동한 후 자세히 메뉴를 선택할 수 있습니다 ![](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) 그룹 이름 옆의 활성화 또는 재활성화를 선택합니다.

이전에는 세부 정보 페이지에서 활성 상태임 확인란을 사용해야만 그룹을 비활성화하거나 다시 활성화할 수 있었습니다.

자세한 내용은 [그룹 비활성화 또는 다시 활성화](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## 사용자 지정 양식에 비디오 추가

이제 비디오를 추가하여 새로운 정보 모드, 시각적 관심사 및 창의성을 사용자 지정 양식에 제공할 수 있습니다. 양식이 개체에 연결되면 개체를 사용하여 작업하는 사용자는 언제든지 비디오를 재생할 수 있습니다.

이전에는 텍스트 기반 필드와 이미지만 사용자 지정 양식에 추가할 수 있었습니다.

자세한 내용은 [사용자 지정 양식에서 이미지 또는 비디오 자산 위젯을 추가하거나 편집합니다](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

