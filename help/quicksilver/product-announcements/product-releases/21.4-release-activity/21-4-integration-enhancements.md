---
title: 21.4 통합 개선 사항
description: 21.4 통합 개선 사항
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# 21.4 통합 개선 사항

이 페이지에서는 미리 보기 환경에 대한 21.4 릴리스에서 향상된 모든 통합 기능을 설명합니다. 이러한 개선 사항은 2021년 10월 4일이 있는 프로덕션 환경에서 사용할 수 있습니다.

21.4 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [21.4 릴리스 개요](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## Dropbox 비즈니스에서 문서 연결

사용 가능한 문서 통합으로 Dropbox 비즈니스 을 추가했습니다. 이제 Workfront 내에서 Analytics Business에 저장한 문서에 직접 액세스할 수 있습니다.

Dropbox 비즈니스에서는 공유 문서를 연결하고 공유 폴더에 문서를 업로드할 수 있습니다. Dropbox(Dropbox 비즈니스 아님)에서는 문서 소유자만 Workfront에서 문서를 볼 수 있습니다.

Workfront 관리자가 조직에 대해 이 통합을 활성화할 수 있습니다.

자세한 내용은 [외부 응용 프로그램에서 문서 연결](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Workfront 관리자가 이 옵션을 활성화할 수 있는 방법에 대한 자세한 내용은 [문서 통합 구성](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Slack용 Workfront 업데이트

이제 Slack 통합을 위해 Workfront에 다음 업데이트가 표시됩니다.

* Workfront for Slack의 새로운 모양과 느낌을 확인해 보십시오.
* 이제 Slack 알림에 대한 Workfront을 실시간으로 받게 됩니다.

   예를 들어, 작업에 할당되면 할당되는 즉시 해당 알림을 받게 됩니다. 이전에는 Slack에 알림이 표시되기 전에 지연이 있을 수 있었습니다.

이 업데이트를 사용하려면 Slack 통합을 위해 Workfront을 재인증해야 합니다. 통합 승인에 대한 자세한 내용은 [Slack에 대한 Adobe Workfront 구성](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Slack 알림용 Workfront에 대한 자세한 내용은 [Slack에서 Adobe Workfront 알림 받기](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Adobe Workfront 통합에 동의할 때 계정 액세스 세부 사항을 보다 명확하게 볼 수 있습니다

이제 Adobe Workfront 통합에 대한 동의 화면이 업데이트됩니다. 이제 통합에 액세스할 수 있는 특정 작업 및 영역을 볼 수 있으므로 통합 또는 애플리케이션에서 액세스할 수 있는 항목을 더 잘 이해할 수 있습니다.

이 새 동의 화면은 OAuth 2.0을 사용하는 모든 Adobe Workfront 통합에 적용됩니다.

특정 통합에 대한 자세한 내용은 해당 통합의 설명서를 참조하십시오.

## 통합에 API 키 인증이 더 이상 필요하지 않습니다

Workfront 통합은 보안 및 유용성 향상을 위해 OAuth2 를 사용하여 최근에 시작되었습니다. 이러한 움직임의 일부로, Workfront에는 통합 인증을 위한 API 키가 더 이상 필요하지 않습니다.
