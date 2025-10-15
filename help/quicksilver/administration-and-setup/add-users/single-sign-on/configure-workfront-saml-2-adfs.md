---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: ADFS를 사용하여 SAML 2.0으로 Adobe Workfront 구성
description: SAML 2.0을 사용하여 Workfront에 대한 인증을 활성화할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: 75fea812b4574191522af4721a013b57aa5d609f
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# ADFS를 사용하여 SAML 2.0으로 Adobe Workfront 구성

{{important-admin-console-onboard}}

Adobe Workfront 관리자는 ADFS(Active Directory Federation Services)를 사용하는 동안 단일 사인온을 위해 Workfront을 SAML(Security Assertion Markup Language) 2.0 솔루션과 통합할 수 있습니다.

이 안내서는 자동 프로비저닝 또는 속성 매핑 없이 ADFS를 설정하는 데 중점을 둡니다. 자동 프로비저닝을 설정하기 전에 설정을 완료하고 테스트하는 것이 좋습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>표준</p><p>플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## SAML 2.0으로 Workfront 인증 활성화

SAML 2.0을 사용하여 Workfront 웹 애플리케이션 및 Workfront 모바일 애플리케이션에 대한 인증을 활성화하려면 다음 섹션을 완료하십시오.

* [Workfront SSO 메타데이터 파일 검색](#retrieve-the-workfront-sso-metadata-file)
* [신뢰 당사자 트러스트 구성](#configure-relying-party-trusts)
* [클레임 규칙 구성](#configure-claim-rules)
* [메타데이터 파일 업로드 및 연결 테스트](#upload-the-metadata-file-and-test-the-connection)

### Workfront SSO 메타데이터 파일 검색 {#retrieve-the-workfront-sso-metadata-file}

{{step-1-to-setup}}

1. 왼쪽 패널에서 **시스템** > **SSO(Single Sign-On)**&#x200B;를 클릭합니다.
1. **Type** 드롭다운 메뉴에서 **SAML 2.0**&#x200B;을(를) 클릭하여 추가 정보 및 옵션을 표시합니다.
1. **메타데이터 URL** 뒤에 표시되는 URL을 복사합니다.
1. [신뢰 당사자 트러스트 구성](#configure-relying-party-trusts) 섹션을 계속합니다.

### 신뢰 당사자 트러스트 구성 {#configure-relying-party-trusts}

1. Windows server 2008 R2를 사용하여 **ADFS 관리자**&#x200B;를 엽니다(버전은 다를 수 있음).
1. **시작**(으)로 이동
1. **관리 도구**&#x200B;를 클릭합니다.
1. **ADFS 2.0 관리를 클릭합니다.**
1. **ADFS**&#x200B;를 선택하고 **트러스트 관계**&#x200B;를 확장합니다.
1. **신뢰 당사자 트러스트**&#x200B;를 마우스 오른쪽 단추로 클릭한 다음 **신뢰 당사자 트러스트 추가**&#x200B;를 선택하여 신뢰 당사자 트러스트 추가 마법사를 시작합니다.
1. **시작 페이지**&#x200B;에서 **시작**&#x200B;을 선택합니다.
1. **날짜 Source 선택** 섹션에서 Workfront의 메타데이터 URL을 붙여 넣습니다.
1. **다음**&#x200B;을 클릭합니다.
1. 경고 메시지를 확인하려면 **확인**&#x200B;을 클릭하세요.
1. **표시 이름 지정** 섹션에서 **표시 이름** 및 **메모**&#x200B;를 추가하여 트러스트를 구분한 후 **다음**&#x200B;을 클릭합니다.
1. **모든 사용자가 이 신뢰 당사자에 액세스할 수 있도록 허용**(또는 나중에 구성하려면 **없음**)을 선택합니다.
1. **다음**&#x200B;을 클릭합니다.

   **트러스트를 추가할 준비가 되었습니다** 섹션으로 이동합니다.

1. [클레임 규칙 구성](#configure-claim-rules) 섹션을 계속합니다.

### 클레임 규칙 구성 {#configure-claim-rules}

1. **트러스트를 추가할 준비가 되었습니다** 섹션에서 **다음**&#x200B;을(를) 클릭한 다음 **클레임 규칙 편집 대화 상자 열기** 옵션이 선택되어 있는지 확인하십시오.

   이 경우 이후 단계에서 클레임 규칙을 편집할 수 있습니다.

1. Click **Close**.
1. **규칙 추가**&#x200B;를 클릭합니다
1. **LDAP 특성을 클레임으로 보내기**&#x200B;를 선택합니다.
1. **다음**&#x200B;을 클릭하여 **클레임 규칙 구성** 단계를 표시합니다.
1. 클레임 규칙을 구성하려면 다음 최소 요구 사항을 지정하십시오. (이 요구 사항은 사용자 설정의 **Federation ID**&#x200B;에서 시작되며 로그인하는 사용자를 구별하는 데 사용됩니다.)


   <table >                
      <tbody>
            <tr>
               <td>클레임 규칙 이름
               </td>
               <td>클레임 규칙의 이름을 지정합니다. 예를 들어 "Workfront"입니다.</td>
            </tr>
            <tr>
               <td>속성 저장소</td>
               <td >드롭다운 메뉴에서 <b>Active Directory</b>을(를) 선택합니다.</td>
            </tr>
            <tr>
               <td>LDAP 속성</td>
               <td>모든 유형의 속성일 수 있습니다. 이 특성에는 <b>SAM-Account-Name</b>을 사용하는 것이 좋습니다.</td>
            </tr>
            <tr>
               <td>나가는 클레임 유형</td>
               <td><b>이름 ID</b>을(를) 보내는 클레임 유형으로 선택해야 합니다.</td>
            </tr>
      </tbody>
   </table>

1. (선택 사항) 자동 프로비저닝을 설정하려면 LDAP 속성과 발신 클레임 유형 모두에 다음 추가 클레임을 추가합니다.

   * 이름
   * 성
   * 이메일 주소

1. **마침**&#x200B;을 클릭한 다음 다음 다음 화면에서 **확인**&#x200B;을 클릭합니다.
1. 새 **신뢰 당사자 트러스트**&#x200B;를 마우스 오른쪽 단추로 클릭한 다음 **속성**&#x200B;을 선택합니다.
1. **고급 탭**&#x200B;을 선택합니다. **보안 해시 알고리즘**&#x200B;에서 SHA-1 또는 SHA-256을 선택합니다.

   >[!NOTE]
   >
   >보안 해시 알고리즘에서 선택하는 옵션은 설정 > 시스템 > SSO(Single Sign-On) 아래의 Workfront에 있는 보안 해시 알고리즘 필드와 일치해야 합니다.

1. 다음 섹션 [메타데이터 파일을 업로드하고 연결을 테스트합니다](#upload-the-metadata-file-and-test-the-connection).

### 메타데이터 파일 업로드 및 연결 테스트 {#upload-the-metadata-file-and-test-the-connection}

1. 브라우저를 열고 `https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml`(으)로 이동합니다.

   메타데이터 파일 FederationMetadata.xml 파일을 다운로드해야 합니다.

1. **ID 공급자 메타데이터에서 필드 채우기**&#x200B;에서 **파일 선택**&#x200B;을 클릭하고 **FederationMetadata.xml** 파일을 선택합니다.

1. (선택 사항) 인증서 정보가 메타데이터 파일로 채워지지 않은 경우 파일을 별도로 업로드할 수 있습니다. **인증서** 섹션에서 **파일 선택**&#x200B;을 선택합니다.

1. **연결 테스트**&#x200B;를 클릭합니다. 올바르게 설정되면 아래 표시된 페이지와 유사한 페이지가 표시됩니다.

   ![SAML 2 성공 메시지](assets/success-saml-2.png)

   >[!NOTE]
   >
   >속성 매핑을 설정하려면 연결 테스트의 속성을 디렉터리 속성으로 복사해야 합니다. 자세한 내용은 사용자 속성 매핑을 참조하십시오.

1. Workfront 관리자가 우회 URL을 사용하여 Workfront 자격 증명을 사용하여 로그인할 수 있도록 하려면 **관리자 예외**&#x200B;을(를) 선택하십시오.

   `<yourdomain>`.my.workfront.com/login을(를) 가리키는 책갈피는 리디렉션을 무시합니다.

1. 구성을 사용하려면 **사용** 상자를 선택하십시오.
1. **저장**&#x200B;을 클릭합니다.

## SSO를 위해 사용자 업데이트 기본 정보

이 안내서에 따라 **SSO 사용자 이름**&#x200B;은(는) **Active Directory 사용자 이름**&#x200B;이 됩니다.

Workfront 관리자는 SSO를 위해 사용자를 일괄 업데이트할 수 있습니다. SSO용 사용자 업데이트에 대한 자세한 내용은 [SSO(Single Sign-On)용 사용자 업데이트](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)를 참조하십시오.

Workfront 관리자는 사용자의 프로필을 편집하고 페더레이션 ID 필드를 완성하는 페더레이션 ID를 수동으로 할당할 수도 있습니다. 사용자 편집에 대한 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하세요.

>[!NOTE]
>
>Federation ID를 포함하도록 사용자 프로필을 편집할 때 **SAML 2.0 인증만 허용**&#x200B;을 선택하면 우회 URL(`<yourdomain>`.my.workfront.com/login)을 사용하여 Workfront에 로그인할 수 있는 기능이 제거됩니다.
