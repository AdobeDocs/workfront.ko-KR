---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP 서버 사용
description: Adobe Workfront MCP 서버를 사용하여 AI 어시스턴트에서 자연어 대화를 통해 Workfront 항목을 검색, 생성, 업데이트 및 관리할 수 있습니다.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 4517d45ecc653d27d435a8192a612241120dd33f
workflow-type: tm+mt
source-wordcount: '1243'
ht-degree: 2%

---


# Adobe Workfront MCP 서버 사용

[!DNL Adobe Workfront] MCP 서버를 사용하면 일반 영어로 AI 도우미에게 요청하여 Workfront 항목을 찾고, 만들고, 업데이트하고, 관리할 수 있습니다. AI 비서는 호출할 Workfront 작업을 결정하고 Workfront과의 대화를 처리합니다.

[!DNL Claude]은(는) 현재 유일하게 지원되는 AI 도우미이지만 이 문서의 예제와 패턴은 Workfront MCP 서버를 지원하는 모든 AI 도우미에 적용됩니다.

이 문서에서는 연결을 이미 설정했다고 가정합니다. 설정에 대한 자세한 내용은 [Adobe Workfront MCP 서버 구성](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)을 참조하십시오. Workfront MCP 서버에 대한 자세한 내용은 [Adobe Workfront MCP 서버 개요](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md)를 참조하십시오.



## Workfront MCP 서버를 통해 사용할 수 있는 작업

Workfront MCP 서버는 승인, 계획 및 워크플로에 걸친 작업을 다룹니다.

<!-- NEEDS DETAIL: Confirm the full inventory of actions exposed through the Workfront MCP server. The five core actions below are confirmed from Hamilton's walkthrough. The approvals, planning, and workflow sections need to be filled in from Jeff's engineering channel post, hands-on access, and the deck Oznur published in the MCP external channel. -->

>[!IMPORTANT]
>
>AI 비서는 Workfront 계정 및 권한을 사용하여 Workfront에서 작동합니다. 귀하와 귀하의 AI 비서 제공업체는 AI 비서가 귀하를 대신하여 취하는 행동에 대해 책임을 집니다. 계속 진행하기 전에 AI 비서가 수행하려고 하는 작업을 확인합니다.


## AI 지원 작업에 대한 책임

AI 비서를 Workfront에 연결하면 AI 비서가 Workfront 계정 및 권한을 사용하여 Workfront에서 작동합니다. AI 비서의 작업은 Workfront 인터페이스에서 직접 수행하는 작업과 동일한 효과를 갖습니다.

귀하와 AI 어시스턴트 공급자는 Workfront에서 AI 어시스턴트가 수행하는 행동에 대해 책임을 집니다. Adobe은 AI 어시스턴트가 Workfront 데이터를 변경할 책임이 없습니다.

AI 비서가 요청을 진행하도록 하기 전에 특히 데이터를 변경하거나 삭제하는 작업의 의도를 이해했는지 확인하십시오.

### 핵심 작업

Workfront MCP 서버에는 다음 핵심 작업이 포함됩니다.

| 액션 | 기능 |
|---|---|
| 만들기 | Workfront에서 새 항목을 만듭니다. |
| 검색 | Workfront에서 항목을 찾아 검색합니다. |
| 업데이트 | Workfront의 기존 항목을 변경합니다. |
| 삭제 | Workfront에서 항목을 제거합니다. |
| 필드 이름 확인 | AI 도우미가 데이터에 대한 정확한 요청을 작성할 수 있도록 올바른 Workfront 필드 이름을 조회합니다. |

<!-- NEEDS DETAIL: Confirm which Workfront object types are supported across the core actions (projects, tasks, issues, portfolios, programs, custom forms, planning records, approvals, etc.). -->

### 승인 작업

<!-- NEEDS DETAIL: List the approval-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request a marketer might make. -->

### 계획 작업

<!-- NEEDS DETAIL: List the planning-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request. -->

### 워크플로우 작업

<!-- NEEDS DETAIL: List the workflow-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request. -->

## 질문 사항의 예

연결되면 AI 도우미에 자연어 요청을 입력합니다. AI 비서가 호출할 Workfront 작업을 결정하고 결과를 반환합니다.

