---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Adobe Experience Manager 통합 문제 해결
description: '문제: Assets이 Adobe Experience Manager에 저장되지 않음'
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: f7e31e20-01e3-462d-9020-005e155f0259
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Adobe Experience Manager 통합 문제 해결

## 문제: Assets이 Adobe Experience Manager에 저장되지 않음

사용자가 Experience Manager Assets으로 내보낼 에셋 또는 폴더를 선택하고 선택을 클릭하면 선택기 창이 닫히지만 에셋이 Experience Manager Assets에 저장되지 않습니다. 자산이 Workfront에 저장되지 않았다는 Experience Manager Assets의 표시는 없습니다.

### 원인

이는 Adobe Cloud Manager의 허용 목록에 추가하다 때문에 발생할 수 있습니다. 조직의 Adobe Cloud Manager 허용 목록이 비어 있으면 IP 주소가 제한되지 않으며 Workfront은 Adobe Experience Manager에서 조직의 폴더 및 에셋에 액세스할 수 있습니다. 단, 단일 IP 주소가 Cloud Manager허용 목록에 추가하다 에 추가되는 경우에도 허용 목록에 추가하다는 목록에 없는 모든 IP 주소가 허용되지 않는다고 가정합니다. 따라서 Cloud Manager에 IP 주소가 포함된 경우 Workfront에서 Experience Manager Assets으로 자산을 전송할 수 있도록 하려면 Workfront 허용 목록에 추가하다 IP 주소도 허용 목록에 추가하다에 추가해야 합니다.

### 해결 방법:

Adobe Cloud Manager Workfront에 허용 목록에 추가하다 IP 주소를 추가합니다.

* Adobe Cloud Manager에 IP 주소를 추가하는 방법에 대한 지침은 Adobe Experience Manager 설명서에서 [IP 허용 목록 소개](https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction)를 참조하십시오.
* Workfront에 추가할 허용 목록에 추가하다 IP 주소 목록을 보려면 [방화벽 구성](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md)을 참조하십시오.
