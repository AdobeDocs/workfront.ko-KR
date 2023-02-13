---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Microsoft Exchange에서 POP 구성
description: 의 POP 이메일 계정 [!DNL Microsoft Exchange] 이 비활성화되어 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# POP 입력 구성 [!DNL Microsoft Exchange]

## 문제

의 POP 이메일 계정 [!DNL Microsoft Exchange] 이 비활성화되어 있습니다.

## 솔루션

문제를 해결하는 데 시간을 보내기 전에 사용자의 POP 계정이 제대로 구성되어 있는지 확인하십시오. POP 계정이 올바르게 구성되었는지 확인한 후 문제가 계속 발생하면 [!DNL Microsoft] 추가 지원을 받으려면 파트너 중 한 명을 지원하십시오.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

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

## POP 입력 구성 [!DNL Microsoft Exchange]

>[!NOTE]
>
>다음 단계는 POP을 구성하기 위한 일반 안내서로 사용할 수 있습니다 [!DNL Microsoft Exchange] 제작 [!DNL Workfront] 시스템. 단계는 Exchange 버전 또는 Microsoft에서 수행한 코드 변경 사항에 따라 크게 다를 수 있습니다.

1. Exchange 2010 서버에서 POP3 서비스를 시작하고 활성화합니다.

   >[!NOTE]
   >
   >기본적으로 POP3 서비스는 시작되지 않습니다.

   1. 시작 [!DNL Microsoft]의 서버 관리자.
   1. 탐색: **[!UICONTROL 서버 관리자]** > **[!UICONTROL 구성]** >**[!UICONTROL 고급 보안이 적용된 Windows 방화벽]** > **[!UICONTROL 서비스]**.

   1. 마우스 오른쪽 단추 클릭 **[!DNL Microsoft Exchange]POP3**&#x200B;를 클릭한 다음 **[!UICONTROL 속성]**.

   1. (조건부) POP 서비스가 자동으로 시작되도록 하려면 **[!UICONTROL 일반]** 탭에서 설정합니다. **[!UICONTROL 시작]** 유형 [!UICONTROL 자동].

1. 서버의 POP3을 구성합니다.

   1. 시작 [!DNL Microsoft Exchange] 관리 콘솔.
   1. 탐색: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL 서버 구성]** > **[!UICONTROL 클라이언트 액세스]**.

   1. 선택 **[!UICONTROL POP3]**.

      POP3은 [!UICONTROL POP3] 및 [!UICONTROL IMAP4] 탭.

   1. 오른쪽 아래 **[!UICONTROL 작업]**, 선택 **[!UICONTROL POP3]**, 그런 다음 **[!UICONTROL 속성]**.

   1. 클릭 **[!UICONTROL POP3 속성]**&#x200B;를 열고 **[!UICONTROL 바인딩]** 탭.

      POP3 서버에 대해 구성된 사용 가능한 모든 IP 주소와 포트 번호가 표시됩니다. 상단 상자에는 암호화되지 않음 이 표시되고 하단 상자에는 SSL/TLS 연결에 대한 IP 및 포트가 표시됩니다.

   1. 클릭 **[!UICONTROL POP3 속성]**&#x200B;를 열고 **[!UICONTROL 인증]** 탭.

   1. **[!UICONTROL 보안 선택]** 로그인.

      클라이언트가 서버를 인증하려면 TLS 연결이 필요합니다.

1. 사용자가 POP에 연결할 수 있도록 하거나 허용합니다.

   1. 시작 [!DNL Microsoft Exchange] 관리 콘솔.
   1. 탐색: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL 수신자 구성]** > **[!UICONTROL 사서함]**.

      사서함 또는 사용자 목록이 표시됩니다.

   1. 내에서 사용되는 이메일을 강조 표시합니다 [!DNL Workfront].
   1. 오른쪽 아래 **[!UICONTROL 작업]**, 선택 **[!UICONTROL 속성]**&#x200B;를 열고 **[!UICONTROL 사서함 기능]** 탭.

   1. (조건부) POP3이 비활성화되어 있으면 **[!UICONTROL POP3]**&#x200B;를 클릭한 다음 **[!UICONTROL 활성화]**.

      사서함 또는 사용자 목록이 표시됩니다.

1. 수신 커넥터를 구성합니다.

   1. 시작 [!DNL Microsoft Exchange] 관리 콘솔.
   1. 탐색: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL 서버 구성]** > **[!UICONTROL 허브 전송]**.

      수신 커넥터 목록이 표시됩니다.

   1. 수신 커넥터 확인 *클라이언트* *EX01* 이 활성화되어 있습니다.

      위치 *클라이언트* *EX01* 은 Exchange 서버의 이름입니다.

   1. 선택 *클라이언트 EX01*&#x200B;을 클릭한 다음 오른쪽의 **[!UICONTROL 작업]**, 선택 **[!UICONTROL 속성]**.

   1. 를 엽니다. **[!UICONTROL 인증]** 탭을 클릭한 다음 **[!UICONTROL TLS(전송 계층 보안)]** 이(가) 선택되어 있습니다.

      >[!NOTE]
      >
      >기본 인증을 받으려면 TLS 및 통합 Windows 인증을 시작해야 할 수 있습니다.
