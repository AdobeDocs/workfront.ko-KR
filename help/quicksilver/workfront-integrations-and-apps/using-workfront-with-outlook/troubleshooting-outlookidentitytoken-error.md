---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: '문제 해결: Outlook용 Workfront을 사용할 때 outlookIdentityToken 오류 발생'
description: Outlook용 Workfront을 사용할 때 outlookIdentityToken 오류가 발생하는 경우 조직에 대해 Microsoft 365 레거시 토큰을 활성화해야 합니다.
author: Becky
feature: Workfront Integrations and Apps
source-git-commit: 571ed00f44322d73183323c4d4154284cd028301
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# 문제 해결: Outlook용 Workfront을 사용할 때 outlookIdentityToken 오류 발생

Outlook용 Workfront을 사용하는 경우 다음 오류가 표시될 수 있습니다.

```
Unexpected error
Unable to get the outlookIdentityToken
```

이 오류를 해결하려면 조직에 대해 Microsoft 365 레거시 토큰을 활성화해야 합니다. 이 작업은 Microsoft 365에서 수행해야 하므로 Workfront에서 조직에 대해 이러한 토큰을 활성화할 수 없습니다.

Microsoft 365 레거시 토큰을 사용하는 방법에 대한 지침은 Microsoft 설명서의 [레거시 Exchange Online 토큰 켜기 또는 끄기](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off)를 참조하십시오.

레거시 토큰에 대한 자세한 내용은 [Exchange Online 레거시 토큰을 다시 켤 수 있습니까?Microsoft 설명서의 ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on).
