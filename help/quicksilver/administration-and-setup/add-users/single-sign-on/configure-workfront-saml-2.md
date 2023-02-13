---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: SAML 2.0으로 Adobe Workfront 구성
description: Adobe Workfront 관리자는 SSO(Single Sign-On)용 SAML(Security Assertion Markup Language) 2.0 솔루션과 통합하도록 Workfront 웹 및 모바일 애플리케이션을 구성할 수 있습니다.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: cf09859c-7d6f-4bf0-9b7f-c57096233c94
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 8%

---

# SAML 2.0으로 Adobe Workfront 구성

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.** </p>
-->

{{important-admin-console-onboard}}

Adobe Workfront 관리자는 SSO(Single Sign-On)용 SAML(Security Assertion Markup Language) 2.0 솔루션과 통합하도록 Workfront 웹 및 모바일 애플리케이션을 구성할 수 있습니다.

다음 섹션에 설명된 대로 Workfront에서 SAML 2.0을 구성한 후에는 다음에 설명된 대로 구성을 유지 관리할 수 있습니다. [ID 공급자에서 SAML 2.0 메타데이터 업데이트](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).

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

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **시스템** > **SSO(Single Sign-On).**

1. 에서 **유형** 드롭다운 목록에서 **SAML 2.0.**

1. 표시되는 옵션 맨 위에 있는 **SAML 2.0 메타데이터 다운로드** 파일을 컴퓨터에 다운로드합니다.

   SAML 2.0 ID 공급자는 Workfront 인스턴스에서 생성된 정보가 있는 XML 파일이 필요합니다. 파일이 다운로드되면 SAML 2.0 ID 공급자 서버로 이동하여 Workfront SAML 2.0 메타데이터 XML 파일을 여기에서 업로드해야 합니다.

