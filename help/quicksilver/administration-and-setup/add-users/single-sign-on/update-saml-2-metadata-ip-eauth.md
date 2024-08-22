---
title: 향상된 인증을 사용할 때 IDP에서 SAML 2.0 메타데이터 업데이트
description: Adobe Workfront 관리자는 SAML(Security Assertion Markup Language) 2.0 프로토콜을 지원하는 ID 공급자와 Workfront SSO(Single Sign-On)를 통합할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: fab7a3a1c66635b11418a216999dee84a30a50bb
workflow-type: tm+mt
source-wordcount: '938'
ht-degree: 0%

---

# 향상된 인증을 사용할 때 IDP에서 SAML 2.0 메타데이터 업데이트

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Adobe Workfront 관리자는 SAML(Security Assertion Markup Language) 2.0 프로토콜을 지원하는 ID 공급자와 Workfront SSO(Single Sign-On)를 통합할 수 있습니다.

다음 섹션에서는 Workfront 계정이 향상된 인증 환경으로 업그레이드된 경우의 통합 프로세스를 설명합니다(일부 조직에서는 아직 사용할 수 없음). 향상된 인증 환경에 대한 자세한 내용은 [향상된 인증 개요](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md)를 참조하십시오.

향상된 인증 환경으로 마이그레이션하기 전에 SAML을 구성하는 방법에 대한 자세한 내용은 [ID 공급자에서 SAML 2.0 메타데이터 업데이트](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)를 참조하십시오.


## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Okta를 ID 공급자로 사용

Okta는 SAML 2.0을 지원하는 ID 공급자의 예입니다. 이 섹션에서는 ID 공급자로서 Okta를 사용하는 방법에 대해 설명합니다. SAML 2.0을 지원하는 다른 ID 공급자를 구성할 때도 유사한 단계가 필요합니다.

>[!NOTE]
>
>사용자는 이메일 주소를 기반으로 매핑됩니다. Okta를 사용하여 Workfront에 로그인하려면 Workfront 고객에서 만든 이메일 주소가 동일한(대/소문자 구분 안 함) 사용자가 있어야 합니다.

다음 섹션을 완료하여 Okta를 Workfront에서 ID 공급자로 구성합니다.

