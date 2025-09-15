---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: SAML 2.0으로 Adobe Workfront 구성하기
description: Adobe Workfront 관리자는 SSO(Single Sign-On)를 위해 SAML(Security Assertion Markup Language) 2.0 솔루션과 통합되도록 Workfront 웹 및 모바일 애플리케이션을 구성할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: cf09859c-7d6f-4bf0-9b7f-c57096233c94
source-git-commit: 93f4c1691210d88531fcc269bd40ee7ed8633309
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 7%

---

# SAML 2.0으로 Adobe Workfront 구성하기

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.** </p>
-->

<!-- Audited: 12/2023 -->



>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 Adobe Admin Console에 아직 온보딩되지 않은 조직에만 적용됩니다.
>
>Adobe Admin Console에 온보딩된 조직의 사용자 특성을 매핑하려면 사용자 특성 매핑 문서에서 [Adobe 통합 경험에서 사용자 특성 매핑](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience)을 참조하십시오.

Adobe Workfront 관리자는 SSO(Single Sign-On)를 위해 SAML(Security Assertion Markup Language) 2.0 솔루션과 통합되도록 Workfront 웹 및 모바일 애플리케이션을 구성할 수 있습니다.

다음 섹션에 설명된 대로 Workfront에서 SAML 2.0을 구성한 후에는 [ID 공급자에서 SAML 2.0 메타데이터 업데이트](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)에 설명된 대로 구성을 유지할 수 있습니다.

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
   <td><p>새로운 기능: 표준 </p>
       <p>또는</p> 
       <p>현재: 플랜 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## SAML 2.0으로 Workfront 인증 활성화

{{step-1-to-setup}}

1. **시스템** > **SSO(Single Sign-On)를 클릭합니다.**

1. **유형** 드롭다운 목록에서 **SAML 2.0.**&#x200B;을(를) 선택합니다.

1. 표시되는 옵션 상단 근처에서 **SAML 2.0 메타데이터 다운로드**&#x200B;를 클릭하여 컴퓨터에 있는 파일을 다운로드합니다.

   SAML 2.0 ID 공급자에는 Workfront 인스턴스에서 생성된 정보가 있는 XML 파일이 필요합니다. 파일을 다운로드한 후 SAML 2.0 ID 공급자 서버에 액세스하고 Workfront SAML 2.0 메타데이터 XML 파일을 업로드해야 합니다.

