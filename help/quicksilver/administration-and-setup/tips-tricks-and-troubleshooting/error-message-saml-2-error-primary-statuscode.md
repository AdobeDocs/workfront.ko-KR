---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '오류 메시지: SAML 2.0 오류: 기본 StatusCode'
description: ADFS에 성공적으로 연결할 수 없습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 1%

---

# 오류 메시지: SAML 2.0 오류: 기본 StatusCode

## 문제

ADFS에 성공적으로 연결할 수 없습니다.

![SAML_2.0_Error_Primary_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

>[!NOTE]
>
>성공적인 테스트 연결을 설정했지만 여전히 문제가 발생하는 경우 잘못된 속성 매핑이나 페더레이션 ID에 문제가 발생할 수 있습니다. 문의 사항은 고객 지원 센터에 문의하십시오.

## 액세스 요구 사항

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
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>[!DNL Workfront] 관리자여야 합니다. 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>를 참조하십시오.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 원인 1: 보안 해시 알고리즘이 SHA-256으로 설정됨

### 솔루션

1. Windows에서는 **[!UICONTROL 시작]** > **[!UICONTROL 관리]** > **[!UICONTROL ADFS 2.0 관리]**&#x200B;를 클릭합니다.\
   [ADFS 2.0 관리] 대화 상자가 표시됩니다.

1. 왼쪽 창에서 **[!UICONTROL 트러스트 관계]** > **[!UICONTROL 신뢰 당사자 트러스트]**&#x200B;를 선택합니다.

1. [!DNL Adobe Workfront]과(와) 관련된 신뢰 당사자 트러스트를 마우스 오른쪽 단추로 클릭한 다음 **[!UICONTROL 속성]**&#x200B;을 선택합니다.
1. **[!UICONTROL 고급]** 탭을 클릭한 다음 **[!UICONTROL 보안 해시 알고리즘]** 드롭다운 메뉴에서 **[!UICONTROL SHA-1]**&#x200B;을(를) 선택합니다.\
   ![](assets/1-350x287.png)

## 원인 2: ADFS 서명 인증서가 곧 만료되며 날짜가 겹치는 새 인증서로 대체되었습니다.

### 솔루션

[!DNL Workfront] SSO 설정 페이지에 인증서 만료 날짜가 나열됩니다. 인증서가 곧 만료되는 경우 ADFS 서버에서 새 서명 인증서를 수동으로 가져와야 합니다.

1. Windows에서는 **[!UICONTROL 시작]** > **[!UICONTROL 관리]** > **[!UICONTROL ADFS 2.0 관리]**&#x200B;를 클릭합니다.\
   [ADFS 2.0 관리] 대화 상자가 표시됩니다.

1. 왼쪽 창에서 **[!UICONTROL 트러스트 관계]** > **[!UICONTROL 신뢰 당사자 트러스트]**&#x200B;를 선택합니다.

1. [!DNL Workfront]과(와) 관련된 신뢰 당사자 트러스트를 마우스 오른쪽 단추로 클릭하고 **[!UICONTROL 속성]**&#x200B;을 선택합니다.
1. **[!UICONTROL 서명]** 탭을 클릭합니다.
1. 서명 인증서의 이름을 클릭하고 **[!UICONTROL 보기]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 파일]**&#x200B;에 복사... 를 클릭하고 **[!UICONTROL 다음]**&#x200B;을 선택합니다.

1. **[!UICONTROL Base-64 인코딩 x.509(CER)]**&#x200B;을(를) 선택하고 **[!UICONTROL 다음]**&#x200B;을 클릭합니다.

1. 파일 이름을 지정하고 **[!UICONTROL 다음]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 마침]**&#x200B;을 클릭합니다.
1. [!DNL Workfront]에서 **[!UICONTROL 설정]** > **[!UICONTROL 시스템]** > **[!UICONTROL SSO(Single Sign-On)]**&#x200B;로 이동하여 서명 인증서를 수동으로 업로드하십시오.

## 원인 3: 인증서 해지 확인 실패

이에 대한 해결 방법은 사용 중인 [!DNL Microsoft] ADFS의 버전에 따라 다릅니다. 버전에 적합한 명령을 구하려면 [!DNL Microsoft]의 설명서를 참조하십시오.
