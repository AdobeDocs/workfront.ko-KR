---
title: '전략적인 홈 구축: 30일 런치패드'
description: 심리적 안전을 우선시하고 중단을 최소화하며 신속한 성공을 제공하는 전략을 사용하여 Workfront Planning을 배포하는 방법에 대해 알아봅니다.
feature: Workfront Planning
role: Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
exl-id: 90b0e019-1b42-4ab2-8b4c-69f85e4c4d78
source-git-commit: 52bf41e146a11a4af4fbebfe5bb20a9765f2bc7b
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 0%

---

# 전략적인 홈 구축: 30일 런치패드

{{planning-important-intro}}

이 안내서를 사용하여 심리적 안전을 우선시하고 중단을 최소화하며 신속한 성공을 제공하는 전략을 설계하는 Adobe Workfront Planning을 배포하는 방법에 대해 알아보십시오.

이 안내서는 Workfront Planning을 구현하는 Workfront 관리자를 위한 것입니다.

## 빠르게 시작하고 지능적으로 확장하는 방법 개요

성공적인 롤아웃의 가장 일반적인 장애물은 기술이 아닙니다. &quot;기술 비난&quot;입니다. 팀이 새로운 사람, 새로운 프로세스 및 새로운 도구를 한 번에 사용하는 데 어려움을 겪게 되면 도구는 좌절의 대상이 됩니다.

30일 런치패드는 &quot;팀 우선&quot; 채택 모델을 기반으로 구축됩니다. 일반적으로 수개월의 조정이 필요한 전사적 롤아웃을 시도하는 대신, 특정 기능 단위 내에서 즉각적인 ROI를 제공하는 분산된 팀 주도의 접근 방식에 집중합니다.

## 단계별 전환을 위한 가이드 자율성 사용

제품을 성공적으로 출시하려면 가이드 자율성을 사용하는 것이 좋습니다. 즉, 관리자는 통제되는 기본값과 템플릿의 구조화된 시스템에서 팀이 작동하는 방식을 정의합니다.

도로(또는 관리되는 기본값 및 템플릿)에서 차선을 정의하는 동시에 팀이 그 안에서 고유한 작업 경로를 유연하게 선택할 수 있습니다.

가장 중요한 것은 가이드 자율성이 진화적으로 이루어져야 한다는 것이다. 첫 번째 날에 완전한 엔터프라이즈 분류법을 적용하는 대신 첫 번째 파일럿 팀의 필요에 따라 최소한의 글로벌 정의로 시작할 수 있습니다.

더 많은 팀이 온보딩됨에 따라 일반적인 패턴을 관찰하고 글로벌 표준을 반복할 수 있습니다.

관리자는 컨트롤을 포기하는 것이 아니라 실제로 작동하는 내용에 따라 지능적으로 크기를 조절합니다.

이 진화적 전환을 활성화하려면 다음을 수행합니다.

1. 혁신할 준비가 되어 있고 의지가 있는 파일럿 팀을 선택하십시오.
2. 론치 후 첫 15일을 사용하여 두 개의 모멘텀이 높은 경로 중 하나를 통해 모델을 증명하십시오.

   * **병렬 경로(또는 이중 추적 접근 방식):** 팀은 현재 워크플로를 유지하면서 Workfront Planning에서 다음 계획 주기를 동시에 모델링합니다.

     이는 단일 실패 지점 위험 없이 근육 기억력과 자신감을 구축합니다.

   * **정리 브레이크:** 샘플 데이터를 사용하여 모델의 유효성을 검사하는 초기 디자인 연습 후에 팀은 다음 주기를 위해 라이브 시작점을 Workfront Planning으로 직접 이동합니다.

   두 가지 경로 모두 이론에서 벗어나 실제 애플리케이션으로 가능한 한 빨리 이동하여 도구를 샌드박스 연습으로 남기지 않고 실제 전략 작업에 사용하도록 하는 것이 목표입니다.


## 획기적인 순간으로 가는 30일 여정 개요

성공적인 롤아웃은 추진력으로 이루어집니다. 이 30일 일정은 구성에서 첫 번째 자동화된 성공으로 이동합니다.

### 1~10일: Team Foundation

