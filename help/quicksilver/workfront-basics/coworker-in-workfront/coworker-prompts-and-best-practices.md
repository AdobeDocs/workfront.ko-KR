---
title: CX Coworker 프롬프트 및 Best Practice
content-type: reference
description: Workfront에서 Coworker를 사용하기 위한 모범 사례에 대해 알아보고 프롬프트 예제 목록을 볼 수 있습니다.
author: Becky
feature: Get Started with Workfront
source-git-commit: 01de260893e5bbf7a228479df2f3fc6a1337d31d
workflow-type: tm+mt
source-wordcount: '2247'
ht-degree: 1%

---

# CX Coworker 프롬프트 및 Best Practice

&lt;!—사용하지 않음—MCP 예제 프롬프트 문서에 대신 링크합니다. MCP에 대한 최신 릴리스로 업데이트되었는지 확인하십시오—>

>[!IMPORTANT]
>
>CX Coworker 는 현재 의료 서비스, 금융 기관 또는 중요한 데이터가 있는 기타 업계 조직에서 사용할 수 없습니다. 이러한 조직에서는 AI Assistant를 사용할 수 있습니다. 자세한 내용은 [AI Assistant 개요](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)를 참조하십시오.

CX Coworker를 사용하면 자연어를 사용하여 Workfront Workflow 및 Workfront Planning과 상호 작용할 수 있습니다.

동료는 Adobe Experience Cloud Agent Orchestrator의 일부입니다.

