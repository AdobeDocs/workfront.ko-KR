---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP 서버 사용
description: Adobe Workfront MCP 서버를 사용하여 AI 에이전트 플랫폼에서 자연어 대화를 통해 Workfront 항목을 검색, 생성, 업데이트 및 관리합니다.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 152486b7850e01f3de23f22bbe3729c5cd3d3aa2
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 0%

---


# Adobe Workfront MCP 서버 사용

[!DNL Adobe Workfront] MCP 서버를 사용하면 일반 영어로 AI 에이전트 플랫폼에 요청하여 Workfront 항목을 찾고, 만들고, 업데이트하고, 관리할 수 있습니다. 플랫폼은 호출할 Workfront 작업을 결정하고 Workfront과의 대화를 처리합니다.

[!DNL Claude]은(는) 현재 유일하게 지원되는 AI Agentic 플랫폼이지만 이 문서의 예제와 패턴은 Workfront MCP 서버를 지원하는 모든 AI Agentic 플랫폼에 적용됩니다.

이 문서에서는 연결을 이미 설정했다고 가정합니다. 설정에 대한 자세한 내용은 [Adobe Workfront MCP 서버 구성](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)을 참조하십시오. Workfront MCP 서버에 대한 자세한 내용은 [Adobe Workfront MCP 서버 개요](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md)를 참조하십시오.

## 사용 가능한 도구

Workfront MCP 서버는 AI 에이전트 플랫폼이 사용자를 대신하여 호출하는 도구 세트(예: Workfront을 검색하고, 항목을 만들고, 필드를 업데이트하고, 승인을 관리하는 도구)를 노출합니다. Workfront 영역별로 그룹화된 전체 참조 목록은 [Adobe Workfront MCP 서버 도구](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md)를 참조하십시오.

>[!IMPORTANT]
>
>AI 에이전트 플랫폼을 Workfront에 연결하면 Workfront 계정 및 권한을 사용하여 Workfront에서 작동합니다. 플랫폼의 작업은 Workfront 인터페이스에서 직접 수행하는 작업과 동일한 효과를 갖습니다.
>
>귀하와 귀하의 AI 에이전트 플랫폼 제공자는 플랫폼이 Workfront에서 취하는 행동에 대해 책임을 집니다. Adobe은 AI 아젠틱 플랫폼이 Workfront 데이터를 변경했을 때 이에 대한 책임이 없습니다.
>
>AI 에이전트 플랫폼에서 요청을 진행하도록 하기 전에 특히 데이터를 변경하거나 삭제하는 작업의 의도를 이해하는지 확인하십시오.


## 질문 사항의 예

연결되면 AI 아젠틱 플랫폼에 자연어 요청을 입력합니다. AI 에이전트 플랫폼은 호출할 Workfront 작업을 결정하고 결과를 반환합니다.

### 작업 찾기 및 보기

찾고 있는 항목과 일치하는 항목을 Workfront에서 검색하려면 다음과 같이 하십시오.

* *Brand Marketing 팀의 모든 활성 프로젝트를 표시합니다.*
* *Joan Harris에게 할당된 모든 작업을 가져옵니다.*
* *&quot;기술&quot; 범주 아래의 &quot;웹 사이트 재디자인&quot; 프로젝트의 모든 문제를 표시합니다.*

### 새 항목 만들기

프로젝트, 작업 또는 기타 Workfront 항목을 만들려면 다음 작업을 수행하십시오.

* *3월 10일부터 4월 30일까지 &quot;Q2 혁신 샌드박스&quot;라는 빈 프로젝트를 만듭니다. 나를 소유자로 설정합니다.*
* *프로젝트에 &quot;랜딩 페이지 QA&quot;라는 새 작업을 추가하고 4월 22일부터 4월 26일까지 예약합니다.*
* *&quot;여름 판매 2026&quot;이라는 새 캠페인 레코드를 만듭니다.*

### 기존 항목 업데이트

Workfront에 이미 있는 항목을 변경하려면 다음 질문을 하십시오.

* *4월 18일에 완료되도록 &quot;디자인 검토&quot; 작업을 업데이트하고 크리에이티브 팀에 할당하십시오.*
* *&quot;Lucent AI Launch - NA&quot; 프로젝트의 경우 4월 중순까지 마침을 푸시하고 예산을 $150,000으로 늘리십시오.*
* *&quot;여름 캠페인&quot; 레코드의 예산 필드를 $75,000로 업데이트하십시오.*

### 항목 삭제

Workfront 항목을 제거하려면 다음 작업을 수행하십시오.

* *Q1 테스트 캠페인이라는 프로젝트를 삭제합니다.*
* *프로젝트에서 &quot;자산 인쇄 프로덕션&quot; 작업을 제거하십시오.*
* *이름이 &quot;이전 프로모션&quot;인 캠페인 레코드를 삭제합니다.*

>[!WARNING]
>
>AI 에이전트 플랫폼을 통해 Workfront에서 항목을 삭제하는 것은 Workfront 인터페이스에서 삭제하는 것과 같습니다. AI 아젠틱 플랫폼이 삭제될 내용을 확인한 후 계속 진행하십시오.

### 승인 작업

문서 및 자산 승인을 관리하려면 다음 사항을 요청하십시오.

* *현재 문서의 승인자로 Sarah Chen과 Miguel Alvarez를 추가하십시오.*
* *응답하지 않은 자산 &quot;봄 캠페인 비디오&quot;의 승인자에게 미리 알림을 보냅니다.*
* *자산 &quot;봄 캠페인 비디오&quot;에 &quot;마케팅 시작&quot; 승인 템플릿을 적용하세요.*


