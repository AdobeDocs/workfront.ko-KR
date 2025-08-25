---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 기존 또는 향상된 커넥터에서 Adobe Experience Manager as a Cloud Service 통합을 위한 Workfront으로 마이그레이션
description: 이 페이지의 정보에서는 Workfront for Experience Cloud 강화 또는 레거시 커넥터에서 Workfront 및 Adobe Experience Manager Assets as a Cloud Service을 연결하는 최신 기본 통합으로 이동하는 모범 사례를 설명합니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: a25eb28800ca8bbeeffedb521b3d72c8df71c697
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# 기존 또는 향상된 커넥터에서 Adobe Experience Manager as a Cloud Service 통합을 위한 Workfront으로 마이그레이션

이 페이지의 정보에서는 Workfront for Experience Cloud 강화 또는 레거시 커넥터에서 Workfront 및 Adobe Experience Manager Assets as a Cloud Service을 연결하는 최신 기본 통합으로 이동하는 모범 사례를 설명합니다.

>[!IMPORTANT]
>
>이 정보는 Adobe Experience Manager Assets On-Premise 또는 Managed Services 환경을 사용하는 고객에게는 적용되지 않습니다.

## Workfront 인스턴스를 Admin Console으로 이동

Workfront과 Adobe Experience Manager Assets as a Cloud Service 간의 새로운 기본 통합을 사용하려는 고객은 Workfront 환경이 Adobe Admin Console에 연결되어 있는지 확인해야 합니다. 기존 Workfront 환경의 경우 연결된 Adobe Admin Console으로 환경을 마이그레이션해야 할 수 있습니다. 이 마이그레이션 및 관련 검사 목록에 대한 자세한 내용은 [Adobe Admin Console에 조직을 온보딩하기 위한 준비](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)를 참조하십시오.

Adobe이 이 마이그레이션을 수행하는 데 도움이 되어야 합니다. 도움말을 요청하려면 다음 중 하나를 수행하십시오.

* Workfront Hub 액세스 권한이 있는 경우 [Adobe Admin Console으로 Workfront 마이그레이션](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=629674d500054a38133cf26e01d06a97&path=)에 요청을 제출하십시오.
* Workfront Hub 액세스 권한이 없는 경우 [Adobe Admin Console에서 Workfront 조기 마이그레이션 요청 큐](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi)로 요청을 제출할 수 있습니다.

## Adobe Experience Manager assets as a Cloud Service 통합을 위한 새 Workfront 구성

Workfront 환경이 Adobe Admin Console으로 마이그레이션된 후 Workfront 관리자는 새로운 기본 통합을 구성할 수 있습니다. 구성 도움말은 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)을 참조하십시오.

## 기존 자산을 Adobe Experience Manager assets as a Cloud Service 통합용 Workfront으로 이동

환경을 구성한 후 연결된 기존 에셋 및 폴더를 Adobe Experience Manager으로 이동할 수 있습니다. 선택적 단계이지만 레거시 또는 향상된 커넥터를 통해 이전에 연결된 폴더 및 자산에 연결된 커넥터를 제거한 후에도 계속 액세스할 수 있습니다.

자산 이동에 대한 자세한 내용은 [연결된 폴더 및 문서 마이그레이션](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md)을 참조하세요.

## 사용하려는 모든 주요 사용 사례 확인

기존 또는 향상된 커넥터를 제거하기 전에 기본 통합을 통해 사용하려는 모든 중요한 사용 사례를 확인해야 합니다.

## 레거시 또는 향상된 커넥터 제거

마지막으로, 기존 또는 향상된 커넥터를 제거해야 합니다. 기본 통합은 두 커넥터 중 하나와 병렬로 실행하기 위한 것이 아닙니다.

제거하려면 다음을 참조하십시오.

* 레거시 커넥터 제거 지침: [Adobe Experience Manager 레거시 커넥터로 Workfront 제거](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* 향상된 커넥터 제거 지침: [Adobe Experience Manager 강화 커넥터를 사용하여 Workfront 제거](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
