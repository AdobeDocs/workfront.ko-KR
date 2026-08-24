---
content-type: release-notes
title: Adobe Workfront Planning의 2026년 4분기 릴리스 활동
description: 2026년 4분기 Adobe Workfront Planning 제품 릴리스 활동입니다.
author: Becky
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 9b6b1157cf93418e8863f2e99ebe87414a23378d
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 0%

---

# Adobe Workfront Planning의 2026년 4분기 릴리스 활동

이 문서에서는 2026년 4분기 릴리스 동안 Workfront Planning에 대해 릴리스되는 기능에 대해 설명합니다.

Adobe Workfront Planning에 대해 릴리스된 모든 기능 목록을 보려면 [Adobe Workfront Planning 릴리스 활동: 문서 색인](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)을 참조하십시오.

## 종속적으로 연결된 레코드 필드에 대한 열 헤더가 업데이트되었습니다.

>[!NOTE]
>
>미리 보기: 2026년 8월 20일
>프로덕션 빠른 릴리스: 2026년 9월 17일
>모두를 위한 프로덕션: 2026년 10월 15일

테이블 보기에서 종속적으로 연결된 레코드 필드의 열 머리글을 시각적으로 개선했습니다.

자세한 내용은 [종속 연결 관리](/help/quicksilver/planning/architecture/manage-dependent-connections.md)를 참조하십시오.

## 여러 행을 끌어다 놓을 때 표 보기 개선 사항

>[!NOTE]
>
>미리 보기: 2026년 8월 13일
>프로덕션 빠른 릴리스: 2026년 8월 13일
>모두를 위한 프로덕션: 2026년 10월 15일
>[!BADGE 일정 해제]{type=Neutral}

테이블 보기에서 여러 행을 끌어다 놓을 때 새로운 시각적 표시기가 있습니다. 이제 더 눈에 띄는 더하기 기호와 숫자 표시기에 끌어서 놓기 작업에 대해 선택한 행 수가 표시됩니다.

자세한 내용은 [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)를 참조하십시오.

<!--

## Collapse and expand all groupings in the timeline view

>[!NOTE]
>
>Preview: August 13, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

Timeline views now include Collapse all and Expand all options for grouped timelines. This makes it easier to navigate large roadmap views: you can quickly reduce the view to grouping headings, then expand only the sections you want to review.

For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).

-->

## 글로벌 레코드 유형을 사용할 때 제출된 요청 개체를 올바른 작업 영역으로 라우팅합니다.

>[!NOTE]
>
>미리 보기: 2026년 8월 13일
>프로덕션 빠른 릴리스: 2026년 9월 17일
>모두를 위한 프로덕션: 2026년 10월 15일

요청 양식을 제출하여 글로벌 레코드 유형에 대해 생성된 레코드는 이제 제출된 작업공간으로 자동으로 라우팅됩니다.

글로벌 레코드 유형의 보조 작업 공간에서 요청을 제출하여 생성된 레코드는 해당 보조 작업 공간에 추가됩니다. 원래 작업 영역 또는 기본 요청 영역에서 요청을 제출하여 생성된 레코드는 원래 작업 영역에 추가됩니다.

접수 양식에 Workspace 필드가 포함되어 있고 사용자가 제출하기 전에 작업 영역을 선택하면 양식 시작 위치에 관계없이 요청이 선택한 작업 영역으로 라우팅됩니다. 이렇게 하면 레코드가 만들어지는 순간부터 의도한 작업 영역에 정리됩니다.

자세한 내용은 [레코드를 만들도록 Adobe Workfront Planning 요청 제출](/help/quicksilver/planning/requests/submit-requests.md)을 참조하십시오.

## Workfront Planning 솔루션 설계자 스킬 소개

>[!NOTE]
>
>미리 보기: 2026년 8월 10일
>프로덕션: 2026년 8월 10일

Workfront Planning에 대한 간결한 모범 사례 지침을 Claude에 직접 제공하는 새로운 기술인 Workfront Planning 솔루션 설계자를 출시합니다.

* Workfront MCP 서버가 사용자 환경에서 설정을 실행하여 지정할 새 계획 작업 영역을 **구성**&#x200B;합니다.
* 규모에 맞게 반대 패턴에 대한 기존 구성을 **감사**&#x200B;합니다.
* 권장 제한(레코드, 연결, 계층 구조 깊이)에 대해 **사용량을 확인**&#x200B;합니다.
* 언제든지 Planning에 대해 **질문하기**.

초기 설정 외에도 이 기술은 마찰을 일으키기 전에 구성 변화를 포착하고, 차단기가 되기 전에 접근 제한에 도달하며, 구성 주체에 관계없이 모든 작업 영역에서 일관된 표준을 적용하고, 전문가를 기다리지 않고 팀원의 누구에게나 정확한 답변을 제공함으로써 지속적인 거버넌스를 지원합니다. 이를 통해 작업 영역을 올바로 설정하고 사용량이 증가할 때 그러한 방식으로 유지하는 전체 라이프사이클을 다룹니다.

자세한 내용은 직접 설치에 사용할 수 있는 [기술](/help/quicksilver/workfront-basics/workfront-mcp-server/direct-skills.md)을 참조하세요.

