---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 기존 또는 향상된 커넥터에서 Adobe Experience Manager as a Cloud Service 통합을 위한 Workfront으로 마이그레이션
description: 이 페이지의 정보에서는 Workfront for Experience Cloud 강화 또는 레거시 커넥터에서 Workfront 및 Adobe Experience Manager Assets as a Cloud Service을 연결하는 최신 기본 통합으로 이동하는 모범 사례를 설명합니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: f381b37e6d4537e6f83e55ed4a2f4ff7f868dd54
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# 기존 또는 향상된 커넥터에서 Adobe Experience Manager as a Cloud Service 통합을 위한 Workfront으로 마이그레이션

이 페이지의 정보에서는 Workfront for Experience Cloud 강화 또는 레거시 커넥터에서 Workfront 및 Adobe Experience Manager Assets as a Cloud Service을 연결하는 최신 기본 통합으로 이동하는 모범 사례를 설명합니다.

>[!IMPORTANT]
>
>이 정보는 Adobe Experience Manager Assets On-Premise 또는 Managed Services 환경을 사용하는 고객에게는 적용되지 않습니다.

## Workfront 인스턴스를 Admin Console으로 이동

>[!IMPORTANT]
>
>모든 Workfront 조직이 Adobe Admin Console으로 마이그레이션되었으므로 이 섹션은 가까운 미래에 제거됩니다.

<!--DELETE THIS SECTION MARCH 2026-->

<!--
Customers that intend to use the new native integration between Workfront and Adobe Experience Manager Assets as a Cloud Service must ensure their Workfront environment is tied to an Adobe Admin Console. For existing Workfront environments, this will likely require a migration of the environment to a connected Adobe Admin Console. For more details regarding this migration and the associated checklist, see [Prepare to onboard your organization to the Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md). 

 Adobe must help carry out this migration. To request help, do one of the following:

* If you have Workfront Hub access, submit your request to the [Workfront Migration to Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=629674d500054a38133cf26e01d06a97&path=).
* If you do not have Workfront Hub access, you can submit your request to the [Workfront to Adobe Admin Console Early Migration Request Queue](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

-->

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
