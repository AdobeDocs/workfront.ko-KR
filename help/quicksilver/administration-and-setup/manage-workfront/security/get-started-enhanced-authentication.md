---
title: 향상된 인증 개요
description: 검색 및 왼쪽 탐색에서 숨김
hidefromtoc: true
hide: true
feature: System Setup and Administration
role: Admin
exl-id: bf3c6c6f-ddd5-42d0-9efe-b5eb94549f85
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 3%

---

# 향상된 인증 개요

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Adobe Workfront이 사용자 및 암호의 시스템 관리를 변경하고 있습니다. 이러한 변경 사항은 이라는 단계별 릴리스에서 롤아웃됩니다. **향상된 인증** 경험. 향상된 인증은 모든 Workfront 제품 및 서비스에서 보다 일관되고 안전한 로그인 환경을 사용자에게 제공합니다.

다음 표는 현재 및 향후 기능에 대한 세부 정보를 제공합니다.

>[!IMPORTANT]
>
>대부분의 고객은 현재 레거시 인증을 사용하고 있으며 일부는 향상된 인증 1.0을 사용하고 있습니다.
> 
>현재 사용 중인 인증 유형을 확인하려면 *your_domain*.my.workfront.com/login입니다. /auth/login으로 리디렉션되면 향상된 인증 1.0을 사용합니다.
> 
>https://login-a-xx.workfront.com/으로 리디렉션되는 경우 위치/플랫폼에 따라 &#39;xx&#39;가 미국(미국), EU(유럽) 또는 GCP(Google Cloud Platform)일 수 있으므로 향상된 인증 2.0을 사용합니다.
>
>모든 고객은 2021년 말까지 향상된 인증 2.0으로 전환할 예정입니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p><strong>기능</strong> </p> </th> 
   <th><strong>레거시 인증</strong> </th> 
   <th><strong>향상된 인증 1.0</strong> </th> 
   <th> <p>향상된 인증 2.0</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="3"> <p><strong>로그인 옵션</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>교육, 지원 등을 포함하여 모든 Workfront 제품 및 서비스에 사용할 단일 사용자 이름을 활성화합니다</p> </td> 
   <td>사용할 수 없음</td> 
   <td> <p>사용할 수 없음</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Workfront 인스턴스에서 동일한 이메일 주소 사용 허용</p> </td> 
   <td> <p>✓</p> <p>2019.3 릴리스에서 사용 가능</p> </td> 
   <td> <p>✓</p> <p>2019.3 릴리스에서 사용 가능</p> </td> 
   <td> <p>✓</p> <p>2019.3 릴리스에서 사용 가능</p> </td> 
  </tr> 
  <tr> 
   <td> <p>이메일 주소는 대소문자를 구분하지 않습니다.</p> </td> 
   <td> <p>✓</p> <p>2019.3 릴리스에서 사용 가능</p> </td> 
   <td> <p>✓</p> <p>주소가 대/소문자만 다른 경우 여러 사용자가 동일한 이메일 주소를 가질 수 없습니다. </p> </td> 
   <td> <p>✓</p> <p>주소가 대/소문자만 다른 경우 여러 사용자가 동일한 이메일 주소를 가질 수 없습니다. </p> <p>Workfront 관리자는 2019년 말에 중복 이메일 주소 수정을 시작하라는 알림을 받게 됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>암호 관리 옵션</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Workfront 관리자로서 사용자에 대한 암호 재설정 이메일 삽입</p> </td> 
   <td> <p>사용할 수 없음 </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Workfront 관리자로서 사용자에 대한 임시 암호 설정</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>계획되지 않음</p> <p>이 기능은 보안 모범 사례가 아닙니다.</p> </td> 
   <td> <p>계획되지 않음</p> <p>이 기능은 보안 모범 사례가 아닙니다.</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>암호 정책 요구 사항</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>일정 기간 후 사용자가 암호를 재설정해야 함</p> </td> 
   <td>✓</td> 
   <td> <p>계획되지 않음</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>사용자가 이전 암호를 사용하지 못하도록 제한 </p> </td> 
   <td>✓</td> 
   <td>계획되지 않음 </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>잘못된 암호 입력 시도에 대한 보호 </p> </td> 
   <td> <p>✓ </p> <p>잘못된 암호 입력을 5회 시도하면 계정을 잠급니다. Workfront 관리자가 잠금 구성 후 필요한 대기 시간</p> </td> 
   <td> <p>✓</p> <p>업계 모범 사례를 기반으로 하는 각각의 연속적인 잘못된 암호 후에는 대기 시간이 기하급수적으로 증가합니다. 필요한 시간은 Workfront 관리자가 구성할 수 없습니다</p> </td> 
   <td> <p>✓</p> <p>다양한 의심스러운 행동을 사전에 차단하는 잠금 알고리즘을 사용합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>소문자, 대문자, 숫자 및 특수 문자를 혼용해야 합니다.</p> </td> 
   <td>✓</td> 
   <td> <p>✓ </p> <p>특정 요구 사항 선택의 유연성 향상</p> </td> 
   <td> <p>✓</p> <p> 
     </p> </td> 
  </tr> 
  <tr> 
   <td> <p>최소 암호 길이 설정 </p> </td> 
   <td> 사용할 수 없음 </td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Restrict users from using more than 2 identical characters in a row</td> 
    <td>Not available</td> 
    <td>Not available</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
  <tr> 
   <td colspan="3"> <p><strong>SSO(Single Sign-On) 프로토콜 지원</strong></p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Active Directory 및 LDAP 프로토콜과 호환되는 SSO 통합 지원</p> </td> 
   <td> ✓ </td> 
   <td> <p> 더 이상 사용되지 않음</p> <p>Active Directory, Azure 및 LDAP 시스템은 SAML 2.0을 사용해야 합니다.</p> </td> 
   <td> <p>더 이상 사용되지 않음</p> <p>Active Directory, Azure 및 LDAP 시스템은 암호화된 SAML 2.0 또는 OpenID Connect로 구성할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>SAML 2.0과 호환되는 SSO 프로토콜 지원 </p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Open ID Connect 프로토콜 지원</p> </td> 
   <td> <p>사용할 수 없음</p> </td> 
   <td> <p>사용할 수 없음</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p> 항상 ID 공급자 로그인 페이지로 리디렉션하도록 Workfront 로그인 페이지를 구성합니다 </p> </td> 
   <td> 기본적으로 활성화되며 비활성화될 수 없음</td> 
   <td> <p>✓</p> <p>Workfront 관리자는 id 공급자 로그인 페이지로 리디렉션하도록 로그인 페이지를 구성하거나 로그인 단추 또는 단추를 구성할 수 있습니다.</p> </td> 
   <td> <p>✓</p> <p> Workfront 관리자는 id 공급자 로그인 페이지로 리디렉션하도록 로그인 페이지를 구성하거나 로그인 단추 또는 단추를 구성할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>각 인스턴스가 여러 SSO 공급자를 사용하도록 허용</p> </td> 
   <td> <p>해당 없음</p> </td> 
   <td> <p>계획되지 않음</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>환경 지원</strong> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>미리보기 환경을 위한 단일 사용자 이름 및 암호</p> </td> 
   <td> <p>사용할 수 없음</p> </td> 
   <td> <p>사용할 수 없음</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>샌드박스 환경을 위한 단일 사용자 이름 및 암호</p> </td> 
   <td> <p>사용할 수 없음</p> </td> 
   <td> <p>사용할 수 없음</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr> 
    <td> <p>Available for Production environments</p> </td> 
    <td>✓</td> 
    <td> ✓&nbsp;</td> 
    <td> <p>✓</p> </td> 
   </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> Available for Preview and Sandbox environments&nbsp;</td> 
    <td> ✓&nbsp;</td> 
    <td> ✓</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>
