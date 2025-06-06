---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: ' [!DNL Adobe Workfront]  및 SAML 2.0에서 사용할 Office용 Outlook 사용'
description: ' [!DNL Adobe Workfront] 시스템이 SAML 2.0과 통합된 경우 사용자가 SAML 2.0 자격 증명을 사용하여 인증할 수 있도록 Office 추가 기능에 대해 SAML 2.0 인증을 사용하도록 설정해야 합니다.'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 72ffceb3-50f0-486e-92b5-0bea4c9a99c8
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# [!DNL Adobe Workfront] 및 SAML 2.0에서 사용할 [!DNL Outlook for Office] 사용

>[!IMPORTANT]
>
>[Microsoft에서 기존 Exchange 온라인 토큰에 대한 지원을 사용하지 않도록 설정하는 중입니다](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens). 이 토큰은 현재 인증을 위해 Workfront Outlook 추가 기능에서 사용됩니다. Microsoft의 이러한 변경 사항은 이미 고객에게 영향을 주기 시작했으며 2025년 10월까지 단계적으로 계속 적용될 예정입니다.
>
>* **Microsoft에서 이 토큰을 완전히 비활성화하면 Microsoft Outlook용 Workfront 통합이 더 이상 작동하지 않습니다.**
>
>이 변경의 일부로 Microsoft은 토큰이 다시 활성화되는 방식을 변경하기로 결정했습니다. **2025년 6월 30일** 이후에는 관리자가 더 이상 토큰을 직접 다시 활성화할 수 없습니다. Microsoft 지원에서만 예외를 허용할 수 있습니다. **2025년 10월 1일부터 모든 테넌트에 대해 레거시 토큰이 꺼집니다. 예외가 부여되지 않습니다.**

[!DNL Adobe Workfront] 시스템이 SAML 2.0과 통합된 경우 사용자가 SAML 2.0 자격 증명을 사용하여 인증할 수 있도록 [!DNL Office] 추가 기능에 대해 SAML 2.0 인증을 사용하도록 설정해야 합니다.

SAML로 [!DNL Workfront]에 로그인할 때 문제가 발생하는 경우 [!DNL Workfront] 관리자에게 문의하여 SAML이 올바르게 구성되었는지 확인하십시오.

SAML 2.0 솔루션을 사용하여 Office 추가 기능을 인증할 수 있도록 하는 방법에 대한 자세한 내용은 [SAML 2.0으로 Adobe Workfront 구성](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md) 문서의 섹션을 참조하십시오.
