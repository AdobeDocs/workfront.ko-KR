---
name: release-notes-formatter
description: Workfront 릴리스 정보의 일관성, 올바른 구조 및 적절한 링크에 대한 형식과 유효성을 검사합니다. 제품 릴리스 디렉토리의 릴리스 노트 파일에 대해서만 사용하거나 사용자가 릴리스 노트, 제품 릴리스 또는 분기별 릴리스에 대해 언급할 때만 사용합니다. 방법 문서 또는 일반 설명서에는 적용되지 않습니다.
source-git-commit: ec081e557ec48adcfcb3833bf11dcee91312ef4e
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 3%

---


# 릴리스 노트 포맷터

`help/quicksilver/product-announcements/product-releases/` 디렉터리에서 Adobe Workfront 릴리스 정보의 형식을 지정하고 유효성을 검사합니다.

## 페이지 유형

파일 경로 및 콘텐츠에서 페이지 유형을 식별합니다.

| 페이지 유형 | 파일 패턴 | 템플릿 |
|-----------|-------------|----------|
| **개요** | `{YY}-q{N}-release-overview.md` | [reference.md#overview](reference.md#overview-page-template) |
| **제품 영역** | `{YY}-q{N}-{area}.md` | [reference.md#product-area](reference.md#product-area-page-template) |
| **계획** | `planning-release-activity-{YY}-q{N}.md` | 제품 영역과 유사 |
| **자세히 보기** | `look-and-feel-updates-{YY}-q{N}.md` | [reference.md#look-and-feel](reference.md#look-and-feel-page-template) |

## 워크플로 서식 지정

### 1단계: Frontmatter 유효성 검사

모든 릴리스 노트 페이지의 필수 필드:

```yaml
---
title: <descriptive title>
description: <matches or summarizes the title>
author: <author name>
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: <existing UUID — never generate or change>
---
```

규칙:
- `feature`은(는) 정확히 `Product Announcements`이어야 합니다.
- `recommendations`은(는) 정확히 `noDisplay, noCatalog`이어야 합니다.
- `exl-id`을(를) 만들지 마십시오. 이미 있는 경우에만 포함합니다.
- 실제 페이지에 `draft: Probably`을(를) 추가하지 않음(템플릿만)

### 2단계: 페이지 유형별 구조 유효성 검사

#### 제품 영역 페이지

1. **시간1**: `{Written Quarter} {Area} enhancements`
   - 예: `# Second Quarter 2026 Administrator enhancements`
   - 분기는 작성해야 합니다. &quot;1분기&quot;, &quot;2분기&quot;, &quot;3분기&quot;, &quot;4분기&quot;

2. **소개 단락**: 영역 및 개요 링크를 설명합니다.
   - **올바른 분기의** 개요 파일에 연결해야 합니다.
   - 일반적인 버그: 이전 분기에 연결(예: `26-q2` 대신 `26-q1`)

3. 기능당 **H2**: 머리글로 기능 제목
   - **최신 기능 먼저** — 가장 최근 릴리스 노트는 소개 단락 다음의 첫 번째 H2로 표시되어야 합니다.
   - 이전 기능은 역연대순으로 표시됩니다

4. 각 H2 이후 **날짜 설명 블록**:

```markdown
>[!NOTE]
>
>Preview: {Month Day, Year}
>Production fast release: {Month Day, Year}
>Production for everyone: {Month Day, Year}
```

5. **본문**: 기능 설명, 도움말 설명서 링크

#### 개요 페이지

1. **시간1**: `{Written Quarter} release overview`

2. 릴리스 예정일이 있는 **단락 소개**

3. 릴리스 일정 테이블이 있는 **`>[!IMPORTANT]`블록**

4. 앵커 링크의 글머리 기호 목록이 있는 **H2`Adobe Workfront enhancements`**:

```markdown
* [Administrator enhancements](#administrator-enhancements)
* [Document enhancements](#document-enhancements)
```

5. HTML 기능 테이블이 포함된 제품 영역당 **H3**([reference.md](reference.md#overview-feature-table) 참조)
   - 각 테이블 내에서 **최신 기능 먼저** — 가장 최근 행이 테이블의 맨 위(머리글 행 뒤)에 나타납니다.

6. **후행 섹션**(H2): 다른 영역에 대한 릴리스 정보, 바탕 화면 교정 뷰어 업데이트, 알림, API 버전, 유지 관리 업데이트, 교육 업데이트

### 3단계: 링크 유효성 검사

- **제품 영역 페이지의 개요 링크**: 같은 분기를 가리켜야 합니다.
   - 올바른 값: `26-q2-release-activity/26-q2-release-overview.md`
   - 잘못됨: `26-q1-release-activity/26-q1-release-overview.md`
- **개요의 앵커 링크**: H3 ID(소문자, 하이픈)와 일치해야 합니다.
- **개요 테이블의 기능 링크**: `class="MCXref xref" xrefformat="{para}"`을(를) 사용해야 합니다.
- **도움말 문서 링크**: `/help/quicksilver/`(으)로 시작해야 함

### 4단계: 날짜 확인

- 형식: `{Month} {Day}, {Year}`(예: &quot;2026년 3월 12일&quot;)
- 알 수 없는 날짜에 `TBD` 사용
- 제품 영역 페이지 `>[!NOTE]` 블록의 날짜는 해당 개요 테이블 행과 일치해야 합니다.
- 미리 보기 날짜는 프로덕션 날짜보다 선행해야 합니다.

### 5단계: 일반적인 수정 사항

서식 지정 시 다음 수정 사항 적용:

| 문제 | 수정 |
|-------|-----|
| 잘못된 개요 링크 분기 | 파일의 자체 분기와 일치하도록 업데이트 |
| `>[!NOTE]` 날짜 블록 누락 | H2 기능 제목 뒤에 블록 추가 |
| 일관성 없는 날짜 형식 | `Month Day, Year`(으)로 표준화 |
| `>[!NOTE]` 앞에 빈 줄 누락 | 빈 줄 추가 |
| 콜아웃 라인의 추가 공백 | 후행 공백 트리밍 |
| 제품 영역 페이지의 HTML | Markdown으로 유지(HTML은 개요 테이블에만 해당) |
| `exl-id` 누락 | 제외합니다. 생성하지 마십시오. |

## 파일 이름 지정 규칙

| 유형 | 패턴 | 예 |
|------|---------|---------|
| 개요 | `{YY}-q{N}-release-overview.md` | `26-q2-release-overview.md` |
| 제품 영역 | `{YY}-q{N}-{area-slug}.md` | `26-q2-admin-and-setup.md` |
| 디렉터리 | `{YY}-q{N}-release-activity/` | `26-q2-release-activity/` |

표준 영역 슬러그: `admin-and-setup`, `documents`, `projects`, `reports`, `requests`, `other`

## 분기 매핑

| 분기 | 작성된 양식 | 개월 |
|---------|-------------|--------|
| Q1 | 첫 분기 | 1월-3월 |
| Q2 | 2분기 | 4월 6월 |
| Q3 | 1/4 분기 | 7월-9월 |
| Q4 | 4분기 | 10월~12월 |

분기별 생산 발표는 일반적으로 해당 분기 마지막 달의 두 번째 주 목요일에 도달합니다.

## 유효성 검사 목록

릴리스 노트 파일을 검토할 때 다음을 확인하십시오.

- [ ] Frontmatter에 올바른 값을 가진 모든 필수 필드가 있습니다.
- [ ]개의 H1이 페이지 형식 형식과 일치합니다.
- [ ] 개요 링크가 올바른 분기를 가리킵니다.
- [ ] 각 기능에 `>[!NOTE]` 날짜 블록(제품 영역 페이지)이 있습니다.
- [ ] 날짜 형식이 일치합니다(`Month Day, Year`).
- [ 개요의 ] 기능 테이블 행이 제품 영역 페이지 콘텐츠와 일치합니다.
- [ ] 끊어진 내부 링크가 없습니다.
- [ 개요의 ] 앵커 링크가 H3 섹션 ID와 일치합니다.
- [ ] 기능은 가장 최신 순으로 정렬됩니다(제품 영역 페이지와 개요 테이블 모두).

## 추가 리소스

- 전체 HTML 템플릿 및 예제는 [reference.md](reference.md)을(를) 참조하십시오
