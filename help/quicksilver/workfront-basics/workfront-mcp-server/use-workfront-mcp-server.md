---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP 서버 사용
description: Adobe Workfront MCP 서버를 사용하여 AI 에이전트 플랫폼에서 자연어 대화를 통해 Workfront 항목을 검색, 생성, 업데이트 및 관리합니다.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 5592c1b93b5e44c732f92d626ed878d2c4647ceb
workflow-type: tm+mt
source-wordcount: '1896'
ht-degree: 0%

---


# Adobe Workfront MCP 서버 사용

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 미리 보기 샌드박스 환경에서만 사용할 수 있습니다.</span>

[!DNL Adobe Workfront] MCP 서버를 사용하면 자연어로 AI 에이전트 플랫폼에 요청하여 Workfront 항목을 찾고, 만들고, 업데이트하고, 관리할 수 있습니다. 플랫폼은 호출할 Workfront 작업을 결정하고 Workfront과의 대화를 처리합니다.

>[!IMPORTANT]
>
>현재 Workfront MCP 서버는 AWS을 사용하는 고객만 사용할 수 있습니다.

## 전제 조건

* AI 에이전트 플랫폼과 Workfront MCP 서버 간 연결을 설정해야 합니다. 설치 지침은 [Adobe Workfront MCP 서버 구성](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)을 참조하십시오.
* Workfront 인스턴스는 Adobe Identity Management System(IMS)에서 활성화되어야 합니다.
* 작업할 항목에 필요한 액세스 수준 및 개체 권한이 있는 Workfront 계정이 있어야 합니다.
* Workfront Planning에서 MCP를 사용하려면 귀사는 Adobe Workfront Planning이 포함된 Workfront 패키지에 있어야 합니다.

이 문서에서는 연결을 이미 설정했다고 가정합니다. 설정에 대한 자세한 내용은 [Adobe Workfront MCP 서버 구성](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)을 참조하십시오.

## 사용 가능한 도구

Workfront MCP 서버는 AI 에이전트 플랫폼이 사용자를 대신하여 호출하는 도구 세트를 노출합니다. 예를 들어 Workfront을 검색하고, 항목을 만들고, 필드를 업데이트하고, 승인을 관리하는 도구입니다. 전체 참조 목록은 [Adobe Workfront MCP 서버 도구](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md)를 참조하십시오.

>[!IMPORTANT]
>
>AI 에이전트 플랫폼을 Workfront에 연결하면 Workfront 계정 및 권한을 사용하여 Workfront에서 작동합니다. 플랫폼의 작업은 Workfront 인터페이스에서 직접 수행하는 작업과 동일한 효과를 갖습니다.<br>
>
>귀하와 귀하의 AI 에이전트 플랫폼 제공자는 플랫폼이 Workfront에서 취하는 행동에 대해 책임을 집니다. Adobe은 AI 아젠틱 플랫폼에서 Workfront 데이터를 변경할 책임이 없습니다.<br>
>
>AI 에이전트 플랫폼에서 요청을 진행하도록 하기 전에 특히 데이터를 변경하거나 삭제하는 작업의 의도를 이해하는지 확인하십시오.


## 질문 사항의 예

연결되면 AI 아젠틱 플랫폼에 자연어 요청을 입력합니다. AI 에이전트 플랫폼은 호출할 Workfront 작업을 결정하고 결과를 반환합니다.

>[!NOTE]
>
>Workfront 설정 영역의 관리자 제어로 인해 일부 작업을 사용할 수 없을 수도 있습니다. 예를 들어 Workfront 관리자가 MCP 서버에 대한 쓰기 작업을 비활성화한 경우 항목을 만들 수 없습니다.


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

<!--
* *Remove Anna Jones from all approvals in this project, and replace with Sione Carter.*
-->


### Planning 레코드 작업

>[!IMPORTANT]
>
>* Workfront Planning에서 MCP를 사용하려면 귀사는 Adobe Workfront Planning이 포함된 Workfront 패키지에 있어야 합니다.

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


## 고려 사항

Workfront MCP 서버를 사용할 때는 다음 사항을 고려해야 합니다.

### AI 아젠틱 플랫폼은 대화 초기의 정보를 활용할 수 있다

AI 에이전트 플랫폼은 경우에 따라 Workfront에 최신 정보를 요청하는 대신 대화 이전 부분의 데이터를 재사용합니다. AI 아젠틱 플랫폼을 마지막으로 확인한 이후 Workfront에서 변경된 사항이 있다면 오래된 정보가 표시될 수 있습니다.

