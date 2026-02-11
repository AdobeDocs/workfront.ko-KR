---
title: 'Bridge 구축: 프로젝트에 전략적 의도 연결'
description: Adobe Workfront Planning의 높은 수준 계획과 Adobe Workfront에서의 일상적인 워크플로 실행 간에 "전략적 스레드"를 만드는 방법을 알아봅니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
exl-id: 567ab223-b282-4b98-9655-7b9766fba869
source-git-commit: 52bf41e146a11a4af4fbebfe5bb20a9765f2bc7b
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 0%

---


# 브리지 구축: 프로젝트에 전략적 의도 연결

{{planning-important-intro}}

Adobe Workfront Planning의 높은 수준 계획과 Workfront의 일일 실행 간에 전략적 스레드를 생성하는 방법을 알아봅니다. 연결을 사용하여 전략과 실행 사이에 브리지를 구축할 수 있습니다.

이 안내서는 Workfront Planning을 구현하는 Workfront 관리자 및 작업 공간 관리자를 위한 것입니다.

## 실행 전략에 맞추기 개요

전략을 일상 업무에 연결하면 비전이 현실로 바뀐다. 높은 수준의 계획이 실행과 동기화되면 모든 프로젝트와 작업이 비즈니스를 진전시킬 수 있도록 하는 전략적 스레드를 생성합니다.

이러한 정렬을 수행하려면 Workfront의 노력과 Workfront Planning의 전략 기록을 연결하는 일련의 기술 링크와 프로세스 가드레일이 필요합니다.

계획과 행동 사이의 차이를 해소함으로써 팀의 에너지가 항상 최우선 목표에 집중되도록 합니다.

## 연결을 만들어 기반 구축

계획 및 실행을 브리지하려면 먼저 작업 영역 관리자로서 연결에 적합한 레코드 유형을 정의해야 합니다.

### 연결 필드 개요

브리지는 연결 필드를 만드는 것으로 시작됩니다.

연결 필드는 레코드 유형 간의 기술적 핸드셰이크 역할을 합니다.

이 필드 유형은 Workfront Planning의 모든 관계에 영향을 주는 엔진입니다. 특정 레코드 유형(예: 채널 전술)이 Planning에 있든 Workfront에 있든 다른 객체 유형에 연결될 수 있도록 허용된다는 점에서 의도의 표현입니다.

자세한 내용은 [연결된 레코드 종류 개요](/help/quicksilver/planning/architecture/connect-record-types-overview.md)를 참조하세요.

### 연결 생성 시점 정의

가장 좋은 방법은 작업을 만들기 전에 연결을 만들어야 하는지 여부를 결정하는 것입니다.

연결 필드를 추가하면 개별 레코드가 생성되는 방식에 관계없이 전략 스레드를 지원하도록 환경을 디자인할 수 있습니다.

## 전략과 실행을 동기화로 설정

전략 레이어의 초점을 계속 유지하려면 전략 실행에 Workfront을 사용하는 동안 계획 레코드를 높은 수준의 의도에 집중하는 것이 좋습니다.

이 방법에서는 다음과 같은 방법으로 두 모듈의 고유한 장점을 사용합니다.

* **Workfront 계획(전략 계층):**&#x200B;은(는) 높은 수준으로 유지됩니다. 캠페인, 채널 전략 및 예산을 추적합니다. 소음이 없고 경영진이 즉시 사용할 수 있습니다.

* **Workfront(실행 계층):** 전술적 세부 정보를 관리합니다. 개별 경험 또는 활동을 프로젝트, 작업 및 문제로 관리할 수 있습니다. 소유권을 할당하고 실행 승인에서 빌드할 수 있습니다.

## 브리지를 활성화하여 의도에서 행동으로 이동

연결이 구성된 후 특정 전략 레코드와 실행 프로젝트 간의 연결을 활성화하는 방법을 결정해야 합니다.

### 표 방향 경로 사용

전략가 및 고급 사용자는 테이블 뷰를 워크벤치로 사용하여 시간이 지남에 따라 계획을 구체화합니다.

테이블에 레코드를 만들어도 기본적으로 Workfront에 대한 링크가 설정되지 않습니다.

실행 프로젝트에 대한 연결은 사용자가 링크를 활성화하기로 결정할 때 설정됩니다.

이 작업은 다음과 같은 방법으로 수행할 수 있습니다.

* Workfront Planning의 연결 필드 또는 레코드 세부 사항 보기의 선택적 연결 페이지에서 직접 다운스트림 연결된 프로젝트를 수동으로 만듭니다.

  수동으로 작성하면 특정 사용자 정의 양식 없이 빈 프로젝트가 생성됩니다.

  자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하세요.

