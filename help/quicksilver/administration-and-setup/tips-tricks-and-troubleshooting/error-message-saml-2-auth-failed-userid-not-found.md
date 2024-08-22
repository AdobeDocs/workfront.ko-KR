---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "오류 메시지: SAML 2.0 인증 실패: 사용자 식별자를 찾을 수 없음"
description: SAML 2.0을 사용하는 경우 "SAML 2.0 인증 실패 사용자 식별자를 찾을 수 없음" 오류는 UID 또는 NAME ID가 ADFS 클레임 규칙에서 전달되지 않음을 의미합니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# 오류 메시지: SAML 2.0 인증 실패: 사용자 식별자를 찾을 수 없음

## 문제

SAML 2.0을 사용할 때 다음 오류가 표시됩니다. &quot;SAML 2.0 인증 실패: 사용자 식별자를 찾을 수 없음.&quot;

## 원인

이 문제는 **ADFS 클레임 규칙**&#x200B;에서 **UID** 또는 **이름 ID**&#x200B;이(가) 전달되지 않을 때 발생합니다.

ADFS에서 **신뢰 당사자 트러스트**&#x200B;에는 **UID** 또는 **이름 ID** 값을 전달하는 **클레임 규칙**&#x200B;이 있어야 합니다. **[!DNL Workfront]테스트 연결**&#x200B;을 실행할 때 성공하면 이 값이 표시됩니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td>
   <p>새로운 기능: 표준</p>
   <p>또는</p>
   <p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>[!DNL Workfront] 관리자여야 합니다. </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 솔루션

1. **[!UICONTROL ADFS 정보]**&#x200B;를 편집할 때 **[!UICONTROL 신뢰 당사자 트러스트]** > 개체 선택 >**[!UICONTROL 클레임 규칙 편집]**&#x200B;에서 확인하세요.

1. **[!UICONTROL LDAP 특성]**(왼쪽 열)에는 **[!UICONTROL 전자 메일 주소]**(또는 고유 식별자)가 있어야 합니다.

1. **[!UICONTROL 보내는 클레임 유형]**(오른쪽 열)은 **[!UICONTROL 이름 ID]**&#x200B;이어야 합니다.

   >[!NOTE]
   >
   >LDAP 속성 E-메일 주소를 가질 필요는 없습니다. 사용자를 식별하는 모든 고유 식별자를 사용할 수 있지만 **NAME ID**(으)로 [!DNL Adobe Workfront]에 전달해야 합니다.
