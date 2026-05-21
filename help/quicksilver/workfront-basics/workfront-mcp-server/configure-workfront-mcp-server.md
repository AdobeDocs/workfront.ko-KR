---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP 서버 구성
description: 자연어 대화를 통해 Workfront과 작업할 수 있도록 Workfront 인스턴스 및 AI 아젠틱 플랫폼을 구성합니다.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 98d5b93bcb99c468de2ad107a2aca3a9a1995429
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 0%

---


# Adobe Workfront MCP 서버 구성

[!DNL Adobe Workfront] MCP 서버를 사용하면 Claude 또는 ChatGPT와 같은 지원되는 AI 에이전트 플랫폼에서 자연어 대화를 통해 Workfront 데이터로 작업할 수 있습니다.

AI 에이전트 플랫폼을 Workfront에 연결하려면 먼저 Workfront 관리자가 Workfront 인스턴스에서 MCP 서버 액세스를 활성화해야 합니다. AI 아젠틱 플랫폼을 연결하는 정확한 단계는 지원되는 AI 아젠틱 플랫폼마다 다릅니다.

Workfront MCP 서버에 대한 자세한 내용은 [Adobe Workfront MCP 서버 개요](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md)를 참조하십시오.

## 지원되는 AI 에이전트 플랫폼

Workfront MCP 서버는 현재 다음 AI 에이전트 플랫폼을 지원합니다.

* [!DNL Claude]
* [!DNL ChatGPT]

## 전제 조건

Workfront을 AI 에이전트 플랫폼에 연결하기 전에 다음을 수행해야 합니다.

* 작업할 데이터에 액세스할 수 있는 권한이 있는 활성 [!DNL Adobe Workfront] 계정이 있습니다.
* [!DNL Claude]과(와) 같은 AI 에이전트 플랫폼에 액세스할 수 있습니다.

### 관리자 사전 요구 사항

MCP 서버 액세스는 두 명의 별도 관리자에 의해 제어됩니다.

* **Workfront 관리자**&#x200B;가 Workfront 인스턴스에 대한 MCP 서버 액세스를 제어합니다. 액세스는 시스템 기본 설정에서 기본적으로 활성화되어 있으므로 관리자가 비활성화하도록 선택하지 않은 경우 별도의 작업이 필요하지 않습니다. <!-- TODO: link to the System Preferences AI preferences article once the Enable MCP toggle is documented there. -->

* 엔터프라이즈 버전의 AI 에이전트 플랫폼을 사용하는 경우 해당 플랫폼의 관리자가 조직에 대해 [!DNL Adobe Workfront] 커넥터를 사용하도록 설정해야 합니다.


## Workfront을 클로드에 연결

[!DNL Claude] 계정당 Workfront에 한 번 연결합니다. 연결은 특정 Workfront 인스턴스에 대해 귀하를 인증하며 연결을 끊도록 선택할 때까지 연결된 상태를 유지합니다.

### connectors 디렉터리에서 연결

+++ 를 확장하여 Workfront을 [!DNL Claude]에 연결하는 단계별 지침을 봅니다.

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

+++

### URL로 연결

+++ 를 확장하여 URL을 사용하여 Workfront을 [!DNL Claude]에 연결하는 단계별 지침을 봅니다.

URL을 사용하여 Workfront을 [!DNL Claude]에 연결하려면 다음을 수행하십시오.

