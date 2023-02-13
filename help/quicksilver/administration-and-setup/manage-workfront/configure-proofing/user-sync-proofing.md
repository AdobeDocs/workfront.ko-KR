---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Adobe Workfront과 Workfront 증명 간의 사용자 동기화
description: 사용자 정보는 Adobe Workfront에서 Workfront 증명으로 동기화됩니다. Workfront Proof에서 Workfront으로 동기화되지 않습니다. 따라서 사용자를 만들거나 수정할 때마다 Workfront 내에서 그러한 변경을 수행해야 합니다. Workfront 증명 내에서 사용자를 변경할 수 없습니다.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
source-git-commit: b310e36c9eb148db631e7a3552a35dcccc652d60
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Adobe Workfront과 Workfront 증명 간의 사용자 동기화

사용자 정보는 Adobe Workfront에서 Workfront 증명으로 동기화됩니다. Workfront Proof에서 Workfront으로 동기화되지 않습니다. 따라서 사용자를 만들거나 수정할 때마다 Workfront 내에서 그러한 변경을 수행해야 합니다. Workfront 증명 내에서 사용자를 변경할 수 없습니다.

다음 섹션에서는 Workfront에서 Workfront 증명으로 사용자 동기화에 대한 정보를 제공합니다.

## 동기화된 정보

Workfront은 다음 사용자 정보를 Workfront Proof에 동기화합니다.

* 이름(사용자의 이름과 성)
* 이메일 주소

## 동기화가 발생할 때

다음 상황에서 사용자 정보는 Workfront에서 Workfront 증명으로 동기화됩니다.

* 사용자의 정보가 Workfront에서 업데이트됩니다
* 사용자가 Workfront에서 만들어집니다

Workfront 증명에 동일한 이메일 주소를 사용하는 사용자가 있는지 여부에 따라 다음 중 하나가 발생합니다.

* **Workfront 증명에 일치하는 이메일을 가진 사용자가 없는 경우**

   * **사용자에 대해 언어 교정이 활성화되어 있습니다.** 사용자가 Workfront 증명의 사용자로 생성됩니다.
   * **사용자에 대해 언어 교정을 사용할 수 없습니다.** 사용자가 Workfront 증명의 연락처로 만들어집니다.

* **일치하는 이메일을 가진 사용자가 Workfront 증명에 있는 경우:** Workfront에서 해당 사용자에 대해 언어 교정이 활성화되고(아직 활성화되지 않은 경우) 두 사용자 간에 정보가 동기화됩니다.

   자세한 내용은 [사용자의 언어 교정 액세스 구성](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) in [사용자의 언어 교정 액세스 구성](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

   >[!IMPORTANT]
   >
   >이메일이 일치하는 사용자가 있거나 자체 또는 다른 교정 환경에 있으면 Workfront에서는 사용자 계정 ID를 이메일에 접미어로 추가하여 별칭 이메일 주소를 만듭니다. 예, *username+accountid@domain.com*. 별칭 전자 메일이 만들어져도 사용자는 여전히 증명 알림을 받게 됩니다.
