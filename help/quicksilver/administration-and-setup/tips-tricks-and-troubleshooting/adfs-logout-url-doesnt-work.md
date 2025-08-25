---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ADFS 로그아웃 URL이 작동하지 않음
description: 이 페이지에 설명된 절차는 Adobe Admin Console에 아직 온보딩되지 않은 조직에만 적용됩니다.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 0%

---

# ADFS 로그아웃 URL이 작동하지 않음

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 [!UICONTROL Adobe Admin Console]에 아직 온보딩되지 않은 조직에만 적용됩니다.
>
>조직이 [!UICONTROL Adobe Admin Console]에 온보딩된 경우 [플랫폼 기반 관리 차이점([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)을 참조하세요.

## 문제

ADFS 로그아웃 URL(https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0)을 사용하는 경우 &quot;사이트에 액세스하는 동안 문제가 발생했습니다. 사이트를 다시 찾아보십시오.&quot;

문제가 지속되면 이 사이트의 관리자에게 문의하여 다음 참조 번호를 제공하여 문제를 식별하십시오. **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

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
   <td role="rowheader">Adobe [!DNL Workfront] 라이선스</td> 
   <td> 
   <p>새로운 기능: 표준</p>
   또는
   <p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>[!UICONTROL 시스템 관리자]</td>  
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 솔루션

1. ADFS 관리자 서버에서 **[!UICONTROL 트러스트 관계]** > **[!UICONTROL 신뢰 당사자 트러스트]** > `<your party trust>` 속성으로 이동합니다.

1. **[!UICONTROL 끝점]** 탭에서 **[!UICONTROL 추가]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 끝점 형식]** = SAML 로그아웃, 바인딩 = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   다른 페이지로 리디렉션하려면 응답 URL을 설정할 수 있습니다. 그러나 ADFS 사이트는 로그오프되었지만 여전히 브라우저를 닫아야 한다고 경고하므로 이 사이트를 사용하는 것이 좋습니다.
