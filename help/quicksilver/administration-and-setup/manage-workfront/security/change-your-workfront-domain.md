---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Adobe Workfront 도메인 변경
description: Adobe Workfront 관리자 및 인증된 Workfront 지원 담당자는 Workfront 지원 팀에 조직의 Workfront 도메인을 변경하는 데 도움을 요청할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: be11c7417023ce2f310fce3e0cf77724d101b89e
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 11%

---

# Adobe Workfront 도메인 변경

<!--Remove me October 2026-->

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 Admin Console에 아직 온보딩되지 않은 조직에만 적용됩니다. 이제 모든 조직이 Adobe Admin Console에 온보딩되었으므로 **Workfront 도메인을 변경할 수 없습니다**.
>
>조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 달라지는 절차 목록은 Adobe Workfront과 Adobe Business Platform 간의 [관리 차이점](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)을 참조하십시오.
>
>이 문서는 가까운 시일 내에 제거될 수 있습니다.

Adobe Workfront 관리자 및 인증된 Workfront 지원 담당자는 Workfront 지원 팀에 조직의 Workfront 도메인을 변경하는 데 도움을 요청할 수 있습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td><p>Any</p></td> 
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

## 도메인 변경 요청

1. Experience League에서 지원 티켓 만들기를 시작합니다.
1. **설명** 상자에 원하는 새 도메인과 새 도메인을 실행하려는 기간을 포함하십시오.
1. 지원 사례에 대한 상자 작성을 완료한 다음 **제출**&#x200B;을 클릭합니다.

Workfront 지원 센터에 문의하여 도메인 변경에 대한 도움을 받을 수도 있습니다.

<!--

## Update the new domain if you are an SSO customer

If your company utilizes SSO, the following steps are required after you have your Workfront domain changed.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

{{step-1-to-setup}}

1. In the left sidebar, click **System** > **Customer Info** and make sure that your domain is updated on the Customer Info page.

1. In the left sidebar, click **System** > **Single Sign-On (SSO)**.

1. Click **Download SAML 2.0 Metadata**.
1. After the file is downloaded, open it and make sure of the following:

   1. **entityID** is pointing to the new domain.
   1. All locations within **`<md:AssertionConsumerService>`** point to the new domain.

1. Provide the downloaded metadata file to your Identity Provider so that they can update it on their end.
1. Make sure the domain is updated for all Workfront integrations used by your organization.


-->
