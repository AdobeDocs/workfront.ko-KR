---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Adobe Experience Manager 통합 문제 해결
description: Experience Manager Assets Essentials - EDIT ME에서 작업과 콘텐츠를 연결합니다.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: e4bf79b8c5d53870aec6d415510acccb53a5c7f6
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Adobe Experience Manager 통합 문제 해결

## 문제: 자산이 Adobe Experience Manager에 저장되지 않음

사용자가 Experience Manager Assets으로 내보낼 에셋 또는 폴더를 선택하고 선택을 클릭하면 선택기 창이 닫히지만 에셋이 Experience Manager Assets에 저장되지 않습니다. 자산이 Workfront에 저장되지 않았다는 Experience Manager Assets의 표시는 없습니다.

### 원인

이는 Adobe 클라우드 관리자의 허용 목록에 추가하다 때문에 발생할 수 있습니다. 조직의 Cloud Manager Adobe허용 목록에 추가하다 가 비어 있는 경우 IP 주소가 제한되지 않으며 Workfront은 Adobe Experience Manager에서 조직의 폴더 및 에셋에 액세스할 수 있습니다. 그러나 단일 IP 주소가 Cloud Cloud Manager에 추가되더라도 허용 목록에 추가하다허용 목록에 추가하다 은 목록에 없는 모든 IP 주소는 허용되지 않는다고 가정합니다. 허용 목록에 추가하다 따라서 Cloud Manager에 IP 주소가 포함되어 있는 경우 Workfront을 Experience Manager Assets으로 전송하기 위해 허용 목록에 추가하다 주소에도 Workfront IP 주소를 추가해야 합니다.

### 해결 방법:

Workfront IP 주소를 Cloud Manager Adobe허용 목록에 추가하다 에 추가합니다.

* Adobe Cloud Manager에 IP 주소를 추가하는 방법에 대한 지침은 다음을 참조하십시오. [IP 허용 목록 소개](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction.html?lang=en) Adobe Experience Manager 설명서에서 확인할 수 있습니다.
* Workfront에 추가할 허용 목록에 추가하다 IP 주소 목록은 을 참조하십시오. [방화벽 구성](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).