<!-- NEEDS DETAIL: Example prompts in this section are adapted from the Workflow Optimization Agent (WOA) examples doc on another branch. Validate each example against a working Claude + Workfront MCP server setup before publication, since WOA and the MCP server may expose different action inventories. -->

### 작업 찾기 및 보기

찾고 있는 항목과 일치하는 항목을 Workfront에서 검색하도록 AI 도우미에 요청하십시오. 예:

* *Brand Marketing 팀의 모든 활성 프로젝트를 표시합니다.*
* *Joan Harris에게 할당된 모든 작업을 가져옵니다.*
* *&quot;기술&quot; 범주 아래의 &quot;웹 사이트 재디자인&quot; 프로젝트의 모든 문제를 표시합니다.*

### 새 항목 만들기

AI 도우미에게 프로젝트, 작업 또는 기타 Workfront 항목을 생성하도록 요청하십시오. 예:

* *3월 10일부터 4월 30일까지 &quot;Q2 혁신 샌드박스&quot;라는 빈 프로젝트를 만듭니다. 나를 소유자로 설정합니다.*
* *프로젝트에 &quot;랜딩 페이지 QA&quot;라는 새 작업을 추가하고 4월 22일부터 4월 26일까지 예약합니다.*
* *&quot;여름 판매 2026&quot;이라는 새 캠페인 레코드를 만듭니다.*

### 기존 항목 업데이트

Workfront에 이미 있는 항목을 변경하려면 AI 도우미에 문의하십시오. 예:

* *4월 18일에 완료되도록 &quot;디자인 검토&quot; 작업을 업데이트하고 크리에이티브 팀에 할당하십시오.*
* *&quot;Lucent AI Launch - NA&quot; 프로젝트의 경우 4월 중순까지 마침을 푸시하고 예산을 $150,000으로 늘리십시오.*
* *&quot;여름 캠페인&quot; 레코드의 예산 필드를 $75,000로 업데이트하십시오.*

### 항목 삭제

AI 도우미에 Workfront 항목을 제거하도록 요청하십시오. 예:

* *Q1 테스트 캠페인이라는 프로젝트를 삭제합니다.*
* *프로젝트에서 &quot;자산 인쇄 프로덕션&quot; 작업을 제거하십시오.*
* *이름이 &quot;이전 프로모션&quot;인 캠페인 레코드를 삭제합니다.*

>[!WARNING]
>
>AI 도우미를 통해 Workfront에서 항목을 삭제하는 것은 Workfront 인터페이스에서 삭제하는 것과 같습니다. 계속 진행하기 전에 AI 도우미가 삭제하려는 내용을 확인합니다.

### 승인 작업

문서 및 자산 승인을 관리하도록 AI 도우미에 문의하십시오. 예:

* *현재 문서의 승인자로 Sarah Chen과 Miguel Alvarez를 추가하십시오.*
* *응답하지 않은 자산 &quot;봄 캠페인 비디오&quot;의 승인자에게 미리 알림을 보냅니다.*
* *자산 &quot;봄 캠페인 비디오&quot;에 &quot;마케팅 시작&quot; 승인 템플릿을 적용하세요.*

<!-- NEEDS DETAIL: Add approvals-specific context from the WOA examples doc, including: content approvals must be enabled for the organization, the AI assistant cannot approve or reject on behalf of humans (except via the Workfront AI Reviewer), and best experience is with the Unified Approvals experience. -->

### Planning 레코드 작업

계획 레코드를 관리하도록 AI 도우미에 문의하십시오. 예:

* *브랜드 마케팅 팀을 위한 &quot;Q2 마케팅 계획&quot;이라는 새 계획 레코드를 만듭니다.*
* *계획 레코드에 &quot;소셜 미디어 감사&quot;라는 새 작업을 추가합니다.*
* *4월 18일에 완료되도록 &quot;소셜 미디어 감사&quot; 작업을 업데이트하고 크리에이티브 팀에 할당합니다.*

### 워크플로우 작업

AI 도우미에게 워크플로우를 관리하도록 요청합니다. 예:

* *Q2 Innovation Sandbox 프로젝트를 혁신 검토 위원회로 라우팅합니다.*
* *여름 캠페인 레코드를 &quot;시작 준비&quot; 상태로 업데이트합니다.*
* *여름 캠페인 레코드를 승인합니다.*