처음부터 중앙집권적 구조를 구축하여 전략적 기반을 구축한다.

복잡한 전사적 분류법은 아직 필요하지 않지만 두 개의 환경을 즉시 만들어야 합니다. 예를 들어 허브 및 스포크 아키텍처 접근 방식을 채택할 경우 다음을 만들 수 있습니다.

* **전역 분류 작업 영역**(허브): 시스템의 일반 구조 및 명명법이어야 합니다.
* 첫 번째 **팀 작업 공간**(spoke): 개별 팀의 작업 접근 방식과 일치해야 합니다.

자세한 내용은 [작업 영역 만들기](/help/quicksilver/planning/architecture/create-workspaces.md)를 참조하십시오.

이 팀 우선 아키텍처를 통해 다음과 같은 작업을 수행할 수 있습니다.

* **Spoke를 지원하는 허브를 디자인합니다.** 파일럿 팀에 가장 중요한 개체(특정 브랜드 또는 제품)에 특히 전역 분류 작업 영역을 집중할 수 있습니다. 이를 통해 설계 작업을 관리 가능한 상태로 유지하면서 기업 지배구조와 팀 자율성 간의 공동 작업을 강화할 수 있습니다.

* **보호자가 아닌 Enabler로 작동:** 규칙 설정에서 기능 구축으로 역할을 전환합니다. 팀과 협력하여 계획 환경을 구성하십시오.

* **디자인 공동 작업:** 파일럿 팀과 직접 협력하여 추상적인 기업 이상이 아닌 실제 요구를 반영하는 레코드 종류 및 필드를 정의하십시오.

* **전략을 작업에 연결:** 계획 레코드와 Workfront 개체 간의 연결을 활성화합니다.

  자세한 내용은 [연결된 레코드 종류 개요](/help/quicksilver/planning/architecture/connect-record-types-overview.md)를 참조하세요.

* **현재 데이터 미러링:** 팀의 기존 도구(예: Excel 또는 기타 핵심 응용 프로그램)를 사용하여 Workfront Planning을 채우면 데이터가 익숙하고 관련성이 있습니다.

* **유연성을 고려한 설계:** Workfront Planning은 발전하도록 설계되었습니다. 팀 수준 프로세스를 시작하여 비즈니스가 준비되면 이를 쉽게 엔터프라이즈 수준 거버넌스로 승격시키거나 마이그레이션할 수 있습니다.

### 15일: 첫 번째 돌파 순간

15일까지는 첫 메이저 우승을 노리는 것이 좋습니다. 이는 자동화된 프로젝트 생성이어야 합니다.

이를 위해서는 다음을 구현해야 합니다.

1. &quot;실행 준비&quot; 상태를 식별하는 기본 자동화를 구성합니다.

2. Workfront에서 연결된 프로젝트 만들기를 트리거합니다.

자세한 내용은 [Adobe Workfront Planning 자동화 구성](/help/quicksilver/planning/records/configure-automations-to-create-records.md)을 참조하십시오.

이렇게 하면 팀이 전략적 의도를 보고 실행 작업을 자동으로 트리거할 수 있습니다. 이 획기적인 순간은 전략과 일, 그리고 매수를 구축하는 교량의 가치를 증명합니다.

### 16~30일: 엔터프라이즈 규모로 점진적으로 전환

번개 순간을 달성하면 팀의 시작점을 Workfront Planning으로 이동할 수 있습니다.

이 팀 우선 모델이 성공하면 작동하는 패턴을 식별하여 엔터프라이즈 확장을 위한 경로를 시작합니다.

우선 팀에서 엔터프라이즈 규모로 이동하려면 다음을 고려하십시오.

* **수신 양식 도입:** 데이터 무결성을 보장하기 위해 전략적 요청을 위한 새 게이트웨이로 요청 양식을 사용합니다.

  자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.

* **관찰 및 표준화:** 전역 분류 작업 영역을 사용하여 파일럿 팀이 도구를 사용하는 방법을 관찰합니다. 이러한 실제 사례는 최종 엔터프라이즈 디자인을 형성합니다.

* **레거시 스프레드시트 사용 중단:** 프로세스가 진행됨에 따라 Workfront Planning으로 완전히 이동합니다.