AI 에이전트 플랫폼에서 새로운 데이터를 가져오도록 하려면 명시적으로 요청합니다. 예:

* *Workfront에서 최신 데이터를 가져옵니다. 캐시된 결과를 사용하지 마십시오.*

### Workfront MCP 서버 업데이트 확인

최신 도구와 기능을 보유하기 위해 Workfront MCP 서버에 대한 연결을 주기적으로 새로 고치고 싶을 수 있습니다.

대부분의 업데이트는 자동으로 수행되어야 합니다. 그러나 Workfront 릴리스 정보를 정기적으로 확인하는 것이 좋습니다.


## 데이터 및 보안

Workfront MCP 서버 도구는 API 호출이 작동하는 방식과 일치합니다. Workfront은 프롬프트, 응답 또는 기타 데이터를 저장하지 않습니다. 요청하는 모든 Workfront 데이터는 Workfront 플랫폼에서 액세스할 수 있습니다.

액세스 수준 및 개체 권한은 Workfront에 쿼리하거나 쓸 수 있는 내용을 결정합니다. Workfront 관리자는 Workfront 설정 영역에서 MCP 읽기 및 쓰기 작업을 제어할 수 있습니다.

### Workfront에 남아 있는 데이터

AI 에이전트 플랫폼 제공자는 Workfront MCP 서버를 통해 상호 작용하는 Workfront 데이터에 액세스할 수 있습니다. 자세한 내용은 AI 에이전트 플랫폼 공급자에게 문의하십시오.


### AI 아젠틱 플랫폼 공급자가 Workfront 데이터를 처리하는 방법

Workfront은 AI 아젠틱 플랫폼 공급자가 Workfront 데이터를 처리하는 방법을 제어하지 않습니다. 자세한 내용은 AI 에이전트 플랫폼 공급자에게 문의하십시오.

## 일상적인 사용 문제 해결

+++ 를 확장하여 Workfront MCP 서버의 일상적인 사용에 대한 문제 해결 팁을 봅니다.

| 문제 | 가능한 원인 | 고정 |
| --- | --- | --- |
| AI 에이전트 플랫폼은 오래된 정보를 제공합니다. | AI 아젠틱 플랫폼은 대화 초기의 데이터를 재사용하고 있다. | Workfront에서 새로운 데이터를 요청합니다. |
| AI 에이전트 플랫폼이 잘못된 Workfront 항목에서 데이터를 반환했습니다. | AI 아젠틱 플랫폼이 모호한 문구를 바탕으로 잘못된 항목을 골랐다. | 더 구체적인 이름, ID 또는 필터를 사용하여 다시 질문합니다. |
| 업데이트 또는 삭제가 Workfront에서 적용되지 않았습니다. | Workfront 관리자가 Workfront MCP 서버에 대한 쓰기 작업을 비활성화했거나 특정 항목에 대한 작업을 수행할 수 있는 권한이 없습니다. | 작업이 실행되었는지 AI 에이전트 플랫폼에 확인합니다. 그런 다음 Workfront MCP 서버에 대해 쓰기 작업이 활성화되어 있는지, 그리고 항목을 변경할 권한이 있는지 확인합니다. |

설정 및 인증 문제에 대한 자세한 내용은 [Adobe Workfront MCP 서버 구성](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)에서 [설정 및 인증 문제 해결](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication)을 참조하십시오.

+++

## 자주 묻는 질문

+++ 를 확장하여 Workfront MCP 서버 사용에 대한 FAQ를 봅니다.

### AI 에이전트 플랫폼이란 무엇입니까?

AI 아젠틱 플랫폼은 을 대신해 작업을 수행할 수 있는 AI 도구입니다.
다른 시스템은 단순히 질문에 대답하는 것이 아닙니다. Workfront에 연결하는 경우
mcp 서버를 통해 Workfront을 찾고 만들고 업데이트하고 삭제할 수 있습니다
자연어로 요청한 것을 기반으로 한 항목입니다. 예: Claude
데스크탑, ChatGPT 및 기타 MCP 호환 AI 클라이언트.


### Workfront MCP 서버를 사용하려면 Workfront 관리자여야 합니까?

아니요. 모든 Workfront 사용자는 연결된 을 통해 Workfront MCP 서버를 사용할 수 있습니다.
AI 에이전트 플랫폼. AI 아젠틱 플랫폼은 Workfront을 사용하여 작동합니다
계정, 액세스 수준 및 개체 권한 등 사용자가 수행할 작업만 가능
은 이미 Workfront에서 직접 수행할 수 있습니다.

