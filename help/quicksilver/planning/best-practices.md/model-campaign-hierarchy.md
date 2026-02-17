---
title: '성공 설계: 캠페인 계층 구조 모델링'
description: 복잡한 비즈니스 프로세스를 "Centers of Gravity" 및 다중 작업 공간 아키텍처를 사용하여 확장 가능하고 관리되는 캠페인 계층으로 변환하는 방법에 대해 알아봅니다.
feature: Workfront Planning
role: Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 02e3b55f-9188-42bf-8d0b-c9fed86c63c4
source-git-commit: 699add479d958b9f3fc01ae30513ddf6689620f1
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 0%

---

# 성공 설계: 캠페인 계층 구조 모델링

<!--see the file again for additional comments from Seth and others-->

{{planning-important-intro}}

Adobe Workfront Planning에서 무게 중심 및 다중 작업 공간 아키텍처를 사용하여 복잡한 비즈니스 프로세스를 확장 가능하고 관리되는 캠페인 계층으로 변환하는 방법을 알아봅니다.

이 안내서는 Workfront Planning에서 환경 아키텍처를 구현하고 디자인하는 Workfront 관리자 및 고급 사용자를 위한 것입니다.

## 성공 아키텍처 개요

마케팅 작업이 발달함에 따라 데이터의 복잡성도 증가합니다. 명확한 청사진이 없으면 귀하의 마케팅 기록 시스템은 연결이 끊긴 기록, 충돌하는 용어 및 보고 사일로의 정크 드로워가 될 수 있습니다.

성공 아키텍처를 구축할 때 Workfront Planning에서 캠페인 계층 구조를 모델링하기 위한 프레임워크를 설정합니다. 이를 통해 스프레드시트 혼돈에서 모든 팀이 동일한 언어를 구사하면서도 실행하는 데 필요한 민첩성을 유지할 수 있는 관리 및 개체 지향 모델로 전환됩니다.

## 계층을 구축하여 의도 수준을 정의합니다.

명확성과 확장성을 유지하려면 Workfront Planning에서 워크플로우를 디자인할 때 검증된 핵심 경로부터 시작하는 것이 좋습니다.

여기에서 아키텍처에 수준을 추가하여 전략을 확장할 수 있습니다.

### 핵심 경로: 전략에서 실행으로 가져오는 방법

조직은 운영 요구 사항이 발전함에 따라 이 계층을 확장할 수 있지만, 아래 섹션에 설명된 세 가지 수준으로 시작하면 전략과 실행 간에 강력한 브리지를 확보할 수 있습니다.

연구 결과에 따르면 Workfront Planning의 가장 성공적인 구현은 Planning과 Workfront을 모두 포괄하는 깔끔한 3계층 모델에서 성공한다는 것을 알게 되었습니다.

다음은 성공적인 Planning 구현의 수준이며, 프로세스에서 지원하기 위해 생성할 수 있는 객체의 수준입니다.

* **수준 1: 캠페인(Workfront 계획)**

   * **포커스:** 장기 전략 지주와 연간 이니셔티브를 정의합니다. 예를 들어 &quot;FY26 Global Brand Awareness&quot;라는 조직의 이니셔티브를 정의합니다. 이는 주어진 시간대에 집중하는 것입니다. 이 이니셔티브를 지원하는 캠페인을 만드십시오.

   * **담당자:** 이 수준에 대한 이해 당사자는 마케팅 책임자, 마케팅 담당 VP 또는 기타 전략 잠재 고객일 수 있습니다.

  자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

* **수준 2: 채널 전술(Workfront 계획)**

   * **포커스:** 특정 채널에 대한 &quot;내용&quot;을 요약하는 운영 브리핑을 정의합니다. 이것은 작업이 시작되기 전에 전략적 의도의 마지막 계층입니다. 예를 들어 &quot;1분기 소셜 미디어 공세&quot; 전술을 만듭니다. 그런 다음 캠페인과 연결할 수 있습니다.

   * **담당자:** 주요 이해 당사자는 마케팅 운영 리더, 채널 리더 또는 캠페인 관리자입니다.

