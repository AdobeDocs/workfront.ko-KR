---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: 사용자 지정 OAuth2 애플리케이션 보기 및 관리
description: Adobe Workfront 관리자는 Workfront 인스턴스에 대한 OAuth2 애플리케이션을 보고 관리할 수 있으며, 이 경우 다른 애플리케이션에서 Workfront에 액세스할 수 있습니다.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: f7e3182776e6b62103cd755b2fbd5057efc95394
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 1%

---

# 사용자 지정 OAuth2 애플리케이션 보기 및 관리

로서의 [!DNL Adobe Workfront] 관리자는 자신의 인스턴스에 대한 OAuth2 응용 프로그램을 보고 관리할 수 있습니다 [!DNL Workfront]: 다른 응용 프로그램이 액세스할 수 있도록 합니다 [!UICONTROL Workfront].

>[!NOTE]
>
>OAuth2 컨텍스트에서 &quot;Oauth2 애플리케이션&quot;은 앱과 서버 간에 이러한 종류의 액세스 링크를 나타냅니다(예: [!DNL Workfront]. 자세한 내용은 [용 OAuth2 애플리케이션 만들기 [!DNL Workfront] 통합](../../administration-and-setup/configure-integrations/create-oauth-application.md)

* 사용자 지정 OAuth2 응용 프로그램 만들기에 대한 내용은 [용 OAuth2 애플리케이션 만들기 [!DNL Workfront] 통합](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* 사용자 자격 증명(인증 코드 흐름)과 함께 OAuth2 응용 프로그램을 구성하고 사용하는 방법에 대한 지침은 [인증 코드 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션을 구성하고 사용합니다](../../wf-api/api/oauth-app-code-token-flow.md).
* 서버 인증(JWT 흐름)을 사용하여 OAuth2 애플리케이션을 구성하고 사용하는 방법에 대한 지침은 [JWT 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션을 구성하고 사용합니다](../../wf-api/api/oauth-app-jwt-flow.md).
* PKCE를 사용하여 OAuth2 응용 프로그램을 구성하고 사용하는 방법에 대한 지침은 [PKCE 플로우를 사용하여 조직의 사용자 지정 OAuth 2 응용 프로그램 구성 및 사용](../../wf-api/api/oauth-app-pkce-flow.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!DNL Pro] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Plan] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> 넌 [!DNL Workfront] 관리자 </p>
    <p>에 대한 자세한 정보 [!DNL Workfront] 관리자 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 전제 조건

만들어야 합니다 [!UICONTROL OAuth2] 조직의 애플리케이션을 보거나 관리하려면 먼저 해당 애플리케이션을 확인합니다.

자세한 내용은 [용 OAuth2 애플리케이션 만들기 [!DNL Workfront] 통합](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## 사용자 지정 OAuth2 애플리케이션 관리

* [사용자 지정 OAuth2 애플리케이션 보기 및 편집](#view-and-edit-custom-oauth2-applications)
* [사용자 지정 OAuth2 애플리케이션 삭제](#delete-custom-oauth2-applications)

### 사용자 지정 OAuth2 애플리케이션 보기 및 편집 {#view-and-edit-custom-oauth2-applications}

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 탐색 패널에서 **[!UICONTROL 시스템]**&#x200B;를 선택하고 을 선택합니다. **[!UICONTROL OAuth 애플리케이션]**.
1. 클릭 **[!UICONTROL 앱 통합 만들기]**.
1. 애플리케이션을 마우스로 가리킨 다음 을 클릭합니다 **[!UICONTROL 편집]** ![](assets/edit-icon.png) 맨 오른쪽에 나타나게 되면
1. (선택 사항) 응용 프로그램의 세부 사항을 편집합니다.

   OAuth2 및 JWT 앱과 관련된 필드는 다음을 참조하십시오 [용 OAuth2 애플리케이션 만들기 [!DNL Workfront] 통합](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### 사용자 지정 OAuth2 애플리케이션 삭제 {#delete-custom-oauth2-applications}

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 탐색 패널에서 **[!UICONTROL 시스템]**&#x200B;를 선택하고 을 선택합니다. **[!UICONTROL OAuth 애플리케이션]**.
1. 클릭 **  **.
1. 애플리케이션을 마우스로 가리킨 다음 을 클릭합니다 **[!UICONTROL 삭제]** ![](assets/delete.png) 맨 오른쪽에 나타나게 되면

## OAuth2 애플리케이션에서 클라이언트 암호 관리

* [클라이언트 암호 세부 정보 보기](#view-client-secret-details)
* [클라이언트 암호 노트 추가 또는 편집](#add-or-edit-notes-for-client-secret)
* [클라이언트 암호를 삭제하시겠습니까](#delete-client-secret)

### 클라이언트 암호 세부 정보 보기 {#view-client-secret-details}

>[!IMPORTANT]
>
>클라이언트 암호 자체를 볼 수 없습니다. 클라이언트 암호를 잃어버린 경우 클라이언트 암호를 삭제하고 새 클라이언트 암호를 만들어야 합니다.
>
>* 클라이언트 암호를 삭제하려면 [클라이언트 암호 삭제](#delete-client-secret) 참조하십시오.
>* 새 클라이언트 암호를 만들려면 [OAuth2 애플리케이션 만들기](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) in [용 OAuth2 애플리케이션 만들기 [!DNL Workfront] 통합](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>




1. 을(를) 클릭합니다. *[!UICONTROL *주 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 탐색 패널에서 **[!UICONTROL 시스템]**&#x200B;를 선택하고 을 선택합니다. **[!UICONTROL OAuth 애플리케이션]**.
1. 애플리케이션을 마우스로 가리킨 다음 **[!UICONTROL 편집]** 맨 오른쪽에 표시될 때 아이콘을 사용합니다.
1. 클라이언트 암호 영역에서 세부 정보를 봅니다.

   * 만든 날짜
   * 마지막으로 사용한 날짜
   * 메모

      클라이언트 암호로 메모를 추가하려면 [클라이언트 암호 노트 추가 또는 편집](#add-or-edit-notes-for-client-secret).

### 클라이언트 암호 노트 추가 또는 편집 {#add-or-edit-notes-for-client-secret}

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 탐색 패널에서 **[!UICONTROL 시스템]**&#x200B;를 선택하고 을 선택합니다. **[!UICONTROL OAuth 애플리케이션]**.
1. 클릭 **[!UICONTROL 앱 통합 만들기]**.
1. 애플리케이션을 마우스로 가리킨 다음 **[!UICONTROL 편집]** 맨 오른쪽에 표시될 때 아이콘을 사용합니다.
1. 메모를 추가하거나 편집할 클라이언트 암호를 찾습니다.
1. 클라이언트 암호 세부 정보가 포함된 상자를 클릭합니다.

   이제 참고 텍스트를 추가하거나 기존 메모 텍스트를 편집할 수 있습니다.

   >[!NOTE]
   >
   >참고 텍스트는 최대 64자입니다.

1. 상자 바깥쪽을 클릭하거나 키를 누릅니다 **[!UICONTROL Enter 키]** 메모 텍스트를 저장하려면

### 클라이언트 암호를 삭제하시겠습니까 {#delete-client-secret}

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 탐색 패널에서 **[!UICONTROL 시스템]**&#x200B;를 선택하고 을 선택합니다. **[!UICONTROL OAuth 애플리케이션]**.
1. 클릭 **[!UICONTROL 앱 통합 만들기]**.
1. 애플리케이션을 마우스로 가리킨 다음 **[!UICONTROL 편집]** 맨 오른쪽에 표시될 때 아이콘을 사용합니다.
1. 삭제할 클라이언트 암호를 찾습니다.
1. 을(를) 클릭합니다. **[!UICONTROL 삭제]** 아이콘 ![](assets/delete.png) 클라이언트 암호 옆의 를 클릭합니다.
