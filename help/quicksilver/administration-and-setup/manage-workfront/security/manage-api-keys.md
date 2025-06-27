---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: API 키 관리
description: API 보안 취약점을 최소화하기 위해 Adobe Workfront 관리자는 애플리케이션이 사용자를 대신하여 Workfront에 액세스할 수 있도록 하는 데 사용되는 API 키를 관리할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
source-git-commit: 8934c3f5681c09c00769442900013844ee7a80ef
workflow-type: tm+mt
source-wordcount: '1336'
ht-degree: 2%

---

# API 키 관리

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

API 보안 취약점을 최소화하기 위해 Adobe Workfront 관리자는 애플리케이션이 사용자를 대신하여 Workfront에 액세스할 수 있도록 하는 데 사용되는 API 키를 관리할 수 있습니다.

현재 관리자 API 키를 재설정 또는 제거하고, 만료되도록 API 키를 구성하고, 모든 사용자에 대한 API 키를 제거할 수 있습니다.

Workfront API를 활용하는 애플리케이션의 예는 다음과 같습니다.

* Dropbox, Google 드라이브 및 Workfront DAM과 같은 문서 통합
* Workfront 모바일 애플리케이션

>[!IMPORTANT]
>
>API 키를 재설정하거나 제거할 때 Workfront API를 활용하고 이 API 키를 통해 Workfront에 대해 인증하는 모든 애플리케이션은 Workfront에 다시 액세스하도록 다시 구성해야 합니다.

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

## Workfront API 키

Workfront의 각 사용자에게는 고유한 API 키가 있습니다. 이 키는 사용자가 Workfront API를 활용하는 통합(예: Workfront 모바일 앱 또는 문서 통합)에 액세스할 때 사용자별로 생성됩니다.

>[!NOTE]
>
> 프로덕션 환경에서 생성하는 API 키는 주별 새로 고침 중에 미리보기 환경에 복사됩니다. 미리보기 환경에서 생성하는 모든 API 키는 주별 새로 고침 중에 프로덕션 API 키로 덮어쓰여집니다.

Workfront 관리자에게도 고유한 API 키가 있습니다. 애플리케이션이 관리자 API 키를 사용하여 Workfront에 액세스하면 애플리케이션이 Workfront에 대한 관리자 액세스 권한을 갖습니다.

## 관리자 API 키 관리

관리자 사용자 계정에 대한 API 키를 생성, 재설정 또는 제거할 수 있습니다.

>[!NOTE]
>
>API를 통해 API 키를 생성할 수도 있습니다. 자세한 내용은 [이벤트 구독 API](../../../wf-api/general/event-subs-api.md)의 [이벤트 구독 API](../../../wf-api/general/event-subs-api.md) 섹션을 참조하십시오.

{{step-1-to-setup}}

1. **시스템 >** **고객 정보**&#x200B;를 클릭합니다.
1. (조건부) 다음 작업 중 하나를 수행합니다.

   API 키를 생성하려면: **API 키 설정** 섹션에서 **API 키 생성**&#x200B;을 클릭하세요.

   또는\
   API 키를 다시 설정하려면 **API 키 설정** 섹션에서 **다시 설정**&#x200B;을 클릭한 다음 **다시 설정**&#x200B;을 클릭합니다.

   또는

   API 키를 제거하려면: **API 키 설정** 섹션에서 **제거**&#x200B;를 클릭한 다음 **제거**&#x200B;를 클릭합니다.

## 관리자가 아닌 사용자를 위한 API 키 생성

Workfront 관리자 이외의 역할의 사용자에 대한 API 키를 생성하고 관리할 수 있습니다.

>[!NOTE]
>
>조직의 Workfront 인스턴스가 Adobe IMS를 사용하여 활성화된 경우 사용할 수 없습니다. 자세한 내용은 네트워크 또는 IT 관리자에게 문의하십시오.

