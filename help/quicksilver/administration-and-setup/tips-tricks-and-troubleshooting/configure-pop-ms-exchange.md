---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Microsoft Exchange에서 POP 구성
description: ' [!DNL Microsoft Exchange] 의 POP 전자 메일 계정을 사용할 수 없습니다.'
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# [!DNL Microsoft Exchange]에서 POP 구성

## 문제

[!DNL Microsoft Exchange]에서 POP 전자 메일 계정을 사용할 수 없습니다.

## 솔루션

문제 해결에 시간을 보내기 전에 사용자의 POP 계정이 제대로 구성되어 있는지 확인하십시오. POP 계정이 올바르게 구성되어 있는지 확인한 후에도 문제가 계속 발생하면 [!DNL Microsoft] 지원 팀이나 파트너 중 한 명에게 추가 지원을 요청하십시오.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

## 액세스 요구 사항

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
   <td>[!UICONTROL 시스템 관리자]</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## [!DNL Microsoft Exchange]에서 POP 구성

>[!NOTE]
>
>다음 단계는 프로덕션 [!DNL Workfront] 시스템에 대해 [!DNL Microsoft Exchange]에서 POP를 구성하기 위한 일반 안내서로 사용할 수 있습니다. 단계는 Exchange 버전이나 Microsoft에서 수행한 코드 변경 사항에 따라 크게 다를 수 있습니다.

1. Exchange 2010 서버에서 POP3 서비스를 시작하고 활성화합니다.

   >[!NOTE]
   >
   >기본적으로 POP3 서비스는 시작되지 않습니다.

   1. [!DNL Microsoft]의 서버 관리자를 시작합니다.
   1. **[!UICONTROL 서버 관리자]** > **[!UICONTROL 구성]** >**[!UICONTROL 고급 보안이 포함된 Windows 방화벽]** > **[!UICONTROL 서비스]**&#x200B;로 이동합니다.

   1. **[!DNL Microsoft Exchange]POP3**&#x200B;을(를) 마우스 오른쪽 단추로 클릭한 다음 **[!UICONTROL 속성]**&#x200B;을 클릭합니다.

   1. (조건부) POP 서비스가 자동으로 시작되도록 하려면 **[!UICONTROL 일반]** 탭에서 **[!UICONTROL 시작]** 유형을 [!UICONTROL 자동](으)로 설정합니다.

1. 서버용 POP3를 구성합니다.

   1. [!DNL Microsoft Exchange] 관리 콘솔을 시작합니다.
   1. [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL 서버 구성]** > **[!UICONTROL 클라이언트 액세스]**&#x200B;로 이동합니다.

   1. **[!UICONTROL POP3]**&#x200B;을(를) 선택하십시오.

      POP3은 [!UICONTROL POP3] 및 [!UICONTROL IMAP4] 탭 아래 목록에 있습니다.

   1. **[!UICONTROL 작업]** 아래의 오른쪽에서 **[!UICONTROL POP3]**&#x200B;을 선택한 다음 **[!UICONTROL 속성]**&#x200B;을 선택하십시오.

   1. **[!UICONTROL POP3 속성]**&#x200B;을 클릭한 다음 **[!UICONTROL 바인딩]** 탭을 엽니다.

      POP3 서버에 대해 구성된 사용 가능한 모든 IP 주소 및 포트 번호가 표시됩니다. 상단 상자에는 암호화되지 않은 IP가 표시되고 하단 상자에는 SSL/TLS 연결을 위한 IP 및 포트가 표시됩니다.

   1. **[!UICONTROL POP3 속성]**&#x200B;을 클릭한 다음 **[!UICONTROL 인증]** 탭을 엽니다.

   1. **[!UICONTROL 보안]** 로그인을 선택하십시오.

      클라이언트가 서버를 인증하려면 TLS 연결이 필요합니다.

1. POP에 연결할 수 있도록 설정하거나 허용합니다.

   1. [!DNL Microsoft Exchange] 관리 콘솔을 시작합니다.
   1. [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL 받는 사람 구성]** > **[!UICONTROL 사서함]**&#x200B;으로 이동합니다.

      사서함 또는 사용자 목록이 표시됩니다.

   1. [!DNL Workfront] 내에서 사용 중인 전자 메일을 강조 표시합니다.
   1. **[!UICONTROL 작업]** 아래 오른쪽에서 **[!UICONTROL 속성]**&#x200B;을 선택한 다음 **[!UICONTROL 사서함 기능]** 탭을 엽니다.

   1. (조건부) POP3를 사용하지 않으려면 **[!UICONTROL POP3]**&#x200B;을 클릭한 다음 **[!UICONTROL 사용]**&#x200B;을 클릭합니다.

      사서함 또는 사용자 목록이 표시됩니다.

1. 수신 커넥터를 구성합니다.

   1. [!DNL Microsoft Exchange] 관리 콘솔을 시작합니다.
   1. [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Server 구성]** > **[!UICONTROL Hub 전송]**&#x200B;으로 이동합니다.

      수신 커넥터 목록이 표시됩니다.

   1. 수신 커넥터 *Client* *EX01*&#x200B;이(가) 활성화되었는지 확인합니다.

      여기서 *Client* *EX01*&#x200B;은(는) Exchange 서버의 이름입니다.

   1. *클라이언트 EX01*&#x200B;을(를) 선택한 다음 **[!UICONTROL 작업]** 아래 오른쪽에서 **[!UICONTROL 속성]**&#x200B;을(를) 선택하십시오.

   1. **[!UICONTROL 인증]** 탭을 연 다음 **[!UICONTROL TLS(전송 계층 보안)]**&#x200B;을(를) 확인합니다.

      >[!NOTE]
      >
      >기본 인증을 받으려면 TLS 및 통합 Windows 인증을 시작해야 할 수 있습니다.
