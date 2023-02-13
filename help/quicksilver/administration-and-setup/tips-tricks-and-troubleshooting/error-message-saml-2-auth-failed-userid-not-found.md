---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '오류 메시지: SAML 2.0 인증 실패: 사용자 식별자를 찾을 수 없음'
description: SAML 2.0을 사용하는 경우 "SAML 2.0 인증 실패 사용자 식별자를 찾을 수 없음" 오류는 ADFS 클레임 규칙에서 UID 또는 NAME ID가 전달되지 않음을 의미합니다. ADFS에서 신뢰 당사자 트러스트에는 UID 또는 NAME ID 값을 전달하는 클레임 규칙이 있어야 합니다. 를 실행할 때 [!DNL Workfront] 연결 테스트. 성공하면 이 메시지가 표시됩니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 1%

---

# 오류 메시지: SAML 2.0 인증 실패: 사용자 식별자를 찾을 수 없음

## 문제

SAML 2.0을 사용할 때 이 오류가 표시됩니다. &quot;SAML 2.0 인증 실패: 사용자 식별자를 찾을 수 없습니다.&quot;

## 원인

이 문제는 **UID** 또는 **이름 ID** 에서 전달되지 않음 **ADFS 클레임 규칙**.

ADFS에서 **신뢰 당사자 트러스트** 다음을 수행해야 합니다. **클레임 규칙** 다음 중 하나를 **UID** 또는 **이름 ID** 값. 를 실행할 때 **[!DNL Workfront]연결 테스트**&#x200B;이면 이 메시지가 표시됩니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>넌 [!DNL Workfront] 관리자 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 솔루션

1. 편집 시 **[!UICONTROL ADFS 정보]**&#x200B;에서 **[!UICONTROL 신뢰 당사자 트러스트]** > 개체 선택 >**[!UICONTROL 클레임 규칙 편집]**.

1. 다음 **[!UICONTROL LDAP 속성]** (왼쪽 열)에는 **[!UICONTROL 이메일 주소]** (또는 모든 고유 식별자).

1. 다음 **[!UICONTROL 발신 클레임 유형]** (오른쪽 열)은 **[!UICONTROL 이름 ID]**.

   >[!NOTE]
   >
   >LDAP 속성 E-Mail Address가 필요 없습니다. 사용자를 식별하는 모든 고유 식별자를 사용할 수 있지만 [!DNL Adobe Workfront] 로서의 **이름 ID**.
