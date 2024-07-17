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
source-wordcount: '425'
ht-degree: 0%

---

# Adobe Experience Manager 레거시 커넥터를 사용하여 Workfront 제거

Workfront과 Adobe Experience Manager Assetsas a Cloud Service 를 연결하는 최신 기본 통합에 Workfront Adobe Experience Manager 레거시 커넥터를 제거해야 합니다.

## Workfront 구독 취소

1. Adobe Experience Manager를 엽니다.
1. Experience Manager에서 **도구** > **Cloud Service** > **Workfront 통합 구성**&#x200B;으로 이동합니다.
1. 구성(기본적으로 global-workfront)을 선택하고 **속성**을 클릭합니다.
   ![workfront에서 구독 취소](assets/unsubscribe-from-workfront.png)
1. 문서, 댓글 및 메타데이터 동기화를 비활성화합니다. 레이블은 비활성화로 설정되어야 합니다.
이렇게 하면 Workfront의 구독이 제거되고 사용자는 Day CQ 링크 외부화에 정의된 동일한 URL을 사용하여 새 구독을 만들 수 있습니다.

## Workfront 통합 구성 삭제

구독을 제거한 후에는 이제 Workfront 통합 구성을 삭제해도 안전합니다.

1. 구성을 열고 **삭제**를 선택합니다.
   ![구성 삭제](assets/delete-wf-configuration.png)

## 매핑 제거

그런 다음 Workfront 속성 매핑을 삭제해야 합니다.

1. Experience Manager에서 **도구** > **Assets** > **Workfront 속성 매핑**&#x200B;으로 이동합니다.

1. 모든 매핑을 선택하고 **삭제**&#x200B;를 클릭합니다.

## 사용자 권한

Workfront에서 AEM Dam에 액세스하는 모든 사용자에게 `/content/dam`에 대한 읽기 권한이 부여되었습니다. 사용자에게 더 이상 필요하지 않은 경우 해당 사용자에게 부여된 권한을 제거할 수 있습니다.

커넥터는 시스템 사용자 workfront-service를 사용하여 작동합니다. 커넥터를 제거하면 제거됩니다.

>[!NOTE]
>
>Connector 버전 2.0.3을 사용 중이며 `workfront-aem-connector-group` 그룹을 추가한 경우 **도구** > **보안** > **그룹**(으)로도 이동하여 이를 제거해야 합니다.

## 일별 CQ 링크 외부화

Day CQ 링크 외부화가 필요하지 않은 경우 `/system/console/configMgr`(으)로 이동하여 &#39;Day CQ 링크 외부화&#39;를 찾으면 이를 `localhost:4502`(으)로 되돌릴 수 있습니다.

>[!NOTE]
>
>Adobe Experience Manager as a Cloud Service을 사용하는 경우 프로젝트를 살펴보고 _ui.apps/src/main/content/jcr_root/apps/mysite/config_ 내의 _com.day.cq.commons.impl.ExternalizerImpl.xml_ 파일을 찾아 이 설정을 변경할 수 있습니다.

![일 CQ 링크 외부화](assets/Day-CQ-Link-Externalizer.png)

## 커넥터 패키지 제거

커넥터 패키지를 제거하는 데 필요한 단계는 사용 중인 Adobe Experience Manager 버전에 따라 다릅니다.

### Adobe Experience Manager On-Premise

Adobe Experience Manager 온-프레미스를 사용하는 경우 _crx/packmgr/index.jsp_(으)로 이동하여 `workfront-aem-connector.all-<version>.zip`을(를) 찾은 다음 **자세히**&#x200B;를 클릭한 다음 **제거**&#x200B;를 클릭합니다.

`/conf` 아래에서 Workfront에서 만든 모든 파일이 제거되었는지 확인하십시오.

### Adobe Experience Manager as a Cloud Service

Adobe Experience Manager as a Cloud Service의 경우 프로젝트의 pom.files에서 커넥터에 대한 종속성을 제거할 수 있습니다.

## 방화벽 및 Dispatcher

통신이 더 이상 필요하지 않은 경우 화이트리스트에 추가한 Workfront URL을 제거하는 것을 잊지 마십시오. 또한 커넥터는 Dispatcher로 설정된 headers apiKey 및 사용자 이름을 사용합니다. 이러한 매개 변수도 제거할 수 있습니다.
