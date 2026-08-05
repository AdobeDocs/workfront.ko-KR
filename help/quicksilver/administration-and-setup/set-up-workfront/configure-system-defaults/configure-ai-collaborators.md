---
user-type: administrator
product-area: system-administration;setup
navigation-upperic: configure-locations
title: AI 공동 작업자 구성
description: Adobe Workfront 관리자는 AI 공동 작업자를 구성하고 프로젝트 및 작업에 할당할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
source-git-commit: d875b7e182b5b1782b4fae9d9b609e357bf876a3
workflow-type: tm+mt
source-wordcount: '1438'
ht-degree: 1%

---

# AI 공동 작업자 구성


<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 미리 보기 샌드박스 환경에서만 사용할 수 있습니다.</span>


AI 공동 작업자는 프로젝트 및 작업에 AI 에이전트를 온보딩하는 방법입니다. AI 공동 작업자를 구성한 다음 사용자와 마찬가지로 할당할 수 있습니다.

예를 들어 브랜드 지침으로 검토자 유형 AI Collaborator를 구성한 다음 해당 Collaborator에 문서를 검토하도록 지정할 수 있습니다.

사용 가능한 AI Collaborator 유형은 다음과 같습니다.

* 검토자: 브랜드 또는 Adobe Brand Intelligence를 사용하여 공동 작업자를 만든 다음 해당 공동 작업자를 에셋에 대한 검토자로 할당합니다.

  자세한 내용은 [Workfront 콘텐츠 검토자 시작](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)을 참조하세요.

* 작업 Collaborator: Copilot 또는 Writer를 사용하여 Collaborator를 생성한 다음 작업에 Collaborator를 할당하여 작업 수준 작업을 완료합니다.

  자세한 내용은 [작업 공동 작업자 사용](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)을 참조하세요.


## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 패키지</td> 
   <td><p>Standard, Prime 또는 Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>[!UICONTROL 시스템 관리자]</td> 
  </tr> 
  </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

### AI 검토자의 경우:

* 파일에 Adobe Gen AI 계약에 서명해야 합니다.

  자세한 내용은 Workfront의 AI Assistant 문서에서 [Adobe Gen AI 계약 서명](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)을 참조하십시오.
* 검토자 유형 AI 공동 작업자에 사용하려면 먼저 Workfront에서 브랜드를 구성해야 합니다.

  지침은 [콘텐츠 검토자를 위한 브랜드 만들기 및 관리](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)를 참조하십시오.
* 검토자 AI 공동 작업자에 Adobe Brand Intelligence를 사용하려면 조직에서 Workfront의 통합된 검토 및 승인 경험을 사용해야 합니다. </span>

  자세한 내용은 [통합 검토 및 승인 시작](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)을 참조하십시오. </span>

<div class="preview">

### 작업 공동 작업자용

작업 공동 작업자로 사용하려면 먼저 Claude, Copilot Studio 또는 Writer에서 에이전트를 구성해야 합니다.

</div>

## 새 검토자 유형 AI 공동 작업자 만들기

검토자 AI 공동 작업자는 Workfront 브랜드 또는 Adobe Brand Intelligence를 사용하도록 구성할 수 있습니다.

* **브랜드**: 브랜드는 Workfront에서 만들어집니다. 브랜드 지침이 포함된 PDF 파일을 업로드하거나 브랜드 요소를 수동으로 입력하여 Workfront에서 브랜드를 만들 수 있습니다.
* **Adobe Brand Intelligence**: AI 공동 작업자가 Adobe Brand Intelligence를 사용하여 에셋을 검토할 때 Frame.io에서 검토자가 작성한 댓글을 볼 수 있습니다.  </span>


{{step-1-to-setup}}

1. 왼쪽 탐색에서 **AI 공동 작업자**&#x200B;를 클릭합니다.
1. 화면 오른쪽 상단의 **새 공동 작업자**&#x200B;를 클릭합니다.
1. **검토자**&#x200B;를 클릭한 다음 **계속**&#x200B;을 클릭합니다.
1. Collaborator Name 필드에 Collaborator의 이름을 입력합니다. 작업에서 사용 가능한 할당자 목록에 표시되는 이름입니다.
1. 공동 작업자가 검토에 브랜드를 사용할지 Adobe Brand Intelligence를 사용할지 선택합니다.
1. (조건부) AI 공동 작업자가 브랜드를 사용하는 경우 사용할 브랜드 및 브랜드 지침을 선택합니다.
1. **저장**&#x200B;을 클릭합니다.

<div class="preview">

