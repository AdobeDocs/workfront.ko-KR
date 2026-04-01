---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---
# 가져오기 요청(PR)

끌어오기 요청 제목이나 설명을 초안 또는 검토할 때(예: GitHub/GitLab에서 또는 에이전트 채팅에서 요청할 때) 다음 규칙을 따릅니다.

## Jira 문제 가져오기

- **Source of truth:** **현재 Git 분기 이름**&#x200B;에서 Jira 문제 ID를 파생합니다(예: `FFENT-8796` 등 프로젝트 키 패턴과 일치하는 세그먼트).
- **분기 이름에 Jira ID가 포함된 경우:** PR 제목(아래 참조)에 해당 ID를 사용하고 `# Context` → `## Jira`에 연결합니다.
- **분기 이름에 Jira ID가 포함되지 않은 경우:** PR을 티켓과 연결되지 않은 것으로 처리합니다. PR 제목에서 Jira 키를 **생략**&#x200B;합니다(티켓을 만들지 마십시오). `# Context` → `## Jira`을(를) 포함합니다. 정확히 콘텐츠는 `No ticket`입니다(링크 없음).

## PR 제목

**분기 이름에 Jira 문제 ID가 포함된 경우**, **모두 포함**:

1. **Jira 문제 ID**(예: `FFENT-8001`).
2. **커밋 유형**(아래 목록 참조)입니다. 다음 패턴을 사용합니다.

`{type}/{JIRA-ID}- {short task description}`

예:

`feat/FFENT-8001- Add validation for numVariations in OCAPI request`

ID 뒤에 간결한 명령형 설명을 사용하십시오. 문자, 슬래시, Jira 키와 후행 하이픈, 공백, 설명 등 표시되는 간격 패턴과 일치합니다.

**분기 이름에 Jira 문제 ID가 포함되지 않은 경우** 제목에서 티켓을 생략하고 다음을 사용하십시오.

`{type}- {short task description}`

예:

`docs- Refresh Object Composite API changelog`

### 허용되는 커밋 유형(`/` 전에 이 레이블을 정확히 사용)

- **기능** — 새 기능을 추가합니다. 새 TOC 항목이 추가되거나 JIRA가 Jira라는 레이블이 지정된 다른 `feat`에 연결된 경우.
- **수정** — 버그 수정
- **리팩터링** — 동작을 변경하지 않고 코드를 재작성/재구성합니다.
- **perf** — 성능 향상(특수 리팩터링)
- **style** — 서식 지정/공백만 사용하며, 의미는 변경되지 않습니다. 편집만 해당
- **test** — 테스트를 추가하거나 수정합니다.
- **docs** — 새 콘텐츠가 추가되었습니다. 설명서만
- **빌드** — 빌드 도구, CI, 종속성, 프로젝트 버전 등
- **ops** — 인프라, 배포, 백업, 복구 등
- **작업** — 기타(예: `.gitignore`)

## PR 본문 — 필수 섹션

**정확히 다음 최상위 섹션을 사용**(Markdown 머리글):

### 1. `# Summary`

변경된 **내용**&#x200B;과(와) **이유**&#x200B;에 대한 간략한 개요(비즈니스 또는 기술 의도).

### 2. `# Changes`

**파일**&#x200B;로 구성합니다. 터치된 각 파일에 대해 레벨 2 머리글을 백틱에 경로를 사용한 다음, 편집 내용을 설명하는 글머리 기호를 사용합니다.

형식:

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.

## `another/file.ts`
* Another bullet for that file.
```

### 3. `# Context`

**아래에 항상** Jira`# Context` 하위 섹션을 포함하십시오.

**분기 이름에 Jira ID가 포함된 경우:** 문제에 대한 클릭 가능한 링크를 사용합니다(분기 이름에서 키 가져오기).

형식:

```markdown
# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

키와 URL을 실제 티켓으로 바꿉니다. 여러 티켓이 적용되는 경우 동일한 하위 섹션에 각 티켓을 개별 라인으로 나열합니다.

**분기 이름에 Jira ID가 포함되지 않은 경우:** `## Jira`을(를) 유지하고 다음을 정확히 사용하십시오.

```markdown
# Context

## Jira
No ticket
```

## 예(전체 PR 설명)

```markdown
# Summary
Adds minimum and maximum constraints for numVariations in the Object Composite API v4 OpenAPI spec.

# Changes

## `static/object-composite-v4.json`
* numVariations in OCAPIRequest now includes minimum: 1 and maximum: 3 to align with the allowed range (number of variations to generate).

# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

## 예 (전체 PR 설명, Jira ID가 없는 분기)

**제목:** `docs- Refresh Object Composite API changelog`

```markdown
# Summary
Refreshes the changelog for the Object Composite API.

# Changes

## `CHANGELOG.md`
* Documents the latest OCAPI v4 constraint updates.

# Context

## Jira
No ticket
```