### AI 아젠틱 플랫폼이 나를 위해 아이템을 생성, 업데이트, 삭제할 수 없는 이유는 무엇인가?

Workfront 관리자는 에서 허용되는 MCP 작업을 제어합니다
Workfront 설정 영역입니다. 쓰기 작업이 비활성화된 경우 AI 에이전트 플랫폼입니다
은 여전히 Workfront 항목을 찾아 읽을 수 있지만 변경할 수 없습니다. 귀하도
특정 항목에 대한 올바른 액세스 수준 및 개체 권한이 필요합니다.
함께 작업하는 경우

### AI 아젠틱 플랫폼이 Workfront 데이터를 변경하거나 삭제하기 전에 나에게 질문합니까?

Workfront이 아니라 AI 에이전트 플랫폼에 따라 다릅니다. 대부분의 플랫폼
특히 삭제의 경우 작업을 실행하기 전에 확인 메시지를 표시합니다.요청을 승인하기 전에 플랫폼에서 수행하려고 하는 작업을 읽어 보십시오.
변경 사항을 적용했을 때와 동일한 방식으로 Workfront에서 변경 사항이 발생합니다
인터페이스에 있는 사용자 자신입니다.

<!--

### Can I undo something the AI agentic platform did in Workfront?

Changes the AI agentic platform makes in Workfront work the same way as 
changes you make in the interface. If Workfront supports undoing or 
restoring a particular action (for example, restoring a deleted item from 
the Recycle Bin), the same options apply. If Workfront doesn't normally let 
you undo an action, you can't undo it through the AI agentic platform either.

-->

### AI 아젠틱 플랫폼이 잘못된 Workfront 항목을 반품한 이유는 무엇입니까?

AI 아젠틱 플랫폼은 사용자가 사용한 단어를 기반으로 항목을 선정한다. 다음의 경우
요청이 모호합니다. 예를 들어 두 프로젝트의 이름이 유사합니다.
잘못 고르실 수도 있어요. 더 구체적인 이름, ID, 날짜,
또는 필터를 사용하여 결과를 좁힐 수 있습니다.


### AI 아젠틱 플랫폼을 통해 작업할 수 있는 Workfront 항목은 무엇입니까?

액세스 수준 및 을 통해 Workfront에서 액세스할 수 있는 모든 항목
개체 권한. 여기에는 프로젝트, 작업, 문제, 문서,
승인, 계획 레코드 등.

### 다른 사람이 AI 아젠틱 플랫폼과 나눈 내 대화를 볼 수 있습니까?

Workfront은 프롬프트 또는 AI 에이전트 플랫폼의 응답을 저장하지 않습니다.AI 아젠틱 플랫폼을 제공하는 사람이 대화 방식을 제어합니다.
저장 또는 공유됩니다. 다음에 대한 내용은 AI 에이전트 플랫폼 공급자에게 문의하십시오.
세부 정보.

### Workfront API 또는 사용할 MCP 도구를 알아야 합니까?

아니요. AI 아젠틱 플랫폼은 자연어 요청을 다음과 같이 번역합니다
적합한 Workfront 작업 및 선택 도구를 선택할 수 있습니다. 만약..
이미 Workfront API를 잘 알고 있는 경우 작업이 익숙해질 것입니다.
하지만 이것은 필수가 아닙니다.

### 내 Workfront 데이터가 AI 아젠틱 플랫폼 공급자에게 전송됩니까? 아니면 AI 아젠틱 플랫폼 공급자가 저장합니까?

자세한 내용은 [데이터 및 보안](#data-and-security)을 참조하세요.
기사.

### 새로운 버전의 Workfront MCP 서버가 릴리스되면 어떻게 됩니까?

MCP 서버는 일반적으로 자동으로 업데이트되지만 최신 도구 및 기능을 보려면 MCP 서버와의 연결을 때때로 새로 고쳐야 할 수 있습니다.

### Workfront 인스턴스가 Adobe IMS(Identity Management System)에서 활성화되지 않은 경우 Workfront MCP 서버를 사용할 수 있습니까?

아니요. Workfront MCP 서버를 사용하려면 Adobe Identity Management System(IMS)에서 Workfront 인스턴스를 활성화해야 합니다. 인스턴스가 IMS에서 활성화되었는지 확실하지 않은 경우 Workfront 관리자에게 문의하십시오.


+++
