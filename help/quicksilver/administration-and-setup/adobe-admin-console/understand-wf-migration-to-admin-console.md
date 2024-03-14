---
user-type: Admin
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Adobe Admin Console으로의 Workfront 마이그레이션 이해
description: Workfront 제품 및 Adobe Admin Console으로의 사용자 마이그레이션 이해
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 54d855e6-c387-458c-9cd3-f32318c8ae02
source-git-commit: 0a638b143d2de4b8ff2948e701ee90acbd1ab857
workflow-type: tm+mt
source-wordcount: '1067'
ht-degree: 0%

---

# Adobe Admin Console으로의 Workfront 마이그레이션 이해

Adobe은 Adobe Workfront 사용자를 관리하는 방법을 변경하여 사용자와 조직에 생산성을 높여줍니다. 이 변경의 일부로 Adobe은 Workfront 인스턴스와 사용자를 Adobe Admin Console으로 마이그레이션하고 있습니다. 이는 필수 마이그레이션이며 보고, 승인 경로, 콘텐츠 또는 자산에는 영향을 주지 않습니다. 사용자 액세스를 관리하는 방법과 사용자가 로그인하는 방법에 영향을 줍니다.

Adobe Admin Console을 사용하여 전체 조직에서 Adobe 권한을 관리하는 방법에 대해 알아보려면 다음을 참조하십시오. [Adobe Admin Console에서 사용자 관리](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

## 변경 사항

마이그레이션의 일부로 사용자 관리가 Workfront 애플리케이션 내에서 다음 관리 역할을 사용하여 Adobe Admin Console으로 이동합니다.

* **시스템 관리자** 는 모든 관리자의 권한을 가진 수퍼 사용자입니다. 모든 관리자 역할을 할당하고 모든 제품에 대해 전체 조직의 사용자를 관리합니다.

* **제품 프로필 관리자(Workfront 시스템 관리자)** 조직에서 Workfront에 액세스할 수 있는 사용자를 관리합니다.

* **사용자는 Adobe ID로 로그인합니다.** Adobe이 기존 사용자를 Adobe Admin Console으로 마이그레이션한 후 사용자는 새로운 Adobe ID(Adobe ID 또는 Adobe Federated ID(SSO)를 사용하여 Workfront 인스턴스에 로그인합니다.

* **다른 모든 기능을 관리하는 방법에는 변경 사항이 없습니다** 기능, 사용자 역할, 작업 공간, 기능 및 비헤이비어 관리를 포함하여 Workfront 애플리케이션 자체 내에서.

## 마이그레이션 여정 타임라인

Adobe은 먼저 Workfront 인스턴스를 Adobe Admin Console으로 마이그레이션한 다음 확인된 이메일 주소를 사용하는 모든 기존 사용자를 마이그레이션합니다. 시스템 관리자 또는 Workfront 제품 프로필 관리자(Workfront 시스템 관리자)인 경우 마이그레이션 여정을 안내하는 이메일을 받게 됩니다. 다음은 예상할 수 있는 작업의 타임라인입니다.

### Adobe Admin Console으로 Workfront 마이그레이션 완료

Adobe Admin Console으로 Workfront 마이그레이션이 완료되면 시스템 관리자에게 이메일이 전송됩니다. 현재 시스템 관리자는 몇 가지 필요한 단계를 완료해야 할 수 있습니다 **사용자 마이그레이션이 시작되기 전**: Workfront 사용자에게 미치는 영향을 최소화합니다.

* **Workfront 사용자가 현재 SSO로 로그인되어 있는 경우**, 사용자가 SSO를 사용하여 계속 로그인할 수 있도록 Adobe Admin Console에서 SSO를 설정해야 합니다. Workfront 사용자가 현재 SSO를 사용하고 있지 않지만 Adobe Admin Console에서 설정하려는 경우 마이그레이션 여정에서 이 시점에서 설정할 수 있습니다.
* **Adobe Admin Console에서 다른 Adobe 제품을 이미 관리하고 있는 경우**, Adobe은 기존 콘솔로 사용자를 자동으로 마이그레이션하는 데 동의할 수 있습니다. 다음을 클릭합니다. **시작** 동의 페이지로 이동하려면 이메일의 버튼을 클릭합니다.
* **이전에 요청자 라이선스 유형을 삭제한 경우**: 시스템에 추가됩니다. 이 라이선스 유형에는 사용자가 할당되지 않지만, Workfront과 Adobe Admin Console 간의 동기화에 필요합니다. 요청자 라이선스 유형과 관련하여 필요한 작업은 없습니다.

현재 사용자 관리에 대한 변경 사항은 없습니다. Workfront 관리자는 Workfront의 사용자를 계속 관리하며, 사용자 마이그레이션이 완료될 때까지 사용자는 Workfront ID 또는 SSO로 계속 로그인합니다.

### 사용자 마이그레이션 예약

시스템 관리자가 이전 섹션에 설명된 사전 요구 사항을 완료하면 Adobe은 이러한 사전 요구 사항이 완료된 후 30일 동안 사용자 마이그레이션을 자동으로 예약하며, Workfront 제품 프로필 관리자(Workfront 시스템 관리자)와 통신하여 사용자 마이그레이션을 관리합니다.

Workfront 제품 프로필 관리자(Workfront 시스템 관리자)는

* 예약된 사용자 마이그레이션 시작 일자(사전 요구 사항이 완료된 후 약 30일)가 포함된 이메일 수신
* 지정된 Workfront 관리자 콘솔에 액세스하여 마이그레이션 날짜를 변경할 수 있습니다

  >[!NOTE]
  >
  >마이그레이션의 복잡성으로 인해 날짜 변경은 예약된 날짜를 30일 이내로 제한됩니다. 더 늦은 날짜가 필요한 경우 지원 센터에 문의하십시오.

* 사용자 마이그레이션 시작일 1일 전에 미리 알림 이메일 수신

### 사용자를 마이그레이션할 날 준비

Workfront 제품 프로필 관리자(Workfront 시스템 관리자)는 모든 사용자가 마이그레이션할 준비가 되었는지 확인할 책임이 있습니다.

* Adobe ID로의 향후 마이그레이션에 대해 모든 사용자에게 다음 사항을 알림으로써 준비합니다.

   * 사용자가 마이그레이션되면 Adobe에서 Workfront에 로그인하는 방식의 변경 사항을 알리는 이메일을 받게 됩니다. 기존 Adobe ID으로 로그인하거나 동일한 이메일 주소를 사용하여 새 사용자를 설정하여 Adobe ID를 사용하여 로그인하라는 초대를 처음으로 수락하도록 사용자를 초대합니다.

### 마이그레이션 당일 기대 사항

* **사용자 마이그레이션은 고객이 호스팅하는 Workfront 데이터 센터의 자정 이후에 시작됩니다.**

* **Adobe은 먼저 Workfront 관리자를 자동으로 마이그레이션합니다.** Workfront 관리자가 Adobe ID로 마이그레이션되면 Adobe 제품 프로필 관리자(Workfront 시스템 관리자) 역할이 할당됩니다. 마이그레이션 전에 사용자가 가질 수 있는 기존 역할은 영향을 받지 않습니다.

  >[!NOTE]
  >
  >사용자 마이그레이션 중에도 제품에 대한 액세스 손실이 발생하지 않습니다. 사용자가 마이그레이션되는 동안 사용자가 로그인하면 아무런 영향이 없습니다. 그러나 다음 로그인 시 Adobe ID를 사용해야 합니다.



* **Adobe이 마이그레이션되면 사용자는 Workfront에 로그인하는 방식으로 변경되었음을 알리는 이메일을 사용자로부터 받게 됩니다.** 기존 Adobe ID으로 로그인하거나 동일한 이메일 주소를 사용하여 새 Adobe ID을 설정하여 Adobe ID를 사용하여 로그인하라는 초대를 처음으로 수락하도록 사용자를 초대합니다.

  Adobe ID으로 Workfront에 로그인하는 방법에 대한 자세한 내용은 [Adobe Experience Cloud에 로그인](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md#log-in-to-adobe-experience-cloud).

### 사용자 마이그레이션 완료

Adobe은 모든 관리자 및 사용자가 마이그레이션된 후 모든 시스템 관리자 및 제품 프로필 관리자(Workfront 시스템 관리자)에게 이메일을 통해 알립니다. 현재 해당 인스턴스에 대한 모든 Workfront 사용자는 Adobe ID를 사용하여 Workfront에 로그인합니다. Workfront 시스템 관리자 및 제품 프로필 관리자(Workfront 시스템 관리자)는 Adobe Admin Console 내에서 사용자 액세스를 관리할 수 있습니다. 고객이 관리자 콘솔 내에서 디렉터리 동기화 형식을 사용하지 않는 경우 Workfront 애플리케이션 내에서 Workfront에 대한 액세스를 계속 관리할 수 있습니다.

## 지원 받기

질문 또는 관심사에 대해서는 이 문서에 설명된 단계를 따르십시오 [고객 지원 문의](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).




