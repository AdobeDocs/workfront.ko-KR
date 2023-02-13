---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ADFS 로그아웃 URL이 작동하지 않습니다
description: 이 페이지에서 설명하는 절차는 아직 Adobe Admin Console에 온보딩되지 않은 조직에만 적용됩니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# ADFS 로그아웃 URL이 작동하지 않습니다

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 아직 [!UICONTROL Adobe Admin Console].
>
>조직에서 [!UICONTROL Adobe Admin Console]를 참조하십시오. [플랫폼 기반의 관리 차이점 ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## 문제

ADFS 로그아웃 URL(https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0)을 사용하는 경우 다음과 같은 오류가 있는 메시지 페이지가 표시됩니다. &quot;사이트에 액세스하는 동안 문제가 발생했습니다. 사이트를 다시 찾아보세요.&quot;

문제가 지속되면 이 사이트의 관리자에게 문의하여 문제를 파악하십시오. **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

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
   <td role="rowheader">Adobe [!DNL Workfront] 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>넌 [!DNL Workfront] 관리자 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 솔루션

1. ADFS 관리자 서버에서 다음 위치로 이동합니다. **[!UICONTROL 신뢰 관계]** > **[!UICONTROL 신뢰 당사자 트러스트]** > `<your party trust>` 속성을 사용합니다.

1. 아래에 **[!UICONTROL 끝점]** 탭, **[!UICONTROL 추가]**.

1. **[!UICONTROL 끝점 유형]** = SAML 로그아웃, 바인딩 = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   다른 페이지로 리디렉션하도록 응답 URL을 설정할 수 있습니다. 그러나 ADFS 사이트는 사용자가 로그오프되었다는 경고를 표시하지만 여전히 브라우저를 닫아야 하므로 권장됩니다.
