---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ADFS 로그아웃 URL이 작동하지 않음
description: 이 페이지에 설명된 절차는 Adobe Admin Console에 아직 온보딩되지 않은 조직에만 적용됩니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# ADFS 로그아웃 URL이 작동하지 않음

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 아직 온보딩되지 않은 조직에만 적용됩니다. [!UICONTROL Adobe Admin Console].
>
>조직이 로 온보딩된 경우 [!UICONTROL Adobe Admin Console], 참조 [플랫폼 기반 관리의 차이점 ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## 문제

ADFS 로그아웃 URL(https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0)을 사용하는 경우 &quot;사이트에 액세스하는 동안 문제가 발생했습니다. 사이트를 다시 찾아보십시오.&quot;

문제가 지속되면 이 사이트의 관리자에게 문의하여 다음 참조 번호를 제공하여 문제를 확인하십시오. **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

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
   <td role="rowheader">Adobe [!DNL Workfront] 라이센스</td> 
   <td> 
   <p>새로운 기능: 표준</p>
   <p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>다음이어야 합니다: [!DNL Workfront] 관리자. 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>.</p>  </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 솔루션

1. ADFS 관리자 서버에서 **[!UICONTROL 트러스트 관계]** > **[!UICONTROL 신뢰 당사자 트러스트]** > `<your party trust>` 속성.

1. 아래 **[!UICONTROL 엔드포인트]** 탭을 클릭하고 **[!UICONTROL 추가]**.

1. **[!UICONTROL 끝점 유형]** = SAML 로그아웃, 바인딩 = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   다른 페이지로 리디렉션하려면 응답 URL을 설정할 수 있습니다. 그러나 ADFS 사이트는 로그오프되었지만 여전히 브라우저를 닫아야 한다고 경고하므로 이 사이트를 사용하는 것이 좋습니다.
