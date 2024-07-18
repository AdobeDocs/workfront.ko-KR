---
title: 22.3 관리자 개선 사항
description: 22.3 관리자 개선 사항
author: Luke
draft: false
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 0%

---

# 22.3 관리자 개선 사항

이 페이지에서는 미리보기 환경에 대한 22.3 릴리스의 모든 관리자 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2022년 7월 11일이 있는 주에 사용할 수 있습니다. 22.3 릴리스에서 사용할 수 있는 모든 변경 사항 목록을 보려면 [22.3 릴리스 개요](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md)를 참조하십시오.

## Adobe Workfront과 JumpSeat 통합

이제 JumpSeat를 Workfront과 통합하여 사용자를 위한 맞춤형 제품 내 지침을 만들 수 있습니다. 통합을 사용하려면 Adobe Workfront 엔터프라이즈 라이선스와 활성 JumpSeat 구독이 있어야 합니다.

자세한 내용은 [JumpSeat 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md)을 참조하십시오.

## 증명 기본 설정이 Workfront으로 이동됨

이제 Workfront 설정 영역 내에서 다음 증명 설정을 편집할 수 있습니다.

* 증명 기본 설정

* 증명 결정 설정

자세한 내용은 [기본 증명 설정 구성](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md)을 참조하십시오.

## 승인 프로세스에서 잠금 해제된 상태 사용

**참고:**&#x200B;이(가) 22.3 프로덕션 릴리스에서 제거되었습니다. 이 기능은 2022년 9월 15일에 프로덕션에 릴리스될 예정입니다.

시스템의 승인 프로세스 및 상태를 보다 세밀하게 제어할 수 있도록 잠금 해제된 시스템 상태를 기반으로 승인 프로세스를 만들 수 있도록 했습니다. 또한 이제 승인 프로세스에서 이미 사용된 모든 상태를 잠금 해제할 수 있습니다.

이전에는 승인 프로세스에 사용되는 시스템 상태를 잠가야 했습니다. 따라서 그룹 관리자는 그룹 상태를 제거하거나 이름을 변경하지 않고도 모든 그룹에서 사용할 수 있으므로 그룹 관리자가 특정 요구 사항에 맞게 그룹 상태 목록을 간소화할 수 없었습니다.

자세한 내용은 다음 문서를 참조하십시오.

* [작업 항목에 대한 승인 프로세스 만들기](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [상태 만들기 또는 편집](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [잠김 및 잠금 해제된 시스템 수준 상태](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## 사용자 정의 양식에 PDF 파일 추가

이미지 및 비디오와 같은 추가할 수 있는 새로운 에셋 위젯을 통해 사용자 정의 양식을 보다 시각적이고 유익하게 만들 수 있도록 지속적으로 지원하고 있습니다. 이제 사용자 정의 양식에 PDF 파일에 대한 링크를 추가할 수 있습니다. 양식이 오브젝트에 첨부되어 있으면 오브젝트와 함께 작업하는 사용자는 양식 내에서 PDF을 보고 상호 작용할 수 있습니다.

## 사용자 정의 양식 필드 계산 편집기에 오류 정보 표시

>[!NOTE]
>
>이 기능은 일시적으로 사용할 수 없습니다. 이 기능을 사용할 수 있으면 이 페이지가 업데이트됩니다.

이제 계산에 직접 표시된 유용한 오류 정보를 사용하여 사용자 정의 필드에 대한 계산을 보다 쉽게 편집할 수 있습니다. 사용자 정의 양식에서 계산된 필드를 만드는 동안 오류가 분홍색으로 강조 표시됩니다. 강조 표시된 부분을 마우스로 가리키면 문제가 무엇인지 설명하는 도구 설명이 표시됩니다.

## 프로젝트 헤더 사용자 정의

이제 Workfront 또는 그룹 관리자는 레이아웃 템플릿을 사용할 때 프로젝트의 헤더에 표시되는 필드를 사용자 정의할 수 있습니다.

이 업데이트에는 다음과 같은 개선 사항이 포함됩니다.

* 프로젝트 헤더에서 기존 필드를 제거합니다.

* 편집할 수 없는 새 프로젝트 개요 필드를 추가합니다. 사용자 정의 필드 또는 편집할 수 있는 필드를 추가할 수 없습니다. 현재 프로젝트 헤더에 있는 편집 가능한 필드는 헤더에 남아 있을 수 있습니다.

* 오브젝트 헤더에는 최대 5개의 필드가 포함될 수 있습니다.


이 릴리스 이전에는 개체 헤더의 필드를 사용자 지정할 수 없었습니다.

자세한 내용은 [레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)을 참조하십시오.

## 빈 프로젝트 만들기 제어

시스템 또는 그룹 관리자는 이제 템플릿을 사용하지 않고도 사용자가 빈 프로젝트를 만들 수 있는지 여부를 제어할 수 있습니다. 다음 영역에서 빈 프로젝트 작성을 비활성화할 수 있는 새 설정이 설정의 프로젝트 환경 설정 영역에 도입되었습니다.

* 프로젝트 목록의 새 프로젝트 옵션에서

* 문제 페이지에서 문제를 프로젝트로 전환할 때


새 설정은 &quot;사용자가 템플릿을 사용하지 않고 프로젝트를 만들 수 있도록 허용&quot;이며 기본적으로 활성화됩니다.

**참고:** 사용자는 작업을 빈 프로젝트로 전환할 수 있습니다.

자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

## 그룹 페이지에서 그룹 비활성화

최근에 그룹을 비활성화하고 다시 활성화하는 기능이 추가되었습니다. 이 작업을 더 빠르고 쉽게 수행하기 위해 그룹의 페이지에 이 작업을 추가했습니다. 이제 그룹 이름을 클릭하여 해당 페이지로 이동한 후 그룹 이름 옆에 있는 기타 메뉴 ![](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png)을(를) 선택한 다음 비활성화 또는 다시 활성화를 선택할 수 있습니다.

이전에는 세부 정보 페이지의 활성 확인란을 통해서만 그룹을 비활성화하거나 다시 활성화할 수 있었습니다.

자세한 내용은 [그룹 비활성화 또는 다시 활성화](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md)를 참조하십시오.

## 사용자 정의 양식에 비디오 추가

이제 비디오를 추가하여 사용자 정의 양식에 새로운 정보, 시각적 관심사 및 창의성 모드를 제공할 수 있습니다. 양식이 오브젝트에 첨부되면 해당 오브젝트로 작업하는 사용자는 언제든지 비디오를 재생할 수 있습니다.

이전에는 사용자 정의 양식에 텍스트 기반 필드 및 이미지만 추가할 수 있었습니다.

