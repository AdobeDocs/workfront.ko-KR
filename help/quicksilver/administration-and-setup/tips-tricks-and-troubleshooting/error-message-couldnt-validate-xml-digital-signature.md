---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "오류 메시지: XML 디지털 서명의 유효성을 검사할 수 없습니다."
description: ADFS에 성공적으로 연결할 수 없습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# 오류 메시지: XML 디지털 서명의 유효성을 검사할 수 없습니다.

## 문제

ADFS에 성공적으로 연결할 수 없습니다.

![error_message.png](assets/error-message.png)

>[!NOTE]
>
>성공적인 테스트 연결을 설정하고 여전히 문제가 발생하는 경우 잘못된 속성 매핑이나 페더레이션 ID에 문제가 있을 수 있습니다. 고객 지원에 문의

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

## 원인 1: 인증서가 잘못되었습니다.

### 솔루션

ADFS 서버에서 서명 인증서를 수동으로 검색합니다.

1. in [!DNL Windows]를 클릭합니다. **[!UICONTROL 시작]** > **[!UICONTROL 관리]** > **[!UICONTROL ADFS 2.0 관리]**.\
   ADFS 2.0 관리 대화 상자가 표시됩니다.

1. 선택 **[!UICONTROL 트러스트 관계]** > **[!UICONTROL 신뢰 당사자 트러스트]** 왼쪽 창에 있습니다.

1. 마우스 오른쪽 단추 클릭 **[!UICONTROL 신뢰 당사자 트러스트]**, 을(를) 선택하고 을(를) 선택합니다. **[!UICONTROL 속성]**.

1. 을(를) 클릭합니다. **[!UICONTROL 서명]** 탭.
1. 서명 인증서 이름을 클릭하고 **[!UICONTROL 보기]**.
1. Copy to 클릭 **[!UICONTROL 파일]**... 을(를) 선택하고 을(를) 선택합니다. **[!UICONTROL 다음]**.

1. 선택 **[!UICONTROL Base-64 인코딩 x.509(CER)]**&#x200B;를 클릭하고 **[!UICONTROL 다음]**.

1. 파일 이름을 지정하고 **[!UICONTROL 다음]**.
1. 클릭 **[!UICONTROL 완료]**.
1. in [!DNL Adobe Workfront], 다음 위치로 이동합니다. **[!UICONTROL 설정]** > **[!UICONTROL 시스템]** > **[!UICONTROL 단일 사인온(SSO)]** 서명 인증서를 수동으로 업로드합니다.

## 원인 2: 다음 경우에 DSA를 사용하여 인증서가 서명됩니다. [!DNL Workfront] RSA 서명이 필요합니다.

### 솔루션

인증서를 다시 만들고 DSA 대신 RSA 서명을 사용하십시오.

## 원인 3: XML 데이터가 잘못되었습니다.

### 솔루션

ADFS 관리 시스템에서 XML 메타데이터를 다시 내보내고 다시 가져옵니다.

## 원인 4: SAML 측의 오류로 인해 요청을 수행할 수 없습니다

### 솔루션

SAML 공급자에게 문의하십시오.
