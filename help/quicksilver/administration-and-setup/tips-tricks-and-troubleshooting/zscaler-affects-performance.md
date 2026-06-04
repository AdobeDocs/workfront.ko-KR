---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ZScaler 설정으로 인해 성능이 저하될 수 있음
description: 사용자 생성 후 사용자를 편집하고 "SAML 2.0 인증만 허용"을 활성화하여 해당 사용자 및 암호를 SAML 시스템에서 제어할 수 있습니다. 이 옵션을 활성화하면 사용자는 SAML을 통해서만 로그인할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 2752a9e2-44fe-49b5-a7ab-4021d91ed37b
TQID: https://experienceleague.adobe.com/-3-p8fzXIiV-gnjIjhRzBmLfspAEEVAuD2lpmcsVjLA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 107
ht-degree: 44%

---

# Workfront: ZScaler 설정으로 인해 성능이 저하될 수 있음

>[!NOTE]
>
>이는 ZScaler의 문제이므로 Workfront에서는 해결되지 않습니다.

ZScaler 웹 서비스는 기본적으로 `http/1.1`을 사용하는데, 이로 인해 Workfront의 성능이 저하될 수 있습니다.

이 문제를 확인하고 해결하려면 `http/2`을(를) 사용하도록 ZScaler 소프트웨어를 구성하십시오. Workfront에서는 이를 구성할 수 없습니다.

`http/2`에 대한 정보는 ZScaler 설명서에서 확인할 수 있습니다.