* **Shift Power Users:** 직접 고속 플랜 관리를 위해 레코드 테이블 보기를 사용합니다.

  자세한 내용은 [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)를 참조하십시오.

## 론치 패드에 대한 성공 지표 개요

성공 표시를 지속적으로 찾고 검색 결과에서 조정하는 것이 좋습니다.

건강의 초기 지표를 찾아보세요.

* **채택:** 처음 5-10개의 전략 레코드가 실행 프로젝트에 성공적으로 연결되었으며 레코드를 만들고 연결된 프로젝트 생성을 자동화하는 프로세스가 매끄럽고 쉽게 반복될 수 있습니다.

* **옹호:** 파일럿 팀은 인접 팀에 도구를 전파하기 시작합니다.

* **효율성:** 자동화는 전략적 승인에서 프로젝트 시작까지의 시간을 줄입니다.

* **신뢰:** 이해 당사자는 검토를 위해 수동 상태 데크가 아닌 Workfront 계획 타임라인을 사용합니다.

## 모범 사례 및 팁

구현 성공은 사용하는 접근 방식과 처음부터 설정한 기대치에 따라 결정됩니다.

다음은 성공적인 구현을 이끌어낼 수 있는 방법에 대한 몇 가지 권장 사항입니다.

### 할 일:

* **활기찬 파일럿 팀으로 시작:** 전역 롤아웃이 중요한 향상임을 확인합니다. 혁신을 위해 열심이며 다른 사람들에게 청사진을 제공할 수 있는 팀과 함께 개념 증명에 집중하십시오.

* **벽이 아닌 차선 정의:** 탐색 활동을 중단하지 않고 구조를 제공하는 가이드 자율성을 사용합니다.

* **심리적 안전 우선 순위 지정:** 기존 도구가 새 워크플로에 익숙해질 때까지 그대로 유지된다는 사실을 팀에 알립니다.

* **빠른 승리를 축하합니다.** 전체 팀에 대한 첫 번째 자동 프로젝트 만들기를 강조 표시합니다.

* **챔피언 설정:** 전환을 이끌 각 팀의 파워 사용자를 식별합니다.

### 금지:

* **대규모의 변경은 강제하지 마십시오.** 모든 사람이 첫날 강제로 전환하면 기술 문제가 발생합니다.

* **그 이유를 무시하지 마십시오.** 모든 팀원이 전략적 스레드를 통해 작업을 보다 명확하게 하는 방법을 이해하는지 확인하십시오.

* **완벽해질 때까지 기다리지 마십시오.** 분류법이 발전합니다. 가장 잘 추측한 것부터 시작해서 점점 더 세련되게 가라.

<!--

Andy's original:

## The 30-Day Launchpad: Rolling Out Your Strategic Home 

 

## Goal 

Learn how to roll out Workfront Planning (WFP) using a strategy that prioritizes psychological safety, minimizes disruption, and delivers quick wins. 

 

## Overview: Start Fast, Scale Smart 

The most common obstacle to a successful rollout isn't technology—it's "technology-blame." When teams face new people, new processes, and new tools at once, the tool becomes a target for frustration. 

 

The 30-day launchpad is built on the **"Team-First" adoption model**. Instead of attempting an **Enterprise-Wide** rollout that usually requires months of coordination, we focus on a decentralized, team-led approach that delivers immediate ROI within a specific functional unit. 

 

## The phased transition: Guided Autonomy 

Successful rollouts use **Guided Autonomy**. This means the Admin defines the "lanes on the road" (governed defaults and templates) while allowing teams the flexibility to choose their own adventure within them.  

 

Crucially, Guided Autonomy is **evolutionary**. Instead of enforcing a complete enterprise taxonomy on Day 1, the Admin starts with minimal global definitions based on the needs of the first pilot team. As more teams are onboarded, the Admin observes common patterns and iterates on the global standards. You aren't surrendering control; you are scaling it intelligently based on what actually works. 

 

To activate this evolutionary shift, choose a pilot team that is ready and willing to innovate. Use the first 15 days to prove the model through one of two high-momentum paths: 

 

*   **The Parallel Path (Dual-Tracking):** The team maintains their current workflow while simultaneously modeling their next planning cycle in WFP. This builds "muscle memory" and confidence without the risk of a single point of failure. 