## 작업 공동 작업자 구성

작업 공동 작업자는 Workfront의 작업에 할당할 수 있는 MCP 에이전트입니다. 이름, 액세스 수준 및 기타 세부 정보를 사용하여 작업 공동 작업자를 구성하고 사용자를 할당할 때처럼 작업에 할당합니다.

작업 공동 작업자는 MCP 에이전트이므로 에이전트를 구성할 때 작업과 능력이 구성됩니다. 현재 작업 공동 작업자로 사용되는 에이전트는 Copilot Studio, Claude 또는 Writer에서 만들 수 있습니다.

작업 공동 작업자는 작업에만 할당할 수 있으며 현재는 문제에 할당할 수 없습니다.

작업 공동 작업자로 작업할 에이전트를 만드는 모범 사례 목록을 보려면 [작업 공동 작업자를 위한 에이전트 만들기 모범 사례](#best-practices-for-creating-an-agent-for-a-task-collaborator)를 참조하세요.

### Workfront에서 작업 공동 작업자 구성

{{step-1-to-setup}}

1. 왼쪽 탐색에서 **AI 공동 작업자**&#x200B;를 클릭합니다.
1. 화면 오른쪽 상단의 **새 공동 작업자**&#x200B;를 클릭합니다.
1. **작업 에이전트**&#x200B;를 선택한 다음 **계속**&#x200B;을 클릭합니다.
1. AI 공동 작업자 이름 필드에 공동 작업자의 이름을 입력합니다. 작업에서 사용 가능한 할당자 목록에 표시되는 이름입니다.
1. AI Collaborator 설명 필드에 Collaborator의 목적이나 수행하는 작업에 대한 설명을 입력합니다.
1. 액세스 수준 필드에서 이 공동 작업자의 액세스 수준을 선택합니다. 이 액세스 수준은 사용자가 수행할 수 있는 작업을 제어하는 것과 같은 방식으로 공동 작업자가 수행할 수 있는 작업을 제어합니다.
1. **에이전트의 원본 선택** 영역에서 Copilot 또는 Writer와 같은 일반 플랫폼에서 만든 에이전트를 연결할지 또는 사용자 지정 에이전트를 사용할지 여부를 선택합니다.
1. (조건부) 일반 플랫폼에서 에이전트를 사용하는 경우 에이전트 플랫폼에 대한 인증 세부 정보를 입력합니다.

   | 플랫폼 | 필수 인증 |
   |---|---|
   | 코파일럿 스튜디오 | 웹 채널 비밀 |
   | Claude Managed Agents | Anthropic API 키<br>에이전트 ID<br>환경 ID |
   | Writer | API 키<br>응용 프로그램 ID |

1. **연결 테스트**&#x200B;를 클릭합니다. 이렇게 하면 연결이 올바르게 설정되었는지 여부를 알 수 있습니다.
1. **Collaborator의 작업이 완료되면** 영역에서 Collaborator가 수행할 작업을 전환할 수 있습니다.
1. **저장**&#x200B;을 클릭합니다.

작업에 할당하는 방법을 포함하여 작업 공동 작업자에 대한 자세한 내용은 [작업 공동 작업자 사용](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)을 참조하세요.


### 작업 공동 작업자를 위한 에이전트 생성 우수 사례

Workfront에서 작업 공동 작업자로 사용할 에이전트를 생성할 때 도움이 되는 모범 사례는 다음과 같습니다. 모범 사례를 보려면 에이전트를 만드는 응용 프로그램의 섹션을 클릭합니다.

+++ 클로드

1. [platform.claude.com](https://platform.claude.com/)의 클라우드 콘솔로 이동합니다.
1. API 키를 만듭니다.
   1. API 키에서 오른쪽 상단의 **키 만들기**&#x200B;를 클릭합니다.
   1. 이름 및 만료 날짜를 입력합니다.
   1. 키를 복사하여 안전하고 안전한 곳에 저장하십시오. Workfront에서 작업 공동 작업자를 구성하려면 이 키가 필요합니다.

1. 환경을 만듭니다.
   1. **관리 에이전트** > **환경**&#x200B;에서 오른쪽 상단의 **환경 만들기**&#x200B;를 클릭합니다.
   1. 해당되는 경우 이름 및 호스팅 유형을 제공합니다.
   1. 필요에 따라 공유 패키지 및 메타데이터를 구성합니다. 환경은 여러 에이전트에서 재사용되고 공유 패키지 및 메타데이터를 허용할 수 있습니다.
      환경 ID는 왼쪽 상단 모서리의 환경 이름 아래에 표시됩니다.

1. 에이전트를 만듭니다.
   1. 관리 에이전트 > 에이전트에서 오른쪽 상단의 **에이전트 만들기**&#x200B;를 클릭합니다.
   1. 이름, 모델, 시스템 프롬프트, 스킬 및 도구를 입력합니다. 설명적이어야 합니다. 작업 공동 작업자가 작업 컨텍스트를 이 에이전트에게 전달한 다음 작업을 실행하기 때문입니다.
      에이전트 ID는 왼쪽 상단 모서리의 에이전트 이름 아래에 나타납니다.

1. Workfront에서 작업 공동 작업자 구성
   1. API 키, 환경 ID 및 에이전트 ID를 입력합니다
   1. 확인하려면 **연결 테스트**&#x200B;를 클릭하십시오.

1. 작업 공동 작업자를 Workfront 작업에 할당합니다.
   1. 작업 공동 작업자는 모든 전임 작업이 완료된 후에 실행됩니다.

+++
<!--
+++ Copilot Studio



+++
-->
+++ Writer

>[!NOTE]
>
> 작성기 에이전트를 작업 공동 작업자로 사용할 수 있지만 작성기 플레이북은 작업 공동 작업자로 사용할 수 없습니다.

Writer에서 작업 공동 작업자로 사용할 에이전트를 만들 때는 다음 워크플로를 사용하는 것이 좋습니다.

에이전트 만들기에 대한 자세한 내용은 [작성기 설명서](https://dev.writer.com/no-code/introduction)를 참조하세요.

1. Writer AI Studio에서 코드 없는 앱을 만듭니다.
1. 단일 텍스트 입력 필드를 추가합니다. 기본 이름 &quot;텍스트 입력&quot;을 사용할 수 있습니다.
1. `@TextInput`을(를) 프롬프트에 추가합니다. 앱 구성의 프롬프트 섹션에서 프롬프트 템플릿이 입력 변수를 참조하는지 확인합니다. 이 옵션이 없으면 모델에 작업 데이터가 표시되지 않습니다.
1. 출력을 즉시 생성하려면 프롬프트를 조정하십시오. 응답하기 전에 사용자에게 명확한 설명 또는 추가 컨텍스트를 요청하는 지침을 제거하십시오. 예: &quot;입력을 받으면 콘텐츠 생성 요청으로 처리하고 출력을 즉시 생성합니다. 설명을 요청하지 마십시오.&quot;
1. API 키 및 애플리케이션 ID를 복사합니다. Workfront에서 작업 공동 작업자를 구성하려면 작업 공동 작업자가 필요합니다.

   * Writer에서 API 키를 설정하는 방법에 대한 지침은 Writer 설명서의 [빠른 시작](https://dev.writer.com/home/quickstart)을 참조하십시오.
   * Writer에서 응용 프로그램 ID를 설정하는 방법은 Writer 설명서에서 [API를 통해 코드 없는 에이전트 호출](https://dev.writer.com/home/applications)을 참조하십시오.

1. Workfront에서 작업 공동 작업자 구성 구성의 일부로 API 키와 응용 프로그램 ID를 입력한 다음 **연결 테스트**&#x200B;를 클릭하여 확인합니다.
1. 작업 공동 작업자를 Workfront 작업에 할당합니다. 공동 작업자는 작업의 전임 작업이 모두 완료되면 작업을 시작합니다.

+++

</div>

## AI 공동 작업자 관리

기존 AI 공동 작업자를 편집, 복사 및 삭제할 수 있습니다.

{{step-1-to-setup}}

1. 왼쪽 탐색에서 **AI 공동 작업자**&#x200B;를 클릭합니다.
1. (조건부) Collaborator를 편집하려면 편집할 Collaborator의 이름을 클릭하고 Collaborator 편집 창에서 편집한 다음 **저장**&#x200B;을 클릭합니다.
1. (조건부) Collaborator를 복사하려면 복사할 AI Collaborator 행에서 복사 아이콘 ![복사 아이콘](assets/copy-ai-collaborator.png)을 클릭하고 복사 이름을 클릭한 다음 Collaborator 편집 창에서 편집을 수행하고 **저장**&#x200B;을 클릭합니다.
1. (조건부) Collaborator를 삭제하려면 삭제하려는 AI Collaborator 행에서 삭제 아이콘 ![삭제 아이콘](assets/delete-collaborator-icon.png)을 클릭한 다음 **삭제**&#x200B;를 클릭합니다.
