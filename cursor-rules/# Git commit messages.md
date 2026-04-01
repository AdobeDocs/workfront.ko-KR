---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 1%

---
# Git 커밋 메시지

항상 이 규칙을 적용합니다. Git 커밋 메시지를 초안 작성하거나 생성할 때(예: Source 컨트롤 커밋 상자 또는 에이전트 채팅에서 요청 시) 이 형식을 따릅니다.

## 제목 줄(첫 줄만)

- 약 **50자 이하**.
- **명령 기분**&#x200B;의 변경 내용을 요약합니다(예: &quot;추가...&quot;, &quot;수정...&quot;, &quot;리팩터링...&quot;).

## 빈 줄

본문 앞에 제목 뒤에 **빈 줄**&#x200B;을 남깁니다.

## 본문(자세한 설명)

- 약 **72자**&#x200B;에서 줄 바꿈(글머리 기호 접두사 및 공백 포함).
- 설명을 보려면 **글머리 기호**&#x200B;를 사용하십시오. 각 글머리 기호는 다음 중 정확히 하나로 시작해야 합니다.
   - **📖** — 변경 **새 파일, 새 섹션, 새 기능, 새 헤더, 새 줄 또는 기타 그린필드 내용 추가**&#x200B;할 때 사용합니다.
   - **✏️** — 변경 **기존 작업을 수정**&#x200B;할 때 사용: 기존 줄 편집, 기존 섹션 업데이트, 기존 코드 리팩터링 또는 현재 콘텐츠 변경.

추가된 내용과 변경된 내용이 명확하게 표시되도록 모든 본문 글머리 기호에 **📖** 또는 **✏️**&#x200B;을(를) 적용합니다.

## 템플릿

자리 표시자를 입력합니다(최종 메시지에 꺾쇠 괄호를 두지 마십시오).

```
<Summarize change(s) in around 50 characters or less>

<More detailed explanatory description of the change wrapped into about 72
characters with bullets. >
```

## 예

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```
