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
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 1a1e8fab8f8ef5c0c9dae032ed0eb5b24c3f364d
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 2%
---
# AI 공동 작업자 구성

AI 공동 작업자는 프로젝트, 작업 및 문제에 AI 에이전트를 온보딩하는 방법입니다. AI 공동 작업자를 구성한 다음 사용자와 마찬가지로 할당할 수 있습니다.

예를 들어 브랜드 지침으로 검토자 유형 AI Collaborator를 구성한 다음 해당 Collaborator에 문서를 검토하도록 지정할 수 있습니다.

사용 가능한 AI Collaborator 유형은 다음과 같습니다.

* AI 검토자: 브랜드 또는 Adobe Brand Intelligence을 사용하여 공동 작업자를 만든 다음 공동 작업자를 에셋에 대한 검토자로 할당합니다.

  자세한 내용은 [Workfront AI 검토자 시작](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)을 참조하세요.

* 작업 에이전트: Claude, OpenAI 또는 Copilot과 같은 표준 AI 플랫폼을 사용하여 공동 작업자를 만든 다음 작업 또는 문제에 공동 작업자를 할당하여 작업 항목을 완료합니다.

  자세한 내용은 [작업 에이전트 사용](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)을 참조하세요.

<!--
* <span class="preview">Project Coordinator: An out-of-the-box collaborator that monitors project status and follows up on overdue tasks automatically, without needing to configure an external agent.</span>

   <span class="preview">For more information, see [Use the Project Coordinator collaborator](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).</span>
-->


## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 패키지</td> 
   <td><p>Select, Prime 또는 Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>[!UICONTROL 시스템 관리자] 또는 그룹 관리자</span></td> 
  </tr> 
  </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