## 테이블 보기에서 행 끌어서 놓기

>[!NOTE]
>
>미리 보기: 2026년 7월 30일
>프로덕션 빠른 릴리스: 2026년 8월 13일
>전체 프로덕션: 2026년 10월 15일

테이블 보기에서 행을 끌어서 놓는 경험이 시각적으로 개선되었습니다.

자세한 내용은 [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)를 참조하십시오.


## 종속 연결된 레코드 필드

>[!NOTE]
>
>미리 보기: 2026년 7월 30일
>프로덕션 빠른 릴리스: 2026년 8월 13일
>모두를 위한 프로덕션: 2026년 10월 15일

이제 Workspace 관리자는 연결된 레코드 유형 간의 종속성을 정의할 수 있습니다. 예를 들어 지역 필드에 선택한 지역에 연결된 값만 표시됩니다. 이는 연결 필드 설정에서 직접 구성됩니다. 지역 레코드 유형에서 종속 레코드 유형(예: 지역)으로 연결을 추가할 때 작업 영역 관리자가 새 설정을 통해 해당 레코드 유형 간에 이미 설정된 관계를 사용하여 지역 레코드 유형에 종속된 것으로 표시할 수 있습니다.

구성하고 나면 두 필드를 참조하는 모든 레코드 유형(예: 캠페인)에 효과가 즉시 표시됩니다. 지역 값을 선택하면 지역 선택기의 범위가 해당 지역에 실제로 연결된 지역으로만 좁혀집니다. 이렇게 하면 레코드 구조가 자동으로 적용되므로 일치하지 않는 조합이 제거되고 수동 정리가 줄어듭니다.

이 업데이트에는 다음 기능이 포함되어 있습니다.

* 레코드 유형을 연결할 때 새 연결 탭에 새 연결 설정 섹션을 추가했습니다
* 이 연결에 종속되도록 하기 설정을 새 섹션에 추가했습니다


자세한 내용은 [종속 연결 관리](/help/quicksilver/planning/architecture/manage-dependent-connections.md)를 참조하십시오.




## 표 보기에서 레코드에 대한 새 주석 표시기 표시

>[!NOTE]
>
>미리 보기: 2026년 7월 30일
>프로덕션 빠른 릴리스: 2026년 8월 13일
>모두를 위한 프로덕션: 2026년 10월 15일

레코드에 읽지 않은 댓글이 있는 경우 표시하는 새 지표를 추가했습니다. 표시기는 표 보기에서 레코드의 기본 필드의 오른쪽 상단 모서리에 표시됩니다.

자세한 내용은 [레코드 주석 관리](/help/quicksilver/planning/records/manage-record-comments.md)를 참조하십시오.

## 사용자 정의 가능한 레코드 색상 및 연결 기반 색상 코딩

>[!NOTE]
> 
>미리 보기: 2026년 7월 23일
>프로덕션 빠른 릴리스: 2026년 8월 13일
>전체 프로덕션: 2026년 10월 15일

이제 레코드는 새 레코드에 자동으로 할당된 색상을 표준 또는 사용자 정의 색상으로 업데이트할 수 있는 사용자 정의 색상 팔레트를 지원합니다.

이 개선 사항에는 다음 변경 사항이 포함되어 있습니다. 

* 다음 영역에 색상 옵션을 추가했습니다.
  * 테이블 보기의 필드 아이콘 
  * 타임라인 및 달력 보기의 설정 영역에 있는 막대 스타일 섹션

    색상 설정을 켜면 새 레코드에 지정된 색상이 레코드가 이러한 보기에서 표시되는 모든 위치에 표시됩니다. 

* 색상 원이 레코드의 세부 사항 페이지에 추가됩니다. 
* 이제 필드 값으로 색상을 지정할 때 타임라인 및 달력 보기에서 막대의 색상 코딩에 단일, 다중 선택 및 연결된 레코드 필드를 추가할 수 있습니다. 
* 연결된 레코드 필드를 만들 때 레코드의 이름 및 이미지 외에 색상을 표시하도록 설정할 수 있습니다. 
* 설정 영역의 색상 섹션도 &quot;없음&quot; 옵션을 제거하여 간소화되었습니다.  

자세한 내용은 [레코드 만들기](/help/quicksilver/planning/records/create-records.md)를 참조하세요. 

## 이제 Designer을 계획하려면 Beta 계약 동의가 필요합니다.

>[!NOTE]
>모든 고객에게 미리보기 및 프로덕션: 2026년 7월 20일
>[!BADGE 일정 해제]{type=Neutral}

이제 Planning Designer에서 사용하려면 승인된 Beta 계약이 필요합니다. 귀사는 AI 계약에 서명할 필요가 없습니다. 모든 고객이 이용할 수 있습니다.

이를 위해 AI 베타에 옵트인 섹션 아래의 설정 섹션에서 계획 Designer 옵션을 이동했습니다.

수락된 Beta 계약 없이 Planning Designer을 실행하면 Workspace 빌더가 열리기 전에 수락 여부를 묻는 메시지가 표시됩니다.

자세한 내용은 [Adobe Workfront Planning Designer 시작](/help/quicksilver/planning/general/planning-ai-designer.md)을 참조하십시오.
