---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Adobe Workfront 사용자 자격 증명과  [!DNL SAML] 사용자 자격 증명 비교
description: 사용자 생성 후 사용자를 편집하고 "SAML 2.0 인증만 허용"을 활성화하여 해당 사용자 및 암호를 SAML 시스템에서 제어할 수 있습니다. 이 옵션을 활성화하면 사용자는 SAML을 통해서만 로그인할 수 있습니다.  [!DNL Workfront] URL로 이동하면 SAML 시스템으로 자동으로 리디렉션되고 SAML 사용자 이름과 암호를 입력하라는 메시지가 표시됩니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Adobe Workfront 사용자 자격 증명과 SAML 사용자 자격 증명 비교

이 문서는 특히 [!DNL Adobe Workfront] 및 SAML에 중점을 두고 있으며 다른 SSO 인증 방법은 다루지 않습니다.

[!DNL Workfront]은(는) 각 사용자의 전자 메일 주소를 [!DNL Workfront] 사용자 이름과 함께 [!DNL Workfront] 암호로 데이터베이스에 저장합니다. 이러한 자격 증명은 미리 보기 및 사용자 지정 새로 고침 샌드박스에서 복제됩니다.

사용자를 만드는 동안 [!DNL Workfront]에서 SAML 2.0이 구성된 것을 검색하면 기본적으로 사용자에 대해 &quot;SAML 2.0 인증만 허용&quot;으로 설정됩니다. &quot;이 사용자에게 초대 이메일 보내기&quot; 상자를 사용하는 경우 [!DNL Workfront]은(는) &quot;SAML 2.0 인증만 허용&quot;을 사용하지 않도록 설정하고 이 옵션을 숨깁니다. &quot;이 사용자에게 초대 이메일 보내기&quot;를 사용하면 사용자가 SAML [!DNL Workfront]이(가) 아닌 사용자가 됩니다.

사용자를 만든 후 사용자를 편집하고 **[!UICONTROL SAML 2.0 인증만 허용]**&#x200B;을 사용하도록 설정하여 해당 사용자와 암호를 SAML 시스템에서 제어할 수 있습니다.

이 작업을 완료하면 사용자는 SAML을 통해서만 로그인할 수 있습니다. [!DNL Workfront] URL로 이동하면 SAML 시스템으로 자동으로 리디렉션되고 SAML 사용자 이름과 암호를 입력하라는 메시지가 표시됩니다.

SAML 자격 증명은 Workfront이 아닌 Microsoft의 ADFS와 같은 외부 SAML 시스템에 저장됩니다.