* [AI 검토자용](#for-ai-reviewers)
* [작업 에이전트용](#for-work-agents)

### AI 검토자의 경우:

* 파일에 Adobe Gen AI 계약에 서명해야 합니다.

  자세한 내용은 Workfront의 AI Assistant 문서에서 [Adobe Gen AI 계약 서명](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)을 참조하십시오.
* AI 검토자에 사용하려면 Workfront에서 브랜드를 구성해야 합니다.

  지침은 [AI 검토자를 위한 브랜드 만들기 및 관리](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)를 참조하십시오.
* AI 검토자에 Adobe Brand Intelligence을 사용하려면 조직에서 Workfront의 통합 검토 및 승인 경험을 사용해야 합니다.

  자세한 내용은 [통합 검토 및 승인 시작](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)을 참조하세요.

### 작업 에이전트용

클라우드, Copilot Studio, OpenAI 또는 IBM에서 에이전트를 구성해야 작업 에이전트로 사용할 수 있습니다.

>[!NOTE]
>
>모든 에이전트 공급자와 연결하고자 하므로 사용 중인 공급자가 작업 에이전트와 현재 호환되지 않는 경우 계정 팀에 도움을 요청하십시오.

## 새 AI 검토자 만들기

Workfront 브랜드 또는 Adobe Brand Intelligence을 사용하도록 AI 검토자를 구성할 수 있습니다.

* **브랜드**: 브랜드는 Workfront에서 만들어집니다. 브랜드 지침이 포함된 PDF 파일을 업로드하거나 브랜드 요소를 수동으로 입력하여 Workfront에서 브랜드를 만들 수 있습니다.
* **Adobe Brand Intelligence**: AI 공동 작업자가 Adobe Brand Intelligence을 사용하여 에셋을 검토할 때 Frame.io에서 AI 검토자가 작성한 댓글을 볼 수 있습니다.


{{step-1-to-setup}}

1. 왼쪽 탐색에서 **AI 공동 작업자**&#x200B;를 클릭합니다.
1. 화면 오른쪽 상단의 **새 공동 작업자**&#x200B;를 클릭합니다.
1. **검토자**&#x200B;를 클릭한 다음 **계속**&#x200B;을 클릭합니다.
1. Collaborator Name 필드에 Collaborator의 이름을 입력합니다. 작업에서 사용 가능한 할당자 목록에 표시되는 이름입니다.
1. 공동 작업자가 검토에 브랜드를 사용할지 Adobe Brand Intelligence을 사용할지 선택합니다.
1. (조건부) AI 공동 작업자가 브랜드를 사용하는 경우 사용할 브랜드 및 브랜드 지침을 선택합니다.
1. **저장**&#x200B;을 클릭합니다.

## 작업 에이전트 구성

작업 에이전트는 Workfront의 작업 또는 문제에 할당할 수 있는 에이전트입니다. 이름, 액세스 수준 및 기타 세부 정보를 사용하여 작업 에이전트를 구성하고 사용자를 할당할 때처럼 작업에 할당합니다.

작업 에이전트는 에이전트이므로 에이전트를 구성하는 위치에 작업 및 기능이 구성됩니다. 현재 Copilot Studio, Claude, OpenAI, IBM 등에서 작업 에이전트로 활용되는 에이전트를 만들 수 있다.

작업 에이전트는 작업 또는 문제에 할당할 수 있습니다.

작업 에이전트로 작업할 에이전트를 만드는 모범 사례 목록을 보려면 [작업 에이전트용 에이전트 만들기 모범 사례](#best-practices-for-creating-an-agent-for-a-work-agent)를 참조하십시오.

* [Workfront에서 작업 에이전트 구성](#configure-a-work-agent-in-workfront)
* [작업 에이전트용 에이전트 생성 모범 사례](#best-practices-for-creating-an-agent-for-a-work-agent)

### Workfront에서 작업 에이전트 구성

>[!NOTE]
>
>작업 에이전트에서 사용한 라이선스는 청구되지 않습니다. 조직에 200개의 Workfront 라이센스가 있고 작업 에이전트를 만드는 경우 201개의 라이센스가 사용 중이지만 200개만 청구됩니다.

{{step-1-to-setup}}

1. 왼쪽 탐색에서 **AI 공동 작업자**&#x200B;를 클릭합니다.
1. 화면 오른쪽 상단의 **새 공동 작업자**&#x200B;를 클릭합니다.
1. **작업 에이전트**&#x200B;를 선택한 다음 **계속**&#x200B;을 클릭합니다.
1. AI 공동 작업자 이름 필드에 공동 작업자의 이름을 입력합니다. 작업에서 사용 가능한 할당자 목록에 표시되는 이름입니다.
1. AI Collaborator 설명 필드에 Collaborator의 목적이나 수행하는 작업에 대한 설명을 입력합니다.
1. 액세스 수준 필드에서 이 공동 작업자의 액세스 수준을 선택합니다. 이 액세스 수준은 사용자가 수행할 수 있는 작업을 제어하는 것과 같은 방식으로 공동 작업자가 수행할 수 있는 작업을 제어합니다.
1. (선택 사항) 그룹 필드에서 작업 에이전트와 연결할 그룹을 선택합니다.

   >[!NOTE]
   >
   >그룹 관리자인 경우 이 필드에는 관리자인 그룹만 표시됩니다. 그룹 관리자는 그룹을 하나 이상 선택해야 합니다.

1. **에이전트의 원본 선택** 영역에서 Copilot과 같은 일반 플랫폼에서 만든 에이전트를 연결할지 또는 사용자 지정 에이전트를 사용할지 여부를 선택합니다.
1. (조건부) 일반 플랫폼에서 에이전트를 사용하는 경우 에이전트 플랫폼에 대한 인증 세부 정보를 입력합니다.

   | 플랫폼 | 필수 인증 |
   |---|---|
   | 코파일럿 스튜디오 | 웹 채널 암호 |
   | Claude Managed Agents | Anthropic API 키<br>에이전트 ID<br>환경 ID |
   | OpenAI 에이전트 | API 키 <br>에이전트 ID |
   | IBM watsonx Orchestrate | 서비스 URL<br>API 키<br> 에이전트 ID |

1. **연결 테스트**&#x200B;를 클릭합니다. 이렇게 하면 연결이 올바르게 설정되었는지 여부를 알 수 있습니다.
1. **Collaborator의 작업이 완료되면** 영역에서 Collaborator가 수행할 작업을 전환할 수 있습니다.

   * 알림 보내기: 에이전트는 업데이트 스트림에 댓글을 달며 작업을 요청하거나, 에이전트를 할당하거나, 프로젝트를 소유한 사용자에게 태그를 지정합니다.
   * 텍스트 기반 문서 업로드
   * 작업을 완료로 표시
   * 작업 필드 쓰기: 에이전트가 쓸 수 있는 양식 및 필드를 선택합니다.
   * 프로젝트 필드 쓰기: 에이전트가 쓸 수 있는 양식 및 필드를 선택합니다.

1. **저장**&#x200B;을 클릭합니다.

작업에 할당하는 방법을 포함하여 작업 에이전트에 대한 자세한 내용은 [작업 에이전트 사용](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)을 참조하십시오.

### 작업 에이전트용 에이전트 생성 모범 사례

Workfront에서 작업 에이전트로 사용할 에이전트를 생성할 때 도움이 되는 모범 사례는 다음과 같습니다. 모범 사례를 보려면 에이전트를 만드는 응용 프로그램의 섹션을 클릭합니다.

+++ Claude

1. [platform.claude.com](https://platform.claude.com/)의 클라우드 콘솔로 이동합니다.
1. API 키를 만듭니다.
   1. API 키에서 오른쪽 상단의 **키 만들기**&#x200B;를 클릭합니다.
   1. 이름 및 만료 날짜를 입력합니다.
   1. 키를 복사하여 안전하고 안전한 곳에 저장하십시오. Workfront에서 작업 에이전트를 구성하려면 이 키가 필요합니다.

1. 환경을 만듭니다.
   1. **관리 에이전트** > **환경**&#x200B;에서 오른쪽 상단의 **환경 만들기**&#x200B;를 클릭합니다.
   1. 해당되는 경우 이름 및 호스팅 유형을 제공합니다.
   1. 필요에 따라 공유 패키지 및 메타데이터를 구성합니다. 환경은 여러 에이전트에서 재사용되고 공유 패키지 및 메타데이터를 허용할 수 있습니다.
      환경 ID는 왼쪽 상단 모서리의 환경 이름 아래에 표시됩니다.

1. 에이전트를 만듭니다.
   1. 관리 에이전트 > 에이전트에서 오른쪽 상단의 **에이전트 만들기**&#x200B;를 클릭합니다.
   1. 이름, 모델, 시스템 프롬프트, 스킬 및 도구를 입력합니다. 작업 에이전트는 작업 컨텍스트를 이 에이전트로 전달한 다음 작업을 실행하므로 설명하십시오.
      에이전트 ID는 왼쪽 상단 모서리의 에이전트 이름 아래에 나타납니다.

1. Workfront에서 작업 에이전트를 구성합니다.
   1. API 키, 환경 ID 및 에이전트 ID를 입력합니다
   1. 확인하려면 **연결 테스트**&#x200B;를 클릭하십시오.

1. Workfront 작업에 작업 에이전트를 할당합니다.
   1. 작업 에이전트는 모든 전임 작업이 완료된 후 실행됩니다.

+++
<!--
+++ Copilot Studio



+++
-->
+++ Writer



>[!IMPORTANT]
>
>작성기가 에이전트 사용을 중단했습니다. 작성기 에이전트를 사용하여 구성된 작업 에이전트는 10월 9일 이후 더 이상 작동하지 않습니다. 2026.
>
>사용 중단에 대한 자세한 내용은 작성기 설명서에서 [에이전트 라이브러리 마이그레이션 및 사용 중단](https://support.writer.com/articles/8335689949-migrating-no-code-agents)을 참조하십시오.


<!--

>[!NOTE]
>
> You can use a Writer agent as a Work Agent, but Writer playbooks cannot be used as Work Agents.

When creating an agent for use as a Work Agent in Writer, we recommend the following workflow.

More detailed information about creating agents can be found in the [Writer documentation](https://dev.writer.com/no-code/introduction).

1. Create a no-code app in Writer AI Studio. 
1. Add a single Text input field. You can use the default name "Text input."
1. Add `@TextInput` to your Prompt. In the Prompts section of your app configuration, make sure your prompt template references the input variable. Without this, the model never sees the task data.
1. Adjust your Prompt to generate output immediately. Remove any instructions that ask the user for clarification or additional context before responding. For example: "When you receive input, treat it as a content generation request and produce the output immediately. Do not ask for clarification."
1. Copy your API key and Application ID. You will need them to configure the Work Agent in Workfront.

   * For instructions on setting up an API key in Writer, see [Quickstart](https://dev.writer.com/home/quickstart) in the Writer documentation.
   * For instructions on setting up an application ID in Writer, see [Invoke no-code agents via the API](https://dev.writer.com/home/applications) in the Writer documentation.
 
1. Configure the Work Agent in Workfront. As part of the configuration, enter your API key and Application ID, then click **Test connection** to verify.
1. Assign the Work Agent to a Workfront task. The Work Agent begins work when all of the task's predecessor tasks are complete.

-->

+++

<div class="preview">

<!--
## Configure a Project Coordinator

The Project Coordinator is an out-of-the-box collaborator that monitors project status and helps keep work on track. Unlike Work Agents, the Project Coordinator does not require you to configure an external agent.

{{step-1-to-setup}}

1. In the left navigation, click **AI Collaborators**.
1. Click **New Collaborator** in the upper-right corner of the screen.
1. Select **Project Coordinator**.
1. In the **AI Collaborator name** field, enter a name for the Project Coordinator. This is the name that appears as the collaborator in your project.
1. In the **AI Collaborator description** field, enter a description of what the Project Coordinator does or its purpose.
1. In the **Access level** field, select an access level for the Project Coordinator. This access level controls what the collaborator can do on projects.
1. (Optional) In the **Send project updates** section, toggle **Allow** to enable project update notifications, then specify update details.
   * In the **Cadence** field, select whether the Coordinator sends updates daily or weekly.
   * If the Coordinator sends updates weekly, in the **Day of week** field, select the day of the week that updates are sent.
   * In the **Time (MST)** field, select the time to send updates.
   * In the **How to send** field, select whether the Coordinator sends updates as an update on the project, or as an email
   * In the **Who gets the update** field, select whether the update is sent only to the project owner, or to all project stakeholders.
   * (Optional) Check **Send additional update immediately when coordinator is assigned** to notify on assignment.
   * (Optional) Check **Send additional update when a date is missed** to send notifications when dates are missed.
1. (Optional) In the **Notify task assignees** section, toggle **Allow** to enable task notifications, then check the boxes for the situations that you want to notify assignees about.
1. (Optional) In the **Remind reviewers and approvers** section, toggle **Allow** to enable reminders for reviewers, then check the boxes for the situations that you want to remind reviewers and approvers about.
1. (Optional) In the **Update the content of project and task fields** section, toggle **Allow** to enable the coordinator to update project and task field values.
1. Click **Save**.

For more information on the Project Coordinator, including how to assign it to projects, see [Use the Project Coordinator collaborator](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).
-->

</div>

## AI 공동 작업자 관리

기존 AI 공동 작업자를 편집, 복사 및 삭제할 수 있습니다.

>[!NOTE]
>
>그룹 관리자는 자신이 관리자인 그룹과 연결된 AI 공동 작업자만 보고 상호 작용할 수 있습니다. 다른 그룹도 주어진 AI 공동 작업자와 연결된 경우 그룹 관리자는 이를 볼 수 있지만 편집할 수는 없습니다.

{{step-1-to-setup}}

1. 왼쪽 탐색에서 **AI 공동 작업자**&#x200B;를 클릭합니다.
1. (조건부) Collaborator를 편집하려면 편집할 Collaborator의 이름을 클릭하고 Collaborator 편집 창에서 편집한 다음 **저장**&#x200B;을 클릭합니다.
1. (조건부) Collaborator를 삭제하려면 삭제하려는 AI Collaborator 행에서 삭제 아이콘 ![삭제 아이콘](assets/delete-collaborator-icon.png)을 클릭한 다음 **삭제**&#x200B;를 클릭합니다.
