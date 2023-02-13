---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '로그인 오류: 다음 필드가 잘못되었습니다. emailAddr은 null일 수 없습니다.'
description: 로그인할 때 [!DNL Adobe Workfront] 내 도메인의 URL을 입력하면 SAML 로그인 포털로 리디렉션된 다음 다시 로 리디렉션됩니다. [!DNL Workfront] emailAddr 필드가 null일 수 없다는 오류가 발생했습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 2%

---

# 로그인 오류: 다음 필드가 잘못되었습니다. emailAddr은 null일 수 없습니다.

## 문제

로그인할 때 [!DNL Adobe Workfront] 내 URL(https://customerdomain.my.workfront.com)을 사용하면 SAML 로그인 포털로 리디렉션된 다음 다시 로 리디렉션됩니다. [!DNL Workfront] 다음 오류가 발생한 경우:

“다시 시도해 보겠습니다. 다음 필드가 잘못되었습니다. emailAddr은 null일 수 없습니다.&quot;

## 원인

이 오류는 SAML 2.0 구성의 사용자 특성 매핑 영역에서 잘못된 항목으로 인해 발생합니다. SAML 2.0용 사용자 특성 매핑에 대한 자세한 내용은 [SAML 2.0으로 Adobe Workfront 구성](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## 솔루션

전자 메일 주소에 대한 속성 매핑을 업데이트하고 를 클릭합니다. **[!UICONTROL 저장]**.
