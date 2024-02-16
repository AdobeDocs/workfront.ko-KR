---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1 기타 개선 사항
description: 이 페이지에서는 2020.1 릴리스와 함께 Workfront의 일반 영역에 대해 향상된 모든 기능을 설명합니다. 이러한 개선 사항은 현재 미리보기 환경에서 사용할 수 있으며 2020년 3월 말 또는 4월 초에 프로덕션 환경에서 사용할 수 있습니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a716590c-c833-458a-a138-9bc0723e5896
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# 2020.1 기타 개선 사항

이 페이지에서는 2020.1 릴리스와 함께 Workfront의 일반 영역에 대해 향상된 모든 기능을 설명합니다. 이러한 개선 사항은 현재 미리보기 환경에서 사용할 수 있으며 2020년 3월 말 또는 4월 초에 프로덕션 환경에서 사용할 수 있습니다.

2020.1 릴리스에서 사용할 수 있는 모든 변경 사항의 목록은 을 참조하십시오. [2020.1 릴리스 개요](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## 허용 목록에 추가하다에 증명을 추가하는 데 필요한 변경 사항

>[!NOTE]
>
>이 기능은 2020.1 릴리스에서 제거되었습니다. 나중에 사용할 수 있게 됩니다.

증명 도메인이 from proofhq.com에서 workfront.com으로 변경됩니다.

방화벽 또는 메일 서버가 특정 공급업체에 대한 액세스만 허용하도록 구성된 경우 브라우저 증명 뷰어와 데스크탑 증명 뷰어 모두에서 Workfront 내의 증명을 사용자가 볼 수 있도록 하기 위해 허용 목록에 추가하다 조직에 다음 추가 URL을 추가해야 합니다.

&#42;.workfront.com

다음 &#42;proofhq.com URL도 필요합니다.

허용 목록에 추가하다 업데이트에 대한 자세한 내용은 다음을 참조하십시오. [허용 목록에 추가하다 방화벽 구성](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

>[!NOTE]
>
>이 업데이트는 Workfront 내의 증명에만 적용되며 Workfront Proof 독립형 응용 프로그램을 사용하는 경우에는 적용되지 않습니다.

## Chrome과의 호환성을 유지하기 위해 업데이트된 Workfront 쿠키 동작

예정된 Google Chrome 업데이트(Chrome v80)와의 호환성을 유지하기 위해 Workfront 플랫폼이 요청으로 쿠키가 적절하게 전송되도록 업데이트했습니다.

이 Chrome 업데이트는 SameSite 쿠키 속성의 기본값을 변경합니다. Google Chrome 업데이트 후 Workfront 인스턴스가 어떻게 작동하는지 테스트하려면 Chrome에서 플래그를 조정하고 다음 옵션을 활성화합니다.

* &quot;SameSite를 기본 쿠키로 지정&quot;
* &quot;SameSite가 없는 쿠키를 보호해야 함&quot;

## Workfront 주석이 Jira에 동기화됨

이제 Workfront for Jira 통합은 Workfront 주석을 Jira의 기본 주석 스트림과 동기화합니다.

이전에는 Jira에서 Workfront으로 주석을 동기화할 수 있었지만 Workfront에서 Jira로 주석을 동기화할 수 없었습니다.

자세한 내용은 [Jira용 Adobe Workfront 구성](../../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Flash Portfolio 최적화 도구 가 제거되었습니다.

모든 고객을 위해 Workfront Classic 환경에서 새 Optimizer와 기존(Flash 기반) Portfolio Optimizer 간 전환 기능을 제거했습니다. 레거시 Portfolio 최적화 프로그램은 더 이상 사용되지 않는 기능이며 새로운 도구는 현재 동일한 기능을 제공합니다.

포트폴리오 최적화 도구에 대한 자세한 내용은 https://experience.workfront.com/s/article/Understanding-the-Portfolio-Optimizer-356650079 을 참조하십시오.

Workfront에서 Flash 기반 도구를 사용하지 않는 방법에 대한 자세한 내용은 다음을 참조하십시오. [Adobe Workfront에서 Flash 기반 도구 교체](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).
