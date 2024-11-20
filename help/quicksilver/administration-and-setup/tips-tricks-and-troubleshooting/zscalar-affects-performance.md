---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ZScalar 설정으로 인해 성능이 저하될 수 있음
description: 사용자 생성 후 사용자를 편집하고 "SAML 2.0 인증만 허용"을 활성화하여 해당 사용자 및 암호를 SAML 시스템에서 제어할 수 있습니다. 이 옵션을 활성화하면 사용자는 SAML을 통해서만 로그인할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: 806a4c4835e47da4fbbdb28ec0c35c990f70239e
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Workfront: ZScalar 설정으로 인해 성능이 저하될 수 있습니다.

>[!NOTE]
>
>이 문제는 ZScalar의 문제이며 Workfront에서 수정되지 않습니다.

ZScalar의 웹 서비스는 기본적으로 `http/1.1`을(를) 사용하므로 Workfront에서 성능이 저하될 수 있습니다.

이 문제를 확인하고 해결하려면 `http/2`을(를) 사용하도록 ZScalar 소프트웨어를 구성하십시오. Workfront에서는 구성할 수 없습니다.

ZScalar 설명서에서 `http/2`에 대한 정보를 찾을 수 있습니다.
