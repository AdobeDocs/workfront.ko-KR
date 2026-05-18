---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP 서버 구성
description: 자연어 대화를 통해 Workfront과 작업할 수 있도록 Workfront 인스턴스 및 AI 비서를 구성합니다.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 4517d45ecc653d27d435a8192a612241120dd33f
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 3%

---


# Adobe Workfront MCP 서버 구성

[!DNL Adobe Workfront] MCP 서버를 사용하면 Claude 또는 ChatGPT와 같은 지원되는 AI 도우미에서 자연어 대화를 통해 Workfront 데이터로 작업할 수 있습니다.

AI 도우미를 Workfront에 연결하려면 먼저 Workfront 관리자가 Workfront 인스턴스에서 MCP 서버 액세스를 활성화해야 합니다. AI 비서를 연결하는 정확한 단계는 지원되는 각 AI 비서에 따라 다릅니다.

Workfront MCP 서버에 대한 자세한 내용은 [Adobe Workfront MCP 서버 개요](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md)를 참조하십시오.

## 지원되는 AI 지원

Workfront MCP 서버는 현재 다음 AI 도우미를 지원합니다.

* [!DNL Claude]

<!-- NEEDS DETAIL: Update this list as Adobe adds support for additional AI assistants (for example, [!DNL Gemini], or [!DNL Microsoft Copilot]). -->

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td><p><!-- NEEDS DETAIL: Confirm Workfront package requirement (Select, Prime, Ultimate, Any?) --></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p><!-- NEEDS DETAIL: Confirm Workfront license requirement (Standard, Work, etc.) --></p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

Workfront을 AI 어시스턴트에 연결하기 전에 다음을 수행해야 합니다.

* 작업할 데이터에 액세스할 수 있는 권한이 있는 활성 [!DNL Adobe Workfront] 계정이 있습니다.
* [!DNL Claude] 같은 AI 도우미에 액세스할 수 있습니다.

  <!-- NEEDS DETAIL: Confirm which Claude tiers are supported. Claude Enterprise is confirmed; Claude Pro and Claude Team support is unconfirmed. -->

### 관리자 사전 요구 사항

MCP 서버 액세스는 두 명의 별도 관리자에 의해 제어됩니다. 연결하려면 먼저 두 권한 모두 액세스 권한을 활성화해야 합니다.

* **Workfront 관리자**&#x200B;가 Workfront 인스턴스에서 MCP 서버 액세스를 사용하도록 설정해야 합니다.

* 엔터프라이즈 버전의 AI Assistant를 사용하는 경우 AI Assistant 관리자가 조직에 대해 [!DNL Adobe Workfront] 커넥터를 활성화해야 합니다.


## Workfront을 클로드에 연결

[!DNL Claude] 계정당 Workfront에 한 번 연결합니다. 연결은 특정 Workfront 인스턴스에 대해 귀하를 인증하며 연결을 끊도록 선택할 때까지 연결된 상태를 유지합니다.


>[!IMPORTANT]
>
>[!DNL Claude] Enterprise를 사용하는 경우 **[!DNL Claude] Enterprise 관리자**&#x200B;가 조직에 대해 [!DNL Adobe Workfront] 커넥터를 사용하도록 설정해야 합니다. [!DNL Claude]에서 검색할 때까지 [!DNL Adobe Workfront] 커넥터가 표시되지 않습니다. 먼저 [!DNL Claude] 관리자에게 문의하십시오.


Workfront을 [!DNL Claude]에 연결하려면:

1. [!DNL Claude] 열기

1. 커넥터 영역으로 이동합니다.

   <!-- NEEDS DETAIL: Exact menu path (for example, "Click Settings, then click Connectors"). -->

