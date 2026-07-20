---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP 서버 구성
description: 자연어 대화를 통해 Workfront과 작업할 수 있도록 Workfront 인스턴스 및 AI 아젠틱 플랫폼을 구성합니다.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 836431c7840647b8f412f848fe22d3e64cc42e44
workflow-type: tm+mt
source-wordcount: '1588'
ht-degree: 0%

---


# Adobe Workfront MCP 서버 구성

[!DNL Adobe Workfront] MCP 서버를 사용하면 지원되는 AI 에이전트 플랫폼에서 자연어 대화를 통해 Workfront 데이터로 작업할 수 있습니다.

AI 에이전트 플랫폼을 Workfront에 연결하려면 먼저 Workfront 관리자가 Workfront 인스턴스에서 MCP 서버 액세스를 활성화해야 합니다. AI 아젠틱 플랫폼을 연결하는 정확한 단계는 지원되는 AI 아젠틱 플랫폼마다 다릅니다.

## 지원되는 AI 에이전트 플랫폼

Workfront MCP 서버는 MCP(Model Context Protocol)를 지원하는 모든 AI 에이전트 플랫폼과 작동합니다.

이 문서에서는 다음 연결 단계를 안내합니다.

* [!DNL Claude]
* [!DNL ChatGPT]

다른 MCP 호환 AI 에이전트 플랫폼(예: [!DNL Gemini] 또는 [!DNL Microsoft Copilot])을 사용하는 경우 해당 플랫폼의 설명서에 나와 있는 단계에 따라 사용자 지정 MCP 서버를 추가합니다. MCP 서버 URL을 입력하라는 메시지가 표시되면 다음을 입력합니다.

```
https://mcp.workfront.adobe.com/mcp/v1/workfront
```

## 전제 조건

Workfront을 AI 에이전트 플랫폼에 연결하기 전에 다음을 수행해야 합니다.

* 작업할 데이터에 액세스할 수 있는 권한이 있는 활성 [!DNL Adobe Workfront] 계정이 있습니다.
* [!DNL Claude]과(와) 같은 AI 에이전트 플랫폼에 액세스할 수 있습니다.
* Workfront 인스턴스는 Adobe Identity Management System(IMS)에서 활성화되어야 합니다.
* Workfront Planning에서 MCP를 사용하려면 귀사는 Adobe Workfront Planning이 포함된 Workfront 패키지에 있어야 합니다.


### 관리자 사전 요구 사항

MCP 서버 액세스는 두 명의 별도 관리자에 의해 제어됩니다.

* Workfront 관리자는 시스템 환경 설정에서 두 가지 전환을 통해 Workfront 인스턴스에 대한 MCP 서버 액세스를 제어합니다. **읽기 전용 MCP 도구**(기본적으로 활성화됨) 및 **MCP 도구 작성**(기본적으로 비활성화됨)입니다. AI 에이전트 플랫폼을 통해 Workfront 항목을 찾을 수 있지만 만들거나 업데이트하거나 삭제할 수 없는 경우 Workfront 관리자에게 쓰기 작업을 활성화하도록 요청하십시오.

  자세한 내용은 [시스템 환경 설정 구성](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)을 참조하십시오.

* 엔터프라이즈 버전의 AI 에이전트 플랫폼을 사용하는 경우 해당 플랫폼의 관리자는 조직의 [!DNL Adobe Workfront] 커넥터를 활성화하거나 Workfront MCP 서버에 연결할 수 있는 사용자 지정 URL 액세스 권한을 제공해야 합니다.


## Workfront을 클로드에 연결

[!DNL Claude] 계정당 Workfront에 한 번 연결합니다. 연결은 특정 Workfront 인스턴스에 대해 귀하를 인증하며 연결을 끊도록 선택할 때까지 연결된 상태를 유지합니다.



### 커넥터 디렉토리에서 클라우드 데스크탑에 연결

+++ 를 확장하여 Workfront을 [!DNL Claude]에 연결하는 단계별 지침을 봅니다.

Workfront을 [!DNL Claude]에 연결하려면:

1. [!DNL Claude] 열기

1. 커넥터 영역으로 이동합니다.