1. 자격 증명을 사용하여 [Cloud](https://claude.ai)에 로그인합니다.
1. 왼쪽 메뉴에서 **사용자 지정** 아이콘을 선택합니다.
1. **커넥터**&#x200B;를 선택한 다음 **+** 아이콘을 선택하여 커넥터를 추가합니다.
1. **앱 만들기** 단추를 선택합니다.
1. 커넥터에 원하는 이름(예: &quot;Workfront&quot;)을 지정하고 원하는 MCP 서버 URL `https://mcp.workfront.adobe.com/mcp/v1/workfront`을(를) 입력하십시오.

1. 커넥터가 생성되면 로그인 창이 나타납니다. Adobe ID 자격 증명을 사용하여 인증합니다. 둘 이상에 속해 있는 경우 원하는 Workfront 인스턴스를 선택해야 합니다.

+++

### 스킬을 사용하여 클라우드 동작 사용자 지정

[!DNL Claude]은(는) 스킬이라는 사용자가 만든 명령 집합을 지원합니다. 스킬을 사용하여 [!DNL Claude]이(가) Workfront에서 작동하는 방식을 사용자 지정할 수 있습니다. 예를 들어 이전 결과에 의존하는 대신 [!DNL Claude]에서 항상 Workfront의 새 데이터를 가져오도록 지시하는 스킬을 만들 수 있습니다.

[!DNL Claude] 스킬에 대한 자세한 내용은 [클라우드 사용 설명서](https://code.claude.com/docs/en/skills)를 참조하거나 클라우드에 스킬에 대한 도움을 요청하세요.

## ChatGPT에 연결

1. 자격 증명을 사용하여 [ChatGPT](https://chatgpt.com)에 로그인합니다.
1. 왼쪽 아래에서 **설정**→ **사용자 이름**&#x200B;을 선택합니다.
1. **앱**&#x200B;을 선택한 다음 **개발자 모드**&#x200B;를 사용하도록 설정합니다.
1. **앱 만들기** 단추를 선택합니다.
1. 앱에 원하는 이름(예: &quot;Workfront&quot;)을 지정하고 원하는 MCP 서버 URL을 입력하십시오. `https://mcp.workfront.adobe.com/mcp/v1/workfront`
1. 인증이 **OAuth**(기본적으로 설정됨)로 설정되어 있는지 확인하고 계속하려면 수락 확인란을 선택하십시오.
1. 앱이 생성되면 로그인 창이 나타납니다. Adobe ID 자격 증명을 사용하여 인증합니다. 둘 이상에 속해 있는 경우 원하는 Workfront 인스턴스를 선택해야 합니다.

### 사용자 지정 GPT로 ChatGPT 동작 사용자 지정

ChatGPT는 사용자 지정 GPT라는 사용자가 만든 도우미를 지원합니다. 사용자 지정 GPT를 사용하여 ChatGPT가 커넥터와 어떻게 동작하는지 사용자 지정할 수 있습니다. 예를 들어 이전 결과에 의존하는 대신 ChatGPT가 연결된 서비스에서 항상 새로운 데이터를 가져오도록 지시하는 사용자 지정 GPT를 만들 수 있습니다.

사용자 지정 GPT에 대한 자세한 내용은 [ChatGPT 사용자 설명서](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts)를 참조하거나 ChatGPT에 사용자 지정 GPT에 대한 도움을 요청하세요.

## 연결 확인

AI 아젠틱 플랫폼이 Workfront에 연결되어 있는지 확인하려면 AI 아젠틱 플랫폼에 Workfront MCP 서버가 사용할 수 있는 작업을 나열해 달라고 요청합니다. 예:

* *수행할 수 있는 Workfront 작업은 무엇입니까?*
* *액세스 권한이 있는 Workfront 도구를 나열합니다.*

[Adobe Workfront MCP 서버 도구](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md)에서 전체 도구 목록을 볼 수도 있습니다.

## 사용 가능한 도구

Workfront MCP 서버는 연결된 AI 에이전트 플랫폼이 사용자를 대신하여 호출하는 도구 세트(예: Workfront을 검색하고, 항목을 만들고, 필드를 업데이트하고, 승인을 관리하는 도구)를 노출합니다. Workfront 영역별로 그룹화된 전체 참조 목록은 [Adobe Workfront MCP 서버 도구](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md)를 참조하십시오.

## 다른 Workfront 인스턴스로 전환

각 연결은 AI 에이전트 플랫폼을 단일 Workfront 인스턴스로 인증합니다. 다른 인스턴스를 사용하려면 연결을 끊고 다시 연결합니다.

다른 Workfront 인스턴스에 연결하려면 다음 작업을 수행하십시오.

1. AI 에이전트 플랫폼에서 Workfront MCP 서버의 연결을 끊습니다.
1. 커넥터를 다시 연결합니다.
1. 새 Workfront 인스턴스 인증

>[!NOTE]
>
>로그아웃만 해도 Workfront 인스턴스는 전환되지 않습니다. 커넥터의 연결을 끊고 다시 연결해야 합니다.

<!--

## Connect to Gemini

>[!IMPORTANT]
>
>You must be an administrator on the Gemini platform to set up the MCP server. If you aren't an administrator, share these instructions with your administrator so they can set up the connection for you.


To set up the connection between Gemini and the Workfront MCP server, follow the instructions provided by Google for [connecting Gemini to external tools using MCP](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/custom-mcp-server/set-up-custom-mcp-server). 

When prompted for the MCP Server URL, enter the following URL for your Workfront MCP server: `https://mcp.workfront.adobe.com/mcp/v1/workfront`
-->

<!--
## Connect to Microsoft Copilot

✅ 1) Copilot Studio (most common for agents / enterprise use)
This is the cleanest "paste a URL" flow.
Steps
1. Open your Copilot Studio agent
2. Go to Tools
3. Click:
    * Add a tool → New tool → Model Context Protocol
4. In the wizard, fill in:
    * Server name (anything)
    * Server description
    * ✅ Server URL (your MCP endpoint)
5. Choose auth (if needed):
    * None / API key / OAuth
6. Click Create
👉 That's it—your MCP server is now attached to the agent.
This flow is explicitly documented:
* You add MCP via Tools → Add tool → Model Context Protocol
* Then provide Server name, description, and URL ￼
￼
What happens next
* Copilot discovers tools automatically from the MCP server
* You can enable/disable tools per agent
* The agent calls them when relevant

-->

## 설정 및 인증 문제 해결

+++ 를 확장하여 Workfront MCP 서버의 설정 및 인증에 대한 문제 해결 팁을 봅니다.

| 문제 | 가능한 원인 | 고정 |
|---|---|---|
| [!DNL Claude]에서 [!DNL Adobe Workfront] 커넥터를 찾을 수 없습니다. | [!DNL Claude] 관리자가 활성화하지 않았습니다. | [!DNL Claude] 관리자(Workfront 관리자 아님)에게 연락하여 [!DNL Adobe Workfront] 커넥터를 사용하도록 요청하십시오. |
| 연결했지만 데이터를 볼 수 없습니다. | 잘못된 Workfront 인스턴스를 인증했습니다. | 커넥터 연결을 끊고 다시 연결한 다음 올바른 인스턴스를 인증합니다. |
| 인증에 실패했거나 연결 작동이 중지되었습니다. | 인증 세션이 만료되었거나 연결 오류가 발생했습니다. | 커넥터를 분리하고 다시 연결합니다. |
| 다른 Workfront 인스턴스로 전환하려고 합니다. | 단일 연결이 사용자를 하나의 인스턴스로 연결합니다. | 새 인스턴스의 연결을 끊고, 다시 연결하고, 인증합니다. |
| Workfront에 연결할 수 없거나 MCP 서버 액세스가 비활성화되었다는 메시지가 표시됩니다. | Workfront 관리자가 인스턴스에 대한 MCP 서버 액세스를 해제했습니다. | Workfront 관리자에게 문의하여 시스템 환경 설정에서 MCP 서버 액세스를 활성화하도록 요청하십시오. |

<!-- NEEDS DETAIL: Add additional setup/authentication troubleshooting scenarios discovered during hands-on testing. -->

연결 후 발생하는 일상적인 문제 해결(예: 부실 결과나 예기치 않은 동작)에 대해서는 [Adobe Workfront MCP 서버 사용](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)을 참조하십시오.


+++


<!--
+++

## Frequently asked questions about setup

+++ Expand to view frequently asked questions about setting up the Workfront MCP server.

### Can I connect to multiple Workfront instances at once?

No. Each connection ties an AI agentic platform to a single Workfront instance. To switch, disconnect and reconnect, authenticating to the new instance.

### Which administrator enables this?

Both your Workfront administrator and the administrator for your AI agentic platform. Your Workfront administrator enables MCP server access on the Workfront side. The administrator for your AI agentic platform enables Workfront access on that platform's side. For [!DNL Claude], the [!DNL Claude] Enterprise administrator enables the [!DNL Adobe Workfront] connector.

+++

-->