---
description: Adobe Workfront 릴리스 노트(개요, 제품 영역, 계획 및 디자인 페이지)에 대한 형식 지정 및 유효성 검사 규칙.
applyTo: "help/quicksilver/product-announcements/product-releases/**/*.md"
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%
---

# 릴리스 노트 포맷터

이 파일은 **릴리스 정보**&#x200B;이며 방법 문서가 아닙니다. **적용하지** 않음
일반적인 쓰기 품질 표준. 편집하기 전에 의 전체 소스를 읽으십시오
템플릿과 릴리스 달력이 포함된 truth:

- [.cursor/skills/release-notes-formatter/SKILL.md](../../.cursor/skills/release-notes-formatter/SKILL.md)
- [.cursor/skills/release-notes-formatter/reference.md](../../.cursor/skills/release-notes-formatter/reference.md)

## 중요 규칙 — 문서 분기 우선 결정

&#x200B;> [!IMPORTANT]
> 달력-분기 계산을 사용하여 문서-분기에 기능을 할당하지 않음
> 미리보기 또는 프로덕션 날짜. Doc-quarter는 **월별 릴리스를 기반으로 합니다.**
> 이 기능은 Workfront의 내부 릴리스 캘린더 그룹화에 따라 제공됩니다.
> 은 달력 분기에서 오프셋됩니다. 예: 프로덕션이 있는 기능
> 2026년 8월 13일 날짜는 `26-q3`이(가) 아닌 `26-q4` 문서에 속합니다. 항상
> 앞의 참조 파일에서 2026년 릴리스 캘린더 표를 상호 확인합니다.
> 파일을 만들거나 편집합니다. 프로덕션 날짜가 해당 테이블을 벗어나는 경우
> 추측하는 대신 업데이트된 달력을 요청합니다.

## 주요 구조 규칙

- **Frontmatter**: `feature`은(는) 정확히 `Product Announcements`이어야 합니다.
  `recommendations`은(는) 정확히 `noDisplay, noCatalog`이어야 합니다. 발명해 본 적 없음
  `exl-id` — 이미 있는 경우에만 포함합니다.
- **최신 기능 먼저**: 가장 최근 릴리스 노트는 다음 H2입니다.
각 기능 테이블의 소개(제품 영역 페이지) 및 맨 위 행(개요
페이지 참조).
- **개요 링크**: 제품 영역 페이지는 **해당 분기 페이지로 연결되어야 합니다.**
개요 파일 — 일반적인 버그가 이전 분기에 연결됩니다.
- **날짜 설명**: 각 기능 H2 뒤에 `>[!NOTE]` 블록이 있습니다.
모든 날짜에 대한 미리 보기 / 프로덕션 빠른 릴리스 / 프로덕션,
개요 테이블 행. 날짜를 `Month Day, Year`(으)로 지정하십시오. 알 수 없는 경우 `TBD`을(를) 사용하십시오.
- **H1s에** 쓰여진 분기 이름: &quot;First Quarter&quot;, &quot;Second Quarter&quot;, &quot;Third
Quarter, 4분기.

## 페이지 추가 시 필요한 컴패니언 업데이트

- **새 페이지(모두)**: 동일한 변경 내용으로 `help/quicksilver/TOC.md`에 추가
(개요 먼저, 제품 영역 페이지를 알파벳순으로 정리하고, 기타 개선 사항을 마지막으로 정리합니다.)
- **새 분기의 개요 페이지**: `help/quicksilver/home.md`도 업데이트 —
&quot;최신 릴리스&quot; 탭 링크 및 계획 활동 링크를 새로 고치고 다음을 추가합니다.
현재 연도 릴리스 탭에 대한 새 분기입니다.

전체 템플릿은 위의 SKILL.md 및 reference.md 파일을 참조하십시오.
파일 이름 지정 규칙, 링크 형식 및 전체 릴리스 달력입니다.