### 대화에 대한 체인 요청

단일 대화에서 요청을 연결할 수 있습니다. AI 도우미가 컨텍스트를 유지하므로 각 요청은 이전 요청을 기반으로 빌드할 수 있습니다. 예:

1. AI 도우미에게 항목 집합을 찾으라고 요청하십시오. *기한이 지난 작업을 찾으십시오.*
1. AI 도우미가 목록을 반환하면 결과에 따라 작업하도록 요청하세요. *다음 금요일로 모두 업데이트하세요.*

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## 고려 사항

Workfront MCP 서버를 사용할 때는 다음 사항을 고려하십시오.

### AI 어시스턴트는 대화에서 앞서 나온 정보를 활용할 수 있다

AI 도우미가 대화에서 Workfront에 최신 정보를 요청하는 대신 이전 버전의 데이터를 재사용하는 경우가 있습니다. AI 도우미가 마지막으로 본 이후 Workfront에서 변경된 사항이 있는 경우 오래된 정보가 표시될 수 있습니다.

AI 도우미가 새로운 데이터를 가져오도록 하려면 명시적으로 요청하십시오. 예:

* *Workfront에서 최신 데이터를 가져옵니다. 캐시된 결과를 사용하지 마십시오.*

### Workfront MCP 서버가 자동으로 업데이트됩니다

Adobe이 Workfront MCP 서버의 새 버전을 출시하면 AI 비서가 자동으로 새 버전을 사용합니다. 다시 연결하거나 변경할 필요가 없습니다.

## 데이터 및 보안

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI assistant. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI assistant provider, what happens to it after the conversation ends, and any differences between AI assistants (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### Workfront에 남아 있는 데이터

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI assistant (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### AI 어시스턴트 공급자가 Workfront 데이터를 처리하는 방법

<!-- NEEDS DETAIL: For each supported AI assistant, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### AI 도우미 간의 차이점

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI assistant handles Workfront data once additional AI assistants are supported. -->

## 일상적인 사용 문제 해결

설정 및 인증 문제에 대한 자세한 내용은 [Adobe Workfront MCP 서버 구성](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)에서 [설정 및 인증 문제 해결](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication)을 참조하십시오.

| 문제 | 가능한 원인 | 고정 |
|---|---|---|
| AI 비서가 오래된 정보를 제공합니다. | AI 비서가 대화 초기의 데이터를 재사용하고 있습니다. | AI 도우미에게 Workfront에서 새 데이터를 가져오도록 요청하십시오. |
| AI 도우미가 잘못된 Workfront 항목에서 데이터를 반환했습니다. | AI 비서가 애매한 문구를 바탕으로 잘못된 항목을 골랐다. | 더 구체적인 이름, ID 또는 필터를 사용하여 다시 질문합니다. |
| 업데이트 또는 삭제가 Workfront에서 적용되지 않았습니다. | AI 관리자가 아직 작업을 호출하지 않았거나 권한이 이를 허용하지 않습니다. | 작업이 실행되었는지 AI 도우미를 통해 확인한 다음 Workfront 권한을 확인합니다. |

<!-- NEEDS DETAIL: Add additional day-to-day troubleshooting scenarios discovered during hands-on testing. -->

## 자주 묻는 질문

### AI 비서를 통해 작업할 수 있는 Workfront 항목은 무엇입니까?

액세스 수준 및 개체 권한을 통해 Workfront에서 액세스할 수 있는 모든 항목입니다.

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### 내 Workfront 데이터가 AI 비서 공급자에게 전송됩니까, 아니면 AI 비서가 저장합니까?

자세한 내용은 이 문서에서 [데이터 및 보안](#data-and-security)을 참조하십시오.

### 새로운 버전의 Workfront MCP 서버가 릴리스되면 어떻게 됩니까?

MCP 서버가 자동으로 업데이트됩니다. 다시 연결하거나 변경할 필요가 없습니다.

### Workfront MCP 서버를 사용하려면 Workfront API를 알아야 합니까?

아니요. AI 도우미는 자연어 요청을 올바른 Workfront 작업으로 변환합니다. Workfront API를 이미 잘 알고 있는 경우 작업이 친숙하게 느껴지지만 요구 사항은 아닙니다.
