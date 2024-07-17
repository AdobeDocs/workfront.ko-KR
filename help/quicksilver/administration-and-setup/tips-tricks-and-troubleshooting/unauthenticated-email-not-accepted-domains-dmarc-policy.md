---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 도메인의 DMARC 정책으로 인해 인증된 이메일이 수락되지 않은 경우
description: 도메인의 DMARC 정책으로 인해  [!DNL Workfront] 시스템에서 보낸 전자 메일이 허용되지 않는 경우 전자 메일 관리자가 workfront.com에서 보낸 모든 전자 메일을 허용하도록 전자 메일 시스템을 구성하여 문제를 해결할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# 도메인의 DMARC 정책으로 인해 인증되지 않은 이메일이 승인되지 않음

## 문제

[테스트] 다음 바운스 백 이메일을 받았습니다.

550-5.7.1 &quot;customer domain.com&quot; 의 인증되지 않은 이메일은 다음 이유로 허용되지 않습니다.\
550-5.7.1 도메인의 DMARC 정책. &quot;customer domain.com&quot; 관리자에게 문의하십시오.\
550-5.7.1 도메인(합법적인 메일인 경우). 다음을 방문하십시오.\
DMARC에 대해 알아보려면 550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690)\
550 5.7.1 이니셔티브.

## 솔루션

DMARC는 회사 전자 메일 시스템에 구성되어 있으며 [!DNL Adobe Workfront]의 일부가 아닙니다. 이 이메일을 수신하면 이메일 관리자에게 문의해야 합니다.

이메일 관리자는 noreply@workfront.com의 이메일 또는 모든 workfront.com의 이메일을 허용/신뢰하도록 이메일 시스템을 구성해야 합니다.

DMARC에 대한 자세한 내용은 [https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690)을 참조하세요.
