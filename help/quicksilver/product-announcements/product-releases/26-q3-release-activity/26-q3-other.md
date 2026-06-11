---
title: 2026년 3분기 릴리스 일정 동안의 기타 개선 사항
description: 2026년 3분기 릴리스 기간 동안의 기타 개선 사항
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 937b49b44f102fee6c9847ab950eb2b274aee89b
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# 2026년 3분기 릴리스 일정 동안의 기타 개선 사항

이 페이지에서는 미리보기 환경에 대한 2026년 3분기 릴리스의 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2026년 3분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2026년 3분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)를 참조하십시오.

## Workfront MCP 커넥터 업데이트

Workfront MCP 커넥터에 대해 다음과 같이 업데이트되었습니다.

* EU<!-- and US instances that are not on AWS. Each MCP server can only connect to one instance, but are no longer limited to US instances on AWS-->의 인스턴스와 작동하도록 MCP 서버를 확장했습니다.
* Workfront MCP 커넥터의 유연성을 확장하기 위해 Claude를 연결하는 기능을 추가했습니다. 이제 Claude의 커넥터 목록에서 Workfront을 찾거나 URL을 사용하여 직접 연결할 수 있습니다.

자세한 내용 및 지침은 [Adobe Workfront MCP 서버 구성](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)을 참조하세요.


## 댓글 알림 이메일에 대한 모양과 느낌을 업데이트했습니다.

>[!NOTE]
>
>고객을 위한 프로덕션 릴리스: 2026년 7월 16일부터 단계적으로 롤아웃

업데이트 영역의 댓글에 대한 이메일 알림은 광범위한 Adobe 이메일 디자인에 맞는 새로운 모양과 느낌을 제공합니다.

업데이트된 이메일 형식에는 다음이 포함됩니다.

* 이전 Workfront 브랜딩을 대체하는 새 Adobe Workfront 헤더입니다.
* 가장 최근 댓글에 중점을 둔 간소화된 레이아웃입니다.
* 항목을 직접 열려면 기본 **Workfront에서 보기** 단추입니다.

이전 주석의 스레드는 더 이상 이메일 본문에 포함되지 않습니다. 항목에 대한 이전 설명을 보려면 **Workfront에서 보기**&#x200B;를 사용하여 Workfront에서 대화를 엽니다.

이러한 변경 사항은 단계적으로 고객에게 전달됩니다. 롤아웃 일정이 확정되면 이 페이지가 업데이트됩니다.

![댓글 알림 email.png](assets/email-look-and-feel-update.png) 업데이트됨

## Workfront MCP 서버를 사용하여 Workfront을 AI 도구에 연결

>[!NOTE]
>
>미리 보기: 2026년 5월 28일>프로덕션 빠른 릴리스: 2026년 6월 11일>모두를 위한 프로덕션: 2026년 7월 16일

팀의 운영 컨텍스트는 Workfront에 있습니다. 이제 Workfront MCP 서버를 사용하면 팀이 이미 사용하고 있는 AI 도구 내에서 해당 컨텍스트를 실행할 수 있습니다.

Workfront을 Claude, ChatGPT, Copilot, Gemini 등의 MCP 호환 AI 플랫폼에 연결하고 자연어를 사용하여 선택한 AI 도구를 종료하지 않고도 Workfront 항목을 찾고, 만들고, 업데이트하고, 관리합니다. 지연된 작업을 요청하고, 프로젝트 완료 날짜를 푸시하고, 승인자에게 알림 메시지를 보내고, 캠페인 예산을 업데이트합니다. 그러면 AI 플랫폼이 Workfront에서 작업을 수행합니다.

또한 Claude의 AI 기술과 예정된 작업을 통해 라이브 Workfront 데이터에 대해 사전 예방적으로 실행되는 반복 워크플로우를 자동화하여 더욱 발전할 수 있습니다. 예를 들어, 월요일 아침 프로젝트 브리핑, 주간 용량 보고서, 월간 캠페인 상태 점검 — 한 번 설정하면 AI가 이를 자동으로 처리하며 작업의 전체 컨텍스트에 기반합니다.

이는 AI가 풍부한 운영 데이터를 기반으로 하며 인간과 AI가 협력하여 작업을 전속력으로 진행할 수 있는 아젠틱 작업 관리 시스템의 기반입니다.

>[!IMPORTANT]
>
>현재 Workfront MCP 서버는 AWS 사용 고객이 미국 지역 고객만 사용할 수 있습니다.

자세한 내용은 [Adobe Workfront MCP 서버 개요](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md)를 참조하십시오.

## 향상된 목록 업데이트

>[!NOTE]
>
>미리 보기: 2026년 5월 28일>프로덕션 빠른 릴리스: 2026년 6월 11일>모두를 위한 프로덕션: 2026년 7월 16일

향상된 목록의 여러 필드 유형이 키보드 탐색 및 기타 향상된 기능을 포함하도록 업데이트되었습니다.

향상된 목록의 할당자 필드에서 이제 키보드 탐색이 제공됩니다.

* 키보드의 위쪽 및 아래쪽 화살표를 사용하여 사람 목록을 이동합니다.
* 스페이스바를 눌러 사용자를 선택하거나 \&lt;Delete\>를 눌러 선택한 사용자를 제거합니다.

고급 목록의 단일 및 다중 선택 필드:

* 이제 키보드에서 필드 상호 작용에 액세스할 수 있습니다. 여기에는 위쪽 및 아래쪽 화살표를 사용한 태그, 검색 옵션, 목록 간의 탐색이 포함됩니다. 항목을 선택하려면 스페이스바를 누르고, 선택한 항목을 제거하려면 \&lt;Delete\>를 누르십시오.
* 결과를 찾을 수 없을 때 편집기에서 직접 새 옵션을 만들 수 있습니다. 일부 목록에서는 이 기능을 사용할 수 없습니다.

자동 완성 및 외부 조회 필드와 같은 참조 필드에 몇 가지 인터페이스 개선 사항이 수신되었습니다.

또한 끌어서 놓기를 사용할 수 있는 목록에서 열을 끌어서 놓는 경험이 시각적으로 개선되었습니다.

자세한 내용은 [향상된 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)을 참조하세요.
