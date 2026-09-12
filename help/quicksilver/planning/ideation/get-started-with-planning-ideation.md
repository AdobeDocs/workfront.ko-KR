---
title: Adobe Workfront Planning용 Ideation Space 시작
description: 이제 Adobe Workfront Planning에서는 캠페인을 시작하기 전에 식별할 수 있는 추가 기능을 제공합니다. AI의 기능을 활용하여 데이터와 직접 입력을 가시적인 계획으로 전환하고 빈 페이지가 아닌 정보에 입각한 시작점을 팀에 제공합니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 1%

---


# Adobe Workfront Planning의 관념화 공간 시작

<!--
Should we add a new Feature to ExL for "Strategic Ideation"?
-->

<!--information in this article come from this document, in addition to my notes for this project up to August 31, 2026:

https://adobe-my.sharepoint.com/:w:/r/personal/alinaw_adobe_com/_layouts/15/Doc.aspx?sourcedoc=%7B513DE769-B70B-4040-8C9E-6A9B8E3167BB%7D&file=getting-started-catalyze.docx&action=default&mobileredirect=true
-->

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. **관념화 공간 Beta** 프로그램의 일부로서만 사용할 수 있습니다. </span>\
</span>

{{planning-important-intro}}

Adobe Ideation 공간은 Adobe Planning에 직접 내장된 Workfront의 AI 기반 전략적 ideation 기능입니다. 이는 마케팅 팀에게 캠페인 전략을 위한 구조화된 데이터 기반의 시작 지점을 제공하며, 수동 연구 및 추측 작업을 조직의 실제 성과 기록에서 기반으로 하는 AI 생성 브리핑으로 대체합니다.

Workfront Planning에서만 액세스할 수 있는 아이디어 공간은 계획, 프로덕션 및 전달을 수행하기 전에 캠페인 라이프사이클의 맨 앞에 있으며 팀이 작업을 계획하고 실행하는 Workfront Planning 작업 공간으로 직접 유입됩니다.

## 제품 가용성

변경될 수 있는 관념화 공간에 대한 계획된 릴리스 타임라인에는 다음 이정표가 포함됩니다.

* **마감된 Beta:** 적은 수의 고객이 있는 2026년 7월에 출시되었습니다.
* **Beta 열기:**&#x200B;은(는) 2026년 9월을 목표로 합니다. 이는 고객이 옵션을 적극적으로 옵트아웃하지 않고 적극적으로 옵션을 켜고 구성해야 하는 옵트인 오퍼입니다.
* **일반 가용성:** 2026년 하반기에 타깃팅됨.

## 제품 요구 사항

조직과 동시에 다음 패키지에 액세스할 수 있는 경우 관념화 공간에 액세스할 수 있습니다.

* Workfront Planning 패키지가 포함된 Adobe Workfront Workflow 패키지

  또는

  독립형 제품으로서의 Adobe Workfront Planning

  >[!NOTE]
  >
  >관념화 공간은 Adobe Planning에서만 액세스할 수 있습니다. Ideation 공간에 액세스하려면 별도의 로그인이 필요하지 않습니다. Workfront Planning에 로그인할 수 있는 경우 즉시 사용할 수 있습니다.

* Adobe GenStudio for Performance Marketing

<!-- only required for closed beta, see below: * Adobe Customer Journey Analytics-->

Ideation 공간을 사용하는 데 필요한 액세스에 대한 자세한 내용은 [Ideation 공간을 사용하는 데 필요한 액세스](/help/quicksilver/planning/ideation/access-needed-to-use-ideation-space.md)를 참조하십시오.

위의 요구 사항 외에, 다음 기준도 충족해야 Closed Beta 프로그램에 참여할 수 있습니다.

* 캠페인 추적 기능이 있는 활성 Adobe Customer Journey Analytics(CJA) 계정이 있음
* 반복 가능한 계획 프로세스를 통해 멀티채널 캠페인 만들기
* 마케팅 작업에 Workfront Planning을 적극적으로 사용
* 기본 관념화 공간 사용자가 될 최소 한 명 이상의 식별된 전략가 또는 관념화 사용자가 있어야 합니다.

## 대상자 및 사용 사례

Ideation 공간은 캠페인 전략을 수립하고 캠페인 브리핑을 제작하는 책임을 지는 제품 및 브랜드 마케터를 위해 설계되었습니다.

<!--
Too much: 

