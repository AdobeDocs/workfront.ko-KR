---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 기존 커넥터에서 향상된 커넥터로 마이그레이션
description: 다음 프로세스에서는 Adobe Experience Manager 레거시 커넥터를 Adobe Workfront과 AEM Assets의 통합을 위한 향상된 커넥터로 이전하는 모범 사례에 대해 간략히 설명합니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# 기존 커넥터에서 향상된 커넥터로 마이그레이션

다음 프로세스에서는 Adobe Experience Manager 레거시 커넥터를 Adobe Workfront과 AEM Assets의 통합을 위한 향상된 커넥터로 이전하는 모범 사례에 대해 간략히 설명합니다.

>[!IMPORTANT]
>
>이 설명서는 Adobe Experience Manager Assets On-Premise 또는 Managed Services 환경을 사용하는 고객에게만 적용됩니다.


Adobe Experience Manager Assets as a Cloud Service을 사용하는 고객의 경우 기존 커넥터의 마이그레이션 경로가 Workfront 내의 새로운 기본 통합으로 변경됩니다. 이 마이그레이션 프로세스에 대한 자세한 내용은 [기존 또는 향상된 커넥터에서 Adobe Experience Manager as a Cloud Service 통합을 위한 Workfront으로 마이그레이션](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md)을 참조하세요.

## 향상된 커넥터 구현

>[!IMPORTANT]
>
>향상된 커넥터를 구현하려면 인증된 파트너 또는 Adobe Consulting 서비스가 필요합니다.
>
> 향상된 커넥터에서 인증하려는 파트너는 다음 문서를 검토하십시오. [Workfront for Experience Manager 향상된 커넥터 전문가 시리즈](https://experienceleague.adobe.com/ko/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview).

향상된 커넥터를 구현하려면 [Experience Manager용 Workfront 강화 커넥터 구성](https://experienceleague.adobe.com/ko/docs/experience-manager-65/content/assets/integrations/workfront-connector-configure)을 참조하십시오.


## 기존 에셋 이동

환경을 구성한 후 연결된 기존 에셋 및 폴더를 Adobe Experience Manager으로 이동할 수 있습니다. 이 단계는 선택 사항이지만, 레거시 커넥터를 제거하면 레거시 커넥터를 통해 이전에 연결된 폴더 및 에셋에 계속 액세스할 수 있습니다.

자산 이동에 대한 자세한 내용은 [연결된 폴더 및 문서 마이그레이션](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md)을 참조하세요.

## 사용하려는 모든 주요 사용 사례 확인

기존 커넥터를 제거하기 전에 향상된 커넥터를 통해 사용하려는 모든 주요 사용 사례를 확인해야 합니다.

## 레거시 커넥터 제거

마지막으로 레거시 커넥터를 제거해야 합니다. 레거시 커넥터는 향상된 커넥터와 병렬로 실행되지 않습니다.

제거하려면 [Adobe Experience Manager 레거시 커넥터로 Workfront 제거](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md)를 참조하십시오.
