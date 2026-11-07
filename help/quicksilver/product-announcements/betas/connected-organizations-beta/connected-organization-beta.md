---
product-area: betas
title: 연결된 조직 기능 Beta 프로그램
description:
author: Alina
feature: Product Announcements
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: b19d0b1bcda5a4f0f2b6b2caf986e1e4dbc9773a
workflow-type: tm+mt
source-wordcount: '1424'
ht-degree: 0%
---
# 연결된 조직 기능 베타 프로그램

>[!IMPORTANT]
>
>연결된 조직 기능은 현재 비공개 베타 단계이며 소수의 고객에게 공개됩니다.
>
>베타 버전은 2026년 말까지 실행됩니다.
>
>질문이 있는 경우 Adobe Beta 프로그램 관리자에게 문의하십시오.

연결된 조직 기능을 사용하면 두 조직이 Adobe Workfront을 구입한 경우 회사와 파트너가 공동 작업을 수행할 수 있습니다.

예를 들어, 고객 회사는 자신의 제공 회사에 수행할 작업에 대한 요청을 제출할 수 있습니다.

각 회사는 자체 사용자, 권한 및 워크플로우를 사용하여 자체 Workfront 인스턴스에서 작업을 계속할 수 있습니다.

작업 객체는 두 인스턴스 간에 미러링되며, 양쪽이 공유에 동의한 데이터만 동기화됩니다.

그 결과, 추가 게스트 로그인, 중복 라이선스 또는 긴 이메일 스레드 없이 요청, 상태 및 의사 결정에 대한 공유 보기가 만들어집니다.

## 오늘날의 다중 조직 워크플로 개요

두 회사가 모두 Workfront에 투자했을 때 두 번 비용을 지불하거나 상대 시스템으로 이직하지 않고 함께 일할 수 있어야 한다.

현재 두 회사가 서로 다른 두 시스템에서 작업할 때 공동 작업에는 다음 워크플로 중 일부가 포함될 수 있습니다.

* 요청과 준비는 따르기 어려운 이메일 스레드를 통해 전달됩니다.

* 핸드오프는 수동이며 감사 가능성이 거의 없습니다.

* 다른 회사의 시스템 내에서 작업한다는 것은 게스트 로그인, 추가 라이선스 또는 둘 다를 의미합니다.

* 여러 개의 파일 복사본이 순환하며 어느 것이 진실의 원인인지 아무도 확신하지 못합니다.

* 상태를 따라가기 어렵기 때문에 계정 관리자는 데크를 구축하고 업데이트 회의를 예약하는 데 시간을 소비합니다.

## 연결된 조직 솔루션 개요

연결된 조직 기능을 사용하면 두 회사는 서로 다른 두 시스템에서 계속 작업하며 공동 작업에는 다음 워크플로 중 일부가 포함됩니다.

* 두 조직 모두 상대 인스턴스의 객체에 액세스하지 않습니다.
* 클라이언트 조직의 요청과 같은 개체가 복제되어 제공자의 인스턴스에 게시됩니다.
* 동기화를 위해 구성된 메타데이터만 두 복제본 간에 최신 상태로 유지됩니다.
* 각 회사는 해당 오브젝트 이상으로 자체 사용자, 권한 및 워크플로우를 관리합니다.

그 지침의 원칙은 그 일을 완수하기 위해 필요한 최소한의 것을 공유하고, 그 밖의 모든 것을 비밀로 유지하는 것이다.

<table>
<tbody>
<tr class="odd">
<td><strong>공유된 항목</strong></td>
<td><strong>비공개로 유지</strong></td>
</tr>
<tr class="even">
<td><ul>
<li><p>개요 및 요청 세부 정보</p></li>
<li><p>합의된 기한 및 이정표</p></li>
<li><p>댓글 검토</p></li>
<li><p>승인 결정</p></li>
<li><p>최종 승인된 에셋</p></li>
</ul></td>
<td><ul>
<li><p>다른 클라이언트 또는 다른 에이전트와의 관계</p></li>
<li><p>재무, 요금 및 고객에게 부과되는 비용</p></li>
<li><p>리소스 계획 및 용량</p></li>
<li><p>내부 프로젝트 구조, 작업 및 공유를 위해 선택되지 않은 필드</p></li>
</ul></td>
</tr>
</tbody>
</table>