1. 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">서비스 공급자 ID </td> 
      <td> 이미 채워져 있는 이 URL은 ID 공급자에서 Workfront을 식별합니다. For example: <code>&lt;yourcompany&gt;.com/SAML2</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">바인딩 유형</span> </td> 
      <td> <p>IDP 서버에서 인증 정보를 전송하는 방법을 선택합니다.</p> 
       <ul> 
        <li>POST</li> 
        <li>리디렉션</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ID 공급자 메타데이터에서 필드 채우기 </td> 
      <td>SAML 2.0 ID 공급자 솔루션에서 서비스 공급자 메타데이터 XML 파일을 내보내고 컴퓨터의 임시 위치에 저장합니다. 선택 <strong>파일 선택</strong>그런 다음 저장한 파일을 찾아 선택하여 Workfront 구성에 추가합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">로그인 포털 URL</span> </td> 
      <td>조직의 일반적인 로그인 포털을 지정합니다. 사용자가 Workfront 및 SAML 2.0과 통합된 다른 모든 애플리케이션에 액세스하기 위해 로그인하는 URL입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">로그아웃 URL</span> </td> 
      <td> <p>IDP 서버의 로그아웃 URL을 지정합니다. Workfront은 Workfront에서 로그아웃하기 전에 이 URL에 HTTP 요청을 전송합니다. 이렇게 하면 Workfront 세션이 닫히면 원격 서버에서 사용자의 세션이 닫힙니다.</p> <p><b>참고</b>: 사용자 프로필에 SAML 2.0 인증만 허용 옵션이 활성화되어 있는 경우에만 로그아웃 URL로 리디렉션됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">암호 변경 URL </td> 
      <td> <p> 사용자가 암호를 변경하도록 리디렉션될 URL을 지정합니다. </p> <p>SAML 2.0 자격 증명은 Workfront에 액세스하는 데 사용되므로 사용자는 Workfront을 통해 이 활동을 완료하는 대신 SAML 2.0 암호를 변경할 수 있는 페이지로 리디렉션해야 합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">SHA(Secure Hash Algorithm) </td> 
      <td> <p>IDP에서 지원하는 SHA(보안 해시 알고리즘)를 선택합니다.</p> 
       <ul> 
        <li>SHA-1</li> 
        <li>SHA-256</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">자동 프로비저닝 사용자</span> </td> 
      <td> <p>디렉토리 사용자 이름과 암호를 사용하는 새 사용자가 처음으로 Workfront에 로그인하려고 하면 시스템에서 사용자를 자동으로 생성합니다.</p> <p>Workfront에서 사용자를 만들려면 Workfront 데이터 속성을 디렉토리 공급자의 다음 사용자 데이터 속성과 매핑해야 합니다.</p> 
       <ul> 
        <li>이름</li> 
        <li>성</li> 
        <li>이메일 주소</li> 
       </ul> 
       <p>다음 옵션이 표시되어 이 작업을 수행할 수 있습니다.</p> 
       <p> <img src="assets/saml-2.0-auto-provision-users-ui.png"> </p> 
       <p>드롭다운 목록에서 매핑할 Workfront 사용자 속성을 선택한 다음 사용자 디렉토리에 해당 디렉토리 속성을 지정합니다.</p> 
       <p>다음 <strong>디렉토리 속성</strong> 필드에는 SAML 2.0 구성을 성공적으로 테스트할 때 저장한 사용자 속성 테이블의 디렉토리 속성 이름이 포함되어야 합니다.</p> 
       <p>에서 기본 Workfront 값 을 설정할 수 있습니다 <strong>기본값</strong> 필드. SAML 2.0 ID 공급자의 값을 기반으로 규칙을 설정할 수도 있습니다.</p> 
       <p><b>경고</b>: Workfront은 사용자가 시스템에 로그인할 때마다 아래에 나열된 속성을 매핑하려고 합니다. 따라서 매핑 액세스 수준은 권장되지 않습니다. 속성이 잘못 매핑되면 관리 액세스를 쉽게 제거할 수 있습니다. 매핑 추가 를 클릭하여 규칙을 더 추가합니다.
       </p> 
       <p>다음 Workfront 속성을 매핑할 수 있습니다.</p> 
      <ul> 
      <li> <p>액세스 수준</p> </li> 
      <li> <p>주소</p> </li> 
      <li> <p>Address2</p> </li> 
      <li> <p>시간당 청구</p> </li> 
      <li> <p>도시</p> </li> 
      <li> <p>회사</p> </li> 
      <li> <p>시간당 비용</p> </li> 
      <li> <p>이메일 주소</p> </li> 
      <li> <p>확장</p> </li> 
      <li> <p>이름</p> </li> 
      <li> <p>홈 그룹</p> </li> 
      <li> <p>홈 팀</p> </li> 
      <li> <p>작업 역할</p> </li> 
      <li> <p>성</p> </li> 
      <li> <p>레이아웃 템플릿</p> </li> 
      <li> <p>관리자</p> </li> 
      <li> <p>휴대폰</p> </li> 
      <li> <p>전화 번호</p> </li> 
      <li> <p>우편번호</p> </li> 
      <li> <p>일정</p> </li> 
      <li> <p>상태</p> </li> 
      <li> <p>타임시트 프로필</p> </li> 
      <li> <p>제목</p> </li> 
      </ul> </td> 
          <td> </td> 
         </tr> 
        </tbody> 
        <p>클릭 <strong>저장</strong> 사용자 특성 매핑을 마치면 를 사용합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">인증서 </td> 
      <td> <p>인증 서비스와 Workfront 간의 보안 연결을 보장하기 위해 올바른 SSL 인증서를 업로드합니다. OnDemand 계정의 경우 인증서가 항상 필요합니다. 이 인증서는 SAML 2.0 시스템 관리자로부터 받을 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">관리자 면제 </td> 
      <td> <p>Workfront 관리자가 Workfront 로그인을 사용하여 Workfront에 액세스할 수 있습니다. 이 옵션을 선택하지 않으면 Workfront 관리자는 SAML 2.0 사용자 이름과 암호를 사용해야 합니다.</p> 
      <p>Workfront은 먼저 Workfront 시스템 관리자 액세스 수준을 가진 사용자에 대해 SAML 2.0을 통해 Workfront에 로그인하려고 합니다. SAML 2.0 인증이 실패하면 Workfront은 Workfront 관리자에 대해 로컬 인증을 사용합니다.</p> 
      <p>SAML 2.0 공급자를 일시적으로 사용할 수 없는 경우 Workfront 관리자가 Workfront에 로그인할 수 있도록 이 옵션을 항상 선택한 것이 좋습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">활성화 </td> 
      <td> <p>Workfront 시스템에서 SSO를 활성화합니다. 사용자에게 로그인 지침을 전달했는지 확인합니다.</p> <p>Workfront에서 SSO 구성을 활성화한 후에는 <strong>SAML 2.0 인증만 허용</strong> SSO를 사용하도록 모든 사용자에 대해 를 설정합니다.</p> <p>SSO용 사용자 업데이트에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">단일 사인온용 사용자 업데이트</a>.</p> <p>사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">사용자 프로필 편집</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">구성 확인 </td> 
      <td> 
      <p>클릭 <strong>연결 테스트</strong> Workfront 및 SAML 2.0 ID 공급자가 서로 통신할 수 있는지 확인하십시오. 이 연결은 XML 파일을 교환한 경우에만 성공합니다.
      </p> 
      <p>SAML 2.0 ID 공급자와 Workfront 간의 링크를 성공적으로 테스트하면 아래 화면과 유사한 화면이 표시됩니다.</p>
      <p><b>참고</b>: 이 화면은 브라우저 팝업에 표시되므로 브라우저에서 팝업 차단기를 비활성화해야 합니다.</p>
      <p>나중에 사용할 수 있도록 표에 표시된 정보를 저장합니다.</p>
      <p><img src="assets/success-table-saml-2.png"></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **저장** SAML 2.0 구성을 저장