| Role | Primary job to be done |
|---|---|
| Brand Marketer | Identify messaging, trends, and cultural shifts that resonate with target audiences |
| Product Marketer | Launch insight-driven, culturally relevant campaigns that deliver business impact |
| Collaborators | Internal creative studios, external agencies, media planners/managers, and executives who need visibility into strategic direction |
-->

작업 영역 관리자는 다음 단계에 따라 관념화 공간을 사용하여 Workfront Planning에서 레코드를 만들 수 있습니다.

* Planning에서 시작한 후 레코드 생성 또는 편집을 시작할 때 Ideation 공간에 대한 간단한 설명을 만듭니다.
* AI 프롬프트를 사용하여 시스템의 다른 레코드나 웹에서 세부 정보를 수집하고 관념설명 만들기를 완료합니다.
* Brief에서 Planning 레코드 유형을 생성합니다.
* Planning에서 Ideation Brief를 구체화하고 기존 레코드 유형을 업데이트합니다.

다음은 관념화 공간을 사용하는 방법에 대한 사용 사례입니다.

* **이전 성능을 사용하여 이전 캠페인을 새로 고치십시오**

  * 예를 들어 새 분기, 시즌 또는 제품 모멘트에 대한 기존 캠페인을 업데이트할 수 있습니다.
  * 이렇게 하면 어떤 것이 유지되고, 어떤 변화가 일어나고, 어떤 이유가 있는지를 대략적으로 설명하는 이전 성능에 기반을 둔 &quot;델타 브리프&quot;가 생성됩니다.

* **과거 성과를 사용하여 순-신규 캠페인 만들기**

  * 예를 들어 직접 캠페인 내역 없이 새 제품, 세그먼트 또는 이니셔티브를 시작할 때 캠페인을 만들 수 있습니다.
  * 이렇게 하면 안내가 있는 관념화, 권장 채널 믹스 및 초기 개념이나 메시지 지침을 통해 완전히 새로운 브리핑이 생성됩니다.

## 관념화 공간에 대한 액세스 권한 얻기

관념화 공간에 액세스하려면 다음 작업을 수행할 수 있습니다.