## Beta에서 사용 가능한 기능

Beta 프로그램의 첫 번째 단계에서는 두 인스턴스를 연결하고 작업을 시작할 수 있습니다.

|                                   |                                                                                                                                                                                                                                                                                                                                       |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **기능** | **기능** |
| **연결된 조직** | 두 조직 간에 두 Workfront 인스턴스를 연결합니다. 베타 기간 동안 Adobe에서 연결을 구성합니다. 셀프 서비스 설정은 현재 개발 중입니다. |
| **요청 양식** | 클라이언트 회사는 요청 양식을 만들어 게시하고 양식의 공유 설정에서 공급자 회사와 공유합니다. |
| **AI 지원 요청 접수** | 클라이언트의 요청자는 AI 양식 작성 기능을 사용하여 긴 양식을 작성하는 대신 프롬프트를 입력하고 파일을 첨부할 수 있습니다. 시스템은 해당 콘텐츠를 양식 필드에 매핑하고 검토를 위해 매핑을 표시합니다. 요청자가 결과를 승인하고 양식을 제출합니다. |
| **미러된 요청** | 제출된 요청은 사용자 정의 필드 값을 포함하여 읽기 전용 사본으로 공급자 회사의 요청 영역에 표시됩니다. |
| **프로젝트 간 전환 요청** | 제공자는 요청을 프로젝트로 전환하고 포트폴리오, 프로그램 및 템플릿을 선택하여 작업을 시작합니다. 공급자 인스턴스의 새 개체가 클라이언트의 원래 요청에 다시 연결됩니다. 제공자 측의 실제 업무 내용은 요청 기업에게 보이지 않는다. |
| **양방향 댓글** | 청탁에 대한 코멘트가 양측에 보이고 거의 즉시 도착하기 때문에 양측이 한 곳에서 합의를 향해 노력할 수 있다. |
| **수락 요청** | 양측이 동의하면 제공자는 요청을 수락하고 고객은 요청이 수락된 것으로 볼 수 있습니다. |
| **AI 초안 상태 업데이트** | 요청자가 댓글에 상태를 묻자 제공자는 AI 명령을 활용해 빠르고 일관성 있게 초안 답글을 생성할 수 있다. <br> 초안에는 계획된 완료 일자, 조건 및 계획된 시간에 대해 기록된 시간과 같은 요청에 연결된 오브젝트의 정보가 포함됩니다. <br> 현장 수출이 아니라 가장 중요한 정보를 정리한 것이다. 개인에게 클라이언트에 응답을 보내기 전에 검토하고 편집합니다. |

## 전체 워크플로

이 섹션에서는 존경하는 조직의 Workfront 인스턴스가 연결된 후 이 통합에 관여하는 두 당사자의 워크플로우에 대해 설명합니다.

클라이언트 및 공급자 워크플로를 예로 사용하고 있습니다.

### 클라이언트의 워크플로

클라이언트의 조직에서 요청자는 다음과 같은 작업을 수행할 수 있습니다.

1. 요청 양식을 만들거나 관리자에게 요청하여 게시하고 연결된 공급자의 조직과 공유합니다.

2. 요청 영역에서 게시된 양식을 열고 프롬프트를 입력하고 파일을 첨부합니다.

3. 콘텐츠가 양식 필드에 매핑되고, 동의하고, 제출하는 방법을 검토합니다.

### 공급자의 워크플로

공급자 조직의 작업 관리자는 다음 작업을 수행합니다.

1. 요청 영역에서 요청을 읽기 전용 사본으로 받습니다.

2. 양쪽이 일치할 때까지 의견을 통해 요청을 논의한 다음 수락합니다.

3. 필요한 경우 요청을 프로젝트로 전환하고 포트폴리오, 프로그램 및 템플릿을 선택합니다.

4. 클라이언트의 요청에 다시 미러링되는 프로젝트 필드를 선택합니다.

5. 주석에서 상태 질문에 답변하거나 초안 상태 업데이트를 생성하고 검토한 다음 요청에 게시합니다. 클라이언트의 원래 요청에도 표시됩니다.

   이 시점에서부터 공급자 측의 요청은 클라이언트의 원래 요청을 복제하는 역할을 하므로 댓글과 합의된 데이터는 계속 동기화됩니다.

