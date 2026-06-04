---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta 최종 릴리스 활동
description: 이 페이지에서는 2018.2 Beta 최종 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 기능은 2018년 6월 20일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2018년 7월에 사용할 수 있습니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 36001571-bf8c-4fe8-a66b-09d3726f66d3
TQID: https://experienceleague.adobe.com/s0vTUKOxP1bju3-LqI8JQZLg7uC7GfK0pe33a-1-G54
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: f1b6c8ba-53d0-432b-b0f4-64800d4b376e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 809
ht-degree: 0%

---

# 2018.2 Beta 최종 릴리스 활동

이 페이지에서는 2018.2 Beta 최종 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 기능은 2018년 6월 20일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2018년 7월에 사용할 수 있습니다.

>[!IMPORTANT]
>
> 이 페이지에 설명된 기능은 프로덕션 환경에서 사용하기 전에 변경될 수 있습니다.

2018.2의 모든 변경 사항 목록은 [2018.2 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md)를 참조하십시오.

18.2 프로덕션 릴리스 당시 다음과 같은 새로운 기능이 릴리스됩니다.

* [Workfront 이메일 알림에 회신할 메일 배달 서비스 지정](#specify-mail-delivery-services-for-replying-to-workfront-email-notifications)
* [문서에 대한 댓글에 대한 전자 메일 알림 받기](#receive-email-notifications-for-comments-on-documents)
* [시스템 추적 업데이트에 더 이상 아이콘이 없습니다](#system-tracked-updates-no-longer-contain-an-icon)
* [댓글을 작업으로 변환하는 옵션이 제거되었습니다.](#option-to-convert-a-comment-to-a-task-was-removed)
* [Salesforce용 Workfront](#workfront-for-salesforce)
* [Slack용 Workfront 개선 사항](#workfront-for-slack-improvements)
* [모바일 개선 사항](#mobile-improvements)

## Workfront 이메일 알림에 회신할 메일 게재 서비스 지정 {#specify-mail-delivery-services-for-replying-to-workfront-email-notifications}

이제 Workfront 관리자는 사용자가 이메일 회신을 통해 오브젝트에 대한 주석을 달 수 있도록 Workfront을 구성할 때 메일 게재 서비스를 선택할 수 있습니다. 기본 이메일 서비스 또는 POP 이메일 계정을 사용하도록 Workfront을 구성할 수 있습니다.

이 업데이트 이전에는 Workfront 관리자가 각 사용자에 대한 POP 계정을 설정해야 했습니다. 

POP 이메일 계정 구성에 대한 자세한 내용은 을 참조하십시오.

기본 메일 서비스에 대한 자세한 내용은 을 참조하십시오.

## 문서에 대한 댓글에 대한 이메일 알림 수신 {#receive-email-notifications-for-comments-on-documents}

이제 사용자가 소유한 문서에 대해 다른 사람이 댓글을 다는 경우 이메일 알림을 받습니다. 이 옵션은 기본적으로 활성화되어 있습니다. &quot;내 문서에 댓글이 추가되었습니다&quot; 알림 설정을 사용하여 이메일 알림 옵션을 비활성화할 수 있습니다.

이 변경 이전에는 다른 사용자가 내가 소유한 문서에 주석을 남겼을 때 알림이 수신되지 않았습니다. 

자세한 내용은 [전자 메일 알림 수정](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)을 참조하세요.

>[!NOTE]
>
>이 기능이 처음 릴리스되면 사용자는 이메일 알림과 함께 인앱 알림을 받게 됩니다. 사용자가 소유한 문서에 대해 댓글을 달 때 더 이상 인앱 알림을 받지 않습니다. 

## 시스템 추적 업데이트에 더 이상 아이콘이 없음 {#system-tracked-updates-no-longer-contain-an-icon}

Workfront 시스템에서 오브젝트(예: 프로젝트 내)의 업데이트 영역에서 업데이트를 만들 때마다 해당 업데이트에는 더 이상 해당 아이콘이 포함되지 않습니다.

이 변경 전에 수행된 업데이트를 나타내는 아이콘도 모든 시스템 업데이트에 포함되었습니다.

시스템 업데이트에 대한 자세한 내용은 [시스템 추적 업데이트](../../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md)를 참조하십시오.

## 댓글을 작업으로 변환하는 옵션이 제거되었습니다. {#option-to-convert-a-comment-to-a-task-was-removed}

댓글을 작업으로 변환하는 옵션이 제거되었습니다.

이전에는 개체의 업데이트 영역에 있는 동안 주석을 작업으로 변환할 수 있었습니다.

## Salesforce용 Workfront {#workfront-for-salesforce}

Salesforce과 Workfront 간의 새로운 기본 통합 기능을 출시할 예정입니다. 다음을 수행할 수 있습니다.

* Salesforce 영업 기회가 특정 단계에 도달하거나, 새 제품이 영업 기회에 추가되거나, 계정 유형이 업데이트될 때 자동으로 새 Workfront 프로젝트를 만듭니다.
* Salesforce Opportunity 또는 Account에서 Workfront Request 를 만듭니다.

이 통합은 Workfront Pro 버전 이상을 보유한 모든 고객이 사용할 수 있으며 무료로 제공됩니다.

Salesforce용 Workfront에 대한 자세한 내용은 [Salesforce용 Adobe Workfront](../../../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce.md)을 참조하세요.

## Workfront for Slack 개선 사항 {#workfront-for-slack-improvements}

Slack Workfront 채널에서 Workfront 알림을 받도록 구성할 수 있습니다.

Slack에서 다음 Workfront 알림을 전달하도록 구성할 수도 있습니다.

* 다른 사용자가 댓글 또는 업데이트에서 귀하를 태그하는 경우.
* 새 작업 또는 문제에 할당되었을 때.
* 항목 승인을 요청 받은 경우.

이 개선 이전에는 Slack에서 Workfront 알림을 받을 수 없었습니다.

Slack의 Workfront 알림에 대한 자세한 내용은 [Slack에서 Adobe Workfront 알림 받기](../../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md)를 참조하십시오.

## 모바일 개선 사항 {#mobile-improvements}

다음 새 기능은 18.2 프로덕션 릴리스 당시 모바일 스토어에 릴리스됩니다.

* 개체 이름에 대한 인라인 편집 

  이제 모바일 앱에서 프로젝트, 작업 또는 문제의 이름과 같은 필드를 인라인 편집할 수 있습니다.

* 문서 업로드 

  이제 Workfront 모바일 앱의 개체에 문서를 업로드할 수 있습니다.

* 프로필 사진 업로드 

  이제 iOS 모바일 앱에서 프로필 사진을 업로드할 수 있습니다.

  이 기능은 iOS 모바일 앱에서만 사용할 수 있습니다.

다음 기능은 Workfront 모바일 앱의 Android Beta 버전에 이미 출시되었으며, 공개 Android 및 iOS 모바일 앱에도 출시되고 있습니다. iOS 플랫폼에 대한 경험에는 이미 릴리스된 Android 경험과 다음과 같은 차이점이 포함되어 있습니다.

* iOS의 새로운 하단 탐색 모음 

* iOS용 새로운 튜토리얼 환경 

이러한 기능에 대한 자세한 정보와 이를 보여 주는 비디오를 보려면 [2018.2 Beta 4 릴리스 활동](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-beta-4-release-activity.md) 및 [2018.2 Beta 5 릴리스 활동](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-beta-5-release-activity.md)을 참조하십시오.
