---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Adobe Workfront과 Workfront Proof 간의 사용자 동기화
description: 사용자 정보는 Adobe Workfront에서 Workfront Proof으로 동기화되며 Workfront Proof에서 Workfront으로 동기화되지 않습니다. 따라서 사용자를 생성하거나 수정할 때마다 Workfront 내에서 해당 사항을 변경해야 합니다. Workfront Proof 내에서는 사용자를 변경할 수 없습니다.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Adobe Workfront과 Workfront Proof 간의 사용자 동기화

사용자 정보는 Adobe Workfront에서 Workfront Proof으로 동기화되며 Workfront Proof에서 Workfront으로 동기화되지 않습니다. 따라서 사용자를 생성하거나 수정할 때마다 Workfront 내에서 해당 사항을 변경해야 합니다. Workfront Proof 내에서는 사용자를 변경할 수 없습니다.

다음 섹션에서는 Workfront에서 Workfront Proof으로의 사용자 동기화에 대한 정보를 제공합니다.

## 동기화된 정보

Workfront은 다음 사용자 정보를 Workfront Proof에 동기화합니다.

* 이름(사용자의 이름과 성)
* 이메일 주소

## 동기화 발생 시

다음과 같은 경우 사용자 정보가 Workfront에서 Workfront Proof으로 동기화됩니다.

* 사용자 정보가 Workfront에서 업데이트됩니다.
* Workfront에서 사용자가 생성됨

이메일 주소가 동일한 사용자가 Workfront Proof에 있는지 여부에 따라 다음 중 하나가 발생합니다.

* **일치하는 전자 메일이 있는 사용자가 Workfront Proof에 없는 경우**

   * **사용자에 대해 증명을 사용할 수 있습니다.** 사용자가 Workfront Proof에서 사용자로 만들어집니다.
   * **사용자에 대해 증명을 사용할 수 없습니다.** 사용자가 Workfront Proof에서 연락처로 만들어집니다.

* **전자 메일이 일치하는 사용자가 Workfront Proof에 있는 경우:** Workfront의 해당 사용자에 대해 증명이 활성화되어 있고(아직 활성화되어 있지 않은 경우) 두 사용자 간에 정보가 동기화됩니다.

  자세한 내용은 [사용자 증명 액세스 구성](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md)에서 [사용자 증명 액세스 구성](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md)을 참조하십시오.

  >[!IMPORTANT]
  >
  >이메일이 일치하는 사용자가 자신의 증명 환경이나 다른 증명 환경에 있으면 Workfront은 사용자의 계정 ID를 이메일에 접미사로 추가하여 별칭 이메일 주소를 만듭니다. 예: *username+accountid@domain.com*. 별칭 이메일이 만들어져도 사용자는 증명 알림을 계속 수신하게 됩니다.
