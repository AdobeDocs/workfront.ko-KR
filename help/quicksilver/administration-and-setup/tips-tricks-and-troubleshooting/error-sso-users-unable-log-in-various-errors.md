---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '오류: 여러 가지 오류로 인해 SSO 사용자가  [!DNL Adobe Workfront] 에 로그인할 수 없습니다.'
description: Federated SSO(Single Sign-On)에 대한 로그인 오류, 사용자 이름/암호 조합 또는  [!DNL Workfront], the problem might be that your [!DNL Workfront] 인스턴스에 대한 액세스가 SSO를 사용하므로 잘못된 URL을 사용하여 로그인하려고 합니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
TQID: https://experienceleague.adobe.com/8L78zoOjC2KgtVKTorhvWDd8MvaficRL2pZKOfrlGSs
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 166
ht-degree: 4%

---

# 오류: 여러 가지 오류로 인해 SSO 사용자가 [!DNL Adobe Workfront]에 로그인할 수 없습니다.

## 문제

[!DNL Workfront]에 로그인할 수 없으며 다음 오류 중 하나를 받았습니다.

* 죄송합니다. 이 로그인 화면에서는 [!DNL Workfront]에 액세스할 수 없습니다. [!DNL Workfront]이(가) SAML 2.0을 사용하여 Federated SSO(Single Sign-On)에 대해 설정되어 있습니다. [!DNL Workfront] 관리자에게 문의하십시오.
* 해당 사용자 이름/암호 조합이 정확하지 않습니다. Caps Lock이 켜져 있지 않은지 확인하고 다시 시도하십시오.
* [!DNL Workfront]에 대한 액세스 권한이 없습니다. 사용자 이름과 암호를 얻으려면 [!DNL Workfront] 관리자에게 문의하십시오.

## 솔루션

[!DNL Workfront] 인스턴스가 SSO를 사용하므로 잘못된 URL을 통해 로그인하려고 합니다. &quot;.com&quot; 다음에 아무 것도 없이 올바른 URL을 사용하여 로그인하는지 확인하십시오.

>[!TIP]
>
>잘못된 URL이 있는 기존 책갈피를 제거합니다.
