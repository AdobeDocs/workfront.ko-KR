---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Adobe Admin Console에 조직 온보딩 준비
description: Adobe Workfront은 Adobe 제품이므로 Adobe Admin Console을 통해 액세스할 수 있습니다. 이를 통해 중앙 위치에서 사용자의 다른 Adobe 계정 및 제품과 함께 Workfront을 관리할 수 있습니다.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Adobe Admin Console에 조직 온보딩 준비

Adobe Workfront은 Adobe 제품이므로 Adobe Admin Console을 통해 액세스할 수 있습니다. 이를 통해 중앙 위치에서 사용자의 다른 Adobe 계정 및 제품과 함께 Workfront을 관리할 수 있습니다.

모든 Workfront 고객은 결국 Adobe Admin Console으로 이동합니다. 조직이 Adobe Admin Console으로 이동하면 Adobe Admin Console에서 Workfront 인증을 관리합니다. 이러한 조치를 보다 신속하게 준비하고 실현하는 것은 향후 작업 관리의 효율성 및 조직의 신속한 혁신을 위한 토대를 마련합니다

Adobe Admin Console에 대한 개요는 다음을 참조하십시오 [Admin Console 개요](https://helpx.adobe.com/enterprise/using/admin-console.html).

## 마이그레이션 체크리스트

조직이 Adobe Admin Console으로 마이그레이션할 수 있도록 하려면 다음 작업을 수행해야 합니다

1. Workfront을 추가할 Adobe Admin Console을 식별합니다.

   * 조직에 기존 Adobe Admin Console이 없거나 기존 Adobe Admin Console을 사용하지 않으려는 경우 Workfront 지원 을 통해 새 만들기를 지원할 수 있습니다.

   * 여러 개의 Adobe Admin Console이 있고 Adobe Workfront을 추가하기에 가장 적합한을 잘 모르는 경우 Workfront 지원 센터에 문의하십시오.

1. Workfront 지원 센터에서 기존 Adobe Admin Console을 사용하거나 새를 생성했는지 확인합니다.

1. Adobe Admin Console에서 ID 관리를 설정합니다.

   >[!IMPORTANT]
   >
   >SSO(Single Sign-On) 또는 비SSO와 같은 인증 환경 설정에 대해서는 Workfront 지원 및 IT 팀과 상의할 수 있습니다.

   지침은 Adobe Admin Console용 배포 안내서(https://helpx.adobe.com/enterprise/using/deployment-planning.html)의 Identity Management 섹션을 참조하십시오.

1. (조건부) Single Sign-On을 사용하는 경우 새 Adobe Admin Console을 기존 SSO 공급자에 연결합니다

   자세한 내용 및 지침은 [ID 설정](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >조직에서 Single Sign-On을 사용하지 않는 경우 Adobe Admin Console으로 마이그레이션된 모든 사용자는 계정 및 암호를 만들 수 있는 이메일을 받게 됩니다.

1. 사용자 이메일 주소가 마이그레이션할 준비가 되었는지 확인합니다.

   1. Workfront에서 중복 이메일 제거

      자세한 내용은 중복 사용자 방지에서 Workfront 인스턴스에 있는 기존 사용자의 이메일 주소 업데이트를 참조하십시오.

      조직에 중복 이메일 주소가 있는 경우 가장 최근 이메일 주소로 해당 사용자가 표시됩니다 `lastLoginDate` Adobe Admin Console 조직으로 이동합니다. 해당 이메일 주소를 사용하는 다른 사용자는 비활성화됩니다.

      >[!NOTE]
      >
      >지정된 이메일 주소를 사용하는 한 사용자만 지정된 시간에 활성 상태가 될 수 있으므로 현재 활성 사용자와 동일한 이메일 주소를 사용하는 다른 사용자를 활성화해야 하는 경우 비활성화된 사용자를 활성화하기 전에 먼저 현재 활성 사용자를 비활성화해야 합니다.

   2. (조건부) 사용자 지정 API 통합을 활용하는 경우 해당 사용자에게 액세스할 수 있는 유효한 이메일 주소가 있는지 확인합니다.

   3. (선택 사항) 더 이상 Workfront에 액세스할 필요가 없는 모든 사용자는 Adobe Admin Console에 추가되지 않도록 하는 것이 좋습니다.
   >[!IMPORTANT]
   >
   >조직이 Adobe Admin Console으로 이동하기 전에 사용자 이메일에 대한 다음 작업을 완료해야 합니다.

1. (선택 사항) OAuth2를 사용하도록 모든 사용자 지정 통합을 업데이트합니다.

   OAuth2 통합 설정에 대한 지침은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   OAuth2 통합 만들기는 새 Workfront 경험에서만 사용할 수 있습니다.

   >[!NOTE]
   >
   >이 단계는 선택 사항이지만, 다른 형태의 API 인증 및 권한은 나중에 더 이상 사용되지 않으므로 적극 권장됩니다.

Adobe Admin Console이 Workfront으로 구성된 후 이 파일을 사용하여 사용자를 관리할 수 있습니다.

자세한 내용은 [Adobe Admin Console에서 사용자 관리](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 다른 작업 목록은 다음을 참조하십시오 [플랫폼 기반의 관리 차이점(Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
