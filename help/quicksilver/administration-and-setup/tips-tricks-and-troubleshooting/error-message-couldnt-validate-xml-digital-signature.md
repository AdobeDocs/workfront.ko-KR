---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "오류 메시지: XML 디지털 서명의 유효성을 검사할 수 없음"
description: ADFS에 성공적으로 연결할 수 없습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 1%

---

# 오류 메시지: XML 디지털 서명의 유효성을 검사할 수 없음

## 문제

ADFS에 성공적으로 연결할 수 없습니다.

![error_message.png](assets/error-message.png)

>[!NOTE]
>
>성공적인 테스트 연결을 설정했지만 여전히 문제가 발생하는 경우 잘못된 속성 매핑이나 페더레이션 ID에 문제가 발생할 수 있습니다. 문의 사항은 고객 지원 센터에 문의하십시오.

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

## 원인 1: 인증서가 올바르지 않음

### 솔루션

ADFS 서버에서 서명 인증서를 수동으로 검색합니다.

1. [!DNL Windows]에서 **[!UICONTROL 시작]** > **[!UICONTROL 관리]** > **[!UICONTROL ADFS 2.0 관리]**&#x200B;를 클릭합니다.\
   [ADFS 2.0 관리] 대화 상자가 표시됩니다.

1. 왼쪽 창에서 **[!UICONTROL 트러스트 관계]** > **[!UICONTROL 신뢰 당사자 트러스트]**&#x200B;를 선택합니다.

1. **[!UICONTROL 신뢰 당사자 트러스트]**&#x200B;를 마우스 오른쪽 단추로 클릭하고 **[!UICONTROL 속성]**&#x200B;을 선택합니다.

1. **[!UICONTROL 서명]** 탭을 클릭합니다.
1. 서명 인증서의 이름을 클릭하고 **[!UICONTROL 보기]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 파일]**&#x200B;에 복사... 를 클릭하고 **[!UICONTROL 다음]**&#x200B;을 선택합니다.

1. **[!UICONTROL Base-64 인코딩 x.509(CER)]**&#x200B;을(를) 선택하고 **[!UICONTROL 다음]**&#x200B;을 클릭합니다.

1. 파일 이름을 지정하고 **[!UICONTROL 다음]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 마침]**&#x200B;을 클릭합니다.
1. [!DNL Adobe Workfront]에서 **[!UICONTROL 설정]** > **[!UICONTROL 시스템]** > **[!UICONTROL SSO(Single Sign-On)]**&#x200B;로 이동하여 서명 인증서를 수동으로 업로드하십시오.

## 원인 2: [!DNL Workfront]에 RSA 서명이 필요한 경우 DSA를 사용하여 인증서에 서명합니다.

### 솔루션

인증서를 다시 만들고 DSA 대신 RSA 서명을 사용합니다.

## 원인 3: XML 데이터가 올바르지 않음

### 솔루션

ADFS 관리 시스템에서 XML 메타데이터를 다시 내보내고 다시 가져옵니다.

## 원인 4: SAML 측의 오류로 인해 요청을 수행할 수 없음

### 솔루션

SAML 공급자에게 문의하십시오.