1. 커넥터 목록에서 **[!DNL Adobe Workfront]**&#x200B;을(를) 찾습니다.

   표시되지 않으면 이 문서에서 [관리자 필수 구성 요소](#admin-prerequisites)를 참조하십시오.

1. **연결**&#x200B;을 클릭합니다.



1. 메시지가 표시되면 Workfront 인스턴스에 로그인합니다.


1. 인증이 완료되면 연결됩니다.



+++

### URL을 사용하여 클라우드에 연결

+++ 를 확장하여 URL을 사용하여 Workfront을 [!DNL Claude]에 연결하는 단계별 지침을 봅니다.

>[!NOTE]
>
>이 절차를 수행하려면 엔터프라이즈 클라우드 환경의 소유자여야 합니다.
>
>소유자 요구 사항에 대한 Claude의 설명을 보려면 Claude 설명서에서 [사용자 지정 커넥터 추가](https://support.claude.com/en/articles/11175166-get-started-with-custom-connectors-using-remote-mcp#:~:text=Note%3A%20While,has%20access%20to)를 참조하십시오.

URL을 사용하여 Workfront을 [!DNL Claude]에 연결하려면 다음을 수행하십시오.

1. 자격 증명을 사용하여 [Cloud](https://claude.ai)에 로그인합니다.
1. 왼쪽 메뉴에서 **사용자 지정** 아이콘을 선택합니다.
1. **커넥터**&#x200B;를 선택한 다음 **+** 아이콘을 선택하여 커넥터를 추가합니다.
1. **앱 만들기** 단추를 선택합니다.
1. 커넥터에 원하는 이름(예: &quot;Workfront&quot;)을 지정하고 MCP 서버 URL을 입력합니다.

   ```
   https://mcp.workfront.adobe.com/mcp/v1/workfront
   ```

1. 커넥터를 만든 후 로그인 창이 나타납니다. Adobe ID 자격 증명을 사용하여 인증합니다. 둘 이상에 속해 있는 경우 원하는 Workfront 인스턴스를 선택해야 합니다.

+++

### 스킬을 사용하여 클라우드 동작 사용자 지정

[!DNL Claude]은(는) 스킬이라는 사용자가 만든 명령 집합을 지원합니다. 스킬을 사용하여 [!DNL Claude]이(가) Workfront에서 작동하는 방식을 사용자 지정할 수 있습니다. 예를 들어 이전 결과에 의존하는 대신 [!DNL Claude]에서 항상 Workfront의 새 데이터를 가져오도록 지시하는 스킬을 만들 수 있습니다.

[!DNL Claude] 스킬에 대한 자세한 내용은 [클라우드 사용 설명서](https://code.claude.com/docs/en/skills)를 참조하거나 클라우드에 스킬에 대한 도움을 요청하세요.

## ChatGPT에 연결

1. 자격 증명을 사용하여 [ChatGPT](https://chatgpt.com)에 로그인합니다.
1. 왼쪽 아래에서 **설정**→ **사용자 이름**&#x200B;을 선택합니다.
1. **앱**&#x200B;을 선택한 다음 **개발자 모드**&#x200B;를 사용하도록 설정합니다.
1. **앱 만들기** 단추를 선택합니다.
1. 앱에 원하는 이름(예: &quot;Workfront&quot;)을 지정하고 MCP 서버 URL을 입력합니다.

   ```
   https://mcp.workfront.adobe.com/mcp/v1/workfront
   ```

1. 인증이 **OAuth**(기본적으로 설정됨)로 설정되어 있는지 확인하고 계속하려면 수락 확인란을 선택하십시오.
1. 앱이 생성되면 로그인 창이 나타납니다. Adobe ID 자격 증명을 사용하여 인증합니다. 둘 이상에 속해 있는 경우 원하는 Workfront 인스턴스를 선택해야 합니다.


### 사용자 지정 GPT로 ChatGPT 동작 사용자 지정

ChatGPT는 사용자 지정 GPT라는 사용자가 만든 도우미를 지원합니다. 사용자 지정 GPT를 사용하여 ChatGPT가 커넥터와 어떻게 동작하는지 사용자 지정할 수 있습니다. 예를 들어 이전 결과에 의존하는 대신 ChatGPT가 연결된 서비스에서 항상 새로운 데이터를 가져오도록 지시하는 사용자 지정 GPT를 만들 수 있습니다.

사용자 지정 GPT에 대한 자세한 내용은 [ChatGPT 사용자 설명서](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts)를 참조하거나 ChatGPT에 사용자 지정 GPT에 대한 도움을 요청하세요.

## Workfront을 Copilot에 연결

Workfront MCP가 연결할 수 있는 사용자 지정 Copilot 에이전트를 빌드하려면 Copilot Studio를 사용합니다.

1. Copilot Studio에서 **빈 에이전트 만들기**&#x200B;를 클릭합니다.
1. 에이전트 이름을 지정하고 **만들기**를 클릭합니다.
에이전트 창이 열립니다.

1. **지침** 필드에서 에이전트에서 수행할 작업을 설명합니다. 프로세스 및 Workfront 사용 방법과 같은 정보를 포함합니다. 세부 정보를 많이 제공하는 것이 좋습니다.
1. 위쪽 탐색에서 **도구**&#x200B;를 클릭한 다음 **도구 추가**&#x200B;를 클릭합니다.
1. **모델 컨텍스트 프로토콜** 타일을 선택하십시오.
1. 표시되는 패널에서 이 연결의 이름과 설명을 입력합니다.
1. 서버 URL 필드에 URL을 입력합니다.

```
https://mcp.workfront.adobe.com/mcp/v1/workfront`
```

1. 인증을 받으려면 **OAuth 2.0**&#x200B;을 선택한 다음 **동적 검색**&#x200B;을 선택하십시오.
1. 패널 하단의 **만들기**&#x200B;를 클릭합니다.

   앱이 등록되었습니다.

1. 앱이 등록되면 나타나는 패널에서 **연결되지 않음**&#x200B;을 클릭한 다음 **새 연결 만들기**&#x200B;를 클릭하고 **만들기**&#x200B;를 클릭합니다.
1. 표시되는 로그인 패널에서 Workfront에 로그인한 다음 사용할 Workfront 인스턴스가 표시되면 **계속**&#x200B;을 선택합니다.
1. 서버를 표시하는 패널에서 **추가 및 구성**&#x200B;을 클릭합니다.

   이제 MCP 서버용 도구를 사용하고 구성할 수 있습니다.
1. 도구를 구성하고 테스트하면 **게시**&#x200B;를 클릭합니다.

   게시할 권한이 없을 수 있습니다. 이 경우 부조종사 관리자에게 문의하십시오.

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
>* 로그아웃만 해도 Workfront 인스턴스는 전환되지 않습니다. 커넥터의 연결을 끊고 다시 연결해야 합니다.


<!--

## Connect to Gemini

>[!IMPORTANT]
>
>You must be an administrator on the Gemini platform to set up the MCP server. If you aren't an administrator, share these instructions with your administrator so they can set up the connection for you.


To set up the connection between Gemini and the Workfront MCP server, follow the instructions provided by Google for [connecting Gemini to external tools using MCP](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/custom-mcp-server/set-up-custom-mcp-server). 

When prompted for the MCP Server URL, enter the following URL for your Workfront MCP server:  
   ```
   https://mcp.workfront.adobe.com/mcp/v1/workfront|
   
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
| --- | --- | --- |
| [!DNL Claude]에서 [!DNL Adobe Workfront] 커넥터를 찾을 수 없습니다. | [!DNL Claude] 관리자가 활성화하지 않았습니다. | [!DNL Claude] 관리자(Workfront 관리자 아님)에게 연락하여 [!DNL Adobe Workfront] 커넥터를 사용하도록 요청하십시오. |
| 연결했지만 데이터를 볼 수 없습니다. | 잘못된 Workfront 인스턴스를 인증했습니다. | 커넥터 연결을 끊고 다시 연결한 다음 올바른 인스턴스를 인증합니다. |
| 인증에 실패했거나 연결 작동이 중지되었습니다. | 인증 세션이 만료되었거나 연결 오류가 발생했습니다. | 커넥터를 분리하고 다시 연결합니다. |
| 다른 Workfront 인스턴스로 전환하려고 합니다. | 단일 연결이 사용자를 하나의 인스턴스로 연결합니다. | 새 인스턴스의 연결을 끊고, 다시 연결하고, 인증합니다. |
| Workfront에 연결할 수 없거나 MCP 서버 액세스가 비활성화되었다는 메시지가 표시됩니다. | Workfront 관리자가 인스턴스에 대한 MCP 서버 액세스를 해제했습니다. | Workfront 관리자에게 문의하여 시스템 환경 설정에서 MCP 서버 액세스를 활성화하도록 요청하십시오. |
| AI 아젠틱 플랫폼은 Workfront 항목을 찾을 수 있지만 생성, 업데이트 또는 삭제할 수 없습니다. | Workfront 관리자가 Workfront MCP 서버에 대한 쓰기 작업을 비활성화했습니다. | Workfront 관리자에게 문의하여 시스템 환경 설정에서 쓰기 작업을 활성화하도록 요청하십시오. |

연결 후 발생하는 일상적인 문제 해결(예: 부실 결과나 예기치 않은 동작)에 대해서는 [Adobe Workfront MCP 서버 사용](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)을 참조하십시오.


+++

## 설정에 대한 FAQ

+++ 를 확장하여 Workfront MCP 서버 설정에 대한 FAQ를 봅니다.

### 여러 Workfront 인스턴스에 동시에 연결할 수 있습니까?

아니요. 각 연결은 AI 에이전트 플랫폼을 단일 Workfront 인스턴스에 연결합니다. 전환하려면 연결을 끊고 다시 연결하여 새 인스턴스를 인증합니다.

### 어느 관리자가 이 기능을 활성화합니까?

Workfront 관리자와 AI 에이전트 플랫폼의 관리자 모두. Workfront 관리자는 Workfront 측에서 MCP 서버 액세스를 활성화합니다. AI 에이전트 플랫폼의 관리자는 해당 플랫폼 측에서 Workfront 액세스를 활성화합니다. [!DNL Claude]의 경우 [!DNL Claude] Enterprise 관리자가 [!DNL Adobe Workfront] 커넥터를 사용하도록 설정합니다.

### Workfront 인스턴스가 Adobe IMS(Identity Management System)에서 활성화되지 않은 경우 Workfront MCP 서버를 사용할 수 있습니까?

아니요. Workfront MCP 서버를 사용하려면 Adobe Identity Management System(IMS)에서 Workfront 인스턴스를 활성화해야 합니다. 인스턴스가 IMS에서 활성화되었는지 확실하지 않은 경우 Workfront 관리자에게 문의하십시오.

+++ 

