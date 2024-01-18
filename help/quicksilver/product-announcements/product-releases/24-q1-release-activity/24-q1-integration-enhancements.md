---
title: 2024년 1분기 통합 개선 사항
description: 2024년 1분기 통합 개선 사항
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0d581f3c-2aaf-4ac1-97a5-df1b01627080
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# 2024년 1분기 통합 개선 사항

이 페이지에서는 미리보기 환경에 대한 2024년 1분기 릴리스의 모든 통합 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2024년 1분기 릴리스를 통해 프로덕션 환경에서 사용할 수 있습니다.

2024년 1분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항의 목록은 을 참조하십시오. [2024년 1분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

## 이제 Experience Manager Assets Essentials의 메타데이터 매핑에서 을 사용합니다. `xcm:keywords` 대신 `dc:subject`

Experience Manager Assets as a Cloud Service 통합의 경험에 맞게 Experience Manager Assets Essentials 통합을 업데이트했습니다. 이제 여러 한 줄 텍스트 필드를 Experience Manager Assets의 단일 필드에 매핑할 때 두 서비스 모두 `xcm:keywords` 필드.

이전에는 이러한 필드가 `dc:subject` Experience Manager Assets Essentials의 필드. Experience Manager Assets as a Cloud Service 기능은 변경되지 않습니다.

현재 매핑된 모든 Experience Manager Assets Essentials 메타데이터 `dc:subject` 을(를) (으)로 다시 매핑해야 합니다. `xcm:keywords`.

Experience Manager Assets Essentials에 메타데이터를 매핑하는 방법에 대한 자세한 내용은 [AEM 키워드](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md#aem-keyword).

## 이제 Adobe Experience Manager 통합에서 자동 완성 필드를 사용할 수 있습니다.

Workfront과 Adobe Experience Manager 간에 필드를 더 쉽게 연결할 수 있도록 메타데이터 매핑에서 자동 완성 필드에 대한 지원이 추가되었습니다. 이제 자동 완성 필드를 Adobe Experience Manager의 해당 필드에 매핑할 수 있습니다.

사용자가 Workfront에서 필드에 대해 다른 값을 선택하면 이러한 변경 사항이 즉시 Adobe Experience Manager에 반영됩니다. 또한 필드 값 옵션이 변경되는 경우(예: 팀이 이름을 새 이름으로 변경하는 경우) 이러한 변경 사항은 Adobe Experience Manager에도 반영됩니다.

Adobe Experience Manager 통합에서의 메타데이터 매핑에 대한 정보 및 지침은 다음을 참조하십시오. [메타데이터 설정](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-metadata-optional).

## Adobe Experience Manager에서 에셋 자동 게시

Adobe Experience Manager 통합에 다른 워크플로우를 추가했습니다. 이제 Adobe Experience Manager으로 전송할 때 자산을 자동으로 게시하도록 설정할 수 있습니다. Adobe Experience Manager 게시 서비스 또는 Adobe Experience Manager Brand Portal에 게시하도록 통합을 구성할 수 있습니다.

Adobe Experience Manager 통합에서 자동 게시 워크플로우를 활성화하고 구성할 수 있습니다. 활성화되면 프로젝트 템플릿 또는 프로젝트 수준에서 워크플로를 편집할 수 있습니다.

자세한 내용은 [자산 게시](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#publishing-assets) 위치: [Experience Manager Assets 통합에서 워크플로우 사용](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).
