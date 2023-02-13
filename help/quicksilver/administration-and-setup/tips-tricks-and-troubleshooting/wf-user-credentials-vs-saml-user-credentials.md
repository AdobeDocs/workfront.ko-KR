---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Adobe Workfront 사용자 자격 증명과 [!DNL SAML] 사용자 자격 증명
description: 사용자 생성 후 사용자를 편집하고 "SAML 2.0 인증만 허용"을 활성화하여 사용자 및 암호가 SAML 시스템에 의해 제어되도록 할 수 있습니다. 이 옵션을 활성화하면 SAML을 통해서만 로그인할 수 있습니다. 로 이동할 때 [!DNL Workfront] URL, SAML 시스템으로 자동 리디렉션되며 SAML 사용자 이름과 암호를 묻는 메시지가 표시됩니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Adobe Workfront 사용자 자격 증명과 SAML 사용자 자격 증명 비교

이 문서는 특히 [!DNL Adobe Workfront] 및 SAML과 는 다른 SSO 인증 방법을 포함하지 않습니다.

데이터베이스에서 [!DNL Workfront] 모든 사용자의 이메일 주소를 [!DNL Workfront] 사용자 이름과 함께 [!DNL Workfront] 암호. 이러한 자격 증명은 미리 보기 및 사용자 지정 새로 고침 샌드박스에 복제됩니다.

사용자를 생성하는 동안, [!DNL Workfront] saml 2.0이 구성되어 있음을 감지하면 기본값은 사용자에 대해 &quot;SAML 2.0 인증만 허용&quot;으로 설정됩니다. &quot;이 사람에게 초대 이메일 보내기&quot; 상자가 활성화된 경우, [!DNL Workfront] &quot;SAML 2.0 인증만 허용&quot;을 비활성화하고 이 옵션을 숨깁니다. &quot;이 사람에게 초대 이메일 보내기&quot;가 활성화되면 사용자는 비 SAML이 됩니다 [!DNL Workfront] 사용자.

사용자가 생성되면 사용자를 편집하고 활성화할 수 있습니다 **[!UICONTROL SAML 2.0 인증만 허용]** SAML 시스템에서 사용자 및 암호를 제어하도록 했습니다.

이 작업을 수행하면 사용자는 SAML을 통해서만 로그인할 수 있습니다. 로 이동할 때 [!DNL Workfront] URL, SAML 시스템으로 자동 리디렉션되며 SAML 사용자 이름과 암호를 묻는 메시지가 표시됩니다.

SAML 자격 증명은 Microsoft의 ADFS와 같은 외부 SAML 시스템에 저장되며 Workfront에는 저장되지 않습니다.
