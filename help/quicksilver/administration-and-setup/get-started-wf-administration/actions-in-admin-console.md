---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 플랫폼 기반 관리의 차이점(Adobe Workfront/Adobe 비즈니스 플랫폼)
description: 조직이 Adobe 비즈니스 플랫폼에 온보딩된 경우 사용자는 Adobe 비즈니스 플랫폼을 사용하여 Adobe Workfront에 액세스합니다. 이는 이용자 관리가 대부분 Adobe Admin Console을 통해 이뤄지고, SSO(Single Sign-On)가 Workfront이 아닌 Adobe 비즈니스 플랫폼을 통해 이뤄지고 있다는 것을 의미한다. Adobe Workfront 관리자는 조직이 Adobe 비즈니스 플랫폼에 온보딩되었는지 여부에 따라 관리 책임과 절차가 다릅니다. 이 문서에서는 다르게 처리해야 하는 절차와 Workfront 및 Adobe Admin Console 모두에 대한 지침 링크를 나열합니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a84a5a8d-7c2a-4b51-a614-91a6dc9aa4ed
source-git-commit: b476c012f825afc4bc48b7172be26accc6bac0d1
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 1%

---

# 플랫폼 기반 관리의 차이점(Adobe Workfront/Adobe 비즈니스 플랫폼)

조직이 Adobe 비즈니스 플랫폼에 온보딩된 경우 사용자는 Adobe 비즈니스 플랫폼을 사용하여 Adobe Workfront에 액세스합니다. 이것은 다음을 의미합니다.

* 시스템 관리자는 Adobe Admin Console을 통해 생성됩니다.
* SSO(Single Sign-On)는 Workfront이 아닌 Adobe 비즈니스 플랫폼을 통해 처리됩니다

Adobe Workfront 관리자는 조직이 Adobe 비즈니스 플랫폼에 온보딩되었는지 여부에 따라 관리 책임과 절차가 다릅니다. 이 문서에서는 다르게 처리되는 절차와 Workfront 및 Adobe Admin Console 모두에 대한 지침 링크를 나열합니다.

## 사용자



>[!NOTE]
>
>Workfront에서 직접 시스템 관리자가 아닌 사용자를 추가하는 것이 좋습니다. Adobe Admin Console에서는 사용자를 추가할 수 있지만 Workfront에서 사용자를 추가하면 생성 중에 액세스 수준을 설정할 수 있으므로 시간을 절약할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>개 액션</th> 
   <th>Workfront에 대한 지침은</th> 
   <th>Adobe Admin Console의 지침은</th> 
  </tr> 
 </thead> 
 <tbody> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">View information about access levels and licenses for your users</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md" class="MCXref xref">List your users' access levels and licenses</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p>The section "View user list" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">사용자 관리자 액세스 권한 부여</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>의 "사용자 세부 정보 편집" 섹션 <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">개별적으로 사용자 관리</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront에 사용자 추가</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">사용자 추가</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Adobe Admin Console에서 사용자 관리</a> </p> </li> 
     <li> <p>의 "사용자 추가" 섹션 <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">개별적으로 사용자 관리</a></p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Add a user to Adobe Workfront Fusion</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../workfront-fusion/organizations/add-user-to-an-organization.md" class="MCXref xref">Add a user to an organization in Adobe Workfront Fusion</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
      <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">사용자 비활성화</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">사용자 비활성화 또는 재활성화</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>의 "사용자 제거" 섹션 <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">개별적으로 사용자 관리</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">사용자 삭제</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">사용자 삭제</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>의 "사용자 영구 삭제" 섹션 <a href="https://helpx.adobe.com/enterprise/using/manage-directory-users.html">디렉터리 사용자 관리</a>
     </p><p>참고: [!DNL Adobe Admin Console] 에서 사용자 비활성화 [!DNL Workfront]에서 삭제하지는 않습니다. [!DNL Workfront].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">사용자 프로필 편집</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">사용자 프로필 편집</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>의 "사용자 세부 정보 편집" 섹션 <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">개별적으로 사용자 관리</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">사용자 프로필 벌크 편집</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">사용자 프로필 일괄 편집</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>의 "사용자 세부 정보 편집" 섹션 <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">일괄 CSV 업로드</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">사용자 가져오기 </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">사용자 가져오기</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>의 "사용자 추가" 섹션 <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">일괄 CSV 업로드</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">다른 사용자로 로그인</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">다른 사용자로 로그인</a> </p> </li> 
    </ul> </td> 
   <td>사용할 수 없음</td> 
  </tr> 
  <tr> 
   <td role="rowheader">SAML 인증서 갱신</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Adobe Workfront SAML 2.0 메타데이터 인증서 갱신</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>의 섹션 "SAML 응답의 디지털 서명이 유효성을 검사하지 않았습니다..." <a href="https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html">문제 해결 Federated ID</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## SSO(Single Sign-On)

Adobe 비즈니스 플랫폼은 사용자의 SSO(Single Sign-On)를 제어하기 때문에 다음 작업 및 기능은 Adobe 비즈니스 플랫폼을 통해 자동으로 처리됩니다. 조직이 아직 Adobe 비즈니스 플랫폼에 온보딩되지 않은 경우 Workfront에서 이러한 작업을 수행해야 합니다.


* [SAML 2.0으로 Adobe Workfront 구성](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [ADFS를 사용하여 SAML 2.0으로 Adobe Workfront 구성](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [Adobe Workfront에서 SSO(Single Sign-On) 비활성화](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [ID 공급자에서 SAML 2.0 메타데이터 업데이트](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [SSO(Single Sign-On)를 위해 사용자 업데이트](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [인증을 위한 암호 정책 구성](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [시스템 보안 환경 설정 구성](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
