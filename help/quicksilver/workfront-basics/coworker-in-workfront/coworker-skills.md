---
title: CX Enterprise Coworker의 Workfront 기술
content-type: reference
description: Adobe Workfront에서 Coworker가 사용할 수 있는 기술에 대해 알아봅니다.
author: Becky
feature: Get Started with Workfront
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: c042179c-157b-516d-b27c-e3bf303e8567
    internal-label: Get Started with Workfront
source-git-commit: 58aec1c9c7dc45c5ecb6ad5d070a4e34b29c458c
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 3%
---
# CX Enterprise Coworker의 Workfront 기술

>[!IMPORTANT]
>
>현재 의료 서비스, 금융 또는 민감한 데이터가 있는 기타 산업의 조직에서는 CX Enterprise Coworker을 사용할 수 없습니다. 이러한 조직에서는 AI Assistant를 사용할 수 있습니다. 자세한 내용은 [AI Assistant 개요](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)를 참조하십시오.

이 문서에는 현재 Workfront의 CX Enterprise Coworker에서 사용할 수 있는 스킬이 나열되어 있습니다.

이러한 스킬이 다루는 능력은 대화 인터페이스를 통해 동료에서 사용할 수 있으며, 이러한 스킬을 직접 호출할 필요는 없습니다. 그러나 스킬을 직접 호출하려면 슬래시 `/`을(를) 입력하고 스킬의 이름을 입력하여 [동료] 패널에서 호출할 수 있습니다.

예를 들어 프롬프트는 문서 [Adobe Workfront MCP 서버 사용](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)에서 프롬프트를 참조하십시오.

## Workfront 계획 기술

### Workfront Planning 솔루션 설계자

이름: `wf-planning-solution-architect`

이 스킬은 다음을 포함하되 이에 제한되지 않는 Workfront Planning과 관련된 질문에 답변할 수 있습니다.

* Workspace 디자인
* 공식 필드 구문
* API 필터링
* 레코드 연결
* 자동화 옵션
* 보고
* 액세스 및 권한
* 통합
* 가격 책정 계층별 제품 제한

### Workfront 계획 관리

이름: `manage-workfront-planning`

이 스킬은 다음과 같은 Workfront Planning 객체를 쿼리하고 관리합니다.

* 작업 영역
* 섹션
* 레코드 유형
* 필드
* 보기 횟수
* 레코드
* 비즈니스 규칙

### 관념화 공간(베타) 기술

>[!NOTE]
>
>관념화 공간은 현재 Workfront Planning의 추가 기능으로 Beta에서 사용할 수 있습니다.
>
>Ideation Space에 대한 자세한 내용은 [Adobe Workfront Planning의 Ideation Space 시작](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)을 참조하십시오.

관념화 공간은 Adobe Planning에 직접 내장된 Workfront의 AI 기반 전략 관념화 기능입니다. 이는 마케팅 팀에게 캠페인 전략을 위한 구조화된 데이터 기반의 시작 지점을 제공하며, 수동 연구 및 추측 작업을 조직의 실제 성과 기록에서 기반으로 하는 AI 생성 브리핑으로 대체합니다.

동료는 Workfront Planning Idea 공간으로 작업할 수 있는 다양한 기술을 보유하고 있습니다. 이러한 커버 작업은 다음과 같습니다.

<!--list duplicated in: help/quicksilver/workfront-basics/coworker-in-workfront/coworker-prompts-and-best-practices.md-->

* 캠페인 아이디어 — 첨부된 소스 문서 및 기타 소스를 사용하여 캠페인 및 기타 주제에 대한 캔버스에 아이디어 카드를 브레인스토밍하고 생성합니다. 이것은 관념화의 주요 출발점이다.
* 캠페인 대화 - Ideation Space 앱 내에서 대화형으로 캠페인 아이디어를 진행합니다.
* 캠페인 개요 — 체계적인 캠페인 개요를 작성하고 구체화합니다. 이때 가드레일을 사용하여 완성도를 높이고 진행 중에 확인할 수 있습니다.
* 문서 Q&amp;A — 아이디어 세션에 첨부한 문서에 대해 질문합니다.
* 연구 — 캔버스에 여러분의 생각을 알리기 위해 연구를 끌어옵니다.
* 시작 프롬프트 — 아이디어를 시작하거나 확장하는 제안 프롬프트를 가져옵니다.
* 캔버스 열기 — Ideation Space 캔버스를 시작하거나 이동합니다(앱 외부의 일반 채팅에서 시작할 때 사용).

## Workfront 스킬

### Workfront 개체 관리

이름: `manage-workfront-objects`

이 스킬은 Workfront 프로젝트, 작업, 문제, 포트폴리오 및 프로그램을 만들고 업데이트합니다. 예로는 다음이 있습니다.

* 프로젝트 만들기
* 작업 추가
* 계획된 일자 설정
* 작업 할당

### Workfront 데이터 쿼리

이름: `query-workfront-data`

이 스킬은 Workfront 오브젝트를 찾고, 나열하고, 보고합니다. 다음은 이러한 Workfront 개체의 몇 가지 예이지만 목록이 완전하지 않습니다.

* 프로젝트
* 작업
* 문제
* 사용자
* 포트폴리오


