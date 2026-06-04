---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 도메인의 DMARC 정책으로 인해 인증되지 않은 이메일이 허용되지 않음
description: 도메인의 DMARC 정책으로 인해  [!DNL Workfront] 시스템에서 보낸 전자 메일이 허용되지 않는 경우 전자 메일 관리자가 workfront.com에서 보낸 모든 전자 메일을 허용하도록 전자 메일 시스템을 구성하여 문제를 해결할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
TQID: https://experienceleague.adobe.com/f44Wkid-gwfXgHKmSKa6oevhN5jA6720JTlOcH8kJKY
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
source-wordcount: 177
ht-degree: 1%

---

# 도메인의 DMARC 정책으로 인해 인증되지 않은 이메일이 허용되지 않음

## 문제

[테스트] 다음 바운스 백 이메일을 받았습니다.

550-5.7.1 &quot;customer domain.com&quot; 의 인증되지 않은 이메일은 다음 이유로 허용되지 않습니다.\
550-5.7.1 도메인의 DMARC 정책 &quot;customer domain.com&quot; 관리자에게 문의하십시오.\
550-5.7.1 도메인(합법적인 메일인 경우). 다음을 방문하십시오.\
DMARC에 대해 알아보려면 550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690)\
550 5.7.1 이니셔티브.

## 솔루션

DMARC은 회사 전자 메일 시스템에 구성되어 있으며 [!DNL Adobe Workfront]의 일부가 아닙니다. 이 이메일을 수신하면 이메일 관리자에게 문의해야 합니다.

이메일 관리자는 noreply@workfront.com의 이메일 또는 모든 workfront.com의 이메일을 허용/신뢰하도록 이메일 시스템을 구성해야 합니다.

DMARC에 대한 자세한 내용은 [https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690)을(를) 참조하십시오.
