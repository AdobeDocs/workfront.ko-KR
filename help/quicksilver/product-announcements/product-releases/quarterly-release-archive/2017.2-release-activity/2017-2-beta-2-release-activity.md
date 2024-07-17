---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 2 릴리스 활동
description: 이 페이지에서는 2017.2 Beta 2 릴리스의 미리보기 환경에서 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 5월 24일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2017년 7월 말에서 8월 초에 제공될 예정입니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0aa8d61e-cf8c-46a7-b093-a0dbc90d37fd
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# 2017.2 Beta 2 릴리스 활동

이 페이지에서는 2017.2 Beta 2 릴리스의 미리보기 환경에서 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 5월 24일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2017년 7월 말에서 8월 초에 제공될 예정입니다.

>[!IMPORTANT]
>
>이 페이지에 설명된 기능은 프로덕션 환경에서 사용하기 전에 변경될 수 있습니다.

2017.2의 모든 변경 사항 목록은 [2017.2 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md)를 참조하십시오.

2017.2 Beta 2 릴리스에는 Workfront 관리자와 기타 사용자를 위한 개선 사항이 포함되어 있습니다.

**관리자용:**

* [API 개선 사항: 이벤트 구독](#api-enhancement-event-subscriptions)

**모든 사용자의 경우:**

* [프로젝트 구독](#subscribe-to-projects)
* [전자 메일에서 항목 구독 취소](#unsubscribe-from-items-from-email)
* [간트 차트에 마일스톤을 표시하는 방법 구성](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [리소스 풀 템플릿](#resource-pools-templates)
* [Workfront 내에서 증명 문서 버전 보기](#view-versions-of-proofed-documents-within-workfront)
* [증명 승인 보고서의 새 요청자 개체](#new-requester-object-in-proof-approval-report)

## API 개선 사항: 이벤트 구독 {#api-enhancement-event-subscriptions}

이제 이벤트 구독이 지원하는 Workfront 개체에서 작업이 발생할 때 원하는 끝점에 응답을 보내도록 Workfront을 구성할 수 있습니다. 즉, 통합은 실시간으로 Workfront API와 상호 작용할 수 있습니다.

자세한 내용은 [이벤트 구독 API](../../../../wf-api/general/event-subs-api.md)를 참조하십시오. 

## 프로젝트 구독 {#subscribe-to-projects}

이제 프로젝트 팀에 속하지 않은 프로젝트에 대한 새 주석을 구독할 수 있습니다. 이번 릴리스 이전에는 문제 및 작업에 대한 의견만 구독할 수 있었습니다.

항목 구독에 대한 자세한 내용은 [Adobe Workfront에서 항목 구독](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)을 참조하세요.

## 이메일에서 항목 구독 취소 {#unsubscribe-from-items-from-email}

구독 이메일 내의 &quot;구독 취소&quot; 링크를 사용하여 항목에서 구독을 취소할 수 있습니다. 이전에는 Workfront 인터페이스에서만 항목 구독을 취소할 수 있었습니다.

구독 이메일 구독 취소에 대한 자세한 내용은 [Adobe Workfront 알림](../../../../workfront-basics/using-notifications/wf-notifications.md)의 &quot;이메일 알림 옵트아웃&quot; 섹션을 참조하십시오. 

## 간트 차트에 마일스톤을 표시하는 방법 구성 {#configure-how-milestones-are-displayed-on-the-gantt-chart}

***수정&#x200B;**: 이 기능은 현재 미리 보기 샌드박스 환경에 없습니다. 이 업데이트는 나중에 2017년 6월 한 달 동안 릴리스될 예정입니다.*

이제 간트 차트에서 마일스톤 정보를 볼 수 있는 두 가지 옵션이 있습니다. 다음 이정표 표시기 중 하나 또는 둘 다를 구성할 수 있습니다.

* 마일스톤 다이아몬드(아이콘)

  이 아이콘은 마일스톤과 연결된 작업 후에 간트 차트에 표시됩니다.

* 마일스톤 라인

  간트 차트의 모든 작업에서 마일스톤과 연결된 작업 뒤에 선이 표시됩니다.

이 변경 이전에는 간트 차트에 &quot;마일스톤&quot;이라는 마일스톤을 표시할 수 있는 옵션이 하나만 있었습니다. 이 옵션을 사용하면 마일스톤 다이아몬드 아이콘과 마일스톤 라인이 모두 활성화됩니다. 이러한 지표는 분리할 수 없습니다. 이제 모든 프로젝트 목록과 보고서를 포함하여 모든 간트 차트에서 두 가지 옵션을 사용할 수 있습니다. 

간트 차트에 정보가 표시되는 방식을 구성하는 방법에 대한 자세한 내용은 [간트 차트에 정보가 표시되는 방식 구성](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)을 참조하십시오.

## 리소스 풀 템플릿 {#resource-pools-templates}

이제 템플릿에 대한 리소스 풀을 지정할 수 있습니다. 이 릴리스 이전에는 리소스 풀을 사용자 및 프로젝트와만 연결할 수 있었습니다.

리소스 풀에 대한 자세한 내용은 [리소스 풀 개요](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)를 참조하십시오.

## Workfront 내에서 증명 문서 버전 보기 {#view-versions-of-proofed-documents-within-workfront}

이제 Workfront 인터페이스 내에서 모든 버전의 증명 문서에서 증명을 볼 수 있습니다. 

이 변경 이전에는 교정된 문서의 최신 버전만 볼 수 있었습니다.

증명 라이선스가 없는 사용자는 다음을 수행할 수 있습니다.

* 이전 버전의 증명 문서에서 증명 열기

증명 라이선스가 있는 사용자는 다음 중 하나를 수행할 수 있습니다.

* 이전 버전의 증명 문서에서 증명 열기
* 증명 문서의 이전 버전에서 증명 세부 정보 보기

자세한 내용은 [문서 버전 관리](../../../../documents/managing-documents/manage-document-versions.md)에서 [문서 버전 관리](../../../../documents/managing-documents/manage-document-versions.md)를 참조하십시오.

## 증명 승인 보고서의 새 요청자 개체 {#new-requester-object-in-proof-approval-report}

이제 증명 승인 보고서를 만들 때 새 요청자 개체가 있습니다. 이 개체를 사용하면 증명 승인을 요청한 사용자에 대한 정보를 보고할 수 있습니다. 

증명 승인 보고서의 새 요청자 개체에는 다른 유형의 개체 보고서에서 기존 사용자 개체와 함께 사용할 수 있는 모든 필드가 포함되어 있습니다.

>[!NOTE]
>
> 이 정보는 이 기능이 각 미리보기 또는 프로덕션 환경에 처음 도입된 시점부터 보고서에서만 사용할 수 있습니다. 이 기능이 도입되기 전의 요청자 오브젝트와 관련된 보고서에 있는 정보는 사용할 수 없습니다.

[사용자 지정 보고서 만들기](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)에 설명된 대로 증명 승인 보고서를 만들 때 요청자 개체에 액세스합니다.

증명 승인 개체 보고서에 대한 자세한 내용은 [Adobe Workfront의 개체 이해](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)의 [Adobe Workfront의 개체 이해](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) 섹션을 참조하십시오.
