---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '로그인 오류: 다음 필드가 잘못되었습니다. emailAddr은 null일 수 없습니다.'
description: ' [!DNL Adobe Workfront] 내 도메인의 URL에 로그인하려고 하면 SAML 로그인 포털로 리디렉션된 다음  [!DNL Workfront] 로 다시 리디렉션됩니다. 이때 emailAddr 필드는 null일 수 없습니다.'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
TQID: https://experienceleague.adobe.com/MfWVOYcQAVjlbxwiqVaPwipyq5ulv0toajH-2tX7c9k
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
source-wordcount: 146
ht-degree: 4%

---

# 로그인 오류: 다음 필드가 잘못되었습니다. emailAddr은 null일 수 없습니다.

## 문제

URL(https://customerdomain.my.workfront.com)을 사용하여 [!DNL Adobe Workfront]에 로그인하려고 하면 SAML 로그인 포털로 리디렉션된 다음 다음 오류가 발생하여 다시 [!DNL Workfront]&#x200B;(으)로 리디렉션됩니다.

“다시 시도해 보십시오. 다음 필드가 잘못되었습니다. emailAddr은 null일 수 없습니다.&quot;

## 원인

이 오류는 SAML 2.0 구성의 사용자 속성 매핑 영역에 잘못된 항목이 있기 때문에 발생합니다. SAML 2.0의 사용자 특성을 매핑하는 방법에 대한 자세한 내용은 [SAML 2.0을 사용하여 Adobe Workfront 구성](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)을 참조하십시오.

## 솔루션

전자 메일 주소의 특성 매핑을 업데이트하고 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
