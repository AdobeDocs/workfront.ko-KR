---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,보안,인증서,관리자,면제,구성,메타데이터
navigation-topic: security
title: Adobe Workfront SAML 2.0 메타데이터 인증서 갱신
description: Adobe Workfront 서버는 인증 및 권한 부여에 SAML 2.0 프로토콜을 사용합니다. 업데이트되면 새 인증서는 1년 동안 유효합니다. ID 공급자에서 인증서를 갱신할 때가 되면 Workfront에서 이 변경이 발생해야 한다는 경고 메시지가 표시됩니다. Workfront 관리자는 시스템 수준에서 이 변경 사항을 관리할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# Adobe Workfront SAML 2.0 메타데이터 인증서 갱신

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 아직 Admin Console에 온보딩되지 않은 조직에만 적용됩니다. 조직이 Adobe Admin Console에 온보딩된 경우 조치가 필요하지 않습니다.
>
>조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 달라지는 절차 목록은 을 참조하십시오. [플랫폼 기반 관리의 차이점(Adobe Workfront/Adobe 비즈니스 플랫폼)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe Workfront 서버는 인증 및 권한 부여에 SAML 2.0 프로토콜을 사용합니다. 업데이트되면 새 인증서는 1년 동안 유효합니다. ID 공급자에서 인증서를 갱신할 때가 되면 Workfront에서 이 변경이 발생해야 한다는 경고 메시지가 표시됩니다. Workfront 관리자는 시스템 수준에서 이 변경 사항을 관리할 수 있습니다.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certificate before the specified date. Mismatched certificates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>조직의 Workfront 인스턴스가 Adobe IMS를 사용하여 활성화된 경우 사용할 수 없습니다. 자세한 내용은 네트워크 또는 IT 관리자에게 문의하십시오.

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
  <td> <p>새로운 기능: 표준 </p>
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

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Workfront 내에서 SAML 2.0 구성

경고 메시지를 검토하고 ID 공급자에서 SAML 2.0 메타데이터의 업데이트를 확인하려면 다음을 수행하십시오.

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **시스템** > **단일 사인온**.

1. 다음에서 **유형** 드롭다운 메뉴에서 다음을 선택합니다. **SAML 2.0**.

1. 클릭 **SAML 2.0 메타데이터 다운로드**.

   이렇게 하면 서버에 대한 올바른 메타데이터가 포함된 SAML 2.0에 대해 갱신된 Workfront 인증서가 다운로드됩니다.

1. ID 공급자에서 현재 ACS(Assertion Consumer Service) URL(회신 URL이라고도 함)을 안전한 장소에 복사합니다.

   >[!CAUTION]
   >
   >6단계에서 Workfront 메타데이터를 SSO(Single Sign-On) 공급자에게 업로드하기 전에 현재 ACS(어설션 소비자 서비스) URL을 안전한 장소에 복사합니다. 회신 URL이라고도 하는 이 URL은 SSO 공급자의 Workfront 구성 페이지에 있습니다.
   >
   >
   >Workfront 메타데이터를 업로드한 후 ACS URL이 변경되면 메타데이터에 잘못된 ACS URL이 포함될 수 있음을 의미합니다. SSO(Single Sign-On) 연결이 끊어지는 것을 방지하려면 복사한 것으로 다시 변경해야 합니다. 이 작업을 수행한 후에도 업데이트된 인증서가 여전히 유효합니다.

1. ID 공급자 서버에서 다운로드한 새 인증서를 업데이트합니다.
1. (조건부) ACS(어설션 소비자 서비스) URL 또는 회신 URL이 ID 공급자에서 변경된 경우 5단계에서 복사한 URL로 다시 변경합니다.
1. Workfront에서 **SSO(단일 인증) 페이지**, 이 옵션이 선택되어 있는지 확인합니다. **새 Workfront 인증서가 이미 ID 공급자에 업로드되었습니다.**.

   >[!NOTE]
   >
   >* 이 옵션은 다음 사항이 모두 적용되는 경우에만 표시됩니다.
   >   * 조직이 이미 SAML 2.0에 대해 설정되어 있습니다.
   >   * 현재 인증서가 만료될 준비가 되었습니다.
   >   * 새 인증서를 사용할 수 있습니다
   >* 이 필드를 선택하면 Workfront 관리자는 SSO 자격 증명 또는 Workfront 자격 증명으로 Workfront에 로그인할 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.

   ID 공급자 서버에서 SAML 2.0 인증서 갱신을 확인했으므로 경고 메시지가 더 이상 표시되지 않습니다.

1. 클릭 **연결 테스트** 구성을 테스트합니다.

   연결이 성공했음을 확인하는 메시지가 표시됩니다.

자세한 내용을 확인하거나 메타데이터의 수동 구성에 대한 지원이 필요한 경우 의 설명에 따라 지원 팀에 문의하십시오. [고객 지원 문의](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