* **수준 3: 프로젝트(계획 및 Workfront)**

   * **포커스:** 이니셔티브를 수행할 정확한 경험이나 활동을 실행하십시오. 일부 결과물은 소셜 게시물, 이메일, 웹 페이지와 같이 구체적입니다.

   * **구현:** Planning에서 전술을 만들고 이를 Workfront의 **프로젝트**&#x200B;에 직접 연결할 수 있습니다. 여기서 개별 결과물을 작업과 문제로 관리할 수 있습니다.

   * **담당자:** 여기에 있는 주요 이해 당사자는 창의적인 사람, 개별 기여자, 이니셔티브를 지원하는 작업을 담당하는 사람입니다.

### 전략적 확장: 수준을 추가하는 방법

핵심 경로를 설정한 후에는 구체적인 비즈니스 복잡성을 신중하게 고려한 후 계층을 추가할 수 있습니다.

다음과 같은 추가 항목을 만드는 것이 유용할 수 있습니다.

* **채널 계획:** 캠페인 및 전술 간의 계층을 사용하여 다양한 기능의 전략을 그룹화합니다. 예를 들어 &quot;디지털 전략&quot;이라는 플랜입니다.

* **활동:** 볼륨이 낮은 환경에서 작업하는 경우(연간 5,000개 이하의 결과물이 있을 수 있음), 일부 팀은 개별 경험을 Workfront 프로젝트가 되기 전에 Workfront Planning 레코드로 추적하는 것을 선호할 수 있습니다.

>[!IMPORTANT]
>
>조직에서 연간 5,000개 이상의 활동을 생성하는 경우 개별 결과물 추적을 Workfront으로 이동해야 합니다.
>
>Planning에서 대량 경험 레코드를 관리하면 데이터가 누적되어 전략적 가시성을 흐리게 할 수 있습니다.
>최대 효율성을 위해 다음과 같은 광범위한 지침을 권장합니다.
>
>* &quot;이유&quot; 및 &quot;내용&quot;에 Planning 사용
>* 대용량 &quot;방법&quot;에 Workfront을 사용합니다.

## 아키텍처 구축을 위한 무게 중심 이해

엔터프라이즈급 기록 마케팅 시스템 은 단일 작업 공간에 구축되지 않습니다. 이 회사는 기록 유형을 자연적인 무게 중심에서 관리하는 &quot;허브 앤 스포크&quot; 아키텍처를 사용합니다.

자세한 내용은 [전략적 홈 롤아웃: 30일 런치패드](/help/quicksilver/planning/best-practices.md/30-day-launchpad.md)를 참조하십시오.

Hub-and-spoke 접근 방식을 사용하여 아키텍처를 구축하려면 다음을 만들어야 합니다.

* 분류 허브
* 전략 계획 작업 공간
* 기능성 바퀴살

### 분류 허브를 분류로 빌드합니다

먼저 글로벌 분류에 대해 하나의 중앙 집중식 작업 영역을 설정하여 조직의 모든 사람이 이해해야 하는 주요 개념을 정의해야 합니다. 예를 들어, 중앙 작업 영역에서 브랜드, 지역, 제품, 가상 사용자 등의 레코드 유형을 만듭니다.

자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

분류를 만들 때 다음을 설정하십시오.

* **기본 위치:** 기본 작업 영역을 선택하십시오. 이 작업 영역은 사용자가 만드는 레코드 종류에 대한 신뢰할 수 있는 소스여야 합니다.

* **이점:** 이러한 정의를 비즈니스의 나머지 부분에 동기화하면 &quot;지역: EMEA&quot;와 같은 개념이 모든 팀에 동일한 의미를 갖는다는 것을 명확히 알 수 있습니다.

### 전략적 Planning 작업 영역을 경영진 센터로 생성

Executive Center는 높은 수준의 캠페인(및 모든 채널 계획)이 살아 있는 곳입니다.

* **기본 위치:** 전략적 의사 결정을 위한 소음 없는 환경을 제공하는 중추의 중심입니다.

* **이점:** 리더쉽은 일상적인 전술적 잡음을 듣지 않고 캠페인 포트폴리오를 관리할 수 있습니다.

### 기능 스포크를 팀의 작업 공간으로 정의합니다.

