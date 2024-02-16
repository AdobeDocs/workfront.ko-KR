---
title: 향상된 인증을 사용할 때 IDP에서 SAML 2.0 메타데이터 업데이트
description: Adobe Workfront 관리자는 SAML(Security Assertion Markup Language) 2.0 프로토콜을 지원하는 ID 공급자와 Workfront SSO(Single Sign-On)를 통합할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# 향상된 인증을 사용할 때 IDP에서 SAML 2.0 메타데이터 업데이트

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Adobe Workfront 관리자는 SAML(Security Assertion Markup Language) 2.0 프로토콜을 지원하는 ID 공급자와 Workfront SSO(Single Sign-On)를 통합할 수 있습니다.

다음 섹션에서는 Workfront 계정이 향상된 인증 환경으로 업그레이드된 경우의 통합 프로세스를 설명합니다(일부 조직에서는 아직 사용할 수 없음). 향상된 인증 경험에 대한 자세한 내용은 [향상된 인증 개요](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

향상된 인증 환경으로 마이그레이션하기 전에 SAML을 구성하는 방법에 대한 자세한 내용은 [ID 공급자에서 SAML 2.0 메타데이터 업데이트](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).


## 액세스 요구 사항

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
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가적인 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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
1. 다음을 확인합니다. **클래식 UI** 은 Okta 인터페이스의 왼쪽 위 모서리에서 선택됩니다.
1. 메뉴에서 다음을 클릭합니다. **애플리케이션** > **애플리케이션**.

1. 클릭 **응용 프로그램 추가**&#x200B;을 클릭한 다음 을 클릭합니다 **새 앱 만들기**.

1. 다음에서 **새 애플리케이션 통합 대화 상자 만들기** 상자, 선택 **SAML 2.0**&#x200B;을 클릭한 다음 을 클릭합니다 **만들기**.

1. Workfront 앱의 이름을 지정한 다음 **다음**.
1. 표시되는 SAML 설정 페이지에서 SAML 설정 페이지에 필요한 정보를 찾습니다.

   1. Okta 인터페이스가 표시된 브라우저 탭을 종료하지 않고 별도의 브라우저 탭이나 창을 엽니다.
   1. 브라우저에서 다음 URL을 지정합니다.

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. 결과 XML 파일에서 **entityID** 및 **위치**.

      ![sso-okta.png](assets/sso-okta.png)

   1. 에서 값 복사 **entityID** 시스템 클립보드에 대한 필드입니다. 이 브라우저 탭을 닫지 마십시오.

1. 6단계에서 연 SAML 설정 페이지로 돌아갑니다.
1. 에서 값 붙여넣기 **entityID** 필드에 값을 입력한 경우 **대상 URI(SP 엔티티 ID)** 필드.

1. 다른 브라우저 탭의 XML 파일에서 **위치** 필드.
1. 에서 값 붙여넣기 **위치** 필드에 값을 입력한 경우 **단일 사인온** **URL** 필드.

1. 다음으로 스크롤 **속성 문(선택 사항)** 섹션.
1. 다음에서 **이름** 필드, 지정 **이메일**.

1. 다음에서 **값** 필드, 지정 **user.email**.

1. (선택 사항) 고급 값을 추가합니다.
1. 클릭 **다음**.
1. 선택, **내부 앱을 추가하는 Okta 고객입니다**&#x200B;을 클릭한 다음 을 클릭합니다 **완료**.

### Workfront에서 ID 공급자로 Okta 인스턴스 추가 {#add-your-okta-instance-as-an-identity-provider-in-workfront}

이 절차에서는 Workfront에서 ID 공급자로 Okta를 구성하는 데 필요한 정보를 제공합니다. 다른 매핑 또는 구성 옵션에 대한 자세한 내용은 [SAML 2.0으로 Adobe Workfront 구성](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

1. Okta 인스턴스에 대한 ID 공급자 메타데이터 다운로드:

   1. Okta 환경에 로그인합니다.
   1. 다음을 확인합니다. **클래식 UI** 은 Okta 인터페이스의 왼쪽 위 모서리에서 선택됩니다.
   1. 메뉴에서 다음을 클릭합니다. **애플리케이션** > **애플리케이션**.

   1. 섹션에 설명된 대로 생성한 Workfront 앱을 클릭합니다. [Okta에서 Workfront 앱 만들기](#create-a-workfront-app-in-okta)
   1. 다음에서 **로그온** 탭을 클릭하고 **ID 공급자 메타데이터**.

      ![idp_okta_metadata.png](assets/idp-okta-metadata.png)

      메타데이터는 새 브라우저 탭에서 XML로 열립니다.

   1. 브라우저 URL 필드에 표시되는 URL을 복사합니다.

1. Workfront에 Workfront 관리자로 로그인합니다.
1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **시스템** > **SSO(단일 인증)**.

1. (조건부) 탭이 두 개 표시되면 **새 SSO 공급자** 탭.

   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >에서 기존 SSO 구성 설정을 삭제하지 마십시오. **현재 SSO 공급자** 계정이 향상된 인증 환경으로 업데이트되고 새 SSO 구성이 완전히 작동할 때까지 를 탭합니다.

1. 클릭 **새 SSO 공급자**.
1. Okta IDP와 같은 이름을 지정한 다음 설명을 지정합니다.
1. 다음에서 **ID 공급자 메타데이터에서 필드 채우기** 섹션에서 1단계에서 복사한 URL을 **메타데이터 URL** 필드.\
   또는 를 클릭할 수 있습니다 **파일 선택** .xml 파일을 업로드하려면 URL을 붙여 넣는 것이 좋습니다.

1. 다음에서 **사용자 속성 매핑** 섹션, **디렉터리 속성** 필드, 유형 **이메일**. (**이메일 주소** 은(는)에 이미 채워져 있습니다. **Workfront 사용자 속성** 필드.)

1. (선택 사항) 활성화 **기본 SSO 공급자로 설정** 인증을 위해 인증되지 않은 사용자를 Workfront 로그인 화면이 아닌 id 공급자 로그인 화면으로 보냅니다. 시스템의 모든 사용자가 ID 공급자를 통해 Workfront에 액세스하는 경우에만 이 옵션을 활성화하는 것이 좋습니다.
1. 다음 항목 선택 **사용** 확인란. 이 작업을 수행하기 전에 시스템의 사용자가 새 로그인 환경을 알고 있는지 확인하여 Workfront 시스템에 대한 액세스 권한을 잃지 않도록 하십시오.
1. 클릭 **연결 테스트**.\
   연결에 성공했다는 메시지가 표시됩니다.

1. **저장**&#x200B;을 클릭합니다.

## 다른 ID 공급자 사용

Okta 이외의 ID 공급자(예: Ping 또는 Centrify)를 사용하는 경우 Workfront 메타데이터를 ID 공급자에게 다시 업로드해야 합니다.
