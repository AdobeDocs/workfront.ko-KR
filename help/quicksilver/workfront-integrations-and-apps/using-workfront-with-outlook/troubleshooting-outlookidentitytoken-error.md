---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: '문제 해결: Outlook용 Workfront을 사용할 때 outlookIdentityToken 오류 발생'
description: Outlook용 Workfront을 사용할 때 outlookIdentityToken 오류가 발생하는 경우 조직에 대해 Microsoft 365 레거시 토큰을 활성화해야 합니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 31%

---

# 문제 해결: Outlook용 Workfront을 사용할 때 outlookIdentityToken 오류 발생

>[!IMPORTANT]
>
>[Microsoft에서 기존 Exchange 온라인 토큰에 대한 지원을 사용하지 않도록 설정하는 중입니다](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens). 이 토큰은 현재 인증을 위해 Workfront Outlook 추가 기능에서 사용됩니다. Microsoft의 이러한 변경 사항은 이미 고객에게 영향을 주기 시작했으며 2025년 10월까지 단계적으로 계속 적용될 예정입니다.
>
>* **Microsoft에서 이 토큰을 완전히 비활성화하면 Microsoft Outlook용 Workfront 통합이 더 이상 작동하지 않습니다.**
>
>이 변경의 일부로 Microsoft은 토큰이 다시 활성화되는 방식을 변경하기로 결정했습니다. **2025년 6월 30일** 이후에는 관리자가 더 이상 토큰을 직접 다시 활성화할 수 없습니다. Microsoft 지원에서만 예외를 허용할 수 있습니다. **2025년 10월 1일부터 모든 테넌트에 대해 레거시 토큰이 꺼집니다. 예외가 부여되지 않습니다.**


Outlook용 Workfront을 사용하는 경우 다음 오류가 표시될 수 있습니다.

```
Unexpected error
Unable to get the outlookIdentityToken
```

이 오류를 해결하려면 조직에 대해 Microsoft 365 레거시 토큰을 활성화해야 합니다. 이 작업은 Microsoft 365에서 수행되어야 하므로 Workfront는 조직에 대해 이들 토큰을 활성화할 수 없습니다.

Microsoft 365 레거시 토큰을 활성화하는 방법에 대한 자세한 내용은 Microsoft 설명서의 [레거시 Exchange Online 토큰 켜기 또는 끄기](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off)를 참조하십시오.

레거시 토큰에 대한 자세한 내용은 Microsoft 설명서의 [Exchange Online 레거시 토큰을 다시 켤 수 있나요?](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on)를 참조하십시오.
