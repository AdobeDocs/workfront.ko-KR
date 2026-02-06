---
title: '30일 실행 패드: 전략적 홈 롤아웃'
description: 심리적 안전을 우선시하고 중단을 최소화하며 신속한 성공을 제공하는 전략을 사용하여 Workfront Planning을 배포하는 방법에 대해 알아봅니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
exl-id: 90b0e019-1b42-4ab2-8b4c-69f85e4c4d78
source-git-commit: b2f1bbfbbec23a5400552eb0f989e0a0dc58413c
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 0%

---

# 30일 런치패드: 전략적 홈 구축

{{planning-important-intro}}

이 안내서를 사용하여 심리적 안전을 우선시하고 중단을 최소화하며 신속한 성공을 제공하는 전략을 설계하는 Adobe Workfront Planning을 배포하는 방법에 대해 알아보십시오.

## 빠르게 시작하고 지능적으로 확장하는 방법 개요

성공적인 롤아웃의 가장 일반적인 장애물은 기술이 아닙니다. &quot;기술 비난&quot;입니다. 팀이 새로운 사람, 새로운 프로세스 및 새로운 도구를 한 번에 사용하는 데 어려움을 겪게 되면 도구는 좌절의 대상이 됩니다.

30일 런치패드는 &quot;팀 우선&quot; 채택 모델을 기반으로 구축됩니다. 일반적으로 수개월의 조정이 필요한 전사적 롤아웃을 시도하는 대신, 특정 기능 단위 내에서 즉각적인 ROI를 제공하는 분산된 팀 주도의 접근 방식에 집중합니다.

## 자율권의 단계적 전환

제품의 성공적인 롤아웃은 가이드 자율성을 사용합니다. 즉, 관리자는 통제되는 기본값과 템플릿으로 구성된 시스템에서 팀이 작업하는 방법을 정의합니다. 팀은 &quot;도로 위의 차선&quot;(기본 사항과 템플릿을 적용함)을 정의하며, 이를 통해 팀이 내부에서 모험을 유연하게 선택할 수 있습니다.

가장 중요한 것은, 안내식 자율성이 진화적이라는 것이다. 관리자는 첫 번째 날에 전체 엔터프라이즈 분류를 적용하는 대신 첫 번째 파일럿 팀의 요구 사항에 따라 최소한의 글로벌 정의로 시작합니다.

더 많은 팀이 온보딩됨에 따라 관리자는 일반적인 패턴을 관찰하고 글로벌 표준을 반복합니다.

관리자는 컨트롤을 포기하는 것이 아니라 실제로 작동하는 내용에 따라 지능적으로 크기를 조절합니다.

이 진화적 전환을 활성화하려면 다음을 수행합니다.

1. 혁신할 준비가 되어 있고 의지가 있는 파일럿 팀을 선택하십시오.
2. 론치 후 첫 15일을 사용하여 두 개의 모멘텀이 높은 경로 중 하나를 통해 모델을 증명하십시오.

   * **병렬 경로(또는 이중 추적 접근 방식):** 팀은 현재 워크플로를 유지하면서 Workfront Planning에서 다음 계획 주기를 동시에 모델링합니다.

     이는 단일 실패 지점 위험 없이 근육 기억력과 자신감을 구축합니다.

   * **정리 브레이크:** 샘플 데이터를 사용하여 모델의 유효성을 검사하는 초기 디자인 연습 후에 팀은 다음 주기를 위해 라이브 시작점을 Workfront Planning으로 직접 이동합니다.

   두 가지 경로 모두 이론에서 벗어나 실제 애플리케이션으로 가능한 한 빨리 이동하여 도구를 샌드박스 연습으로 남기지 않고 실제 전략 작업에 사용하도록 하는 것이 목표입니다.

<!--left here-->

## 30일 일정: &quot;번개 순간&quot;

성공적인 롤아웃은 추진력으로 이루어집니다. 이 30일 일정은 구성에서 첫 번째 자동화된 성공으로 이동합니다.



### 1~10일: Team Foundation

1일부터 **경량 허브 및 스포크 아키텍처**&#x200B;를 설정하여 전략적 기반을 구축합니다. 복잡한 전사적 분류법이 아직 필요하지 않지만 **전역 분류 Workspace**(허브)과 첫 번째 **팀 Workspace**(스포크)의 두 가지 환경을 즉시 만들어야 합니다.



이 **Team-First** 아키텍처를 사용하면 다음 작업을 수행할 수 있습니다.



