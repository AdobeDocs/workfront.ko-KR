---
title: 작업 공동 작업자 사용
content-type: reference
description: 작업 공동 작업자, Workfront 작업에 할당할 수 있는 AI 공동 작업자를 사용하는 방법에 대해 알아봅니다.
author: Becky
feature: Work Management, Tasks
source-git-commit: f1bdb685cb7974c5c445377e0baa4f4b4e7dfa13
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 3%

---

# 작업 공동 작업자 사용

{{highlighted-preview-article-level}}

작업 공동 작업자는 문서 및 에셋 검토에 사용되는 기존 검토자 유형의 AI 공동 작업자 외에도 Workfront 작업에 직접 할당할 수 있는 AI 공동 작업자입니다. 다른 AI 공동 작업자와 마찬가지로 작업 공동 작업자도 설정 영역에서 구성되어 사용자와 마찬가지로 작업에 할당됩니다.

작업 공동 작업자는 MCP 서버와 매우 유사하게 사용자가 구성한 에이전트에 연결합니다.

Workfront에서 작업 공동 작업자를 만드는 방법에 대한 정보와 지침은 AI 공동 작업자 구성 문서에서 [작업 공동 작업자 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator)을 참조하십시오.

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

* Copilot, Claude 또는 Writer.ai에서 에이전트를 구성해야 작업 공동 작업자로 사용할 수 있습니다.

## 작업 Collaborator 개요

작업 공동 작업자는 Workfront의 특정 작업에 MCP 에이전트를 할당하는 방법입니다. Copilot Studio, Claude 또는 Writer.ai와 같은 앱에서 에이전트를 구성한 다음 해당 에이전트를 작업 공동 작업자로 Workfront에 연결합니다. 그런 다음 사용자를 할당할 때처럼 작업에 할당할 수 있습니다.

일부 예제 워크플로에는 다음이 포함될 수 있습니다.

* 작업에 업로드된 이미지를 감지하고 에이전트에 지정된 기준을 기반으로 변형을 생성하고, 새 이미지를 작업에 업로드합니다.
* 작업 설명에서 복사본을 생성하고, 에이전트에 구성된 지침에 따라 복사본을 검토하고, 복사본을 업데이트 스트림에 게시합니다.
* 이벤트의 세부 정보를 읽고, 누락된 세부 정보를 식별하고, 업데이트 스트림에 누락된 세부 정보에 대한 질문을 게시합니다.

>[!NOTE]
>
>* 에이전트의 책임 및 능력에 대한 특정 세부 정보는 Workfront이 아니라 에이전트가 생성된 애플리케이션에서 구성됩니다.
>* 작업 공동 작업자는 현재 Copilot Studio, Claude 및 Writer.ai에서 생성된 에이전트를 지원합니다.
>* Copilot Studio에서 에이전트를 구성할 때 보안을 **인증 안 함**(으)로 설정해야 합니다.
>* Workfront에서 작업 공동 작업자를 만드는 방법에 대한 정보와 지침은 AI 공동 작업자 구성 문서에서 [작업 공동 작업자 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator)을 참조하십시오.

## 작업에 작업 협력자 할당

작업 공동 작업자는 사용자가 할당된 것과 동일한 방식으로 작업에 할당됩니다.

지침은 [작업 할당](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md)을 참조하세요.
