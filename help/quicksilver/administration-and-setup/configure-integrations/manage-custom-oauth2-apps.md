---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: 사용자 정의 OAuth2 애플리케이션 보기 및 관리
description: Adobe Workfront 관리자는 Workfront 인스턴스에 대한 OAuth2 애플리케이션을 보고 관리할 수 있으며, 이를 통해 다른 애플리케이션이 Workfront에 액세스할 수 있습니다.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 0%

---

# 사용자 정의 OAuth2 애플리케이션 보기 및 관리

(으)로 [!DNL Adobe Workfront] 관리자는 의 인스턴스에 대한 OAuth2 애플리케이션을 보고 관리할 수 있습니다 [!DNL Workfront]: 다른 애플리케이션이 액세스할 수 있도록 허용 [!UICONTROL Workfront].

>[!NOTE]
>
>* OAuth2의 컨텍스트에서 &quot;Oauth2 애플리케이션&quot;은 앱과 서버(예: ) 간의 이러한 종류의 액세스 링크를 나타냅니다. [!DNL Workfront]. 자세한 내용은 [용 OAuth2 애플리케이션 만들기 [!DNL Workfront] 통합](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>* 한 번에 최대 10개의 OAuth2 애플리케이션을 보유할 수 있습니다.

* 사용자 지정 OAuth2 애플리케이션 만들기에 대한 자세한 내용은 [용 OAuth2 애플리케이션 만들기 [!DNL Workfront] 통합](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* 사용자 자격 증명(인증 코드 흐름)을 통해 OAuth2 애플리케이션을 구성하고 사용하는 방법에 대한 지침은 을 참조하십시오. [인증 코드 흐름을 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션 구성 및 사용](../../wf-api/api/oauth-app-code-token-flow.md).
* 서버 인증(JWT 흐름)을 사용한 OAuth2 애플리케이션 구성 및 사용에 대한 지침은 을 참조하십시오. [JWT 플로우를 사용하여 조직의 사용자 지정 OAuth 2 애플리케이션 구성 및 사용](../../wf-api/api/oauth-app-jwt-flow.md).
* PKCE를 사용하여 OAuth2 애플리케이션을 구성하고 사용하는 방법에 대한 지침은 를 참조하십시오. [PKCE 플로우를 사용하여 조직의 사용자 정의 OAuth 2 애플리케이션 구성 및 사용](../../wf-api/api/oauth-app-pkce-flow.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <td> 다음이어야 합니다: [!DNL Workfront] 관리자. </p>
    <p>다음에 대한 정보: [!DNL Workfront] 관리자, 참조 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

## 전제 조건

다음을 만들어야 합니다. [!UICONTROL OAuth2] 보거나 관리하기 전에 조직에 대한 응용 프로그램.

자세한 내용은 [용 OAuth2 애플리케이션 만들기 [!DNL Workfront] 통합](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## 사용자 정의 OAuth2 애플리케이션 관리

* [사용자 정의 OAuth2 애플리케이션 보기 및 편집](#view-and-edit-custom-oauth2-applications)
* [사용자 정의 OAuth2 애플리케이션 삭제](#delete-custom-oauth2-applications)

### 사용자 정의 OAuth2 애플리케이션 보기 및 편집 {#view-and-edit-custom-oauth2-applications}

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Adobe Workfront]을 클릭한 다음 을 클릭합니다 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 탐색 패널에서 을 클릭합니다. **[!UICONTROL 시스템]**&#x200B;을 선택한 다음 을 선택합니다. **[!UICONTROL OAuth 애플리케이션]**.
1. 클릭 **[!UICONTROL 앱 통합 만들기]**.
1. 애플리케이션 위로 마우스를 가져간 다음 **[!UICONTROL 편집]** ![](assets/edit-icon.png) 오른쪽 끝에 표시될 때
1. (선택 사항) 응용 프로그램의 세부 정보를 편집합니다.

   OAuth2 및 JWT 앱과 관련된 필드는 을 참조하십시오. [용 OAuth2 애플리케이션 만들기 [!DNL Workfront] 통합](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### 사용자 정의 OAuth2 애플리케이션 삭제 {#delete-custom-oauth2-applications}

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Adobe Workfront]을 클릭한 다음 을 클릭합니다 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 탐색 패널에서 을 클릭합니다. **[!UICONTROL 시스템]**&#x200B;을 선택한 다음 을 선택합니다. **[!UICONTROL OAuth 애플리케이션]**.
1. ** 를 **.
1. 애플리케이션 위로 마우스를 가져간 다음 **[!UICONTROL 삭제]** ![](assets/delete.png) 오른쪽 끝에 표시될 때

## OAuth2 애플리케이션에서 클라이언트 암호 관리

* [클라이언트 암호 세부 정보 보기](#view-client-secret-details)
* [클라이언트 암호에 대한 메모 추가 또는 편집](#add-or-edit-notes-for-client-secret)
* [클라이언트 암호 삭제](#delete-client-secret)

### 클라이언트 암호 세부 정보 보기 {#view-client-secret-details}

>[!IMPORTANT]
>
>클라이언트 암호 자체를 볼 수 없습니다. 클라이언트 암호를 잃어버린 경우 클라이언트 암호를 삭제하고 새 클라이언트 암호를 만들어야 합니다.
>
>* 클라이언트 암호를 삭제하려면 [클라이언트 암호 삭제](#delete-client-secret) 이 문서에서.
>* 새 클라이언트 암호를 만들려면 다음을 참조하십시오 [OAuth2 애플리케이션 만들기](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) 위치: [용 OAuth2 애플리케이션 만들기 [!DNL Workfront] 통합](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>



1. 다음을 클릭합니다. *[!UICONTROL *메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Adobe Workfront]을 클릭한 다음 을 클릭합니다 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 탐색 패널에서 을 클릭합니다. **[!UICONTROL 시스템]**&#x200B;을 선택한 다음 을 선택합니다. **[!UICONTROL OAuth 애플리케이션]**.
1. 애플리케이션 위로 마우스를 가져간 후 **[!UICONTROL 편집]** 아이콘 을 클릭하여 맨 오른쪽에 나타납니다.
1. 클라이언트 보안 영역에서 세부 정보 보기:

   * 제작 일자
   * 마지막으로 사용한 날짜
   * 메모

     클라이언트 암호에 메모를 추가하려면 [클라이언트 암호에 대한 메모 추가 또는 편집](#add-or-edit-notes-for-client-secret).

### 클라이언트 암호에 대한 메모 추가 또는 편집 {#add-or-edit-notes-for-client-secret}

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Adobe Workfront]을 클릭한 다음 을 클릭합니다 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 탐색 패널에서 을 클릭합니다. **[!UICONTROL 시스템]**&#x200B;을 선택한 다음 을 선택합니다. **[!UICONTROL OAuth 애플리케이션]**.
1. 클릭 **[!UICONTROL 앱 통합 만들기]**.
1. 애플리케이션 위로 마우스를 가져간 후 **[!UICONTROL 편집]** 아이콘 을 클릭하여 맨 오른쪽에 나타납니다.
1. 메모를 추가하거나 편집할 클라이언트 암호를 찾습니다.
1. 클라이언트 암호에 대한 세부 정보가 포함된 상자를 클릭합니다.

   이제 메모 텍스트를 추가하거나 기존 메모 텍스트를 편집할 수 있습니다.

   >[!NOTE]
   >
   >참고 텍스트는 최대 64자입니다.

1. 를 클릭하거나 를 누릅니다. **[!UICONTROL 입력]** 메모 텍스트를 저장합니다.

### 클라이언트 암호 삭제 {#delete-client-secret}

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Adobe Workfront]을 클릭한 다음 을 클릭합니다 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 탐색 패널에서 을 클릭합니다. **[!UICONTROL 시스템]**&#x200B;을 선택한 다음 을 선택합니다. **[!UICONTROL OAuth 애플리케이션]**.
1. 클릭 **[!UICONTROL 앱 통합 만들기]**.
1. 애플리케이션 위로 마우스를 가져간 후 **[!UICONTROL 편집]** 아이콘 을 클릭하여 맨 오른쪽에 나타납니다.
1. 삭제할 클라이언트 암호를 찾습니다.
1. 다음을 클릭합니다. **[!UICONTROL 삭제]** 아이콘 ![](assets/delete.png) 클라이언트 암호 옆에 있습니다.