* **Spoke를 지원하도록 Hub 디자인:** 파일럿 팀에 가장 중요한 개체(예: 특정 브랜드 또는 제품)에 특히 전역 분류 작업 영역을 집중하십시오. 이 회사는 설계 작업을 관리 가능하게 유지하면서 기업 거버넌스와 팀 자율성 간의 **공동 작업을 지원합니다**.

* **보호자가 아닌 Enabler로 작동:** 규칙 설정에서 기능 구축으로 역할을 전환합니다. 팀과 협력하여 계획 환경을 구성하십시오.

* **디자인 공동 작업:** 파일럿 팀과 직접 협력하여 추상적인 기업 이상이 아닌 실제 요구를 반영하는 레코드 종류 및 필드를 정의하십시오.

* **전략에 연결:** 계획 레코드와 워크플로 모듈 간의 연결을 활성화합니다.

* **현재 데이터 미러링:** 팀의 기존 도구(Excel/Core)를 사용하여 Workfront Planning을 채우면 데이터가 익숙하고 관련성이 있습니다.

* **유연성을 고려한 설계:** Workfront Planning은 발전하도록 설계되었습니다. 팀 수준 프로세스를 시작하여 비즈니스가 준비되면 이를 쉽게 엔터프라이즈 수준 거버넌스로 승격시키거나 마이그레이션할 수 있습니다.



### 15일: 첫 번째 &quot;번개 순간&quot;

15일까지 첫 번째 메이저 우승을 노립니다. **자동화된 프로젝트 만들기**.

* &quot;실행 준비&quot; 상태를 감지하는 기본 자동화를 구성합니다.

* 워크플로 모듈에서 연결된 프로젝트 만들기를 트리거합니다.

* **값:** 팀이 전략적 의도를 보고 실행 작업을 자동으로 트리거합니다. 이 &quot;번개 순간&quot;은 다리의 가치를 증명하고 바이인을 구축합니다.



### 16~30일: 엔터프라이즈 규모로 점진적으로 전환

&quot;번개 순간&quot;을 달성한 상태에서 팀의 시작점을 Workfront Planning으로 이동합니다. 이 **Team-First** 모델이 성공하면 작동하는 패턴을 식별하여 **Enterprise Scale**&#x200B;에 대한 경로를 시작합니다.



* **수신 양식 도입:** 양식을 전략적 요청에 대한 새 게이트웨이로 사용하여 데이터 무결성을 확인합니다.

* **관찰 및 표준화:** 기본 Workspace을 사용하여 파일럿 팀이 도구를 사용하는 방법을 관찰합니다. 이러한 실제 사례는 최종 엔터프라이즈 디자인을 형성합니다.

* **레거시 스프레드시트 사용 중단:** 프로세스가 진행됨에 따라 Workfront Planning으로 완전히 이동합니다.

* **Shift Power Users:** **테이블 보기**&#x200B;를 사용하여 직접 고속 플랜 관리



## 실행 패드에 대한 성공 지표

건강의 초기 지표를 찾아보세요.

* **채택:** 처음 5-10개의 전략 레코드가 실행 프로젝트에 성공적으로 연결되었습니다.

* **옹호:** 파일럿 팀은 인접 팀에 도구를 전파하기 시작합니다.

* **효율성:** 자동화는 전략적 승인에서 프로젝트 시작까지의 시간을 줄입니다.

* **신뢰:** 이해 당사자는 검토를 위해 수동 상태 데크가 아닌 Workfront 계획 타임라인을 사용합니다.



## 모범 사례 및 팁



### 수행:

* **흥분한 파일럿 팀으로 시작하십시오.** 전역 롤아웃이 중요한 향상임을 확인합니다. 혁신을 위해 열심이며 다른 사람들에게 청사진을 제공할 수 있는 팀과의 POC에 주력한다.

* **벽이 아닌 차선을 정의합니다.** 탐색을 중단하지 않고 구조를 제공하기 위해 가이드 자율성을 사용합니다.

* **심리적 안전을 우선시합니다.** 이전 도구가 새 흐름에 익숙해질 때까지 유지된다는 사실을 팀에 알려 줍니다.

* **빠른 승리를 축하합니다.** 전체 팀에 대한 첫 번째 자동화된 프로젝트 만들기를 강조 표시합니다.

* **챔피언을 설정합니다.** 전환을 이끌 각 팀의 고급 사용자를 식별합니다.



### 금지:

* **&quot;대박&quot; 변경을 요구하지 않습니다.** 모든 사람을 1일에 강제로 전환하면 기술 문제가 발생합니다.

* **&quot;이유&quot;를 무시하지 마십시오.** 모든 팀원이 전략적 스레드를 통해 작업을 보다 쉽게 볼 수 있도록 하는 방법을 이해하는지 확인합니다.

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