기능 단위(소셜, Creative, 이메일)에는 전략을 관리할 수 있는 자체 작업 공간이 있습니다.

* **기본 위치:** 이러한 작업 공간은 로컬 팀 실행을 위한 개별 중추입니다.

* **이점:** 팀은 고유한 로컬 개체를 유지하면서 허브의 전역 캠페인과 분류를 사용합니다.

  예를 들어 팀은 중앙 작업 공간의 캠페인 레코드 유형을 팀의 작업 공간에 추가할 수 있지만, 해당 작업 공간에만 관련된 캠페인을 만들 수 있습니다. 캠페인의 예로는 &quot;미디어 아울렛&quot; 또는 &quot;사용 권한&quot;이 있습니다.

## 명사 기반 거버넌스 접근 방식 사용

아키텍처가 압박을 받지 않도록 하려면 명사 기반 거버넌스의 원칙을 따르십시오.

Workfront Planning에서 엔티티를 생성할 때 다음 사항을 권장합니다.

* **동사가 아닌 명사 사용:** 수행할 작업이 아니라 추적 중인 항목 뒤에 레코드 종류의 이름을 지정합니다(&quot;Campaign&quot; 또는 &quot;Tactional&quot;). 이름을 &quot;Campaign&quot; 또는 &quot;Planning&quot;으로 지정하지 마십시오.

* **명명법 표준화:** 모든 작업 영역에서 동일한 이름을 사용합니다. 이를 통해 경영진 보고를 위해 전체 포트폴리오에 걸쳐 데이터를 집계할 수 있습니다.

## 기존 포트폴리오와 프로그램은 어떻게 됩니까?

성숙 조직에 대한 일반적인 질문은 Workfront에서 이미 빌드한 포트폴리오 및 프로그램을 처리하는 방법입니다. 과거에는 이런 것들이 전략기획을 흉내내는 데 자주 사용됐다.

이제 이러한 접근 방식을 Workfront Planning으로 전환하여 자연스럽게 전략적인 계획 수립 방식에 맞는 것을 권장합니다.

### 포트폴리오 및 프로그램을 레코드 유형으로 바꾸기

많은 조직에서 포트폴리오는 높은 수준의 브랜드 또는 사업부를 나타내는 데 사용되며 프로그램은 전략적 주제를 나타냅니다.

Workfront Planning에서 이들은 분류 허브에서 레코드 유형으로 가장 잘 모델링됩니다.

브랜드 또는 비즈니스 단위를 레코드 유형으로 취급하여 기업 전체의 캠페인 또는 전술에 연결할 수 있으므로, 정적 Portfolio - 프로그램 구조보다 훨씬 유연한 보고를 제공할 수 있습니다.

### 보고 브리지 전략 사용

Workfront Planning은 전략적 의도의 미래이지만 Canvas Dashboard를 통한 기본 보고는 아직 성숙되고 있습니다.

많은 조직이 여전히 Workfront의 기존 Portfolio 및 프로그램 구조에 연결된 강력한 보고 기능을 사용하고 있습니다.

다음 자료를 참조하십시오.

* 포트폴리오 및 프로그램을 삭제하지 마십시오.
* Planning 자동화를 사용하여 레코드 유형과 포트폴리오 및 프로그램 간에 브리지를 생성합니다.

  Workfront Planning에서 전술이나 캠페인을 만들면 해당 레코드가 Workfront에서 해당 Portfolio 또는 프로그램을 생성할 수 있습니다.

  자세한 내용은 [Adobe Workfront Planning 레코드 자동화를 사용하여 개체 만들기](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)를 참조하십시오.

이를 통해 다음을 수행할 수 있습니다.

* 타임라인 및 캘린더를 사용하여 Workfront Planning의 우수한 전략 시각화를 즐겨보십시오.

* 아직 캔버스로 이동할 준비가 되지 않은 이해 당사자를 위해 Workfront에서 기존 보고를 유지 관리합니다.

## 모범 사례 및 팁

### 도스

* **핵심 경로 우선 접근 방식을 고수하십시오.** 복잡성을 추가하기 전에 Campaign-to-Tactic-to-Project 흐름을 설정하십시오.