### Planning 레코드 작업

계획 레코드를 관리하려면 다음을 묻습니다.

* *브랜드 마케팅 팀을 위한 &quot;Q2 마케팅 계획&quot;이라는 새 계획 레코드를 만듭니다.*
* *계획 레코드에 &quot;소셜 미디어 감사&quot;라는 새 작업을 추가합니다.*
* *4월 18일에 완료되도록 &quot;소셜 미디어 감사&quot; 작업을 업데이트하고 크리에이티브 팀에 할당합니다.*

### 워크플로우 작업

워크플로우를 관리하려면 다음 사항을 질문합니다.

* *Q2 Innovation Sandbox 프로젝트를 혁신 검토 위원회로 라우팅합니다.*
* *여름 캠페인 레코드를 &quot;시작 준비&quot; 상태로 업데이트합니다.*
* *여름 캠페인 레코드를 승인합니다.*


### 대화에 대한 체인 요청

단일 대화에서 요청을 연결할 수 있습니다. AI 에이전트 플랫폼은 컨텍스트를 유지하므로 각 요청이 이전 요청을 기반으로 빌드할 수 있습니다. 예:

1. 항목 집합 요청: *기한이 지난 작업을 찾습니다.*
1. 목록을 받은 후 결과에 대한 작업을 요청하세요. *다음 금요일로 모든 결과를 업데이트하세요.*

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## 고려 사항

Workfront MCP 서버를 사용할 때는 다음 사항을 고려하십시오.

### AI 아젠틱 플랫폼은 대화 초기의 정보를 활용할 수 있다

AI 에이전트 플랫폼은 경우에 따라 Workfront에 최신 정보를 요청하는 대신 대화 이전 부분의 데이터를 재사용합니다. AI 아젠틱 플랫폼을 마지막으로 확인한 이후 Workfront에서 변경된 사항이 있다면 오래된 정보가 표시될 수 있습니다.

AI 에이전트 플랫폼에서 새로운 데이터를 가져오도록 하려면 명시적으로 요청합니다. 예:

* *Workfront에서 최신 데이터를 가져옵니다. 캐시된 결과를 사용하지 마십시오.*

### Workfront MCP 서버가 자동으로 업데이트됩니다

Adobe이 Workfront MCP 서버의 새 버전을 출시하면 AI 에이전트 플랫폼이 새 버전을 자동으로 사용합니다. 다시 연결하거나 변경할 필요가 없습니다.

## 데이터 및 보안

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI agentic platform. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI agentic platform provider, what happens to it after the conversation ends, and any differences between AI agentic platforms (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### Workfront에 남아 있는 데이터

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI agentic platform (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### AI 아젠틱 플랫폼 공급자가 Workfront 데이터를 처리하는 방법

<!-- NEEDS DETAIL: For each supported AI agentic platform, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### AI 에이전트 플랫폼 간의 차이점

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI agentic platform handles Workfront data once additional AI agentic platforms are supported. -->

## 일상적인 사용 문제 해결

+++ 를 확장하여 Workfront MCP 서버의 일상적인 사용에 대한 문제 해결 팁을 봅니다.

| 문제 | 가능한 원인 | 고정 |
|---|---|---|
| AI 에이전트 플랫폼은 오래된 정보를 제공합니다. | AI 아젠틱 플랫폼은 대화 초기의 데이터를 재사용하고 있다. | Workfront에서 새로운 데이터를 요청합니다. |
| AI 에이전트 플랫폼이 잘못된 Workfront 항목에서 데이터를 반환했습니다. | AI 아젠틱 플랫폼이 모호한 문구를 바탕으로 잘못된 항목을 골랐다. | 더 구체적인 이름, ID 또는 필터를 사용하여 다시 질문합니다. |
| 업데이트 또는 삭제가 Workfront에서 적용되지 않았습니다. | AI 아젠틱 플랫폼이 아직 작업을 호출하지 않았거나 권한이 허용하지 않습니다. | AI 에이전트 플랫폼에서 작업이 실행되었는지 확인한 다음 Workfront 권한을 확인합니다. |

설정 및 인증 문제에 대한 자세한 내용은 [Adobe Workfront MCP 서버 구성](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)에서 [설정 및 인증 문제 해결](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication)을 참조하십시오.

+++

## 자주 묻는 질문

+++ 를 확장하여 Workfront MCP 서버 사용에 대한 FAQ를 봅니다.

### AI 아젠틱 플랫폼을 통해 작업할 수 있는 Workfront 항목은 무엇입니까?

액세스 수준 및 개체 권한을 통해 Workfront에서 액세스할 수 있는 모든 항목입니다.

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### 내 Workfront 데이터가 AI 아젠틱 플랫폼 공급자에게 전송됩니까? 아니면 AI 아젠틱 플랫폼 공급자가 저장합니까?

자세한 내용은 이 문서에서 [데이터 및 보안](#data-and-security)을 참조하십시오.

### 새로운 버전의 Workfront MCP 서버가 릴리스되면 어떻게 됩니까?

MCP 서버가 자동으로 업데이트됩니다. 다시 연결하거나 변경할 필요가 없습니다.

### Workfront MCP 서버를 사용하려면 Workfront API를 알아야 합니까?

아니요. AI 아젠틱 플랫폼은 자연어 요청을 올바른 Workfront 작업으로 변환합니다. Workfront API를 이미 잘 알고 있는 경우 작업이 친숙하게 느껴지지만 요구 사항은 아닙니다.

+++
