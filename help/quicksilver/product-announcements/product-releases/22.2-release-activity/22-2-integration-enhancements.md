---
title: 22.2 통합 개선 사항
description: 22.2 통합 개선 사항
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# 22.2 통합 개선 사항

이 페이지에서는 미리보기 환경에 대한 22.2 릴리스의 모든 통합 개선 사항에 대해 설명합니다. 이러한 개선 사항은 프로덕션 환경에서 사용할 수 있습니다

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022년 4월 4일이 있는 주

22.2 릴리스에서 사용할 수 있는 모든 변경 사항 목록을 보려면 [22.2 릴리스 개요](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md)를 참조하십시오.

## 이제 Adobe Workfront과 Anaplan 통합을 사용할 수 있습니다.

이제 Workfront을 Anaplan 계정과 통합하여 Workfront 프로젝트의 재무 측면에서 보다 나은 유연성과 insight을 제공할 수 있습니다. Workfront 오브젝트를 Anaplan 오브젝트에 연결하면 두 계정 간의 정보를 자동으로 업데이트하여 두 계정의 정보가 모두 최신 상태이고 동일한지 확인할 수 있습니다. Workfront의 작업을 기반으로 Anaplan에서 자동화된 프로세스를 트리거할 수도 있습니다(또는 그 반대의 경우도 가능).

예를 들어 Anaplan에서 캠페인을 만든 다음 캠페인에 연결된 Workfront 프로젝트 또는 프로그램을 만들 수 있습니다. 그런 다음 Workfront에서 추적한 모든 비용을 Anaplan에 다시 업로드하여 캠페인 성과를 검토할 수 있습니다.

Workfront을 Anaplan에 통합하는 데 사용할 수 있는 기타 워크플로우는 다음과 같습니다.

* 새 Workfront 프로젝트에서 Anaplan 예산 요청 생성
* 새 Anaplan 목록 항목에서 Workfront 프로젝트 만들기
* Workfront 프로젝트에서 Anaplan 공급자 요청 시작

자세한 내용은 [Anaplan이 있는 Adobe Workfront](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md)을 참조하세요.

## Workfront for Experience Manager 강화 커넥터 업데이트

이제 Workfront for Experience Manager 강화 커넥터에 다음 업데이트가 포함됩니다.

* 이제 여러 개의 프로젝트로 연결된 폴더 구성이 있는 경우에도 Adobe Workfront 및 Adobe Experience Manager Assets as a Cloud Service 간에 연결된 폴더를 만들 수 있습니다.
* 이벤트 구독 페이지 매김에 대한 지원을 추가했습니다.
* AEM 6.4.x에 대한 지원이 추가되었습니다
* 프록시 환경에 대한 지원이 추가되었습니다
* 파트너 및 고객 피드백을 기반으로 한 몇 가지 버그 수정

자세한 내용은 [Workfront for Experience Manager 강화 커넥터 개요](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md)를 참조하십시오.

>[!NOTE]
>
>이 커넥터를 배포하고 구성하려면 인증된 파트너가 필요합니다. 자세한 내용은 [Experience Manager 강화 커넥터용 Workfront 설치](https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install)를 참조하십시오.

## 이제 Adobe Creative Cloud 통합에서 OAuth2를 사용합니다

보안을 강화하고 통합 전반에서 보다 일관된 환경을 제공하기 위해 사용자를 인증하는 업계 표준 방법인 OAuth2 인증을 사용하도록 Adobe Creative Cloud 통합을 업데이트했습니다. 이제 사용자가 로그인하면 통합에서 액세스할 수 있는 특정 작업과 영역을 볼 수 있으며 액세스를 허용할 수 있습니다. 이 후에는 를 자주 로그인할 필요가 없습니다.

자세한 내용은 [Illustrator 및 InDesign용 Workfront 확장 사용](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md)을 참조하십시오.

## 사용자 정의 OAuth2 또는 JWT 통합을 위한 클라이언트 암호 세부 사항 을 참조하십시오

사용자 정의 OAuth2 및 JWT 통합 사용에 대한 투명성을 제공하기 위해 통합 사용 중인 클라이언트 암호에 대한 세부 사항을 볼 수 있도록 했습니다. 이제 클라이언트 암호가 만들어지고 마지막으로 사용된 날짜를 볼 수 있습니다. 클라이언트 암호에 대한 자신의 메모를 추가하고 볼 수도 있습니다.

이전에는 이러한 세부 정보를 사용할 수 없었습니다.

OAuth2 또는 JWT 사용자 지정 통합의 클라이언트 암호에 대한 자세한 내용은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../../../administration-and-setup/configure-integrations/create-oauth-application.md)를 참조하십시오.

## 사용자 지정 OAuth2 애플리케이션 목록에서 인증 유형 을 참조하십시오

이제 조직의 사용자 지정 OAuth2 애플리케이션 목록을 보면 각 애플리케이션이 사용자 인증을 사용하는지 아니면 서버 인증을 사용하는지 확인할 수 있습니다.

이전에는 각 애플리케이션의 편집 옵션으로 이동해야만 이 정보를 볼 수 있었습니다.

자세한 내용은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../../../administration-and-setup/configure-integrations/create-oauth-application.md)를 참조하십시오.

## 사용자 지정 OAuth2 통합에서 새로 고침 토큰에 대한 만료 설정

이제 사용자 지정 OAuth2 통합에 대한 액세스 및 보안을 더 잘 제어하기 위해 새로 고침 토큰의 수명을 사용자 지정할 수 있습니다. 사용자의 새로 고침 토큰이 만료되면 다시 통합에 로그인해야 합니다.

자세한 내용은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../../../administration-and-setup/configure-integrations/create-oauth-application.md)를 참조하십시오.

## 서버 간 앱에 대한 사용자 지정 OAuth2 통합에서 공개 및 개인 키 사용

이제 사용자 정의 통합에서 서버 간 OAuth2 애플리케이션을 설정할 수 있습니다. 공개 및 개인 키를 설정하면 Workfront이 로그인 자격 증명을 사용하지 않고 다른 애플리케이션과 통신할 수 있습니다.

이전에는 사용자 정의 OAuth2 애플리케이션의 모든 인증이 사용자의 로그인 자격 증명을 사용했습니다.

자세한 내용은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../../../administration-and-setup/configure-integrations/create-oauth-application.md)를 참조하십시오.

## Google Google Workspace 통합에서 이제 OAuth2를 사용합니다

보안을 강화하고 통합 전반에서 보다 일관된 환경을 제공하기 위해 사용자를 인증하는 업계 표준 방법인 OAuth2 인증을 사용하도록 Google Google Workspace 통합을 업데이트했습니다. 이제 사용자가 로그인하면 통합에서 액세스할 수 있는 특정 작업과 영역을 볼 수 있으며 액세스를 허용할 수 있습니다. 이 후에는 를 자주 로그인할 필요가 없습니다.

자세한 내용은 [Google Workspace용 Adobe Workfront 로그인 및 로그아웃](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md)을 참조하세요.
