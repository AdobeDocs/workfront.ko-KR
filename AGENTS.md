---
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%
---
# AGENTS.md

**workfront.en** 저장소에 대한 에이전트 지침(Adobe Workfront 영어)
설명서). 이 파일은 모든 에이전트를 가리키는 표준 지침을 가리킵니다.
읽는 규칙 파일에 관계없이 동일한 규칙을 따릅니다.

## 표준 지침 파일

- **저장소 전체 규칙**: [.github/copilot-instructions.md](.github/copilot-instructions.md)
— 후보 문서 검색, 편집 전 제안, 커밋 메시지 및 PR 형식
&quot;지능적으로 공백을 채웁니다.&quot;
- **쓰기 표준**(`help/**/*.md`에 자동 적용):
  [.github/instructions/writing-quality.instructions.md](.github/instructions/writing-quality.instructions.md),
의 모든 세부 사항 포함
  [.cursor/skills/writing-quality/reference.md](.cursor/skills/writing-quality/reference.md).
- **릴리스 정보**(`product-announcements/product-releases/**`에 자동 적용):
  [.github/instructions/release-notes-formatter.instructions.md](.github/instructions/release-notes-formatter.instructions.md).
- **미리 보기 강조 정리**(주문형 워크플로):
  [.github/prompts/remove-preview-highlighting.prompt.md](.github/prompts/remove-preview-highlighting.prompt.md).

## 협상할 수 없는 행동

1. **새 문서를 만들기 전에 후보 문서를 찾으십시오.** 새 콘텐츠 제공 시
에서 `help/`을(를) 검색하고 맞출 수 있는 기존 문서의 등급 목록을 표시합니다.
그럼 초안을 작성하기 전에 어디 있는지 물어 보세요.
2. **도움말 `.md` 문서를 편집하기 전에 변경 내용을 제안합니다.** 제안된 항목 표시
차이를 두고 명시적 승인을 기다립니다. 유일한 예외는 내가 &quot;그냥 고쳐&quot;라고 말할 때입니다
같은 순서로 &quot;묻지 말고 편집해&quot;라는 식이다. 읽기 전용 리서치 및 채팅
초안은 언제나 괜찮습니다.
3. **간격을 지능적으로 채웁니다.** 의도가 명확하면 다음을 커밋하십시오.
모범 사례 답변과 주변 기사 제목 일치,
옵션 메뉴를 표시하는 대신 용어 및 구조를 사용합니다.
4. `help/`번 편집할 때마다 **쓰기 표준을 미리 적용**&#x200B;합니다. 기다리지 마십시오.
다시 생각하게.

## 커밋 및 PR 규칙

자세한 내용은 [.github/copilot-instructions.md](.github/copilot-instructions.md)을(를) 참조하십시오
커밋 메시지 형식(명령형 제목 ≤ ~50자, 추가 📖, 추가 ✏️
수정 사항) 및 PR 구조(분기 이름의 Jira ID; `# Summary`,
`# Changes` 파일, `# Context` → `## Jira`).