1. Workfront에서 다음 정보를 지정합니다.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">서비스 공급자 ID </td>
      <td> 이 URL은 이미 채워져 있으며 ID 공급자의 Workfront을 식별합니다. 예: <code>&lt;yourcompany&gt;.com/SAML2</code>.</td>
     </tr>
     <tr>
      <td role="rowheader">바인딩 형식</span> </td>
      <td> <p>IDP 서버에서 지원하는 인증 정보 전송 방법을 선택하십시오.</p>
       <ul>
       <li>POST</li>
       <li>리디렉션</li>
       </ul> </td>
     </tr>
     <tr>
      <td role="rowheader">ID 공급자 메타데이터에서 필드 채우기 </td> 
      <td>SAML 2.0 ID 공급자 솔루션에서 서비스 공급자 메타데이터 XML 파일을 내보내고 컴퓨터의 임시 위치에 저장합니다. <strong>파일 선택</strong>을 선택한 다음 저장한 파일을 찾아 선택하여 Workfront 구성에 추가합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">로그인 포털 URL</span> </td> 
      <td>조직의 공통 로그인 포털을 입력합니다. 사용자가 Workfront 및 SAML 2.0과 통합된 다른 모든 애플리케이션에 액세스하기 위해 로그인하는 URL입니다.</td> 
     </tr>
     <tr>
      <td role="rowheader">로그아웃 URL</span> </td> 
      <td> <p>IDP 서버의 로그아웃 URL을 입력합니다. Workfront은 Workfront에서 로그아웃하기 전에 이 URL에 HTTP 요청을 보냅니다. Workfront 세션이 닫히면 원격 서버에서 사용자의 세션이 닫힙니다.</p> <p><b>참고</b>: 사용자 프로필에 <strong>SAML 2.0 인증만 허용</strong> 옵션이 활성화된 경우에만 로그아웃 URL로 리디렉션됩니다.</p> </td>
     </tr>
     <tr>
      <td role="rowheader">암호 변경 URL </td> 
      <td> <p> 사용자가 암호를 변경하도록 리디렉션될 URL을 지정하십시오. </p> <p>SAML 2.0 자격 증명은 Workfront에 액세스하는 데 사용되므로 사용자는 Workfront을 통해 이 활동을 완료하는 대신 SAML 2.0 암호를 변경할 수 있는 페이지로 리디렉션되어야 합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">SHA(Secure Hash Algorithm) </td> 
      <td> <p>IDP에서 지원하는 보안 해시 알고리즘(SHA)을 선택합니다.</p> 
       <ul> 
       <li>SHA-1</li> 
       <li>SHA-256</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 자동 프로비저닝</span> </td> 
      <td> <p>이 옵션은 디렉토리 사용자 이름과 암호를 가진 새 사용자가 처음으로 Workfront에 로그인할 때 시스템에 사용자를 자동으로 생성합니다.</p> <p>Workfront에서 사용자를 만들려면 디렉터리 공급자에서 Workfront 데이터 속성을 다음 사용자 데이터 속성과 매핑해야 합니다.</p> 
       <ul> 
       <li>이름</li> 
       <li>성</li> 
       <li>이메일 주소</li> 
       </ul> 
       <p>확인란을 선택하면 다음 옵션이 표시됩니다.</p> 
       <p> <img src="assets/saml-2.0-auto-provision-users-ui.png"> </p> 
       <p>드롭다운 목록에서 매핑할 Workfront 사용자 속성을 선택한 다음 사용자 디렉토리에서 해당 디렉토리 속성을 지정합니다.</p> 
       <p><strong>디렉터리 특성</strong> 필드에는 SAML 2.0 구성을 성공적으로 테스트할 때 저장한 사용자 특성 테이블의 디렉터리 특성 이름이 포함되어야 합니다.</p> 
       <p><strong>기본 값</strong> 필드에서 기본 Workfront 값을 설정할 수 있습니다. SAML 2.0 ID 공급자의 값을 기반으로 규칙을 설정할 수도 있습니다.</p> 
       <p><b>경고</b>: Workfront은 사용자가 시스템에 로그인할 때마다 아래 나열된 특성을 매핑하려고 합니다. 이러한 이유로 매핑 액세스 수준을 권장하지 않습니다. 속성이 잘못 매핑된 경우 관리 액세스 권한을 쉽게 제거할 수 있습니다. 규칙을 추가하려면 <strong>매핑 추가</strong>를 클릭하십시오.
       </p> 
       <p>다음 Workfront 속성을 매핑할 수 있습니다.</p> 
      <ul> 
      <li> <p>액세스 수준</p> </li> 
      <li> <p>주소</p> </li> 
      <li> <p>주소2</p> </li> 
      <li> <p>시간당 청구</p> </li> 
      <li> <p>구/군/시</p> </li> 
      <li> <p>회사</p> </li> 
      <li> <p>시간당 비용</p> </li> 
      <li> <p>이메일 주소</p> </li> 
      <li> <p>확장 기능</p> </li> 
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
      <li> <p>예약</p> </li> 
      <li> <p>주/도</p> </li> 
      <li> <p>타임시트 프로필</p> </li> 
      <li> <p>제목</p> </li> 
      </ul>
      <p>사용자 특성 매핑을 마치면 <strong>저장</strong>을 클릭합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">인증서 </td> 
      <td> <p>유효한 SSL 인증서를 업로드하여 인증 서비스와 Workfront 간 보안 연결을 보장합니다. 온디맨드 계정의 경우 항상 인증서가 필요합니다. 이 인증서는 SAML 2.0 시스템 관리자로부터 받을 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">관리자 면제 </td> 
      <td> <p>Workfront 관리자는 Workfront 로그인을 사용하여 Workfront에 액세스할 수 있습니다. 이 옵션을 선택하지 않으면 Workfront 관리자는 SAML 2.0 사용자 이름과 암호를 사용해야 합니다.</p> 
      <p>Workfront은 먼저 Workfront 시스템 관리자 액세스 수준이 있는 사용자를 위해 SAML 2.0을 통해 Workfront에 로그인합니다. SAML 2.0 인증이 실패하면 Workfront은 Workfront 관리자에 대한 로컬 인증을 사용합니다.</p> 
      <p>SAML 2.0 공급자를 일시적으로 사용할 수 없는 경우 Workfront 관리자가 Workfront에 로그인할 수 있도록 항상 이 옵션을 선택하는 것이 좋습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">활성화 </td> 
      <td> <p>Workfront 시스템에서 SSO 활성화. 로그인 지침을 사용자에게 전달했는지 확인합니다.</p> <p>Workfront에서 SSO 구성을 사용하도록 설정한 후에는 모든 사용자가 SSO를 사용할 수 있도록 <strong>SAML 2.0 인증만 허용</strong> 설정을 사용하도록 설정해야 합니다.</p> <p>SSO용 사용자 업데이트에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">SSO(Single Sign-On)용 사용자 업데이트</a>를 참조하십시오.</p> <p>사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">사용자 프로필 편집</a>을 참조하세요.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">구성 확인 </td> 
      <td> 
      <p><strong>연결 테스트</strong>를 클릭하여 Workfront과 SAML 2.0 ID 공급자가 서로 통신할 수 있는지 확인합니다. 이 연결은 XML 파일을 교환한 경우에만 성공한 것입니다.
      </p> 
      <p>SAML 2.0 ID 공급자와 Workfront 간 링크를 성공적으로 테스트하면 아래 이미지와 유사한 화면이 표시됩니다.</p>
      <p><b>참고</b>: 이 화면은 브라우저 팝업에 표시되므로 브라우저에서 팝업 차단기를 사용하지 않도록 설정하십시오.</p>
      <p>나중에 사용할 수 있도록 표에 표시된 정보를 저장합니다.</p>
      <p><img src="assets/success-table-saml-2.png"></p></td> 
     </tr> 
    </tbody> 
   </table>

1. SAML 2.0 구성을 저장하려면 **저장**&#x200B;을 클릭합니다.
