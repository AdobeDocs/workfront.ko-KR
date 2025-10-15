---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: ' [!DNL Workfront Proof]의 단일 사인온'
description: SSO(Single Sign-On)를 통해 사용자는 조직의 기존 사용자 이름과 암호를 사용하여  [!DNL Workfront Proof] 에 로그인할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# [!DNL Workfront Proof]에서 SSO(Single Sign-On)

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

이 기능을 사용하려면 [!UICONTROL Enterprise] [!DNL Workfront] 플랜이 필요합니다. 사용 가능한 다양한 플랜에 대한 자세한 내용은 [Workfront 플랜](https://business.adobe.com/kr/products/workfront/pricing.html)을 참조하십시오.

SSO(Single Sign-On)를 통해 사용자는 조직의 기존 사용자 이름과 암호를 사용하여 [!DNL Workfront Proof]에 로그인할 수 있습니다.

이 기능을 제공하기 위해 ID 공급자와 웹 서비스 간에 데이터를 승인하고 인증을 교환할 수 있는 XML 기반 프로토콜인 [!DNL Security Assertion Markup Language]&#x200B;(SAML) 2.0을 사용합니다.

즉, [!DNL Workfront Proof]의 로그인 페이지가 아니라 사용자의 로그인 시스템에 대해 인증합니다.

SAML을 사용하려면 [!DNL Workfront] 증명 계정에 사용자 지정 하위 도메인 또는 도메인이 설정되어 있어야 합니다.

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* [사이트 브랜드 [!DNL Workfront Proof] 사이트 - 고급](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md)에서 완전히 맞춤화된 도메인에 대한 자세한 내용을 읽을 수 있습니다.

계정에서 SSO 설정에 대한 자세한 내용은 [사용자를 위한 SSO 구성 [!DNL Workfront Proof] 을 참조하십시오](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md).
