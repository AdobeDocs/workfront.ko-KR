---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Workfront 및 SAML 2.0에서 사용할 Outlook 활성화
description: SAML 2.0 인증을 사용하도록 설정하고 사용자가 SAML 2.0 자격 증명을 사용하여 Microsoft Outlook에서 Workfront에 로그인할 수 있도록 하려면 Office 추가 기능에서 인증하도록 SAML 2.0을 사용하도록 설정해야 합니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Workfront 및 SAML 2.0에서 사용할 Outlook 활성화

SAML 2.0 인증을 사용하도록 설정하고 사용자가 SAML 2.0 자격 증명을 사용하여 Microsoft Outlook에서 Workfront에 로그인할 수 있도록 하려면 Office 추가 기능에서 인증하도록 SAML 2.0을 사용하도록 설정해야 합니다.

>[!NOTE]
>
>조직의 Workfront 인스턴스가 사용자 정의 SSO 포털을 사용하는 경우에는 사용할 수 없습니다.>
><!--
>or is enabled with Adobe IMS>
>-->
>자세한 내용은 네트워크 또는 IT 관리자에게 문의하십시오.

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

## Workfront 및 SAML 2.0에서 사용할 Outlook 활성화

{{step-1-to-setup}}

1. **시스템** > **기본 설정**&#x200B;을 클릭합니다.

1. **보안** 섹션에서 **Office 365 추가 기능에서 SAML 2.0 인증 허용**&#x200B;이 활성화되어 있는지 확인하십시오.

   이 옵션을 사용하면 Office 365 추가 기능에 대해서만 Workfront을 Iframe에 포함할 수 있습니다. 클릭할 수 있는 콘텐츠가 포함되어 있지 않으므로 클릭재킹 위반은 열리지 않습니다.

   이 옵션은 기본적으로 활성화되어 있습니다.

   >[!NOTE]
   >
   >**iframe에 Workfront 포함 허용** 옵션을 사용하면 **Office 365 추가 기능에서 SAML 2.0 인증 허용** 옵션이 흐리게 표시되어 활성화됩니다.
   >
   >![포함 옵션 허용](assets/if-you-enable.png)
   >

1. **저장**&#x200B;을 클릭합니다.

   여기에 저장한 변경 사항은 Workfront의 모든 사용자 경험에 영향을 줍니다.
