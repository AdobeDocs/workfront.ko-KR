---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 레거시 커넥터 제거
description: 텍스트
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4b3834bf-2e6d-4588-8d77-671e14390115
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Adobe Experience Manager 레거시 커넥터를 사용하여 Workfront 제거

Workfront 및 Adobe Experience Manager 자산을 연결하는 최신 기본 통합으로 Adobe Experience Manager 레거시 커넥터를 사용하는 Workfront을 제거해야 합니다.

## Workfront 구독 취소

1. Adobe Experience Manager를 엽니다.
1. Experience Manager에서 **도구** > **Cloud Services** > **Workfront 통합 구성**.
1. 구성(기본적으로 글로벌 워크플로우)을 선택하고 **속성**.
   ![workfront 구독 취소](assets/unsubscribe-from-workfront.png)
1. 문서, 주석 및 메타데이터 동기화를 사용하지 않도록 설정합니다. 레이블은 Disabled로 표시되어야 합니다.
이렇게 하면 Workfront에서 구독이 제거되고 사용자가 Day CQ Link Externalizer에 정의된 동일한 URL을 사용하여 새 구독을 만들 수 있습니다.

## Workfront 통합 구성 삭제

이제 구독을 제거한 후 Workfront 통합 구성을 삭제하는 것이 안전합니다.

1. 구성을 열고 을 선택합니다. **삭제**.
   ![구성 삭제](assets/delete-wf-configuration.png)

## 매핑 제거

그런 다음 Workfront 속성 매핑을 삭제해야 합니다.

1. Experience Manager에서 **도구** > **자산** > **Workfront 속성 매핑**.

1. 모든 매핑을 선택하고 **삭제**.

## 사용자 권한

Workfront에서 AEM Dam에 액세스하는 모든 사용자에게는 `/content/dam`. 사용자가 더 이상 필요하지 않으면 해당 사용자에게 제공된 권한을 제거할 수 있습니다.

커넥터는 시스템 사용자 workfront 서비스를 사용하여 작동합니다. 커넥터를 제거할 때 제거됩니다.

>[!NOTE]
>
>커넥터 버전 2.0.3을 사용하고 그룹을 추가한 경우 `workfront-aem-connector-group`를 채울 때는 다음 위치로 이동하십시오. **도구** > **보안** > **그룹**.

## Day CQ Link Externalizer

일 CQ Link Externalizer가 필요하지 않으면 이 작업을 다시 로 되돌릴 수 있습니다. `localhost:4502` 다음으로 이동 `/system/console/configMgr` 및 &#39;Day CQ Link Externalizer&#39;를 찾습니다.

>[!NOTE]
>
>Adobe Experience Manager as a Cloud Service을 사용하는 경우 프로젝트를 검토하고 파일을 찾아 변경할 수 있습니다 _com.day.cq.commons.impl.ExternalizerImpl.xml_ 내부 _ui.apps/src/main/content/jcr_root/apps/mysite/config_.

![Day CQ Link Externalizer](assets/Day-CQ-Link-Externalizer.png)

## 커넥터 패키지 제거

커넥터 패키지를 제거하는 데 필요한 단계는 보유한 Adobe Experience Manager 버전에 따라 다릅니다.

### Adobe Experience Manager On-Premise

Adobe Experience Manager 온-프레미스를 사용하는 경우, 다음 위치로 이동하십시오. _crx/packmgr/index.jsp_&#x200B;를 검색하고 `workfront-aem-connector.all-<version>.zip`를 클릭합니다. **자세히** 그리고 **제거**.

다음 항목을 확인하십시오 `/conf` Workfront에서 만든 모든 파일이 제거되었는지 확인합니다.

### Adobe Experience Manager as a Cloud Service

Adobe Experience Manager as a Cloud Service의 경우 프로젝트의 pom.files에서 커넥터에 대한 종속성을 제거할 수 있습니다.

## 방화벽 및 디스패처

커뮤니케이션이 더 이상 필요하지 않은 경우 화이트리스트에 추가한 Workfront URL을 제거하는 것을 잊지 마십시오. 또한 커넥터는 디스패처에 설정된 헤더 apiKey 및 사용자 이름을 사용합니다. 이러한 매개 변수도 제거할 수 있습니다.