* **기본 작업 공간 지정:** 각 레코드 유형에 보고를 위한 집계 역할을 하는 하나의 홈 작업 공간이 있는지 확인합니다.

* **수신 프로세스에 대한 요청 양식의 우선 순위 지정:** 메타데이터 무결성을 보장하려면 Workfront Planning에서 정교도가 낮은 그룹에 대해 레코드 양식을 사용하십시오.

  >[!CAUTION]
  >
  >고급 사용자는 표 보기에서 직접 데이터를 입력할 때 많은 이점을 얻을 수 있지만 이 경우 주의해서 접근해야 합니다.
  >테이블의 일괄 변경 사항은 다른 관련자들에게 쉽게 데이터 문제를 초래할 수 있습니다.

### 금지

* **일반화를 사용하지 않음:** 예를 들어 &quot;핵심&quot; 환경에 대해 말하는 대신 실행에 대해 말할 때 Workfront 및 프로젝트 개체를 구체적으로 참조하십시오.

* **복잡하게 만들지 않음:** 모든 추가 수준의 계층에서 관리 세금을 추가합니다. 현재 대답할 수 없는 비즈니스 질문에 답변하는 수준만 추가합니다.

* **사일로를 만들지 않음:** 팀이 동일한 데이터를 다시 입력하지 않도록 레코드 형식이 작업 영역 간에 공유되어 있는지 확인하십시오.


<!--original content:


## Goal 

Learn how to translate your complex business processes into a scalable, governed campaign hierarchy using "Centers of Gravity" and a multi-workspace architecture. 

 

## Overview 

As your marketing operations scale, so does the complexity of your data. Without a clear blueprint, your Marketing System of Record (MSOR) can quickly become a "junk drawer" of disconnected records, conflicting terminology, and reporting silos. 

 

The "Blueprint of Success" is a framework for modeling your campaign hierarchy in Workfront Planning. It moves you from "spreadsheet chaos" to a governed, object-oriented model that ensures every team speaks the same language while maintaining the agility they need to execute. 

 

## The Hierarchy: Finding Your Levels of Intent 

To maintain clarity and scalability, we recommend starting with a proven **Core Path**. While organizations can expand this hierarchy as their operational needs evolve, beginning with these three levels ensures a strong bridge between strategy and execution. 

 

### The Core Path: Strategy to Action 

Most successful implementations thrive on a clean, three-tier model that spans both Planning and Workflow: 

 

1. **Level 1: Campaigns (Planning Module)** 

    * **Focus:** Long-term strategic pillars and annual initiatives (e.g., "FY26 Global Brand Awareness").  

    * **Persona:** CMO, VP of Marketing, Strategic Leads. 

2. **Level 2: Channel Tactics (Planning Module)** 

    * **Focus:** The operational briefs defining the "what" for specific channels (e.g., "Q1 Social Media Blitz"). This is the final layer of strategic intent before work begins. 

    * **Persona:** Marketing Ops, Channel Leads, Campaign Managers. 

3. **Level 3: Workflow Projects (Workflow Module)** 

    * **Focus:** The actual execution of "Experiences" or "Activities" (e.g., specific social posts, emails, web pages).  

    * **Implementation:** Tactics in Planning link directly to **Projects** in the Workflow module, where individual deliverables are managed as tasks and issues. 

    * **Persona:** Creatives, Individual Contributors. 

 

### Strategic Expansion: Adding More Levels 

Once the core path is established, organizations may choose to add additional layers after careful consideration of their specific business complexity: 

 

* **Channel Plans:** A layer between *Campaigns* and *Tactics* to group cross-functional strategies (e.g., "Digital Strategy"). 

* **Workfront Planning Activities:** In lower-volume environments (typically <5,000 deliverables/year), some teams prefer to track individual "Experiences" as Workfront Planning records before they become projects. 


>[!TIP]
>
>**Crucial Tip: The 5,000 Deliverable Threshold** 
>
>If your organization produces more than 5,000 activities per year, you should **always** offload individual deliverable tracking to the **Workflow module**. Managing high-volume "Experience" records in Planning can lead to data accumulation that obscures your strategic visibility. Use Planning for the "Why" and "What," and the Workflow module for the high-volume "How." 

 