1. 커넥터 목록에서 **[!DNL Adobe Workfront]**&#x200B;을(를) 찾습니다.

   표시되지 않으면 이 문서에서 [관리자 필수 구성 요소](#admin-prerequisites)를 참조하십시오.

1. **연결**&#x200B;을 클릭합니다.

   <!-- NEEDS DETAIL: Confirm the exact button label. -->

1. 메시지가 표시되면 Workfront 인스턴스에 로그인합니다.

   <!-- NEEDS DETAIL: Describe the auth flow — does it open a new browser tab, an in-app window, prompt for a Workfront domain? -->

1. 인증이 완료되면 연결됩니다.

   <!-- NEEDS DETAIL: Add a screenshot of the connected state in Claude. -->

### 연결 확인

[!DNL Claude]이(가) Workfront에 연결되어 있는지 확인하려면 [!DNL Claude]에게 Workfront MCP 서버에서 사용할 수 있는 작업을 나열하도록 요청하십시오. 예:

* *수행할 수 있는 Workfront 작업은 무엇입니까?*
* *액세스 권한이 있는 Workfront 도구를 나열합니다.*

[!DNL Claude]이(가) 사용 가능한 작업 목록을 반환합니다.

<!-- NEEDS DETAIL: Add a screenshot of the tool-list response. -->

### 다른 Workfront 인스턴스로 전환

각 연결은 단일 Workfront 인스턴스에 대해 [!DNL Claude]을(를) 인증합니다. 다른 인스턴스를 사용하려면 연결을 끊고 다시 연결합니다.

다른 Workfront 인스턴스에 연결하려면 다음 작업을 수행하십시오.

1. [!DNL Claude]에서 [!DNL Adobe Workfront] 커넥터의 연결을 끊습니다.
1. 커넥터를 다시 연결합니다.
1. 새 Workfront 인스턴스 인증

>[!NOTE]
>
>[!DNL Claude]에서 로그아웃해도 Workfront 인스턴스가 전환되지 않습니다. 커넥터의 연결을 끊고 다시 연결해야 합니다.

## 스킬을 사용하여 클라우드 동작 사용자 지정

<!-- NEEDS DETAIL: Confirm whether Adobe is shipping any pre-built Claude skills alongside the MCP server. If yes, list them and link to download or installation guidance. If no, decide whether to mention skills as a user-driven workaround at all, or remove this section. -->

[!DNL Claude]은(는) 스킬이라는 사용자가 만든 명령 집합을 지원합니다. 스킬을 사용하여 [!DNL Claude]이(가) Workfront에서 작동하는 방식을 사용자 지정할 수 있습니다. 예를 들어 이전 결과에 의존하는 대신 [!DNL Claude]에서 항상 Workfront의 새 데이터를 가져오도록 지시하는 스킬을 만들 수 있습니다.

## 설정 및 인증 문제 해결

| 문제 | 가능한 원인 | 고정 |
|---|---|---|
| [!DNL Claude]에서 [!DNL Adobe Workfront] 커넥터를 찾을 수 없습니다. | [!DNL Claude] 관리자가 활성화하지 않았습니다. | [!DNL Claude] 관리자(Workfront 관리자 아님)에게 연락하여 [!DNL Adobe Workfront] 커넥터를 사용하도록 요청하십시오. |
| 연결했지만 데이터를 볼 수 없습니다. | 잘못된 Workfront 인스턴스를 인증했습니다. | 커넥터 연결을 끊고 다시 연결한 다음 올바른 인스턴스를 인증합니다. |
| 인증에 실패했거나 연결 작동이 중지되었습니다. | 인증 세션이 만료되었거나 연결 오류가 발생했습니다. | 커넥터를 분리하고 다시 연결합니다. |
| 다른 Workfront 인스턴스로 전환하려고 합니다. | 단일 연결이 사용자를 하나의 인스턴스로 연결합니다. | 새 인스턴스의 연결을 끊고, 다시 연결하고, 인증합니다. |

<!-- NEEDS DETAIL: Add additional setup/authentication troubleshooting scenarios discovered during hands-on testing. -->

연결 후 발생하는 일상적인 문제 해결(예: 부실 결과나 예기치 않은 동작)에 대해서는 [Adobe Workfront MCP 서버 사용](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)을 참조하십시오.

## 설정에 대한 FAQ

### 여러 Workfront 인스턴스에 한 번에 연결할 수 있습니까?

아니요. 각 연결은 AI 도우미를 단일 Workfront 인스턴스에 연결합니다. 전환하려면 연결을 끊고 다시 연결하여 새 인스턴스를 인증합니다.

### 이는 Claude Pro 또는 Claude Team 또는 Claude Enterprise에서만 작동합니까?

<!-- NEEDS DETAIL: Confirm Claude tier support and answer this directly. -->

### 어느 관리자가 이 기능을 활성화합니까?

Workfront 관리자와 AI 관리자 둘 다. Workfront 관리자는 Workfront 측에서 MCP 서버 액세스를 활성화합니다. AI 비서 관리자가 AI 비서 측에서 Workfront 액세스를 활성화합니다. [!DNL Claude]의 경우 [!DNL Claude] Enterprise 관리자가 [!DNL Adobe Workfront] 커넥터를 사용하도록 설정합니다.