1. 이 문서의 [제품 요구 사항](#product-requirements) 섹션에 설명된 대로 제품 요구 사항을 충족하는지 확인하십시오.
1. Adobe 계정 담당자에게 문의하여 폐쇄된 Beta에 참여하거나 Beta 열기 대기 목록에 참여하십시오.
1. 새로 고침할 최근 캠페인 또는 처음부터 새로 만들 새 이니셔티브와 같은 첫 번째 캠페인을 식별합니다.

관념화 공간 사용에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [관념화 공간을 사용하는 데 필요한 액세스 권한](/help/quicksilver/planning/ideation/access-needed-to-use-ideation-space.md)
* [Ideation Space Brief에서 계획 레코드 생성](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md)
* [Ideation Space에서 개요 만들기](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md)

## 관념화 공간 개요

관념화 공간은 브랜드 및 제품 마케터가 더 강력한 캠페인을 더 빠르고 더 나은 팀 정렬로 구축할 수 있는 전략적 마케팅 관념화 도구입니다. 과거 브리프, 성과 데이터, 대상 통찰력, 브랜드 지침 및 기존 캠페인 자산과 같은 실제 마케팅 컨텍스트에서 AI 제안을 기반으로 하므로 결과는 일반적이지 않고 관련성이 있습니다.

다음은 브리프를 만들 때 아이디어를 최대한 활용하는 방법에 대한 몇 가지 예입니다.

* 문서 또는 소셜 의견 수렴 인사이트 업로드
* 작성 중인 개요와 관련된 웹 콘텐츠에 액세스
* 캠페인 목표 정의
* 대상자 인사이트 요약 가져오기
* 대상자 가상 사용자 생성
* 캠페인 메시지 아이디어
* AI 프롬프트를 사용하여 텍스트, 이미지, 파일, 차트 및 insight 카드를 생성하여 큰 시각적 캔버스에서 작업
* 카드를 구성, 수정 및 확장하여 최종적으로 캠페인 브리핑으로 번역할 수 있습니다
* 간단한 작업을 완료하기 전에 아이디어를 추가하거나 특정 캔버스 항목에 주석을 달거나 자유 형식 아이디어에 스티커 메모를 사용할 수 있는 여러 사용자와 공동 작업하십시오
* 관념화 공간을 사용할 때는 다음 모범 사례를 권장합니다.

  * **고유해야**. 캠페인 설명이 풍부하면 보다 관련성이 높고 근거가 좋은 카드가 생성됩니다.
  * **완료하기 전에 확인**. AI에서 생성한 응답이 정확하지 않을 수 있으므로 레코드를 완료하기 전에 항상 카드에서 **소스**&#x200B;를 확인하고 연결된 소스를 확인하십시오.
  * **AI 카드와 실제 레코드를 혼합**&#x200B;합니다. 관념화 공간에 실제 레코드를 끌어서 놓습니다.

## Adobe CX Coworker에서 사용할 수 있는 관념화 공간

관념화 공간은 Adobe의 CX Coworker을 통해 대화형, 전후 모드도 지원합니다.

사용자는 후속 질문을 하고 일회성 결과를 얻기보다는 짧은 대화를 개선할 수 있습니다.

개요 가 라이브 Workfront Planning 연결에 연결되면 Coworker는 기본 계획이 그대로 유지되도록 덮어쓰기를 보류합니다.

<!--
**************** CONSIDER INCLUDING THIS INFORMATION FROM JESH BARLOW ABOUT COWORKER IN CATALYZE?? - https://adobecorpdev.slack.com/archives/C091C0Y735W/p1788917610365089?thread_ts=1788917251.550099&cid=C091C0Y735W

Catalyze Coworker needs — panel inside Catalyze, not a rail from Unified ShellWhy this matters. Catalyze is AI-first. You can't use it without a prompt, so the prompting surface can't be something you open and close from Unified Shell. Coworker's rail was built to bolt onto apps that already work fine without AI. We need the opposite.

What we need

* Coworker embedded as a panel inside Catalyze (the Photoshop/Illustrator model), always present, minimized or expanded, never fully closeable.
* Not the Unified Shell rail that slides in, pushes the app, and only opens and closes from the shell.
* Quick terminology flag, since Coworker inverts it. By "panel" we mean embedded in the app. Their team uses "panel" for the shell version, so we have to be explicit every time.


Must-haves

* Minimized and expanded prompt bar states that live inside Catalyze, not tied to the shell.
* Minimize, never close. There's no state where the prompt disappears.
* Full UI control over how the prompt behaves.
* Headless Coworker so the panel can always sit on the canvas.


Where it stands (Aug 20 Shell/Catalyze sync with Stephen Gould)

* Headless is technically possible. Coworker can be hosted in Catalyze's own front-end.
* But Horia's team has no capacity to build or own an in-app rail. Deeper embedding means Catalyze eng builds the panel and owns it going forward.
* The open question is ownership, one-time integration vs owning the panel long-term. Still unresolved, and it's the thing that decides this.


Worth noting

* Experience Workspace and Brand Visibility (AM) already run Coworker without the shell, so headless isn't net-new. Let's learn how they did it before anyone calls it infeasible.
* Next step everyone agreed on is getting clarity from Horia's team and Joshua on rail ownership.

*************************************
-->

## 추가 리소스

* [Adobe Workfront 캠페인 계획](https://business.adobe.com/kr/products/workfront/campaign-planning.html)
* [Adobe Workfront Planning 설명서](/help/quicksilver/planning/planning-information.md)
* [Adobe GenStudio 개요](https://business.adobe.com/kr/products/genstudio.html)
* [Adobe Customer Journey Analytics](https://business.adobe.com/kr/products/adobe-analytics/customer-journey-analytics.html)


<!--

Not sure if we should disclose this: 

## The problem the Ideation space solves

Before the Ideation space, campaign strategy relied on two slow, manual processes:

- **Gathering insights** — fragmented, time-consuming, and difficult when no prior audience data exists
- **Aligning stakeholders** — without a shared, data-backed "hook," executives, creatives, and channel partners often work from different assumptions, causing rework and delays

The Ideation space automates insight synthesis and generates a structured brief that gives everyone a shared starting point.
-->

<!--
## What's included, phase by phase

| Phase | Timeline | What's included |
|---|---|---|
| Closed Beta | July 2026 | Limited customers/users/campaigns; core agent skills (strategy framing, messaging ideation, audience definition, data ingestion, brief generation); CJA data integration |
| Open Beta | ~Sept 2026 (planned) | Quality/performance improvements; CJA integration refinements; Workfront Planning handoff; data visualization; Planning workspace structure ingestion; Unity/Conversational UI integration |
| General Availability | H2 2026 (planned) | Bring Your Own Data Source (BYODS); Workfront/Workfront Planning data integration; audience data integration; social data integration; workflow ingestion; strategy testing capabilities |

At GA, the Ideation space is also expected to be accessible through the GenStudio Home conversational UI, running as part of Adobe's Agent Orchestrator suite of agents.
-->