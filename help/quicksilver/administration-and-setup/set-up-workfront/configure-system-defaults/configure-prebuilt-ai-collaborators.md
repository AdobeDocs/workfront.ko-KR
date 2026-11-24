---
user-type: administrator
product-area: system-administration;setup
title: 사전 빌드된 AI 공동 작업자 구성
description: Adobe Workfront 관리자는 Intake 코디네이터와 같은 Adobe에서 사전 빌드된 AI 공동 작업자를 사용자가 작업 및 문제에 할당할 수 있는 작업 에이전트로 구성할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: 71c1855166c2f950509cc8b7dc63792eabb6de16
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 4%
---
# 사전 빌드된 AI 공동 작업자 구성

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 미리보기에 릴리스된 후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 매월 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

## 개요

사전 빌드된 AI 공동 작업자는 누락된 정보에 대한 요청 확인과 같은 특정 작업을 수행하도록 설정된 Adobe의 준비된 작업 에이전트입니다. Adobe 기본 작업 에이전트로 사용할 수 있으므로 외부 플랫폼에서 에이전트를 구성하거나 외부 플랫폼 자격 증명을 제공할 필요가 없습니다.

작업 에이전트를 구성할 때 미리 빌드된 Collaborator를 에이전트의 소스로 선택합니다. 그런 다음 작업 에이전트의 이름을 지정하고, 액세스 수준을 설정하고, 수행할 수 있는 작업을 선택할 수 있습니다. 사용자는 구성된 작업 에이전트를 다른 작업 에이전트를 할당하는 것과 같은 방식으로 작업 또는 문제에 할당합니다. 사용자는 에이전트가 사전 빌드된 공동 작업자임을 알 필요가 없습니다.

작업 에이전트 및 기타 AI 공동 작업자 유형에 대한 자세한 내용은 [AI 공동 작업자 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md)을 참조하십시오.

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
   <td><p>[!UICONTROL Standard]</p></td> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>[!UICONTROL 시스템 관리자] 또는 그룹 관리자</td> 
  </tr> 
  </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

조직에 Adobe CX Coworker이 활성화되어 있어야 합니다. 자세한 내용은 [Workfront의 CX Enterprise Coworker 개요](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md)를 참조하십시오.

## 사전 빌드된 AI Collaborator 구성

작업 에이전트를 구성할 때 사전 빌드된 AI Collaborator를 구성합니다. **에이전트의 원본 선택** 영역에서 **Adobe 네이티브**&#x200B;를 선택한 다음 아래 목록에서 사용할 미리 빌드된 공동 작업자를 선택하십시오.

전체 단계는 [Workfront에서 작업 에이전트 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent-in-workfront)을 참조하십시오.

공동 작업자가 구성되면 사용자는 이를 작업 또는 문제에 할당할 수 있습니다. 자세한 내용은 [작업 에이전트 사용](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)을 참조하세요.

## 사전 빌드된 AI 공동 작업자 사용 가능

### CX Enterprise Coworker {#cx-enterprise-coworker}

Adobe Agent Orchestrator에서 제공하는 CX Enterprise Coworker 에이전트입니다.

자세한 내용은 [Workfront의 CX Enterprise Coworker 개요](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md)를 참조하십시오.

### Intake 코디네이터 {#intake-coordinator}

Intake 코디네이터는 요청의 세부 사항, 사용자 정의 양식 및 첨부 파일에서 누락되거나 명확하지 않거나 일관되지 않은 정보를 확인합니다. 피드백을 게시하거나 사용자의 승인으로 변경합니다.

<!--
### Context Carrier {#context-carrier}

The Context Carrier keeps brief information flowing downstream so that context doesn't get scattered. It helps campaign managers and project managers keep the project team current without writing reports.

Requirements: A Workfront project and a Workfront Planning project must be connected to a Planning record. The Context Carrier must be triggered to run.

Steps to be added.

### Production Specialist {#production-specialist}

The Production Specialist produces images in every size you need, so designers don't have to resize them manually.

Requirement: Users must assign the Production Specialist to a task or issue.

Steps to be added.

### Version Comparer {#version-comparer}

The Version Comparer compares versions of a document so project teams can move content faster instead of spotting differences by hand.

Requirement: The document must have more than one version.

Steps to be added.

### Metadata Manager {#metadata-manager}

The Metadata Manager helps marketing teams find, tag, and label documents while work is in progress instead of later in the process.

Requirement: The Metadata Manager is available when you upload a document. Users must trigger it from the toolbar.

Steps to be added.

### Resource PTO Detector {#resource-pto-detector}

The Resource PTO Detector helps project teams make sure delivery isn't affected by time off, by identifying tasks assigned to people who are out of office.

Requirements: Tasks must be assigned, and PTO must be logged in Workfront.

Steps to be added.

### Campaign Summarizer {#campaign-summarizer}

Description and steps to be added.
-->