## Architecture: Centers of Gravity 

An enterprise-grade MSOR isn't built in a single workspace. It uses a "Hub-and-Spoke" architecture where record types are managed in their natural **Centers of Gravity**. 

 

### 1. The Taxonomy Hub (Classifications) 

Establish one centralized workspace for your "Global Classifications" (e.g., Brands, Regions, Products, Personas). 

* **Primary Location:** This workspace is the "Source of Truth" for these objects. 

* **The Benefit:** By syndicating these definitions to the rest of the business, you solve "Semantic Drift"—ensuring that "Region: EMEA" means the same thing to every team. 

 

### 2. The Strategic Planning Workspace (Executive Center) 

This is where high-level **Campaigns** (and any **Channel Plans**) live.  

* **Primary Location:** This is the executive center of gravity, providing a noise-free environment for strategic decision-making. 

* **The Benefit:** Leadership can manage the portfolio without seeing the day-to-day tactical mess. 

 

### 3. Functional Spokes (Team Workspaces) 

Functional units (Social, Creative, Email) have their own workspaces to manage their **Tactics**. 

* **Primary Location:** These workspaces are the center of gravity for local team execution.  

* **The Benefit:** Teams "consume" the global campaigns and classifications from the hubs, while maintaining their own local objects (like *Media Outlets* or *Usage Rights*). 

 

## Noun-Based Governance: Speak One Language 

To ensure your blueprint holds up under pressure, follow the principle of **Noun-Based Governance**.  

 

* **Use Nouns, Not Verbs:** Name your record types after the "things" you are tracking (`Campaign`, `Tactic`), not the "actions" (`Campaigning`, `Planning`). 

* **Standardize Nomenclature:** Use the same names across all workspaces. This allows you to aggregate data across the entire portfolio for executive reporting. 

 

## What About Existing Portfolios and Programs? 

A common question for mature organizations is how to handle the Portfolios and Programs they've already built in the **Workflow module**. In the past, these objects were often used to mimic strategic planning. 

 

### 1. Portfolios & Programs → Record Types 

In many organizations, **Portfolios** are used to represent high-level Brands or Business Units (BUs), while **Programs** represent strategic themes. 

* **The Shift:** These are best modeled as **Record Types** in your **Taxonomy Hub**. By treating "Brand" or "Business Unit" as a record type, you can link them to any campaign or tactic across the entire enterprise, providing much more flexible reporting than a static Portfolio/Program structure. 

 

### 2. The "Reporting Bridge" Strategy 

While Workfront Planning is the future of strategic intent, its native reporting via **Canvas Dashboards** is still maturing. Many organizations still rely on the robust reporting capabilities tied to their legacy Portfolio and Program structures in the Workflow module. 

* **The Recommendation:** Don't delete your Portfolios and Programs yet. Instead, use **Fusion automations** to create a bridge.  

* **How it Works:** When a Tactic or Campaign is created in Workfront Planning, Fusion can automatically mirror that record into a corresponding Portfolio or Program in the Workflow module. This allows you to: 

    1. Enjoy Workfront Planning's superior **strategic visualization** (Timelines/Calendars). 

    2. Maintain your **legacy reporting** in the Workflow module for stakeholders who aren't yet ready to move to Canvas. 

## Best Practices & Tips 

### Do: 

* **Stick to the Core Path first.** Establish your Campaign-to-Tactic-to-Project flow before adding more complexity. 

* **Designate Primary Workspaces.** Ensure each record type has one "home" workspace (its center of gravity) that acts as the aggregator for reporting. 

* **Prioritize Forms for Intake.** Use record forms for groups with less sophistication in Workfront Planning to ensure metadata integrity. While Power Users may benefit from direct data entry in Table views, this should be approached with caution—bulk changes in a table can easily create data headaches for other stakeholders. 
 

### Don't: 

* **Don't say "Core".** Refer specifically to the **Workflow module** and the **Project** objects when talking about execution. 

* **Don't over-complicate.** Every additional level of hierarchy adds a "management tax." Only add levels that answer a business question you can't currently answer. 

* **Don't create silos.** Ensure your record types are shared across workspaces so teams aren't re-typing the same data.
-->