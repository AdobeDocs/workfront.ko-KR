---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 도메인의 DMARC 정책으로 인해 인증된 이메일이 수락되지 않는 경우
description: 에서 보낸 이메일이 [!DNL Workfront] 도메인의 DMARC 정책으로 인해 시스템이 수락되지 않으므로 이메일 관리자가 workfront.com의 모든 이메일을 허용하도록 이메일 시스템을 구성하여 문제를 해결할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# 도메인의 DMARC 정책으로 인해 인증되지 않은 전자 메일이 수락되지 않습니다.

## 문제

[테스트] 다음 바운스 백 이메일을 받았습니다.

다음 이유로 인해 &quot;customer domain.com&quot;의 인증되지 않은 전자 메일이 수락되지 않습니다.\
550-5.7.1 도메인의 DMARC 정책. &quot;customer domain.com&quot;의 관리자에게 문의하십시오\
합법적인 우편인 경우 550-5.7.1 도메인 방문\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) DMARC에 대해 알아보기\
550 5.7.1 이니셔티브.

## 솔루션

DMARC는 회사의 이메일 시스템에 구성되며, 이 회사의 일부가 아닙니다 [!DNL Adobe Workfront]. 이 이메일을 받으면 이메일 관리자에게 문의해야 합니다.

이메일 관리자는 noreply@workfront.com 또는 workfront.com의 모든 이메일을 허용/신뢰하도록 이메일 시스템을 구성해야 합니다.

DMARC에 대한 자세한 내용은 [https://support.google.com/mail/answer/2451690](https://support.google.com/mail/answer/2451690)