*   **The Clean Break:** After an initial design exercise using sample data to validate the model, the team moves their "live" planning start point directly into WFP for their next cycle. 

 

In both paths, the goal is to move beyond theory and into real-world application as quickly as possible, ensuring the tool is used for actual strategic work rather than remaining a "sandbox" exercise. 

 

## The 30-day timeline: Your "lightning moment" 

A successful rollout is powered by momentum. This 30-day schedule moves you from configuration to your first automated win. 

 

### Days 1-10: The team foundation 

Build a strategic foundation by establishing a **lightweight Hub-and-Spoke architecture** from Day 1. While a complex enterprise-wide taxonomy is not required yet, you should immediately create two environments: a **Global Classification Workspace** (the Hub) and your first **Team Workspace** (the Spoke). 

 

This **Team-First** architecture allows you to: 

 

*   **Design the Hub to support the Spoke:** Focus the global classification workspace specifically on the objects that matter most to your pilot team (e.g., their specific Brands or Products). This firms up the **collaborative handshake between enterprise governance and team autonomy** while keeping the design effort manageable. 

*   **Act as an Enabler, not a Guardian:** Shift your role from rule-setting to capability-building. Partner with the team to structure their planning environment. 

*   **Collaborate on design:** Work directly with your pilot team to define the record types and fields that reflect their real-world needs, not an abstract corporate ideal. 

*   **Connect strategy to work:** Enable the link between your planning records and the workflow module. 

*   **Mirror current data:** Use the team's existing tools (Excel/Core) to populate WFP, ensuring the data feels familiar and relevant. 

*   **Built for flexibility:** Remember that Workfront Planning is designed to evolve. You can start with team-level processes and easily elevate or migrate them to enterprise-level governance when the business is ready. 

 

### Day 15: The first "lightning moment" 

Aim for your first major win by Day 15: **automated project creation**. 

*   Configure a native automation that detects a "Ready to Execute" status. 

*   Trigger the creation of a linked project in the workflow module. 

*   **The value:** Your team sees their strategic intent automatically trigger execution work. This "lightning moment" proves the value of the bridge and builds buy-in. 

 

### Days 16-30: Gradual transition toward Enterprise Scale 

With the "lightning moment" achieved, move the team's start point into WFP. As this **Team-First** model succeeds, you begin the path toward **Enterprise Scale** by identifying patterns that work. 

 

*   **Introduce the intake form:** Use the form as the new gateway for strategic requests to ensure data integrity. 

*   **Observe and standardize:** Use the Primary Workspace to observe how the pilot team uses the tool. These real-world examples will shape your eventual enterprise design. 

*   **Decommission legacy spreadsheets:** Move fully into WFP as the process matures. 

*   **Shift power users:** Use the **table view** for direct, high-velocity plan management. 

 

## Success metrics for the launchpad 

Look for these early indicators of health: 

*   **Adoption:** The first 5-10 strategic records successfully link to execution projects. 

*   **Advocacy:** The pilot team begins evangelizing the tool to adjacent teams. 

*   **Efficiency:** Automation reduces the time from strategic approval to project start. 

*   **Trust:** Stakeholders use WFP timelines rather than manual status decks for reviews. 

 

## Best practices and tips 

 

### Do: 

*   **Start with an excited pilot team.** Acknowledge that a global rollout is a significant lift. Focus on a POC with a team that is eager to innovate and can provide a blueprint for others. 

*   **Define lanes, not walls.** Use Guided Autonomy to provide structure without killing exploration. 

*   **Prioritize psychological safety.** Let teams know that legacy tools stay until they are comfortable with the new flow. 

*   **Celebrate the quick wins.** Highlight the first automated project creation to the entire team. 

*   **Establish a champion.** Identify a power user in each team to lead the transition. 

 

### Don't: 

*   **Don't mandate "big bang" changes.** Forcing everyone to switch on Day 1 causes technology-blame. 

*   **Don't ignore the "why."** Ensure every team member understands how the strategic thread makes their work more visible. 

*   **Don't wait for perfection.** Your taxonomy will evolve. Start with your best guess and refine as you go. 

-->