* 보다 복잡한 요구 사항에 대해 Workfront Planning 자동화를 사용하여 자동으로 수행합니다.

  이러한 자동화는 테이블에서 행을 선택할 때 작업 표시줄의 버튼으로 사용할 수 있습니다.

  이렇게 하면 사람이 감독하거나 자리 표시자를 만들어 프로젝트가 실제로 필요할 때만 워크플로우 환경에서 생성하도록 할 수 있습니다.

  자세한 내용은 [Adobe Workfront Planning 레코드 자동화를 사용하여 개체 만들기](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)를 참조하십시오.


### 자동화된 활성화 빌드

대량 요청 또는 고급 자동화 요구 사항이 있는 조직의 경우 특정 이벤트나 요청 양식에 구성된 필드 값을 기반으로 브리지를 자동으로 활성화할 수 있습니다.

이 접근 방식을 사용하려면 Adobe Workfront Fusion 라이선스가 필요합니다.

자세한 내용은 [Workfront Fusion 설정 및 관리: 문서 인덱스](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-workfront-fusion-toc)를 참조하십시오.

* **전송 트리거 사용:** 양식은 깔끔한 단일 전송 이벤트를 제공하므로 Fusion 자동화의 트리거로 사용할 수 있습니다. Fusion 시나리오는 양식 제출을 감지하고 즉시 Workfront에서 연결된 프로젝트를 생성할 수 있습니다.

* **필드 값 트리거 사용:** 더 자세한 자동화를 위해 특정 필드를 모니터링하도록 Fusion을 구성할 수 있습니다. 예를 들어 &quot;실행 준비 완료&quot;라는 간단한 확인란이 촉매 역할을 할 수 있으므로 브리지를 선택하면 자동으로 브리지를 설정할 수 있습니다.

## 표면 가시성에 조회 필드 추가

프로젝트가 연결되면 프로젝트의 조회 필드를 추가하여 Planning 레코드 내에서 직접 Workfront의 실시간 데이터를 표시할 수 있습니다.

작업 영역 관리자는 조회 필드를 설정하여 연결된 프로젝트(예: 실제 완료 일자 또는 Creative 리드)의 모든 시스템 또는 사용자 정의 필드를 계획 레코드 유형으로 가져올 수 있습니다. 캡처되면 이 데이터를 여러 수준의 전략적 계층을 통해 캠페인 수준까지 롤업할 수 있습니다. 이렇게 하면 전체 마케팅 라이프사이클에서 관련자를 위한 강력한 집계 보고를 제공하여 계획 환경을 종료하지 않고도 정보를 얻을 수 있습니다.

## 전략을 작업에 연결하여 가시성 달성

이 다리의 궁극적인 가치는 실시간 가시성입니다.

작업 의도를 연결하여 중요한 비즈니스 질문에 한 눈에 답변할 수 있습니다. 다음은 이러한 질문의 예입니다.

* 당사의 &#39;FY26 브랜드 인지도&#39; 캠페인은 현재 활발하게 성과를 제공하고 있습니까?

* 우리의 전략 전술은 어느 부분에서 더 창의적인 지원이 필요한가?

* 가장 중요한 전략적 요충에 맞춰 자원을 어떻게 조정할 것인가?

## 모범 사례 및 팁

### 할 일:

* **전략 스레드&quot; 메타포를 사용합니다.** 팀에게 모든 프로젝트는 전략적 문자열에서 &quot;구슬&quot;이어야 함을 상기시킵니다.

* **전달 자동화:** 자동화를 사용하여 프로젝트 생성을 트리거하여 시간과 노력을 절약하는 동시에 데이터 연결 및 거버넌스를 개선합니다.

* **링크, 복제 안 함:** 조회 필드를 사용하여 전략 레코드에서 실시간 실행 데이터(예: 상태 또는 완료 날짜)를 표시합니다. 이를 통해 팀의 수동 업데이트 없이 항상 전략적 관점이 정확해집니다.

### 금지:

* **계획 레코드를 작업 목록으로 취급하지 마십시오.** 브리지는 전략적 의도를 실행 프로젝트에 연결하도록 설계되었습니다. 계획 기록을 &quot;내용&quot; 및 &quot;이유&quot;에 초점을 맞추고 작업 및 문제를 통해 워크플로 모듈이 세부적인 &quot;방법&quot;을 처리할 수 있도록 합니다.

* **너무 동기화하지 않음:** 모든 프로젝트 수준 세부 정보를 다시 Planning에 동기화할 필요가 없습니다. 전략 레이어를 높은 레벨과 노이즈가 없는 상태로 유지합니다.

* **브리지를 우회하지 마십시오.** Planning에 대한 링크 없이 워크플로 모듈에서 작업을 시작하는 경우 리더십에 보이지 않는 &quot;그림자 계획&quot;을 만들었습니다.

<!--original content:

# The Bridge: Connecting Strategic Intent to Projects 

 

## Goal 

Learn how to create a "strategic thread" between your high-level plans in Workfront Planning and your daily execution in the Workflow module. 

 

