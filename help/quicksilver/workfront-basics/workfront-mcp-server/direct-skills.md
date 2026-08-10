---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: 직접 설치에 사용할 수 있는 기술
description: Workfront에서는 LLM에 직접 설치할 수 있는 몇 가지 기술을 제공합니다.
author: Becky
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
source-git-commit: 7fd4c07f2ea1e47e7abb7d3dd78638a6a01d0f47
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# 직접 설치에 사용할 수 있는 기술

Adobe Workfront에서는 LLM에 직접 설치할 수 있는 몇 가지 기술을 제공합니다. 스킬은 해당 도구를 특정 작업에 사용하는 방법에 대해 안내하며, 올바른 단계는 이미 내장되어 있습니다.

이러한 기술은 Adobe 기술 GitHub 리포지토리에서 파일로 찾을 수 있습니다. 이 저장소에는 다양한 Adobe 제품에 대한 파일이 있습니다. 이러한 파일을 다운로드하여 Claude에 복사하면 Claude는 파일에 설명된 기술을 사용할 수 있습니다.

예를 들어 Cloud는 계획 솔루션 설계자 기술을 통해 Workfront Planning에 대한 질문에 답변하고 일부 작업을 수행할 수 있습니다.

이러한 스킬이 LLM에 복사된 후에는 호출하거나 트리거할 필요가 없습니다. 대신 LLM과 평소와 같이 자연어로 질문하고 상호 작용할 수 있으며, LLM은 대화에 적합한 스킬에 설명된 정보와 작업을 사용합니다.

>[!NOTE]
>
>현재 이러한 스킬은 클로드만 사용할 수 있습니다.
>Adobe으로 Cloud를 설정하는 방법에 대한 지침은 Adobe Developer 설명서에서 [시작하기](https://developer.adobe.com/adobe-for-creativity/getting-started/)를 참조하십시오.

## Workfront GitHub 리포지토리에서 Claude에 스킬 설치

1. GitHub의 [Adobe Workfront 기술 저장소](https://github.com/adobe/skills/tree/main/plugins/workfront)&#x200B;(으)로 이동합니다.
1. 사용할 스킬 폴더를 다운로드합니다.
1. 폴더를 클라우드 스킬 라이브러리로 복사합니다.

   * 클라우드 데스크톱: `~/Library/Application Support/Claude/skills/`(macOS) 또는 동급 버전.
   * 클라우드 코드: `~/.claude/skills/`.

<!--

1. Go to the [Adobe Workfront skills repository](https://github.com/adobe/skills/tree/main/plugins/workfront) on GitHub.
1. Download the skill file you want to use.
1. In Claude, click **Customize**.
1. Select **Skills**.
1. Click **Create skill** -> **Upload a skill**.
1. Upload the zipped skill file to Claude, then click **Confirm** to install.

-->

## 현재 사용 가능한 스킬

| 스킬/폴더에 링크 | 스킬 설명 | 다음에 사용 가능: |
|---|---|---|
| [계획 솔루션 설계자](https://github.com/adobe/skills/tree/main/plugins/workfront/skills/wf-planning-solution-architect) | 요구 사항에 맞게 Workfront Planning 작업 영역을 구성하고 Workfront Planning에 대한 질문에 답변합니다. | 클로드 |
