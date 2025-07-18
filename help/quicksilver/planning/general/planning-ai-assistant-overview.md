---
title: Adobe Systems Workfront Planning AI Assistant 개요
description: AI 도우미를 사용하여 현재 페이지 컨텍스트 및 레코드 구조에 따라 레코드를 생성, 업데이트 또는 제거할 수 있습니다. 사용자 명령과 AI의 명령 실행이 함께 작동하여 AI의 변경 사항이 환경에 정확하게 반영되도록 합니다.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: a36968bdae5756f0f8283da04a2afca83b4dd94a
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 0%

---


# Adobe Systems Workfront Planning AI Assistant 개요

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> -->


{{planning-important-intro}}

AI Assistant를 사용하여 현재 페이지 컨텍스트 및 레코드 구조에 따라 레코드를 생성, 업데이트 또는 제거할 수 있습니다.

사용자 명령과 AI의 명령 실행이 함께 작동하여 AI의 변경 사항이 환경에 정확하게 반영되도록 합니다.

## AI Assistant에 대한 고려 사항

* AI Assistant를 조직에서 사용하도록 설정해야 회사의 사용자가 AI Assistant를 사용할 수 있습니다. 자세한 내용은 AI Assistant 개요를[ 참조하세요](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).
* Workfront에서 조직에 대해 AI Assistant를 활성화하면 기본 Workfront 관리자가 AI Assistant를 사용할 수 있습니다. 자세한 내용은 시스템에[ 대한 기본 정보 구성을 참조하십시오](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Workfront 관리자는 다른 모든 사용자에 대해 AI Assistant를 활성화해야 합니다. 자세한 내용은 AI Assistant 활성화 또는 비활성화를[ 참조하세요](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* AI 어시스턴트는 각 페이지 컨텍스트에서 작동합니다. AI Assistant에 대해 제출하는 요청은 열려 있는 페이지 내에서 사용할 수 있는 기능을 참조해야 합니다.

* Planning 영역에서 AI Assistant가 수행하는 작업은 Workfront Planning 권한 및 Workfront 액세스 수준의 컨텍스트에 있습니다. 자세한 내용은 다음 문서를 참조하세요.

   * [Adobe Systems Workfront Planning의 공유 권한 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Adobe Systems Workfront Planning을 사용하는 경우의 라이센스 유형 개요](/help/quicksilver/planning/access/license-type-overview.md)

* 사용자 대신 AI Assistant가 변경한 내용은 레코드의 기록 패널에서 추적됩니다.

* 명령을 사용하여 작업을 실행 취소할 수 있습니다. 예를 들어 &quot;실행 취소 last change&quot;를 입력하여 변경 사항을 되돌릴 수 있습니다.

* AI Assistant를 통해 개체를 생성, 업데이트 또는 삭제할 때 AI Assistant는 의도한 작업을 표시하고 확인을 요청합니다. 그런 다음 작업을 확인하거나 취소할 수 있습니다.

## 현재 AI Assistant에서 사용할 수 있는 기능

현재 AI Assistant는 Workfront의 계획 영역에서 다음 페이지에 사용할 수 있습니다.

* 작업 영역 페이지
* 레코드 유형 페이지
* 레코드 페이지

이때 AI Assistant를 사용하여 다음 작업을 수행할 수 있습니다.

* 레코드에 대한 Search. 레코드 필드에 포함된 정보로 검색 할 수 있습니다.
* 레코드를 만들기. 레코드가 만들어진 후 새 레코드에 대한 링크 파일이 있는 ID가 표시됩니다. 생성 프로세스 중에 업데이트할 필드, 좋아요 날짜 또는 설명을 지정할 수 있습니다.
* 업로드한 문서를 기준으로 레코드를 만들기. Workfront는 AI Assistant에 대해 다음과 같은 문서 형식을 지원합니다.

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT 및 대부분의 이미지 형식
* 화면에 표시되는 레코드에 대한 필드 업데이트
* 레코드 삭제
* 방금 삭제한 레코드 복원


## Workfront Planning에서 AI Assistant 찾기

AI Assistant는 Workfront Planning의 다음 영역에서 찾을 수 있습니다.

* 화면의 오른쪽 상단 모서리에 있는 기본 탐색 막대입니다.
* 레코드의 세부 정보 영역 내에서, 미리 보기에서 레코드를 연 후 또는 레코드의 페이지.

## 계획 영역에서 AI Assistant에 액세스합니다.

1. Workfront에 로그인한 다음 화면 오른쪽 상단 모서리에 있는 메인 메뉴&#x200B;**아이콘 Dots 메인 메뉴** 또는 ![왼쪽 상단 모서리에 있는 메인 메뉴](assets/dots-main-menu.png) 아이콘 **Lines 메인 메뉴**(사용 가능한 경우)를 클릭합니다![](assets/lines-main-menu.png).

. 계획을&#x200B;**클릭합니다**. 계획 영역이 열립니다.

1. **작업 영역 카드**&#x200B;를 클릭합니다.

1. (선택 사항) **레코드 종류 카드** 클릭

1. (선택 사항) **레코드를** 클릭하여 레코드의 **세부 정보** 페이지 열기

1. **글로벌 탐색 막대의 화면 오른쪽 상단 모서리 또는 레코드 미리 보기 또는 페이지 오른쪽 상단 모서리에 있는 AI Assistant 아이콘을** 클릭합니다.

   ![AI Assistant 아이콘](assets/ai-assistant-icon-highlighted.png)

1. 제공된 공간에서 AI Assistant에 대한 명령을 입력하기 시작한 다음, 완료되면 Enter 키를 클릭합니다.

   ![빈 명령 상자가 있는 AI Assistant 패널](assets/ai-assistant-panel-with-empty-command-box.png)

   예를 들어 다음 중 하나를 입력할 수 있습니다.

   * 시작 날짜가 7월 4일이고 종료 날짜가 7월 30일인 캠페인 만들기
   * Summer Campaign 레코드의 설명 필드를 결정할 날짜로 업데이트합니다
   * 마지막 레코드 삭제
   * 레코드 복원

   AI Assistant가 명령을 처리하는 동안 시각적 표시기가 표시되어 응답 시간에 대한 기대치를 설정합니다.

   성공적인 응답을 받은 후 제공된 링크를 팔로우 하거나 왼쪽의 변경 사항을 확인합니다.



