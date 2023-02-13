---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 레거시 커넥터에서 고급 커넥터로 마이그레이션
description: 다음 프로세스에서는 Adobe Workfront과 AEM Assets을 통합하기 위해 Adobe Experience Manager 레거시 커넥터를 고급 커넥터로 이동하는 우수 사례를 간략하게 설명합니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# 레거시 커넥터에서 고급 커넥터로 마이그레이션

다음 프로세스에서는 Adobe Workfront과 AEM Assets을 통합하기 위해 Adobe Experience Manager 레거시 커넥터를 고급 커넥터로 이동하는 우수 사례를 간략하게 설명합니다.

>[!IMPORTANT]
>
>이 설명서는 Adobe Experience Manager Assets 온-프레미스 또는 Managed Services 환경을 사용하는 고객에게만 적용됩니다.


Adobe Experience Manager Assets as a Cloud Service의 고객을 위해 기존 커넥터의 마이그레이션 경로는 Workfront 내의 새로운 기본 통합으로 설정됩니다. 이 마이그레이션 프로세스에 대한 자세한 내용은 [레거시 또는 향상된 커넥터에서 Adobe Experience Manager as a Cloud Service 통합을 위한 Workfront으로 마이그레이션](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md).

## 향상된 커넥터 구현

>[!IMPORTANT]
>
>향상된 커넥터를 구현하려면 인증된 파트너 또는 Adobe 컨설팅 서비스가 필요합니다.
>
> enhanced 커넥터에 대한 인증을 원하는 파트너는 다음 문서를 검토하십시오. [Workfront for Experience Manager enhanced connector Expert Series](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview.html?lang=en).

향상된 커넥터를 구현하려면 다음을 참조하십시오 [Experience Manager Enhanced Connector에 대한 Workfront 구성](https://experienceleague.adobe.com/docs/experience-manager-65/assets/integrations/workfront-connector-configure.html?lang=en).


## 기존 자산 이동

환경을 구성한 후 기존의 연결된 자산 및 폴더를 Adobe Experience Manager으로 이동할 수 있습니다. 이 단계는 선택적 단계이지만 레거시 커넥터를 제거한 후에도 레거시 커넥터를 통해 이전에 연결된 폴더 및 자산에 계속 액세스할 수 있도록 합니다.

자산 이동에 대한 자세한 내용은 [연결된 폴더 및 문서 마이그레이션](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## 사용할 모든 중요한 사용 사례 확인

레거시 커넥터를 제거하기 전에 고급 커넥터를 통해 사용해야 하는 중요한 사용 사례를 모두 확인해야 합니다.

## 레거시 커넥터 제거

마지막으로 기존 커넥터를 제거해야 합니다. 레거시 커넥터는 향상된 커넥터와 병렬로 실행되지 않습니다.

제거하려면 다음을 참조하십시오 [Adobe Experience Manager 레거시 커넥터를 사용하여 Workfront 제거](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