## 보안 및 관리

각 조직의 데이터를 안전하게 보호하는 것은 핵심 설계 요구 사항입니다.

Beta가 설정하고자 하는 기준 중 하나는 IT 및 보안 팀이 인스턴스 간의 연결을 얼마나 쉽게 승인하고 관리할 수 있는가입니다.

다음은 연결된 조직 워크플로의 이점입니다.

* **인스턴스 간 액세스 없음**: 인스턴스에 파트너 조직의 사용자가 필요하지 않으므로 게스트 로그인과 추가 라이선스가 없습니다.

* **필요한 최소 공유**: 동기화에 대해 구성된 데이터만 공유됩니다. 다른 모든 인스턴스는 원래 인스턴스에 유지됩니다.

* **독립 제어**: 각 조직은 자체 사용자, 권한 및 워크플로를 유지합니다.

* **팀 수준 범위**: 요청은 기존 Workfront 액세스 제어를 사용하여 해당 고객과 작업하도록 설정된 에이전시 팀에만 도달하기 위한 것입니다.

## 로드맵 전망

아래 단계에서는 현재 개발 및 릴리스 계획을 설명합니다. Beta 단계에서 학습한 내용에 따라 시퀀싱이 변경될 수 있습니다. 이후 단계는 약정이 아닙니다.

<table>
<tbody>
<tr class="odd">
<td><strong>단계</strong></td>
<td><strong>중점 및 계획된 기능</strong></td>
<td><strong>상태</strong></td>
</tr>
<tr class="even">
<td><strong>단계 1</strong></td>
<td>인스턴스 연결 및 시작 작업: 요청 양식, AI 지원 접수, 미러링된 요청, 프로젝트 전환, 주석 및 상태 초안 작성.</td>
<td>베타</td>
</tr>
<tr class="odd">
<td><strong>단계 2</strong></td>
<td><ul>
<li><p>프레임 및 통합 검토 및 승인 경험을 사용하여 검토 및 승인</p></li>
<li><p>보류 중인 검토는 관련자가 근무하는 곳마다 Workfront 또는 프레임에 표시됩니다</p></li>
<li><p>주석은 작업 파일에 연결되어 있으므로 크리에이티브 팀이 한 곳에서 피드백을 볼 수 있습니다</p></li>
</ul></td>
<td>계획됨</td>
</tr>
<tr class="even">
<td><strong>단계 3</strong></td>
<td><ul>
<li><p>요청 외에 작업 기반 작업 할당</p></li>
<li><p>공유 또는 비공유 필드를 통해 제공되는 보다 자동화된 상태</p></li>
<li><p>브리핑 도중 정의된 메타데이터가 최종 승인된 에셋에 상속된 새 결과물 객체 유형</p></li>
<li><p>승인된 최종 에셋을 브랜드의 AEM에 직접 전달하여 수동 메타데이터 입력 감소</p></li>
</ul></td>
<td>계획됨</td>
</tr>
<tr class="odd">
<td><strong>4단계</strong></td>
<td><ul>
<li><p>파트너 간 컨텍스트 공유</p></li>
<li><p>검토 전 Adobe Brand Intelligence <!--by the agency--> 사용(팀에서 액세스 제어)</p></li>
<li><p>추정과 같은 컨텍스트 기반 기능</p></li>
</ul></td>
<td>장기간</td>
</tr>
</tbody>
</table>

## Beta에 참여

Adobe Beta 프로그램 관리자에게 문의하여 Beta에 참여하십시오.

### 참가자에게 요구하는 사항

* 주간 피드백 호출에 참여하십시오.

* 일주일에 한 시간 정도 시간을 할애하여 스스로 실습 테스트를 하도록 한다. 호출에 대한 실시간 작업 세션은 옵션입니다.

* 가능한 경우 모임에 대한 파트너의 관점을 모두 가져와라.

* 연결할 Workfront 환경을 식별하고, 연결을 확인할 수 있도록 적은 수의 Adobe 엔지니어를 위한 관리자 계정을 프로비저닝합니다.

### 배우고 싶은 사항

