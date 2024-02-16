---
title: 21.4 통합 개선 사항
description: 21.4 통합 개선 사항
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# 21.4 통합 개선 사항

이 페이지에서는 미리보기 환경에 대한 21.4 릴리스의 모든 통합 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 10월 4일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다.

21.4 릴리스에서 사용할 수 있는 모든 변경 사항의 목록은 을 참조하십시오. [21.4 릴리스 개요](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## Dropbox 비즈니스에서 문서 연결

Dropbox 비즈니스를 사용 가능한 문서 통합으로 추가했습니다. 이제 Workfront 내부에서 직접 Dropbox 비즈니스에 저장한 문서에 액세스할 수 있습니다.

Dropbox 비즈니스를 사용하면 공유 문서를 연결하고 문서를 공유 폴더에 업로드할 수 있습니다. Dropbox(Dropbox 비즈니스 아님)에서는 문서 소유자만 Workfront에서 문서를 볼 수 있습니다.

Workfront 관리자가 조직에 대해 이 통합을 활성화할 수 있습니다.

자세한 내용은 [외부 애플리케이션에서 문서 연결](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Workfront 관리자가 이 옵션을 활성화할 수 있는 방법에 대한 자세한 내용은 [문서 통합 구성](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Slack을 위한 Workfront 업데이트

이제 다음 업데이트가 Slack 통합을 위한 Workfront에 표시됩니다.

* Workfront for Slack은 새로운 모양과 느낌을 제공합니다.
* 이제 실시간으로 Slack 알림용 Workfront을 받게 됩니다.

  예를 들어 작업에 할당되면 할당되자마자 해당 알림을 받습니다. 이전에는 Slack에 알림이 표시되기 전에 지연이 있을 수 있었습니다.

이 업데이트를 사용하려면 Slack 통합을 위해 Workfront을 재승인해야 합니다. 통합 인증에 대한 자세한 내용은 다음을 참조하십시오. [Slack을 위한 Adobe Workfront 구성](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Slack 알림용 Workfront에 대한 자세한 내용은 [Slack에서 Adobe Workfront 알림 수신](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Adobe Workfront 통합에 동의할 때 계정 액세스에 대한 세부 사항을 보다 명확하게 볼 수 있습니다

이제 Adobe Workfront 통합에 대한 동의 화면이 업데이트되었습니다. 이제 통합에서 액세스할 수 있는 특정 작업 및 영역을 볼 수 있으므로 통합 또는 애플리케이션에서 액세스를 허용하는 내용을 더 잘 이해할 수 있습니다.

이 새 동의 화면은 OAuth 2.0을 사용하는 모든 Adobe Workfront 통합에 적용됩니다.

특정 통합에 대한 자세한 내용은 해당 통합의 설명서를 참조하십시오.

## 통합을 위해 더 이상 API 키 인증이 필요하지 않음

Workfront 통합은 최근 강화된 보안 및 유용성을 위해 OAuth2를 사용하기 시작했습니다. 이러한 움직임의 일부로 Workfront에는 통합 인증을 위한 API 키가 더 이상 필요하지 않습니다.