Agent Orchestrator에 대한 자세한 내용은 [Adobe Experience Platform Agent Orchestrator](https://experienceleague.adobe.com/ko/docs/experience-cloud-ai/experience-cloud-ai/agents/agent-orchestrator)을 참조하세요.

## 액세스 요구 사항

<!--Add info about how to qualify for agent orchestrator stuff-->

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>Select, Prime 또는 Ultimate </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>표준 또는 라이트</p>
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td><p>기본 기술 이외의 기능을 사용하려면 조직에서 Adobe Agent Orchestrator을 구매해야 합니다.</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td><p>Coworker를 통해 모든 오브젝트와 상호 작용할 수 있는 적절한 권한이 있어야 합니다.</p> <p>예를 들어 Coworker를 통해 프로젝트에 대한 정보를 받으려면 해당 프로젝트에 대한 보기 권한 이상이 있어야 합니다.</p></td>
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

* Workfront 관리자가 조직에 대해 AI Assistant를 활성화해야 합니다.

  자세한 내용은 AI Assistant 개요 문서의 [AI Assistant에 대한 필수 구성 요소](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)를 참조하십시오.
* Workfront 관리자가 귀하의 액세스 수준에 대해 AI Assistant를 활성화해야 합니다.

  자세한 내용은 [AI Assistant 사용 또는 사용 안 함](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)을 참조하십시오.

## 고려 사항

CX Coworker 를 사용할 때는 다음 제한 사항을 고려하십시오.

### 가역성

일부 작업은 되돌릴 수 있습니다. 예를 들어, 개체가 만들어지면 그 만들기를 되돌릴 수 있습니다.

그러나 개체 삭제와 같은 일부 작업은 **되돌릴 수 없습니다**. Coworker를 통해 데이터에 대한 작업을 수행할 때는 이 점을 염두에 두는 것이 좋습니다.

### 데이터 / 객체 범위 제한

* 사용자 정의 필드에 대한 쿼리 및 보고는 초기 단계이며, 일부 기술(예: API 기반 쿼리 도우미)은 아직 집계 및 필터링을 위해 임의의 사용자 정의 필드를 처리하지 않습니다.

### 상호 작용/UX 제한 사항

* CX Coworker는 현재 개별 사용자의 스타일 또는 환경 설정을 장기간 &quot;학습&quot;하지 않습니다. 모든 채팅은 현재 대화와 제품 지식만 사용합니다.
* 대화 컨텍스트는 단일 채팅 세션 내에 유지됩니다. 새 페이지를 열거나 도우미를 닫으면 대화 내용이 재설정됩니다.
* 승인 절차가 Confluence 또는 SharePoint과 같은 외부 애플리케이션에 있고 URL 필드를 통해서만 연결되는 경우, Coworker는 현재 해당 페이지를 가져오지 않고 해당 페이지를 합리화합니다.

### 데이터 스토리지 / 고객 관리 키

* CX Coworker는 Adobe Experience Platform Agent Orchestrator의 일부이므로 Coworker와의 상호 작용 데이터는 Workfront이 아닌 Adobe Experience Platform에 저장됩니다. 따라서 이 데이터는 Workfront BYOK(Customer Managed Keys) 계약의 적용을 받지 않습니다.

## 기본 AI 기술 사용

>[!IMPORTANT]
>
>이러한 일반 사용 기능은 조직에서 파일에 대해 서명된 Adobe AI 계약을 보유한 모든 사용자가 사용할 수 있습니다.

이러한 일반 사용 기술에 대한 모범 사례와 프롬프트는 [AI Assistant 프롬프트 및 모범 사례](/help/quicksilver/workfront-basics/ai-assistant/ai-prompts-best-practices.md)를 참조하십시오.

<!--Follow up with Oznur-->

### 제품 지식

CX 동료는 Workfront 설명서에서 가져온 지침이나 참조 정보를 제공할 수 있습니다.

Workfront 설명서에서 정보를 가져오는 방법에 대한 자세한 내용은 [AI Assistant에서 도움 받기](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md)를 참조하십시오.

예: 작업 기간 유형은 어떻게 변경합니까?

### 프로젝트, 작업 및 문제 요약

CX 동료는 Workfront에 업로드된 프로젝트, 작업 또는 문제<!--, or documents-->를 요약할 수 있습니다.

프로젝트, 작업 및 문제 요약에 대한 자세한 내용은 [AI Assistant를 사용하여 요약](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md)을 참조하십시오.

예: Fall Campaign 2026이라는 프로젝트를 요약합니다.

<!--

### Locate work items

CX Coworker can find work items like projects, tasks, and issues

Example: Find all tasks assigned to me that are due this week.

For more information on using AI Assistant to locate project, tasks, and issues, see [se AI Assistant to work with projects, tasks, and issues](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

-->

<!--

Follow up on this to see if it's going away or what

### Catch Me Up 

Catch Me Up summarizes updates, uploaded documents, and other notable changes that have about your projects that have occurred in the last 24 hours, 3 days, or 7 days.  

For more information on Catch me up, see [Catch up on work in Priorities](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).

-->

<!--

### Smart filters

You can use natural language filters in Priorities to replace status, pre-built views to help you filter your work.

For more information on using Smart Filters, see [Filter your work with Smart filters](/help/quicksilver/workfront-basics/priorities/filter-group-work-priorities.md) in the article Filter and group your work with Priorities.

-->

## Workfront의 CX 동료

* [프로젝트, 작업 및 문제 정보](#project-task-and-issue-information)
* [프로젝트 및 작업 관리](#project-and-work-management)
* [컨텐츠 및 승인](#content-and-approvals)

### 프로젝트, 작업 및 문제 정보

CX 동료는 요약 및 프로젝트 상태를 포함하여 프로젝트, 작업 및 문제에 대한 정보를 제공할 수 있습니다.

다음 영역에서 문서 및 자산 승인을 위한 프롬프트 예를 참조하십시오.

* [프로젝트, 작업 또는 문제에 대한 정보 찾기](#find-information-about-projects-tasks-or-issues)
* [프로젝트, 작업 또는 문제 요약](#summarize-projects-tasks-or-issues)
* [프로젝트, 프로그램 또는 포트폴리오의 프로젝트 상태 표시](#show-project-health-for-projects-programs-or-portfolios) <!--remove any mention of project health-->

#### 프로젝트, 작업 또는 문제에 대한 정보 찾기

* 프로젝트
  * 브랜드 마케팅 팀에 대한 모든 활성 프로젝트 표시
  * 에는 &quot;디지털&quot; 범주 아래에 4분기 캠페인 포트폴리오의 프로젝트 목록이 필요합니다.
  * Creative Services 회사의 프로젝트 관리자인 사용자가 관리하는 프로젝트를 표시합니다.
* 작업
  * 조앤 해리스의 모든 임무를 맡겨주세요
  * UX 팀에 할당된 &quot;디자인&quot; 범주의 작업을 표시합니다.
  * 휴가 프로모션 프로그램에서 카피라이터에게 배정된 작업이 필요합니다.
* 문제
  * &quot;기술&quot; 범주 아래의 &quot;웹 사이트 재디자인&quot; 프로젝트의 모든 문제를 표시합니다.
  * QA 그룹에서 보고한 해결되지 않은 모든 문제를 가져옵니다.
  * 글로벌 테크 회사의 개발자에게 할당된 이슈가 필요합니다.

#### 프로젝트, 작업 또는 문제 요약

* &quot;이 프로젝트 요약&quot;
* &quot;이 프로젝트의 마지막 주 요약&quot;

#### 프로젝트, 프로그램 또는 포트폴리오에 대한 프로젝트 상태 표시

>[!NOTE]
>
>이 기능을 사용하려면 조직이 프로젝트 상태 Beta에 등록되어 있어야 합니다.

* &quot;내 활성 프로젝트의 상태 표시&quot;
* &quot;이 프로그램의 상태 표시&quot;

### 프로젝트 및 작업 관리

CX Coworker를 사용하면 작업 및 할당과 같은 프로젝트를 만들고 관리할 수 있습니다.

다음 영역에서 프로젝트 및 작업 관리에 대한 프롬프트 예를 참조하십시오.

* [프로젝트 만들기, 업데이트 또는 삭제](#create-update-or-delete-projects)
* [사용자 프롬프트에 따라 올바른 프로젝트 템플릿 식별](#identify-the-right-project-template-based-on-user-prompt)
* [프로젝트에서 작업 추가, 편집 또는 사용자 지정](#add-edit-or-customize-tasks-in-a-project)
  <!--* [Create, update, or delete assignments](#create-update-or-delete-assignments)-->
  <!--* [Recommend best matching user assignments for the task based on users' job role and availability](#recommend-best-matching-user-assignments-for-the-task-based-on-users-job-role-and-availability)-->

#### 프로젝트 만들기, 업데이트 또는 삭제

처음부터 또는 템플릿에서 프로젝트를 만들고, 프로젝트를 업데이트하고, 삭제할 수 있습니다.

* 3월 10일에 시작하여 4월 30일에 끝나는 Q2 Innovation Sandbox라는 빈 프로젝트를 만듭니다. 나를 소유자로 설정하십시오.
* 통합 마케팅 캠페인 템플릿을 사용하여 Lucent AI Launch - NA라는 프로젝트를 만듭니다. 2월 5일부터 시작하여 현재로 설정합니다.
* 3월 1일부터 6월 15일까지 웹 사이트 재디자인 - EMEA라는 프로젝트를 만듭니다. EMEA Marketing이 소유하고 마케팅 담당 부사장이 후원하는 이 프로그램은 25만 달러(약 1,200시간 계획)로 예산을 책정했으며 전환율 향상을 목표로 유럽에 중점을 두고 진행되었습니다.
* Lucent AI Launch - NA 프로젝트의 경우 2분기로 이동하고, 목표를 무료 체험판으로 변경하고, 4월 중순까지 마감을 추진하고, 예산을 15만 달러로 늘리고, 긴급으로 표시합니다.
* 2분기에 완료되고 높거나 긴급한 우선 순위이며 가장 빠른 종료 날짜별로 정렬된 현재 마케팅 프로젝트를 모두 표시하십시오.

#### 작업 추가 또는 편집

프로젝트에서 작업을 추가하거나 편집할 수 있으며, 프로젝트를 생성하는 데 사용하는 템플릿의 작업 목록을 사용자 지정할 수 있습니다.

* 랜딩 페이지 QA라는 새 작업을 프로젝트에 추가하고 4월 22일부터 4월 26일까지 예약합니다.
* 디자인 검토 작업을 업데이트하여 4월 18일에 완료하고 크리에이티브 팀에 할당합니다.
* 프로젝트에서 자산 인쇄 프로덕션 작업을 제거합니다.
* 완료되지 않았고 4월 1일부터 4월 30일 사이에 시작하기로 예정된 이 프로젝트의 모든 작업을 표시합니다.
* 법적 승인을 Campaign Launch 작업의 전임 작업으로 설정합니다.
* 4월 15일부터 4월 16일까지 예약된 최종 복사 폴리쉬라는 새 작업을 추가하고, 복사 검토 작업을 4월 10일로 이동하고, 추가 검토 라운드 작업을 제거하고, 최종 복사 폴리쉬를 이메일 빌드의 전임 작업으로 설정합니다.
* 프로젝트 생성 흐름 동안 프로젝트 아래 작업이 되는 것이 이상적인 결과물에 대한 정보를 최대한 제공해 보십시오.

#### 할당 만들기, 업데이트 또는 삭제

사용자 또는 작업 역할 할당을 생성, 갱신 및 삭제할 수 있습니다.

* &#39;제품 출시를 위한 랜딩 페이지 디자인&#39; 프로젝트의 경우, 현재 할당되지 않은 모든 작업에 적절한 작업 역할과 권장 계획 시간을 식별합니다.
* &#39;캠페인 사이트에 대한 GA4 추적 구현&#39;, &#39;전환 이벤트 설정&#39; 및 &#39;분석 데이터 유효성 검사&#39;를 포함하여 할당 해제된 작업이 여러 개 있습니다. 적합한 작업 역할과 각각에 대한 예상 시간을 제안할 수 있습니까?
* 크리에이티브 작업 &quot;EMEA 디스플레이 광고에 대한 3개의 배너 변형 만들기&quot;, &quot;개정 적용&quot; 및 &quot;최종 자산 내보내기&quot;에 대해 최상의 작업 역할을 할당하고 각 작업에 필요한 노력을 예측합니다.
* &#39;Q2 제품 출시&#39;, &#39;웹 사이트 재디자인 - EMEA&#39; 및 &#39;유료 미디어 캠페인 - NA&#39; 프로젝트에서 할당되지 않은 모든 작업을 식별하고 각각에 대한 권장 계획 시간을 사용하여 적절한 작업 역할을 할당합니다.

<!--

#### Identify the right project template based on user prompt

* We're launching a new product feature with a landing page, emails, paid ads, and social posts. Which project template should we use?
* Create a project for a global marketing campaign with multiple channels and regional rollouts. (should suggest a template if provided more info)
* For Website Redesign – EMEA project, recommend and attach the correct project template.

-->

<!--

#### Recommend best matching user assignments for the task based on users' job role and availability

* Who is the best available user to assign to 'Design Landing Page Hero', considering who still has capacity today?
* Who should be assigned to 'Backend API integration for campaign reporting', considering engineering role alignment?
* For all unassigned tasks in this project, recommend the best users based on job role match and daily availability.
* Recommend users for the tasks 'QA testing for website launch' and 'Content review', prioritizing users whose job roles match and who are not over-allocated today.

-->

### 컨텐츠 및 승인

CX Coworker 는 Workfront에서 문서 및 에셋 승인을 관리하는 데 도움이 됩니다.

문서 및 자산 승인 작업 시 다음 사항을 고려하십시오.

* Coworker에서 이 기능을 사용하려면 먼저 조직에 대해 컨텐츠 승인을 활성화해야 합니다.
* AI는 인간을 대신하여 승인하거나 거부할 수 없다. Workfront AI 검토자를 제외하고 의사 결정은 사용자에 의존합니다.

  Workfront AI 검토자에 대한 자세한 내용은 [Workfront AI 검토자 시작](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)을 참조하십시오.
* 이 기능은 Workfront 내에 있으며 외부 도구 또는 문서 공급자와 상호 작용하는 데 사용할 수 없습니다.
* 최상의 경험을 위해 이 기능을 통합 승인 경험에 사용하십시오.

  통합 승인에 대한 자세한 내용은 [통합 승인 개요](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)를 참조하십시오.

다음 영역에서 문서 및 자산 승인을 위한 프롬프트 예를 참조하십시오.

* [승인 참가자 추가 또는 제거](#add-or-remove-approval-participants)
* [이해 당사자에게 검토 대기 중인 단일 에셋에 대해 알림](#remind-stakeholders-of-a-single-asset-waiting-for-review)
* [단일 자산에 대한 승인 템플릿을 추가, 업데이트 또는 적용](#add-update-or-apply-approval-templates-for-a-single-asset)

#### 승인 참가자 추가 또는 제거

* 현재 문서에서 Sarah Chen 및 Miguel Alvarez를 승인자로 추가합니다.
* 이 승인에서 Jennifer Otto를 제거합니다.
* 승인 결정을 내리지 않은 모든 사용자를 제거합니다.
* spring-campaign.pdf에 &quot;최종 검토&quot;라는 새 단계를 추가합니다.
* Winter-campaign.pdf의 두 번째 단계에서 승인자로 Mark와 Sarah를, 검토자로 Phil을 추가합니다.
* winter-campaign.pdf의 경우 첫 번째 단계에 오늘 오후 5시로 기한을 지정하고 최종 검토에 내일 오후 5시로 기한을 지정하십시오
* 목요일 오후 5시로 마감되는 fall-campaign.png에 최종 점검 단계를 추가하고 승인자로 Jim과 Pam을 포함하고 검토자로 Oscar를 포함하십시오.
* Mark Jones를 fall-campaign.png에 검토자로 첫 번째 및 마지막 단계에 추가합니다.
* 3단계, 1디자인 2 카피라이팅 및 3리걸 (Legal)로 fall-campaign.png에 대해 만들어진 다단계 승인을 받겠습니다. 각 단계마다 필요한 결정은 단 한 가지뿐입니다. 마이크, 샐리, 제인은 디자인에, 크리스, 리차드, 마크는 카피라이팅에, 필, 톰, 사라는 리갈에 추가합니다.

#### 이해 당사자에게 검토 대기 중인 단일 에셋에 대해 알림

* 응답하지 않은 &#39;봄 캠페인 비디오&#39; 에셋의 승인자에게 미리 알림을 보냅니다.
* 이 에셋 &#39;봄 캠페인 비디오&#39;를 승인하지 않은 모든 사용자에게 알립니다.
* 자산 &#39;브랜드 가이드라인 PDF&#39;에 대해 아직 결정을 내리지 않은 사람? 상기시켜줘

#### 단일 자산에 대한 승인 템플릿을 추가, 업데이트 또는 적용

* &#39;봄 캠페인 비디오&#39;라는 이름의 자산에 &#39;마케팅 시작&#39; 승인 템플릿을 적용합니다.
* Creative 검토, 법적 승인 및 최종 승인의 3단계로 구성된 새 승인 템플릿을 만듭니다.
* 1단계에 줄리아 산토스와 쉐인 베이커를 추가하세요.
* &#39;제품 출시&#39; 템플릿을 편집하여 Elizabeth Peterson을 최종 승인 단계에 추가합니다.
* 한 단계로 &#39;긴급 검토&#39;라는 템플릿을 만들어 올리비아 김에게 할당합니다.
* Rick Kuvec를 제거하고 Karen Sterling을 2단계에 추가하여 &#39;Creative 검토&#39; 템플릿을 업데이트합니다.


## Workfront Planning의 CX Coworker

### Planning 레코드 작업

* [레코드 만들기, 삭제, 복제 또는 복원](#create-delete-duplicate-or-restore-records)
* [다른 레코드에 레코드 연결](#link-records-to-other-records)
* [필드를 레코드에 편집, 업데이트 또는 추가](#edit-update-or-append-a-field-to-a-record)
* [레코드 변경 내역 액세스](#access-record-change-history)

#### 레코드 만들기, 삭제, 복제 또는 복원

* Summer Sale 2026이라는 새로운 캠페인 레코드 만들기
* Widget Pro라는 이름과 $299의 가격으로 새로운 제품 레코드를 추가하십시오.
* John Smith에 대한 새 리드 레코드를 만들 수 있습니까?
* 이전 프로모션이라는 캠페인 레코드 삭제
* 방금 만든 테스트 레코드 제거
* 레코드 ID Rc123abc456을 삭제할 수 있습니까?
* 1분기 캠페인 레코드 복제
* 새 캠페인을 만들기 위해 이 캠페인을 복사할 수 있습니까?
* 휴일 프로모션 캠페인의 사본 만들기
* 내가 실수로 삭제한 캠페인 복원
* 당신은 삭제 된 프로젝트 레코드를 복구 할 수 있습니까?
* 실수로 레코드를 삭제했는데, 복원 가능한가요?

#### 다른 레코드에 레코드 연결

* 여름 캠페인 기록을 2분기 이니셔티브에 연결
* 이 제품을 관련 마케팅 캠페인에 연결할 수 있습니까?
* 이 세 개의 가망 고객을 엔터프라이즈 계정 레코드와 연결해야 합니다.

#### 필드를 레코드에 편집, 업데이트 또는 추가

* 여름 캠페인의 예산 필드를 $75,000로 업데이트
* 이 프로젝트 레코드의 상태를 완료됨으로 변경할 수 있습니까?
* 이 이니셔티브의 팀원 필드에 John Doe 추가

#### 레코드 변경 내역 액세스

* 여름 캠페인 레코드에 대한 변경 내역 표시
* 이 프로젝트를 수정한 사람과 변경한 내용을 표시할 수 있습니까?
* 지난 주에 이 레코드에 대한 모든 업데이트를 확인해야 합니다.

### Workfront Planning에서 시스템 Designer 사용

* [작업 공간 만들기 및 구성](#create-and-configure-workspaces)
* [레코드 유형 정의](#define-record-types)
* [디자인 필드 및 공식 필드](#design-fields-and-formula-fields)
* [사용자 정의 보기 작성](#build-custom-views)


#### 작업 공간 만들기 및 구성

* 마케팅 캠페인 2026이라는 새 계획 작업 영역 만들기
* 제품 계획 작업 영역을 업데이트하여 색상을 파란색으로 변경하고 설명을 추가합니다.
* 액세스 권한이 있는 모든 Planning 작업 영역 표시

#### 레코드 유형 정의

* 내 Planning 작업 영역에서 캠페인이라는 새 레코드 유형 만들기
* 이니셔티브 레코드 유형을 업데이트하여 아이콘 및 설명 변경
* 내 Marketing Planning 작업 영역의 모든 레코드 유형 표시

#### 디자인 필드 및 공식 필드

* 통화 유형으로 내 계획 캠페인 레코드 유형에 예산 필드 추가
* 캠페인 종료일까지 남은 일수를 계산하는 Planning의 공식 필드를 생성합니다.
* 내 Planning 작업 공간에서 우선 순위 필드를 업데이트하여 드롭다운 옵션을 더 추가합니다.

#### 사용자 정의 보기 작성

* Planning에서 타임라인 보기를 만들어 시작 및 종료 날짜별로 내 캠페인 일정 보기
* 활성 상태만 필터링하는 새 테이블 보기를 내 Planning 이니셔티브에 추가
* 내 Planning 활성 캠페인 보기를 복제하고 정렬을 수정합니다.
