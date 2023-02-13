---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,보안,인증서,관리,면제,구성,메타데이터
navigation-topic: security
title: Adobe Workfront SAML 2.0 메타데이터 인증서 갱신
description: 이 페이지에 설명된 절차는 Admin Console에 아직 온보딩되지 않은 조직에만 적용됩니다. 조직이 Adobe Admin Console에 온보딩된 경우 Adobe Admin Console을 통해 이 작업을 수행해야 합니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 3f84f6b8d6cb36fdb23ff332c4078ac1da4a8745
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Adobe Workfront SAML 2.0 메타데이터 인증서 갱신

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 Admin Console에 아직 온보딩되지 않은 조직에만 적용됩니다. 조직에서 Adobe Admin Console에 온보딩된 경우 조치가 필요하지 않습니다.
>
>조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 다른 절차 목록은 [플랫폼 기반의 관리 차이점(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe Workfront 서버는 인증 및 인증에 SAML 2.0 프로토콜을 사용합니다. 업데이트되면 새 인증서는 1년 동안 유효합니다. ID 공급자에서 인증서를 갱신할 시간이 되면 Workfront에서 이 변경 사항이 발생해야 한다고 알리는 경고가 표시됩니다. Workfront 관리자는 시스템 수준에서 이 변경 사항을 관리할 수 있습니다.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certiﬁcate before the speciﬁed date. Mismatched certiﬁcates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>Adobe IMS에서 조직의 Workfront 인스턴스가 활성화된 경우에는 사용할 수 없습니다. 자세한 내용은 네트워크 또는 IT 관리자에게 문의하십시오.

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

## Workfront 내에서 SAML 2.0 구성

경고 메시지를 검토하고 ID 공급자에서 SAML 2.0 메타데이터 업데이트를 승인하려면 다음을 수행하십시오.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **시스템** > **단일 사인온**.

1. 에서 **유형** 드롭다운 메뉴에서 **SAML 2.0**.

1. 클릭 **SAML 2.0 메타데이터 다운로드**.

   이렇게 하면 서버에 대한 올바른 메타데이터가 포함된 SAML 2.0에 대해 갱신된 Workfront 인증서를 다운로드합니다.

   >[!CAUTION]
   >
   >5단계에서 Workfront 메타데이터를 SSO(Single Sign-On) 공급자에게 업로드하기 전에 현재 ACS(Assertion Consumer Service) URL을 안전한 위치에 복사합니다. 이 URL은 회신 URL이라고도 하며 SSO 공급자의 Workfront 구성 페이지에서 확인할 수 있습니다.
   >
   >
   >Workfront 메타데이터를 업로드한 후 ACS URL이 변경되는 경우 메타데이터에 잘못된 ACS URL이 있을 수 있습니다. 단일 사인온 연결을 끊지 않도록 다시 복사한 연결로 변경해야 합니다. 이 작업을 수행한 후에도 업데이트된 인증서가 여전히 정확합니다.

1. ID 공급자 서버로 이동하여 다운로드한 새 인증서를 업데이트합니다.
1. Workfront에서 **SSO(Single Sign-On) 페이지**&#x200B;를 눌러 이 옵션을 선택해야 합니다. **새 Workfront 인증서가 이미 ID 공급자에 업로드되었습니다**.

   이 필드를 선택하면 Workfront 관리자는 SSO 자격 증명 또는 Workfront 자격 증명으로 Workfront에 로그인할 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.

   ID 공급자 서버에서 SAML 2.0 인증서 갱신을 확인했으므로 경고 메시지가 더 이상 표시되지 않습니다.

1. 클릭 **연결 테스트** 구성을 테스트하려면 다음을 수행하십시오.

   연결에 성공했음을 확인하는 메시지가 표시됩니다.

자세한 정보나 메타데이터의 수동 구성에 대한 도움이 필요하면 에 설명된 대로 지원 팀에 문의하십시오. [고객 지원에 문의](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
