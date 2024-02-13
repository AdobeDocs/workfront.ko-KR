---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Adobe Admin Console에 조직 온보딩 준비
description: Adobe Workfront은 Adobe 제품이므로 Adobe Admin Console을 통해 액세스할 수 있습니다. 이를 통해 Workfront을 다른 Adobe 계정 및 제품과 함께 중앙 위치에서 관리할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: 5d4434d090c4b6cdefc9c313fecccf6d6e9a510b
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 0%

---

# Adobe Admin Console에 조직 온보딩 준비

<!-- Audited: 12/2023 -->

Adobe Workfront은 Adobe 제품이므로 Adobe Admin Console을 통해 액세스할 수 있습니다. 이를 통해 Workfront을 다른 Adobe 계정 및 제품과 함께 중앙 위치에서 관리할 수 있습니다.

모든 Workfront 고객은 결국 Adobe Admin Console으로 이동됩니다. 조직이 Adobe Admin Console으로 이동하면 Workfront 인증이 콘솔에서 관리됩니다. 이러한 조치를 보다 빨리 준비하고 이행하면 향후 보다 빠른 혁신을 위해 작업 관리의 효율성을 높이고 조직을 포지셔닝할 수 있는 토대가 마련됩니다

Adobe Admin Console에 대한 개요는 를 참조하십시오. [Admin Console 개요](https://helpx.adobe.com/enterprise/using/admin-console.html).

## 마이그레이션 검사 목록

조직이 Adobe Admin Console으로 마이그레이션할 수 있도록 하려면 다음 작업을 수행해야 합니다.

1. Workfront을 추가하려는 원하는 Adobe Admin Console을 식별합니다.

   * 조직에 기존 Adobe Admin Console이 없거나 기존 Adobe Admin Console을 사용하지 않으려는 경우 Workfront 지원 센터에서 새 템플릿을 만드는 데 도움을 줄 수 있습니다.

   * 여러 Adobe Admin Console이 있고 어떤 것이 Workfront을 추가하기에 가장 적합한지 확실하지 않은 경우 Workfront 지원 센터에 문의하십시오.

1. 기존 Workfront을 사용하거나 새 Adobe Admin Console을 생성하려는 경우 지원 팀에 문의하십시오.

1. Adobe Admin Console에서 ID 관리를 설정합니다.

   >[!IMPORTANT]
   >
   >SSO(Single Sign-On) 또는 SSO 이외 인증 환경 설정과 같은 인증 환경 설정에 대해 Workfront 지원 센터 및 IT 팀과 논의할 준비를 하십시오.

   자세한 내용은 의 Identity Management 섹션을 참조하십시오. [Adobe Admin Console용 배포 안내서](https://helpx.adobe.com/enterprise/using/deployment-planning.html).

1. (조건부) SSO(Single Sign-On)를 사용하는 경우, 새 Adobe Admin Console을 기존 SSO 공급자에 연결합니다.

   자세한 내용 및 지침은 [ID 설정](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >조직에서 SSO(Single Sign-On)를 사용하지 않는 경우 Adobe Admin Console으로 마이그레이션된 모든 사용자는 계정과 암호를 생성할 수 있는 이메일을 받게 됩니다.

1. 사용자 이메일 주소를 마이그레이션할 준비가 되었는지 확인합니다.

   1. Workfront에서 중복 이메일을 제거합니다.

      자세한 내용은 [Workfront 인스턴스에서 기존 사용자의 이메일 주소 업데이트](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md#update-email-addresses-of-existing-users-in-your-workfront-instance) 위치: [중복 사용자 방지](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md).

      조직에 중복 이메일 주소가 있는 경우 사용자는 가장 최근의 이메일 주소로 표시됩니다 `lastLoginDate` 은 Adobe Admin Console 조직으로 이동됩니다. 해당 이메일 주소를 사용하는 다른 모든 사용자는 비활성화됩니다.

      >[!NOTE]
      >
      >지정된 이메일 주소를 가진 한 명의 사용자만 지정된 시간에 활성화할 수 있으므로, 현재 활성 사용자와 동일한 이메일 주소를 가진 다른 사용자를 활성화해야 하는 경우, 비활성화된 사용자를 활성화하기 전에 먼저 현재 활성 사용자를 비활성화해야 합니다.

   1. (조건부) 사용자 정의 API 통합을 활용하는 경우 해당 사용자가 액세스할 수 있는 유효한 이메일 주소가 있는지 확인하십시오.

   1. (선택 사항) Workfront에 추가되지 않도록 더 이상 Adobe Admin Console에 액세스할 필요가 없는 사용자는 비활성화하는 것이 좋습니다.

   >[!IMPORTANT]
   >
   >사용자 이메일에 대한 이러한 작업은 조직이 Adobe Admin Console으로 이동하기 전에 완료되어야 합니다.

1. (선택 사항) OAuth2를 사용하도록 모든 사용자 지정 통합을 업데이트합니다.

   OAuth2 통합 설정에 대한 지침은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   >[!NOTE]
   >
   >이 단계는 선택적이지만 다른 형태의 API 인증 및 권한 부여가 향후에 더 이상 사용되지 않으므로 적극 권장합니다.

Adobe Admin Console이 Workfront으로 구성된 후 이를 사용하여 Workfront 시스템 관리자를 만들 수 있습니다.

자세한 내용은 [Adobe Admin Console에서 시스템 관리자 관리](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 다른 기타 작업 목록은 을 참조하십시오. [플랫폼 기반 관리의 차이점(Adobe Workfront/Adobe 비즈니스 플랫폼)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
