---
title: Workfront OAuth2에서 Adobe Developer Console으로 마이그레이션
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Workfront의 기존 사용자 지정 OAuth2 애플리케이션 서비스가 사용 중단됩니다. 변경 사항, 영향을 받는 사용자 및 사용자 정의 통합을 Adobe Developer Console으로 마이그레이션하는 방법에 대해 알아봅니다.
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
source-git-commit: db7e6a6fa0c5fc5332213c388d9b4db3a5c59f53
workflow-type: tm+mt
source-wordcount: '1473'
ht-degree: 1%

---

# Workfront OAuth2에서 Adobe Developer Console으로 마이그레이션

Workfront의 이전 사용자 지정 OAuth2 애플리케이션 서비스(**설정** > **시스템** > **OAuth2**&#x200B;에서 설정한 통합)가 중단됩니다. 앞으로 Workfront에 대해 인증하는 모든 사용자 지정 통합은 대신 Adobe Developer Console(developer.adobe.com) 인증 흐름을 사용해야 합니다.

이 변경 사항은 현재 Workfront에서 발급한 OAuth2 클라이언트 ID 및 암호를 사용하여 인증하는 사용자 지정 통합, 스크립트 또는 타사 도구에 영향을 줍니다. Workfront에 로그인하는 방식에는 영향을 주지 않으며 Adobe에서 개별적으로 마이그레이션하는 패키지화된 Microsoft Teams 또는 Slack 통합과 같은 Adobe 관리 표준 통합에는 영향을 주지 않습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 액세스 수준 구성</td> 
   <td><p>시스템 관리자</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Developer Console 권한</td> 
   <td><p>Workfront용 Adobe Developer Console에 액세스하려면 전체 IMS 조직 관리자 권한이 필요합니다. 전체 Workfront 조직과 그 아래의 모든 제품을 관리하기 때문에 Adobe 제품 관리자 역할보다 더 폭넓습니다.</p></td> 
  </tr> 
 </tbody> 
</table>

+++

## 주요 일자

| 일자 | 마일스톤 | 어떤 의미입니까? |
|---|---|---|
| 2026년 11월 1일 | 새 앱 만들기 비활성화됨 | Workfront에서는 더 이상 새 사용자 지정 OAuth2 애플리케이션을 만들 수 없습니다. 기존 애플리케이션은 계속 작동합니다. |
| 2027년 2월 1일 | 레거시 서비스가 중단됨 | 기존 사용자 지정 OAuth2 애플리케이션은 완전히 작동하지 않습니다. Adobe Developer Console으로 마이그레이션되지 않은 모든 통합은 이 시점에서 Workfront API에 액세스할 수 없습니다. |

>[!IMPORTANT]
>
>통합이 중단 없이 계속 실행되므로 2027년 2월 1일 하드 마감시한에 대해 마이그레이션하지 않을 수 있도록 2026년 11월 1일 전에 마이그레이션을 계획하고 완료하는 것이 좋습니다.

## 영향을 받는 조직

조직은 Workfront의 이전 OAuth2 설정 화면을 통해 발급된 사용자 지정 OAuth2 클라이언트 ID 및 암호를 사용하여 Workfront에 연결하는 통합, 스크립트 또는 도구가 있는 경우 이 변경의 영향을 받습니다. 일반적인 예는 다음과 같습니다.

* 엔지니어링 팀이 Workfront API에 대해 유지 관리하는 사용자 지정 통합.
* Workfront 발급 클라이언트 ID로 구성된 서드파티 또는 파트너가 빌드한 커넥터. 통합 인증 방법을 모를 경우 공급업체에 확인하는 것이 좋습니다.
* Workfront API를 직접 호출하는 내부 자동화, 보고 또는 데이터 동기화 스크립트입니다.

조직에 이러한 항목이 있는지 모를 경우 Workfront 관리자가 **설정** > **시스템** > **OAuth2** 아래의 OAuth2 애플리케이션 목록을 확인하여 현재 등록된 항목을 확인할 수 있습니다. 자세한 내용은 [사용자 지정 OAuth2 응용 프로그램 보기 및 관리](/help/quicksilver/administration-and-setup/configure-integrations/manage-custom-oauth2-apps.md)를 참조하십시오.

## Adobe Developer Console 인증 유형 이해

Adobe Developer Console은 두 가지 이상의 인증 방법을 지원합니다. 통합 작동 방식과 일치하는 유형을 선택할 수 있습니다.

* **서버 간 인증**: 최종 사용자 없이 조직을 대신하여 Adobe API를 호출하는 백엔드에서 실행 중인 응용 프로그램입니다. 이는 클라이언트 ID 및 암호로 작동한 기존 Workfront OAuth2 패턴과 가장 일치하는 것으로, 가장 사용자 지정 Workfront 통합, 스크립트 및 자동화가 사용해야 하는 유형입니다.
* **사용자 인증**: 응용 프로그램에서 데이터를 보거나 편집하기 전에 Adobe 사용자가 로그인하고 동의해야 하는 경우입니다. 통합에서 조직 전체가 아니라 로그인한 특정 Workfront 사용자를 대신하여 활동해야 하는 경우 이 유형을 대신 사용하십시오.

  사용자 인증을 선택하는 경우 애플리케이션 아키텍처에 따라 세 가지 추가 옵션이 있습니다.

  * **OAuth 웹 앱**: 프론트엔드 UI 및 백엔드 서버가 있는 응용 프로그램용. 서버는 클라이언트 암호를 안전하게 저장하고 토큰을 가져옵니다.
  * **OAuth 단일 페이지 앱**: 백 엔드 서버가 없는 브라우저 전용 웹 애플리케이션용. 웹 앱 자체는 토큰을 가져옵니다.
  * **OAuth 네이티브 앱**: 장치에서 기본적으로 실행되고 백엔드 서버가 없는 모바일 또는 데스크톱 응용 프로그램용. 기본 앱은 토큰을 가져옵니다.

기존 OAuth2 서비스에서 백엔드 통합, 스크립트 또는 자동화를 마이그레이션하는 대부분의 조직은 서버 간 인증을 원합니다.

## 기능 비교: 이전 OAuth2와 Adobe Developer Console

기존 Workfront OAuth2 서비스(**설정** > **시스템** > **OAuth2 응용 프로그램**&#x200B;의 개수)는 Workfront 인스턴스당 10개의 OAuth2 응용 프로그램 제한으로 세 가지 응용 프로그램 유형을 제공합니다. 다음은 이러한 측면을 Adobe Developer Console과 비교하는 방법입니다.

| 기존 Workfront 유형 | 플로우/인증 방법 | Developer Console 동등 | 맞춤 |
|---|---|---|---|
| 시스템 간 애플리케이션(CLI, 데몬, 백엔드 스크립트) | 공개/개인 키 쌍이 있는 JWT | 서버 간 인증 | 최종 사용자를 포함하지 않는 것과 동일한 목적이지만 메커니즘이 변경됩니다. 레거시 흐름은 공개/개인 키 쌍 및 JWT를 사용하는 반면, 서버 간 흐름은 OAuth 클라이언트 자격 증명 부여와 함께 클라이언트 ID 및 클라이언트 암호를 사용합니다. 이는 드롭인 자격 증명 교환이 아닙니다. 자격 증명 값뿐만 아니라 통합의 인증 코드도 변경해야 합니다. 자세한 내용은 [사용자 지정 OAuth 2 애플리케이션에 JWT 흐름 사용](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md)을 참조하십시오. |
| 웹 애플리케이션(서버측 앱: Go, Java, .NET, Node, PHP) | OAuth 2.0 인증 코드 흐름 | OAuth 웹 앱(사용자 인증 아래) | 가장 가까운 1:1 일치. 백엔드 서버가 클라이언트 암호를 저장하는 동일한 흐름 및 동일한 기본 모양이 있습니다. 자세한 내용은 [사용자 지정 OAuth 2 애플리케이션에 대한 인증 코드 흐름](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md)을 참조하십시오. |
| 단일 페이지 웹 애플리케이션(JS, Angular, React, Vue) | 클라이언트 암호가 없는 PKCE의 인증 코드 흐름 | OAuth 단일 페이지 앱(사용자 인증 아래) | 가장 가까운 1:1 일치에 동일한 PKCE 기반 비밀 없는 흐름이 있습니다. 자세한 내용은 [OAuth 2 애플리케이션에 PKCE 흐름 사용](/help/quicksilver/wf-api/api/oauth-app-pkce-flow.md)을 참조하십시오. |
| (기존의 해당 항목 없음) | — | OAuth 네이티브 앱(사용자 인증 아래) | 이는 새로운 기능입니다. 기존 Workfront OAuth2에는 기본 모바일 또는 데스크탑 애플리케이션에 대한 전용 유형이 없습니다. |

<!--

>[!NOTE]
>
>A few legacy capabilities don't have a confirmed equivalent yet in Adobe Developer Console, and are being validated with the Developer Console team:
>
>* Per-app controls the legacy UI offers: refresh token rotation toggle, absolute vs. inactivity refresh token expiration, custom logo, privacy policy URL, and developer contact fields.
>* Whether Developer Console enforces a cap on credentials or projects similar to the legacy 10-app-per-instance limit.
>* Whether a JWT/key pair-based option remains available anywhere in Developer Console for Machine to Machine customers, or whether all such integrations must move to the client-secret-based Server-to-Server grant.

-->

## 마이그레이션 프로시저

### Workfront 시스템 관리자인 경우

>[!NOTE]
>
>Workfront 제품 관리자이지 조직 관리자가 아닌 경우 조직 관리자와 협력하여 이 마이그레이션을 완료하거나 마이그레이션을 만들도록 요청해야 합니다.

1. [developer.adobe.com](https://developer.adobe.com)에 로그인하고 새 프로젝트를 만듭니다. 프로젝트는 콘솔이 다양한 통합 또는 클라이언트 앱을 구성하는 방법입니다.
1. 프로젝트에서 API를 추가하고 **Adobe Workfront**&#x200B;을(를) 선택합니다. 이 API는 Experience Cloud 범주 아래에 있습니다. 계획, 워크플로우, 검토 및 승인을 포함한 모든 Workfront API는 이 단일 API를 공유합니다.
1. **서버 간** 인증 옵션을 선택한 다음 IMS 조직에 Workfront 인스턴스가 두 개 이상 있는 경우 올바른 인스턴스를 선택합니다.

   인증 유형 선택에 대한 지침은 이 문서의 [Adobe Developer Console 인증 유형 이해](#understand-adobe-developer-console-authentication-types)를 참조하십시오.
1. 프로젝트 페이지에서 새 OAuth 서버 간 자격 증명의 세부 사항을 열어 클라이언트 ID, 클라이언트 암호 및 액세스 토큰 생성에 필요한 정보를 찾습니다.
1. 이전 Workfront OAuth2 클라이언트 ID 및 암호 대신 이러한 새 자격 증명으로 인증하도록 통합, 스크립트 또는 도구를 업데이트합니다.
1. Workfront에서 액세스를 확인합니다. API 클라이언트를 만들면 Workfront 사용자 &quot;`techacct`&quot;(으)로 자동으로 추가됩니다. 기본적으로 액세스 권한이 제한된 기여자로 추가되지만, 다른 사용자의 경우와 마찬가지로 액세스 수준을 조정할 수 있습니다.
1. (선택 사항) `techacct` 사용자 관리자 권한을 부여하려면 Admin Console에서 관련 제품 프로필의 관리자로 기술 계정 이메일을 추가하십시오.
1. 통합을 처음부터 끝까지 테스트합니다.
1. 새 연결이 작동하는 것을 확인한 후 Workfront에서 이전 OAuth2 애플리케이션 항목을 폐기합니다.

전체 단계별 세부 정보 및 스크린샷은 Adobe의 Developer Console 설명서에서 [액세스 권한 얻기](https://developer.adobe.com/workfront-apis/guides/gaining_access/)를 참조하십시오.

### 시스템 관리자가 아닌 경우

Adobe Developer Console에서 새 자격 증명을 설정하려면 해당 액세스 수준이 필요하므로 마이그레이션을 완료하려면 조직의 IMS 조직 관리자에서 반복해야 합니다. 통합을 관리하거나 유지 관리하지만 조직의 IMS 조직 관리자가 누구인지 알고 있는 경우 다음 중 하나에 문의하십시오.

* Workfront 계정 팀
* 내부 IT 팀
* 엔지니어링 담당자

## 마이그레이션하지 않는 경우

2027년 2월 1일 이후에도 기존 OAuth2 클라이언트 ID/암호 패턴을 사용하는 통합은 Workfront API에 대해 인증할 수 없으며, 모든 종속 워크플로우, 동기화 또는 자동화에 실패합니다. 이 날짜 이후에 계획된 확장이 없으므로 통합보다 훨씬 앞서 마이그레이션하십시오.

## 자주 묻는 질문

**Slack 또는 Microsoft Teams과 같이 Adobe에서 제공하는 패키지 통합에 영향을 줍니까?**

아니요. Adobe에서 관리하는 글로벌 애플리케이션은 Adobe에서 직접 마이그레이션되므로 별도의 작업이 필요하지 않습니다.

**기존 통합이 2027년 2월 1일 전에 작동을 중지합니까?**

아니요. 기존 사용자 정의 OAuth2 애플리케이션은 2027년 2월 1일까지 정상적으로 작동합니다. 2026년 11월 1일부터 새로운 사용자 지정 OAuth2 애플리케이션을 만드는 기능만 영향을 받습니다.

**마이그레이션하는 데 비용이 듭니까?**

아니요. Adobe Developer Console을 통한 인증과 관련된 추가 비용은 없습니다.

**어디에서 도움을 받을 수 있습니까?**

특정 통합 또는 타임라인에 대한 질문이 있는 경우 Workfront 계정 팀에 문의하거나 지원 사례를 엽니다. 스크린샷이 포함된 공식적인 최신 설치 연습은 Adobe의 Developer Console 설명서에서 [액세스 권한 얻기](https://developer.adobe.com/workfront-apis/guides/gaining_access/)를 참조하십시오.