## Overview 

Connecting your strategy to your daily work turns vision into reality. When high-level plans are in sync with execution, you create a **strategic thread** that ensures every project and task moves the business forward. 

 

Achieving this alignment requires a set of technical links and process guardrails that connect efforts in the **Workflow module** with strategic records in **Workfront Planning (WFP)**. By bridging the gap between planning and action, you ensure that your team's energy is always focused on your highest-priority goals. 

 

## The foundation: Establishing the connection 

Before you can bridge planning and execution, a workspace manager must define which record types are eligible for a connection. 

 

### The connection field: The technical handshake 

The bridge begins with a **connection field**. This field type is the engine behind all relationships in WFP. It is an expression of intent, in that it establishes that a specific record type (like a *channel tactic*) is allowed to be linked to other objects, whether they live in the workflow module or within planning itself. 

 

### Deciding to connect 

Establishing this allowance is a configuration-level decision that typically happens before any work is created. By adding a connection field, you are architecting your environment to support a "strategic thread," regardless of how the individual records are eventually created. 

 

## Strategy and execution in sync 

To keep your strategic layer focused, we recommend focusing your planning records on high-level intent while using the Workflow module for tactical execution. This approach uses the unique strengths of both modules: 

 

*   **Workfront Planning (The strategic layer):** Stays high-level. It tracks the *Campaign*, the *Channel Tactic*, and the *Budget*. It is noise-free and executive-ready. 

*   **Workflow module (The execution layer):** Manages the tactical details. Individual "Experiences" or "Activities" are managed here as **projects, tasks, and issues**. 

 

## Activating the bridge: From intent to action 

Once the connection is configured, you must decide how to activate the link between a specific strategic record and an execution project. 

 

### Professional triage: The table-led path 

Strategists and power users often use the **table view** as their "workbench" to refine plans over time.  

*   **Deliberate handoff:** By default, creating a record in a table does not establish a link to the Workflow module. The connection to an execution project is established when a user decides to activate the link. This can be done by manually creating a downstream connected project directly from the connection field in WFP or an optional **connection view page** in the record's detail view. Note that manual creation results in a blank project without specific custom forms; for more complex needs, you can use a **native WFP automation**. These automations are available when you select a row in a table, appearing as buttons in the blue action bar at the bottom of your screen. This allows for human oversight or placeholder creation, ensuring that projects are only generated in your workflow environment when they are truly needed. 

 

### Automated activation 

For organizations with high-volume requests or advanced automation needs, the bridge can be activated automatically based on specific events or field values. 

*   **Submission triggers:** Because forms provide a single, clean "submission event," they can be used as triggers for **Fusion automations**. A scenario can detect a form submission and immediately generate a linked project in the workflow module. 

*   **Field-value triggers:** For deeper automation, you can configure **Fusion** to monitor specific fields. For example, a simple checkbox labeled "ready for execution" can serve as the catalyst, establishing the bridge automatically the moment it is checked. 

 

## Surfacing visibility: Lookup fields 

Once a project is linked, you can surface real-time data from the Workflow module directly within the WFP record. 

 

A workspace manager can set up **lookup fields** to pull any native or custom field from the linked project (such as *actual completion date* or *creative lead*) into the WFP record type. Once captured, this data can be rolled up through multiple levels of your strategic hierarchy—even all the way to the campaign level. This provides powerful aggregate reporting for stakeholders across the entire marketing lifecycle, keeping them informed without needing to leave the planning environment. 

 

## Strategy-to-action visibility 

The ultimate value of the bridge is **real-time visibility**. By connecting intent to action, you can answer critical business questions at a glance: 

 

*   "Is our 'FY26 Brand Awareness' campaign actively delivering results right now?" 

*   "Where do our strategic tactics need more creative support to stay on schedule?" 

*   "How are we aligning our resources with our highest-priority strategic pillars?" 

 

## Best practices & tips 

 

### Do: 

*   **Use the "strategic thread" metaphor.** Remind teams that every project should be a "bead" on a strategic string. 

*   **Automate the handoff.** Use automations to trigger project creation to save time and effort while also improving data connectivity and governance. 

*   **Link, don't duplicate.** Use lookup fields to surface real-time execution data (like status or completion dates) in your strategic records. This ensures your strategic views are always accurate without requiring manual updates from your team. 

 

### Don't: 

*   **Don't treat planning records as task lists.** The bridge is designed to connect strategic intent to execution projects. Keep your planning records focused on the "what" and "why," and let the workflow module handle the granular "how" through tasks and issues. 

*   **Don't over-sync.** You don't need to sync every project-level detail back to Planning. Keep the strategic layer high-level and noise-free. 

*   **Don't bypass the bridge.** If work starts in the Workflow module without a link to Planning, you've created a "Shadow Plan" that is invisible to leadership. 

-->