* 개체를 미러링하고 선택한 데이터만 동기화하는 것이 올바른 공유 모델입니까? 양쪽 모두 융통성이 있나요?

* 단계 순서 지정이 적절합니까? 또는 이후 기능이 더 빨리 와야 합니까?

* 협업에서 누락된 터치포인트는 무엇입니까?

* 두 인스턴스 간에 필드 이름 지정 및 매핑은 어떻게 작동해야 합니까?

  이제 양식과 요청은 클라이언트가 소유하며 공급자는 클라이언트의 필드 이름이 있는 읽기 전용으로 표시됩니다.

* IT에서 연결을 승인하고 관리하는 데 필요한 사항은 무엇입니까?




<!--

Original pdf from team:

**ADOBE WORKFRONT | BETA PROGRAM**

**Agency Brand Connectors**

Product overview for beta participants

# **Overview**

Agency Brand Connectors lets a brand and its agency collaborate on work when both organizations run Adobe Workfront. Each side keeps working in its own Workfront instance, with its own users, permissions, and workflows. Work objects are mirrored between the two instances, and only the data both sides agree to share is synchronized.

The result is a shared view of requests, status, and decisions without guest logins, duplicate licenses, or long email threads.

# **The challenge this addresses**

When a brand and an agency are both invested in Workfront, they should be able to work together without either one paying twice or moving into the other's system. Today the collaboration usually looks like this:

  - Requests and briefs travel through email threads that are hard to follow.

  - Handoffs are manual, with little auditability.

  - Working inside a partner's system means guest logins, extra licenses, or both.

  - Multiple copies of files circulate, and no one is sure which is the source of truth.

  - Status is hard to see, so producers and account managers spend time building decks and scheduling update meetings.

# **How it works: the sharing model**

Neither organization accesses an object in the other's instance. Instead, an object such as a request is duplicated and published into the partner's instance, and only the metadata configured for sync is kept up to date between the two copies. Each side manages its own users, permissions, and workflows downstream of that object.

The guiding principle is to share the minimum needed to get the work done, and to keep everything else confidential.

<table>
<tbody>
<tr class="odd">
<td><strong>What is shared</strong></td>
<td><strong>What stays private</strong></td>
</tr>
<tr class="even">
<td><ul>
<li><p>Briefs and request details</p></li>
<li><p>Agreed deadlines and milestones</p></li>
<li><p>Review comments</p></li>
<li><p>Approval decisions</p></li>
<li><p>Final approved assets</p></li>
</ul></td>
<td><ul>
<li><p>Relationships with other clients or other agencies</p></li>
<li><p>Financials, rates, and what is charged to the client</p></li>
<li><p>Resource planning and capacity</p></li>
<li><p>Internal project structure, tasks, and any fields not selected for sharing</p></li>
</ul></td>
</tr>
</tbody>
</table>

# **Features available in the beta**

The first phase of the beta covers connecting two instances and kicking off work.

|                                   |                                                                                                                                                                                                                                                                                                                                       |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Feature**                       | **What it does**                                                                                                                                                                                                                                                                                                                      |
| **Connected organizations**       | Links a brand instance and an agency instance. During the beta, Adobe configures the connection. A self-serve setup is being worked on.                                                                                                                                                                                               |
| **Request forms**                 | The brand creates a request form, publishes it, and shares it with a connected organization from the form's Share settings.                                                                                                                                                                                                           |
| **AI-assisted request intake**    | The requester types a prompt and attaches files instead of filling out a long form. The system maps that content to the form fields and shows the mapping for review. The requester accepts the result and submits. This uses Workfront's existing form-filling technology.                                                           |
| **Mirrored requests**             | The submitted request appears in the agency's request area as a read-only copy, including custom field values.                                                                                                                                                                                                                        |
| **Request-to-project conversion** | The agency converts the request into a project and selects the portfolio, program, and template. The new object is linked back to the request. Downstream work on the agency side is not visible to the brand.                                                                                                                        |
| **Two-way comments**              | Comments on the request are visible on both sides and arrive almost immediately, so both parties can work toward agreement in one place.                                                                                                                                                                                              |
| **Request acceptance**            | Once both sides agree, the agency accepts the request and the brand sees that it has been accepted.                                                                                                                                                                                                                                   |
| **AI-drafted status updates**     | When a brand asks for status in a comment, the agency can use a slash command to generate a draft reply. The draft draws on connected objects, such as planned completion date, condition, and hours logged against hours planned. It is a summary, not a field-by-field export, and a person reviews and edits it before publishing. |