1. (조건부) 조직에서 SSO(Single Sign-On) 액세스 관리를 사용하는 경우, SSO 인증을 요구하는 옵션을 일시적으로 비활성화하십시오.

   {{step-1-to-setup}}

   1. **시스템**&#x200B;을 확장한 다음 **SSO(Single Sign-On)**&#x200B;을 클릭합니다.
   1. **유형** 필드에서 조직에서 사용하는 SSO 유형을 선택합니다.
   1. 유형을 선택한 상태에서 아래로 스크롤하여 **활성화** 확인란의 선택을 취소합니다.
      ![SSO 사용](assets/sysadmin-security-sso-disable-31620-350x320.png)
   1. **저장**&#x200B;을 클릭합니다.


1. 브라우저의 주소 표시줄에 다음 API 호출을 입력합니다.

   `<domain>`.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&amp;username=**사용자 이름**&amp;password=**암호**&amp;method=PUT

   `<domain>`을(를) Workfront 도메인 이름으로 바꾸고 사용자 이름 및 암호를 사용자의 Workfront 자격 증명으로 바꿉니다.

1. (조건부) 1단계에서 SSO 인증을 사용하지 않도록 설정한 경우 SSO 인증을 요구하는 옵션을 활성화합니다.

   {{step-1-to-setup}}

   1. **시스템**&#x200B;을 확장한 다음 **SSO(Single Sign-On)**&#x200B;을 클릭합니다.

   1. **유형** 드롭다운 메뉴에서 SSO 메서드를 선택합니다.
   1. SSO 인증이 필요한 확인란을 선택하십시오.

## API 키가 만료되는 시기 구성

API 키가 시스템의 모든 사용자에 대해 만료되도록 구성할 수 있습니다. 사용자의 API 키가 만료되면 사용자는 Workfront API를 사용하여 Workfront에 액세스하는 모든 애플리케이션에 다시 인증해야 합니다. API 키가 만료되는 빈도를 변경할 수 있습니다. 사용자의 암호가 만료될 때 API 키가 만료되는지 여부를 구성할 수도 있습니다.

{{step-1-to-setup}}

1. **시스템** > **고객 정보**&#x200B;를 클릭합니다.
1. **API 키 설정** 영역의 **생성 후**, **API 키가**&#x200B;에 만료됩니다. 드롭다운 목록에서 API 키를 만료하려는 시간대를 선택합니다.

   이 옵션을 변경하면 변경한 시점부터 새 일정이 시작됩니다. 예를 들어 이 옵션을 *1개월*&#x200B;에서 *6개월*(으)로 변경하면 변경한 시점부터 6개월이 API 키가 만료됩니다.

   기본적으로 API 키는 매월 만료됩니다.

1. 사용자의 암호가 만료되는 시점에 만료되도록 API 키를 구성하려면 **사용자의 암호가 만료될 때 API 키 제거**&#x200B;를 사용하도록 설정하십시오.

   기본적으로 이 옵션은 활성화되어 있지 않습니다.

   사용자 암호를 만료되도록 구성하는 방법에 대한 자세한 내용은 [시스템 보안 환경 설정 구성](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)을 참조하십시오.

1. **저장**&#x200B;을 클릭합니다.

## 모든 사용자에 대한 API 키 제거

Workfront 시스템과 관련된 특정 보안 침해가 우려되는 경우 모든 사용자에 대해 동시에 API 키를 제거할 수 있습니다.

>[!IMPORTANT]
>
>모든 사용자에 대한 API 키를 제거하면 시스템의 모든 사용자에 대한 모든 API 키가 무효화됩니다. 이 작업을 수행하면 Workfront에서 새 API 키를 생성하고 모든 통합을 업데이트할 때까지 Workfront의 모든 통합이 실패합니다.

{{step-1-to-setup}}

1. **시스템**&#x200B;을 확장한 다음 **고객 정보**&#x200B;를 클릭합니다.

1. **API 키 설정** 영역에서 **모든 API 키 제거**&#x200B;를 클릭한 다음 **제거** **모두**&#x200B;를 클릭합니다.

## X.509 인증서로 API 로그인 제한

