---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Adobe Workfront의 Single Sign-On 개요
description: Workfront은 Workfront을 기존 회사 SSO 솔루션과 쉽게 통합하는 중앙 집중식 관리 SSO(Single Sign-On) 구성을 제공합니다. 이 구성은 설정 및 관리가 쉬우며 OnDemand 및 OnPremise 엔터프라이즈 고객 모두 사용할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87f1b6c0-6b74-4eac-87cd-899b1c74af25
source-git-commit: 4e3cafafb121371249fb73f2f001477bdbad2d77
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# Adobe Workfront의 Single Sign-On 개요

<!--Audited: 12/2023-->

{{important-admin-console-onboard}}


Workfront은 Workfront을 기존 회사 SSO 솔루션과 통합하는 중앙 관리 SSO(Single Sign-On) 구성을 제공합니다. 이 구성은 OnDemand 및 OnPremise 엔터프라이즈 고객 모두 사용할 수 있습니다.

Workfront에서 SSO 기능을 사용하려면 조직에서 SSO 애플리케이션을 설정해야 합니다. 그런 다음 SSO 솔루션과 통신할 수 있도록 Workfront을 구성할 수 있습니다.

Federated Solutions는 사용자가 중앙 집중식 로그인 포털에 사용자 이름과 암호를 입력하여 모든 애플리케이션에 로그인할 수 있도록 합니다.

![](assets/overview-sso-wf-fed-only.png)


## 방화벽 구성

SSO 솔루션을 사용하는 경우 Workfront은 지정된 포트에서 서버에 연결을 시작합니다.

방화벽 메일 서버가 특정 공급업체에 대한 액세스만 허용하도록 구성된 경우 방화벽 IP에 특정 Workfront 허용 목록에 추가하다 IP 주소를 추가해야 합니다. 허용 목록에 추가하다 자세한 내용은 [방화벽 구성](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)을 참조하십시오.

## 단일 사인온 구성

Workfront은 다음 SSO 솔루션과 통합됩니다.

* SAML 2.0을 지원하는 Federated 솔루션

  SAML 2.0과 Workfront 통합에 대한 자세한 내용은 [SAML 2.0과 Adobe Workfront 구성](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)을 참조하십시오.

* ADFS를 사용하여 SAML 2.0을 지원하는 페더레이션 솔루션

  ADFS를 사용하여 Workfront을 SAML 2.0과 통합하는 방법에 대한 자세한 내용은 [ADFS를 사용하여 Adobe Workfront을 SAML 2.0과 구성](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)을 참조하십시오.