# **End-to-end workflow**

## **Brand side**

1.  Create a request form, publish it, and share it with the connected agency.

2.  Open the published form, enter a prompt, and attach any files.

3.  Review how the content maps to the form fields, accept, and submit.

## **Agency side**

1.  Receive the request in the request area as a read-only copy.

2.  Discuss the request through comments until both sides are aligned, then accept it.

3.  Convert the request into a project, choosing the portfolio, program, and template.

4.  Choose which project data is mirrored back to the brand.

5.  Answer status questions in comments, or generate a draft status update, review it, and publish.

From that point on, the request on the agency side acts as a replica of the request on the brand side, so comments and agreed data stay in step.

# **Security and governance**

Keeping each organization's data protected is a core design requirement, and one of the baselines we want the beta to establish is how easily IT and security teams can approve and administer a connection between instances.

  - **No cross-instance access.** No users from the partner organization are needed in your instance, so there are no guest logins and no additional licenses.

  - **Minimum necessary sharing.** Only the data configured for sync is shared. Everything else stays in the originating instance.

  - **Independent controls.** Each organization keeps its own users, permissions, and workflows.

  - **Team-level scoping.** Requests are intended to reach only the agency teams set up to work on that brand, using existing Workfront access controls.

# **Roadmap**

The phases below describe our current plan. Sequencing may change based on what we learn in the beta, and later phases are not commitments.

<table>
<tbody>
<tr class="odd">
<td><strong>Phase</strong></td>
<td><strong>Focus and planned capabilities</strong></td>
<td><strong>Status</strong></td>
</tr>
<tr class="even">
<td><strong>Phase 1</strong></td>
<td>Connect instances and kick off work: request forms, AI-assisted intake, mirrored requests, project conversion, comments, and status drafting.</td>
<td>In beta</td>
</tr>
<tr class="odd">
<td><strong>Phase 2</strong></td>
<td><ul>
<li><p>Review and approval using Frame and the unified review and approval experience</p></li>
<li><p>Pending reviews appear in Workfront or Frame, wherever the stakeholder works</p></li>
<li><p>Annotations stay tied to the working file so creative teams see feedback in one place</p></li>
</ul></td>
<td>Planned, next</td>
</tr>
<tr class="even">
<td><strong>Phase 3</strong></td>
<td><ul>
<li><p>Task-based work assignment in addition to requests</p></li>
<li><p>More automated status, informed by shared or unshared fields</p></li>
<li><p>A new deliverable object type, with metadata defined during briefing and inherited by the final approved asset</p></li>
<li><p>Direct delivery of approved final assets into the brand's AEM, reducing manual metadata entry</p></li>
</ul></td>
<td>Planned, next</td>
</tr>
<tr class="odd">
<td><strong>Phase 4</strong></td>
<td><ul>
<li><p>Shared context between brand and agency</p></li>
<li><p>Use of Adobe Brand Intelligence by the agency before review, with access controlled by team</p></li>
<li><p>Context-informed capabilities such as estimating</p></li>
</ul></td>
<td>Longer term</td>
</tr>
</tbody>
</table>

# **Participating in the beta**

## **What we ask of participants**

  - Join a weekly feedback call.

  - Set aside about one hour per week for hands-on testing. Live working sessions on the call are an option if time is tight.

  - Bring both the brand and the agency perspective where possible.

  - Identify the Workfront environments to connect, and provision admin accounts for a small number of Adobe engineers so they can validate the connection.

## **What we want to learn**

  - Is mirroring an object and syncing only selected data the right sharing model, and is it flexible enough for each side?

  - Is the phase sequencing right, or should a later capability come sooner?

  - What touchpoints are missing from the collaboration?

  - How should field naming and mapping work between brand and agency instances? Today, the form and request are owned by the brand, and the agency sees them read-only with the brand's field names.

  - What does IT need to approve and administer a connection?

The beta runs through the end of the year. For questions or blockers, contact your Adobe beta program manager.


-->