>[!IMPORTANT]
>
>이 섹션에 설명된 절차는 Adobe 비즈니스 플랫폼에 아직 온보딩되지 않은 조직에만 적용됩니다. 조직이 Workfront Business Platform에 온보딩된 경우 Workfront API를 통해 Adobe에 로그인할 수 없습니다.
>
>조직이 Adobe Business Platform에 온보딩되었는지 여부에 따라 달라지는 절차 목록은 [플랫폼 기반 관리 차이점(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)을 참조하십시오.

>[!NOTE]
>
>조직의 Workfront 인스턴스가 Adobe IMS를 사용하여 활성화된 경우 사용할 수 없습니다. 자세한 내용은 네트워크 또는 IT 관리자에게 문의하십시오.

서드파티 애플리케이션은 API를 통해 Workfront과 통신할 수 있습니다. Workfront 사이트의 보안을 강화하기 위해 X.509 인증서를 Workfront에 업로드하여 API 로그인 요청을 제한하도록 Workfront을 구성할 수 있습니다. 활성화되면 API를 통한 모든 로그인 요청에 사용자 이름 및 암호 외에 클라이언트 인증서가 포함되어야 합니다.

* [X.509 인증서 받기](#obtain-the-x-509-certificate)
* [인증서를 Workfront에 업로드](#upload-the-certificate-to-workfront)
* [API 로그인 호출이 제한되는지 확인](#verify-api-login-calls-are-restricted)

### X.509 인증서 받기 {#obtain-the-x-509-certificate}

신뢰할 수 있는 인증 기관(예: Verisign)에서 유효한 X.509 인증서를 가져와 워크스테이션의 임시 위치에 저장합니다.

### 인증서를 Workfront에 업로드 {#upload-the-certificate-to-workfront}

인증 기관에서 X.509 인증서를 얻은 후에는 Workfront에 업로드해야 합니다.

1. Adobe Workfront 오른쪽 상단의 **주 메뉴** 아이콘 ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **설정** ![톱니바퀴 설정 아이콘](assets/gear-icon-settings.png)을 클릭합니다.

1. **시스템**&#x200B;을 확장한 다음 **고객 정보**&#x200B;를 클릭합니다.

1. **API 키 설정** 영역에서 **API 로그인에 X.509 인증서 필요**&#x200B;를 선택합니다.
1. **인증서 변경**&#x200B;을 클릭합니다.
1. 워크스테이션에서 이전에 다운로드한 X.509 인증서로 이동하여 선택합니다.
1. (선택 사항) 인증서에 대한 다음 세부 정보를 보려면 인증서 이름 옆에 있는 **세부 정보 보기**&#x200B;를 클릭합니다.

   * 주체 일반 이름
   * 주체 조직
   * 주체 조직 단위
   * 발급자 일반 이름
   * 발급자 조직
   * 발급자 조직 유닛
   * 일련번호
   * 문제 일자
   * 만료일

1. **저장**&#x200B;을 클릭합니다.

### API 로그인 호출이 제한되는지 확인 {#verify-api-login-calls-are-restricted}

X.509 인증서가 필요하도록 Workfront 인스턴스를 구성하기 전에 올바른 사용자 이름 및 암호 매개 변수를 사용하여 `/login` 끝점에 대한 API 요청을 수행하십시오. sessionID가 포함된 200개의 응답을 받게 됩니다.

Workfront 인스턴스에서 고객 정보 페이지를 통해 X.509 인증서를 요구 사항으로 설정한 후 다른 로그인을 시도합니다. 이번에는 500 오류 응답을 받게 됩니다. 다음과 같은 메시지가 표시됩니다. &quot;Untrusted request. 시스템 관리자에게 연락하고 인증서를 첨부하십시오.&quot;

X.509 인증서가 필요한지 확인한 후, apiCertificate에 대한 추가 매개 변수를 인증서 값으로 설정하여 동일한 로그인 요청을 수행합니다. 이 작업이 올바르게 수행되면 유효한 sessionID가 포함된 200 응답이 수신됩니다.
