---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: ADFS를 사용하여 SAML 2.0으로 Adobe Workfront 구성
description: SAML 2.0을 사용하여 Workfront에 대한 인증을 활성화할 수 있습니다.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 0%

---

# ADFS를 사용하여 SAML 2.0으로 Adobe Workfront 구성

{{important-admin-console-onboard}}

Adobe Workfront 관리자는 ADFS(Active Directory Federation Services)를 사용하는 동안 단일 사인온용 Workfront을 SAML(Security Assertion Markup Language) 2.0 솔루션과 통합할 수 있습니다.

이 안내서에서는 자동 프로비저닝 또는 속성 매핑 없이 ADFS를 설정하는 데 중점을 둡니다. 자동 프로비전을 설정하기 전에 설정을 완료하고 테스트하는 것이 좋습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## SAML 2.0을 사용하여 Workfront에 인증 활성화

SAML 2.0을 사용하여 Workfront 웹 애플리케이션 및 Workfront 모바일 애플리케이션에 대한 인증을 활성화하려면 다음 섹션을 완료하십시오.

* [Workfront SSO 메타데이터 파일 검색](#retrieve-the-workfront-sso-metadata-file)
* [신뢰 당사자 트러스트 구성](#configure-relying-party-trusts)
* [클레임 규칙 구성](#configure-claim-rules)
* [메타데이터 파일을 업로드하고 연결을 테스트합니다](#upload-the-metadata-file-and-test-the-connection)

### Workfront SSO 메타데이터 파일 검색 {#retrieve-the-workfront-sso-metadata-file}

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).
1. 왼쪽 패널에서 **시스템** > **단일 사인온(SSO)**.
1. 에서 **유형** 드롭다운 메뉴에서 **SAML 2.0** 추가 정보 및 옵션을 표시합니다.
1. 다음에 표시되는 URL을 복사합니다 **메타데이터 URL**.
1. 다음 섹션으로 계속 진행합니다. [신뢰 당사자 트러스트 구성](#configure-relying-party-trusts).

### 신뢰 당사자 트러스트 구성 {#configure-relying-party-trusts}

1. 를 엽니다. **ADFS 관리자** windows server 2008 R2 사용(버전은 다를 수 있음).
1. 이동 **시작.**
1. 클릭 **관리 도구.**
1. 클릭 **ADFS 2.0 관리.**
1. 선택 **ADFS** 확장 **신뢰 관계**.
1. 마우스 오른쪽 단추 클릭 **신뢰 당사자 트러스트**&#x200B;를 선택하고 을 선택합니다. **신뢰 당사자 트러스트 추가** 신뢰 당사자 트러스트 추가 마법사를 시작하려면 다음을 수행합니다.
1. 에서 **시작 페이지**, 선택 **시작**.
1. 에서 **날짜 소스 선택** 섹션에서 Workfront의 메타데이터 URL을 붙여넣습니다.
1. 클릭 **다음**.
1. 클릭 **확인** 경고 메시지를 확인합니다.
1. 에서 **표시 이름 지정** 섹션, 추가 **표시 이름** 및 **참고** 트러스트를 구분하려면 **다음**.
1. 선택 **모든 사용자가 이 신뢰 당사자에 액세스할 수 있도록 허용** (또는 **없음** 나중에 구성하려는 경우).
1. 클릭 **다음**.

   이렇게 하면 로 이동합니다 **신뢰 추가 준비 완료** 섹션을 참조하십시오.

1. 다음 섹션으로 계속하십시오 [클레임 규칙 구성](#configure-claim-rules).

### 클레임 규칙 구성 {#configure-claim-rules}

1. 클릭 **다음** 에서 **신뢰 추가 준비 완료** 섹션을 클릭한 다음 **클레임 규칙 편집 대화 상자를 엽니다.** 옵션이 선택되어 있습니다.

   이를 통해 향후 단계에서 클레임 규칙을 편집할 수 있습니다.

1. Click **Close**.
1. 클릭 **규칙 추가.**
1. 선택 **LDAP 속성을 청구로 전송**.
1. 클릭 **다음** 를 **클레임 규칙 구성** 단계.
1. 클레임 규칙을 구성하려면 다음 최소 요구 사항을 지정합니다. (이 작업은 **페더레이션 ID** 를 사용 중인지 확인합니다.


   <table >                
      <tbody>
            <tr>
               <td>클레임 규칙 이름
               </td>
               <td>클레임 규칙의 이름을 지정합니다. 예: "Workfront"</td>
            </tr>
            <tr>
               <td>속성 저장소</td>
               <td >선택 <b>Active Directory</b> 를 클릭합니다.</td>
            </tr>
            <tr>
               <td>LDAP 속성</td>
               <td>이는 모든 유형의 속성이 될 수 있습니다. 을 사용하는 것이 좋습니다 <b>SAM-Account-Name</b> 이 속성을 사용합니다.</td>
            </tr>
            <tr>
               <td>발신 클레임 유형</td>
               <td>선택해야 합니다 <b>이름 ID</b> 보내는 클레임 유형으로</td>
            </tr>
      </tbody>
   </table>

1. (선택 사항) 자동 프로비전을 설정하려면 LDAP 속성 및 발신 클레임 유형 모두에 다음과 같은 추가 클레임을 추가합니다.

   * 지정된 이름
   * 성
   * 전자 메일 주소

1. 클릭 **완료**&#x200B;를 클릭한 다음 **확인** 다음 화면에 표시됩니다.
1. 새 항목을 마우스 오른쪽 단추로 클릭합니다. **신뢰 당사자 트러스트**&#x200B;를 선택하고 을 선택합니다. **속성**.
1. 을(를) 선택합니다&#x200B;**고급 탭**. 및 아래 **보안 해시 알고리즘** sha-1 또는 SHA-256을 선택합니다.

   >[!NOTE]
   >
   >보안 해시 알고리즘에서 선택하는 옵션은 설정 > 시스템 > SSO(Single Sign-ON) 아래의 Workfront의 보안 해시 알고리즘 필드와 일치해야 합니다.

1. 다음 섹션으로 계속하십시오 [메타데이터 파일을 업로드하고 연결을 테스트합니다](#upload-the-metadata-file-and-test-the-connection).

### 메타데이터 파일을 업로드하고 연결을 테스트합니다 {#upload-the-metadata-file-and-test-the-connection}

1. 브라우저를 열고 다음 위치로 이동합니다. `https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml` .

   메타데이터 파일 FederationMetadata.xml을 다운로드해야 합니다.

1. 클릭 **파일 선택** 아래에 **ID 공급자 메타데이터에서 필드 채우기**, 을(를) 선택하고 을(를) 선택합니다. **FederationMetadata.xml** 파일.

1. (선택 사항) 인증서 정보가 메타데이터 파일로 채워지지 않은 경우 파일을 별도로 업로드할 수 있습니다. 선택 **파일 선택** 에서 **인증서** 섹션을 참조하십시오.

1. 클릭 **연결 테스트**. 올바르게 설정하면 아래 표시된 페이지와 유사한 페이지가 표시됩니다.

   ![](assets/success-saml-2.png)

   >[!NOTE]
   >
   >속성 매핑을 설정하려면 테스트 연결의 속성을 디렉토리 속성으로 복사해야 합니다. 자세한 내용은 사용자 속성 매핑을 참조하십시오.

1. 선택 **관리자 면제** Workfront 관리자가 bypass url이 있는 Workfront 자격 증명을 사용하여 로그인할 수 있도록 허용.

   을 가리키는 책갈피 `<yourdomain>`.my.workfront.com/login 리디렉션을 건너뜁니다.

1. 을(를) 선택합니다 **활성화** 상자를 사용하여 구성을 활성화합니다.
1. **저장**&#x200B;을 클릭합니다.

## SSO용 사용자 업데이트 정보

이 안내서에 따르면, **SSO 사용자 이름** 그들의 **Active Directory 사용자 이름**.

Workfront 관리자는 SSO용 사용자를 대량 업데이트할 수 있습니다. SSO용 사용자 업데이트에 대한 자세한 내용은 [단일 사인온용 사용자 업데이트](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md).

Workfront 관리자는 사용자의 프로필을 편집하고 페더레이션 ID 필드를 수동으로 할당할 수도 있습니다. 사용자 편집에 대한 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>[!NOTE]
>
>페더레이션 ID를 포함하도록 사용자의 프로필을 편집할 때 선택 **SAML 2.0 인증만 허용** url 무시(`<yourdomain>`.my.workfront.com/login).
