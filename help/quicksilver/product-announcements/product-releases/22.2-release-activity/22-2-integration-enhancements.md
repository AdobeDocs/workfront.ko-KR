---
title: 22.2 통합 개선 사항
description: 22.2 통합 개선 사항
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# 22.2 통합 개선 사항

이 페이지에서는 미리 보기 환경에 대한 22.2 릴리스에서 향상된 모든 통합 기능을 설명합니다. 이러한 개선 사항은 프로덕션 환경에서 사용할 수 있습니다

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022년 4월 4일이 있는 주.

22.2 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [22.2 릴리스 개요](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## 이제 Anaplan 통합을 통해 Adobe Workfront 사용 가능

Workfront 프로젝트의 재무 측면에 대한 보다 나은 유연성과 통찰력을 제공하기 위해 이제 Workfront을 Anaplan 계정과 통합할 수 있습니다. Workfront 개체를 Anaplan 개체에 연결하면 두 계정 간에 정보를 자동으로 업데이트하여 두 계정의 정보가 최신 정보와 동일하도록 할 수 있습니다. Workfront의 작업에 따라 Anaplan에서 자동화된 프로세스를 트리거하거나 그 반대로 실행할 수도 있습니다.

예를 들어 Anaplan에서 캠페인을 만든 다음 캠페인에 연결된 Workfront 프로젝트 또는 프로그램을 만들 수 있습니다. Workfront에서 추적한 모든 비용을 다시 Anaplan에 업로드하여 캠페인 성과를 검토할 수 있습니다.

Workfront을 사용하여 Anaplan 통합을 수행할 수 있는 기타 워크플로우에는 다음이 포함됩니다.

* 새 Workfront 프로젝트에서 Anaplan 예산 요청 생성
* 새 Anaplan 목록 항목에서 Workfront 프로젝트 만들기
* Workfront 프로젝트에서 Anaplan 공급자 요청을 시작하는 중

자세한 내용은 [Adobe Workfront 및 안팔란](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

## Workfront for Experience Manager 향상된 커넥터 업데이트

이제 Workfront for Experience Manager enhanced connector에 다음 업데이트가 포함됩니다.

* 이제 여러 프로젝트에 연결된 폴더 구성이 있더라도 Adobe Workfront과 Adobe Experience Manager Assets 사이에 연결된 폴더를 만들 수 있습니다.
* 이벤트 구독 페이지 매김에 대한 지원이 추가되었습니다
* AEM 6.4.x에 대한 지원이 추가되었습니다.
* 프록시 환경에 대한 지원이 추가되었습니다
* 파트너 및 고객 피드백을 기반으로 몇 가지 버그 수정

자세한 내용은 [Workfront for Experience Manager 고급 커넥터 개요](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md).

>[!NOTE]
>
>이 커넥터를 배포하고 구성하려면 인증된 파트너가 필요합니다. 자세한 내용은 [Experience Manager Enhanced Connector용 Workfront 설치](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install.html?lang=en#) 추가 정보.

## 이제 Adobe Creative Cloud 통합에서 OAuth2 사용

보안을 강화하고 통합 전반에서 더 일관된 경험을 제공하기 위해 사용자를 인증하는 업계 표준 방법인 OAuth2 인증을 사용하도록 Adobe Creative Cloud 통합을 업데이트했습니다. 이제 사용자가 로그인하면 통합에 액세스할 수 있는 특정 작업 및 영역을 보고 액세스할 수 있습니다. 이후 자주 로그인할 필요가 없습니다.

자세한 내용은 [Illustrator 및 InDesign용 Workfront 확장 사용](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md).

## 사용자 지정 OAuth2 또는 JWT 통합에 대한 클라이언트 암호 세부 사항을 참조하십시오

사용자 지정 OAuth2 및 JWT 통합 사용에 대한 투명성을 제공하기 위해 Adobe에서는 통합에 사용하는 클라이언트 비밀의 세부 사항을 볼 수 있도록 했습니다. 이제 클라이언트 암호 생성 및 마지막으로 사용한 날짜를 확인할 수 있습니다. 클라이언트 암호와 관련된 고유한 메모를 추가하고 볼 수도 있습니다.

이전에는 이러한 세부 사항을 사용할 수 없었습니다.

OAuth2 또는 JWT 사용자 지정 통합의 클라이언트 비밀에 대한 자세한 내용은 를 참조하십시오 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## 사용자 지정 OAuth2 애플리케이션 목록에서 인증 유형을 참조하십시오

이제 조직의 사용자 지정 OAuth2 응용 프로그램 목록을 볼 때 각 응용 프로그램이 사용자 인증을 사용하는지 서버 인증을 사용하는지 확인할 수 있습니다.

이전에는 각 애플리케이션의 편집 옵션으로 이동해야만 이 정보를 볼 수 있었습니다.

자세한 내용은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## 사용자 지정 OAuth2 통합에서 새로 고침 토큰에 대한 만료를 설정합니다

사용자 지정 OAuth2 통합에 대한 액세스 및 보안을 더 잘 제어하기 위해 이제 새로 고침 토큰의 수명을 사용자 지정할 수 있습니다. 사용자의 새로 고침 토큰이 만료되면 통합에 다시 로그인해야 합니다.

자세한 내용은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## 서버 간 앱에 사용자 지정 OAuth2 통합에서 공개 및 개인 키 사용

이제 사용자 지정 통합에서 서버 간 OAuth2 애플리케이션을 설정할 수 있습니다. 공개 및 개인 키를 설정하여 Workfront에서 로그인 자격 증명을 사용하지 않고 다른 애플리케이션과 통신할 수 있도록 할 수 있습니다.

이전에는 사용자 지정 OAuth2 애플리케이션의 모든 인증이 사용자의 로그인 자격 증명을 사용했습니다.

자세한 내용은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## 이제 Google G Suite 통합에서 OAuth2를 사용합니다

보안을 강화하고 통합 전반에서 더 일관된 경험을 제공하기 위해 사용자를 인증하는 업계 표준 방법인 OAuth2 인증을 사용하도록 Google G Suite 통합을 업데이트했습니다. 이제 사용자가 로그인하면 통합에 액세스할 수 있는 특정 작업 및 영역을 보고 액세스할 수 있습니다. 이후 자주 로그인할 필요가 없습니다.

자세한 내용은 [G Suite용 Adobe Workfront 로그인 및 체크아웃](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md).
