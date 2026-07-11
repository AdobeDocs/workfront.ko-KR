---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP 서버 개요
description: Adobe Workfront MCP 서버가 수행하는 작업과 AI 아젠틱 플랫폼에서 자연어 대화를 통해 Workfront과 작업할 수 있는 방법을 알아봅니다.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 5592c1b93b5e44c732f92d626ed878d2c4647ceb
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---


# Adobe Workfront MCP 서버 개요

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 미리 보기 샌드박스 환경에서만 사용할 수 있습니다.</span>

[!DNL Adobe Workfront] MCP 서버는 Workfront 인스턴스를 [!DNL Claude] 또는 [!DNL ChatGPT]과(와) 같은 AI 에이전트 플랫폼에 연결합니다. AI 아젠틱 플랫폼에서 자연어 요청을 통해 Workfront 항목을 찾고 만들고 업데이트하고 관리할 수 있습니다.

예를 들어 다음과 같은 질문을 할 수 있습니다.

* *Brand Marketing 팀의 모든 활성 프로젝트를 표시합니다.*
* *4월 18일에 끝나도록 &quot;디자인 검토&quot; 작업을 업데이트하십시오.*
* *응답하지 않은 자산 &quot;봄 캠페인 비디오&quot;의 승인자에게 미리 알림을 보냅니다.*

Workfront API 또는 Workfront MCP 서버를 사용하기 위해 MCP 서버가 작동하는 방식을 알 필요가 없습니다.

>[!IMPORTANT]
>
>현재 Workfront MCP 서버는 AWS을 사용하는 고객만 사용할 수 있습니다.

## MCP 서버 소개

MCP 서버는 AI 에이전트 플랫폼이 다른 시스템과 연동할 수 있도록 하는 연결점이다. Workfront MCP 서버는 AI 아젠틱 플랫폼이 연결되어 귀하를 대신하여 Workfront 데이터를 읽고 처리할 수 있습니다.

MCP는 모델 컨텍스트 프로토콜을 의미합니다. 이는 AI 아젠틱 플랫폼과 외부 시스템이 서로 어떻게 대화하는지를 정의하는 표준이다.

## 연결 설정

Workfront MCP 서버는 MCP 호환 AI 에이전트 플랫폼(예: [!DNL Claude] 또는 [!DNL ChatGPT])과 작동합니다. 이를 사용하려면 먼저 다음 작업을 수행해야 합니다.

* Workfront 관리자는 Workfront 인스턴스에서 MCP 서버 액세스를 활성화해야 합니다.
* 사용자(또는 관리자)는 AI 아젠틱 플랫폼을 Workfront에 연결해야 합니다.

자세한 내용은 [Adobe Workfront MCP 서버 구성](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)을 참조하십시오.

## Workfront MCP 서버 사용 시작

설정 후 AI 에이전트 플랫폼에 자연어로 된 Workfront 항목을 검색, 생성, 업데이트 및 관리하도록 요청할 수 있습니다.

예제 요청, 주의해야 할 사항, 데이터 및 보안에 대한 정보 등 자세한 내용은 [Adobe Workfront MCP 서버 사용](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)을 참조하십시오.