* [Okta에서 Workfront 앱 만들기](#create-a-workfront-app-in-okta)
* [Workfront에서 ID 공급자로 Okta 인스턴스 추가](#add-your-okta-instance-as-an-identity-provider-in-workfront)

### Okta에서 Workfront 앱 만들기 {#create-a-workfront-app-in-okta}

1. Okta 환경에 로그인합니다.
1. Okta 인터페이스의 왼쪽 상단 모서리에서 **클래식 UI**&#x200B;이(가) 선택되어 있는지 확인합니다.
1. 메뉴에서 **응용 프로그램** > **응용 프로그램**&#x200B;을 클릭합니다.

1. **응용 프로그램 추가**&#x200B;를 클릭한 다음 **새 앱 만들기**&#x200B;를 클릭합니다.

1. **새 응용 프로그램 통합 만들기** 상자에서 **SAML 2.0**&#x200B;을 선택한 다음 **만들기**&#x200B;를 클릭합니다.

1. Workfront 앱의 이름을 지정한 후 **다음**&#x200B;을 클릭합니다.
1. 표시되는 SAML 설정 페이지에서 SAML 설정 페이지에 필요한 정보를 찾습니다.

   1. Okta 인터페이스가 표시된 브라우저 탭을 종료하지 않고 별도의 브라우저 탭이나 창을 엽니다.
   1. 브라우저에서 다음 URL을 지정합니다.

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. 결과 XML 파일에서 **entityID** 및 **Location**&#x200B;의 값을 식별하십시오.

      ![sso-okta.png](assets/sso-okta.png)

   1. **entityID** 필드의 값을 시스템 클립보드에 복사합니다. 이 브라우저 탭을 닫지 마십시오.

1. 6단계에서 연 SAML 설정 페이지로 돌아갑니다.
1. **entityID** 필드의 값을 **대상 URI(SP 엔티티 ID)** 필드에 붙여 넣으십시오.

1. 다른 브라우저 탭의 XML 파일에서 **위치** 필드의 값을 복사합니다.
1. **위치** 필드의 값을 **단일 사인온** **URL** 필드에 붙여 넣으십시오.

1. **특성 문(선택 사항)** 섹션으로 스크롤합니다.
1. **이름** 필드에 **전자 메일**&#x200B;을(를) 지정하십시오.

1. **값** 필드에 **user.email**&#x200B;을(를) 지정합니다.

1. (선택 사항) 고급 값을 추가합니다.
1. **다음**&#x200B;을 클릭합니다.
1. **내부 앱을 추가하는 Okta 고객입니다**&#x200B;를 선택하고 **마침**&#x200B;을 클릭합니다.

### Workfront에서 ID 공급자로 Okta 인스턴스 추가 {#add-your-okta-instance-as-an-identity-provider-in-workfront}

이 절차에서는 Workfront에서 ID 공급자로 Okta를 구성하는 데 필요한 정보를 제공합니다. 다른 매핑 또는 구성 옵션에 대한 자세한 내용은 [SAML 2.0을 사용하여 Adobe Workfront 구성](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)을 참조하십시오.

1. Okta 인스턴스에 대한 ID 공급자 메타데이터 다운로드:

   1. Okta 환경에 로그인합니다.
   1. Okta 인터페이스의 왼쪽 상단 모서리에서 **클래식 UI**&#x200B;이(가) 선택되어 있는지 확인합니다.
   1. 메뉴에서 **응용 프로그램** > **응용 프로그램**&#x200B;을 클릭합니다.

   1. [Okta에서 Workfront 앱 만들기](#create-a-workfront-app-in-okta) 섹션에 설명된 대로 만든 Workfront 앱을 클릭합니다
   1. **로그온** 탭에서 **ID 공급자 메타데이터**&#x200B;를 클릭합니다.

      ![idp_okta_metadata.png](assets/idp-okta-metadata.png)

      메타데이터는 새 브라우저 탭에서 XML로 열립니다.

   1. 브라우저 URL 필드에 표시되는 URL을 복사합니다.

1. Workfront에 Workfront 관리자로 로그인합니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **시스템** > **SSO(Single Sign-On)**&#x200B;를 클릭합니다.

1. (조건부) 두 개의 탭이 표시되면 **새 SSO 공급자** 탭을 클릭합니다.

   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >계정을 향상된 인증 환경으로 업데이트하고 새 SSO 구성이 완전히 작동할 때까지 **현재 SSO 공급자** 탭에서 기존 SSO 구성 설정을 삭제하지 마십시오.

1. **새 SSO 공급자**&#x200B;를 클릭합니다.
1. Okta IDP와 같은 이름을 지정한 다음 설명을 지정합니다.
1. **ID 공급자 메타데이터에서 필드 채우기** 섹션에서 1단계에서 복사한 URL을 **메타데이터 URL** 필드에 붙여 넣습니다.\
   또는 **파일 선택**&#x200B;을 클릭하여 .xml 파일을 업로드할 수 있지만 URL을 붙여 넣는 것이 좋습니다.

1. **사용자 특성 매핑** 섹션의 **디렉터리 특성** 필드에 **전자 메일**&#x200B;을(를) 입력하십시오. (**전자 메일 주소**&#x200B;이(가) 이미 **Workfront 사용자 특성** 필드에 채워져 있습니다.)

1. (선택 사항) 인증되지 않은 사용자를 인증을 위해 Workfront 로그인 화면이 아닌 ID 공급자 로그인 화면으로 보내려면 **기본 SSO 공급자로 설정**&#x200B;을 활성화합니다. 시스템의 모든 사용자가 ID 공급자를 통해 Workfront에 액세스하는 경우에만 이 옵션을 활성화하는 것이 좋습니다.
1. **사용** 확인란을 선택하십시오. 이 작업을 수행하기 전에 시스템의 사용자가 새 로그인 환경을 알고 있는지 확인하여 Workfront 시스템에 대한 액세스 권한을 잃지 않도록 하십시오.
1. **연결 테스트**&#x200B;를 클릭합니다.\
   연결에 성공했다는 메시지가 표시됩니다.

1. **저장**&#x200B;을 클릭합니다.

## 다른 ID 공급자 사용

Okta 이외의 ID 공급자(예: Ping 또는 Centrify)를 사용하는 경우 Workfront 메타데이터를 ID 공급자에게 다시 업로드해야 합니다.
