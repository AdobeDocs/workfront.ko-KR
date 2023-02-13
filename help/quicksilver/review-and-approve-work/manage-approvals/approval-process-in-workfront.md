---
content-type: overview
product-area: projects
navigation-topic: approvals
title: 승인 프로세스 개요
description: 승인 프로세스를 만들고 객체에 연결하여 지정된 사용자가 객체가 진행되기 전에 특정 변경 사항을 검토하는지 확인할 수 있습니다.
author: Courtney
feature: Work Management
exl-id: dd0822b6-80f1-4a2e-bf6a-0c425984f4d0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1747'
ht-degree: 0%

---

# 승인 프로세스 개요

승인 프로세스를 만들고 객체에 연결하여 지정된 사용자가 객체가 진행되기 전에 특정 변경 사항을 검토하는지 확인할 수 있습니다.

Adobe Workfront의 다음 개체 유형에 사용할 수 있습니다.

* 작업 항목(프로젝트, 작업 또는 문제, 템플릿, 템플릿 작업)
* 문서
* 증명

승인 프로세스 만들기에 대한 지침은 [작업 항목에 대한 승인 프로세스 생성](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

이 문서에는 작업 항목과 관련된 승인 프로세스에 대한 일반적인 정보가 포함되어 있습니다.

## 승인 프로세스 유형

Adobe Workfront 관리자나 승인 프로세스에 대한 관리자 액세스 권한이 있는 사용자는 프로젝트, 작업 및 문제에 대해 다음과 같은 승인 프로세스를 만들 수 있습니다.

* **시스템 수준 글로벌 승인 프로세스**: 사용자는 다음 중 하나에 첨부할 수 있습니다.

   * 승인 섹션의 프로젝트, 작업 또는 문제
   * 프로젝트 편집 상자의 작업 기본 승인 프로세스 영역에서
   * 프로젝트의 대기열 세부 정보 또는 대기열 항목 섹션에서 기본 승인 프로세스 영역에 있습니다. 프로젝트를 요청 큐로 활성화해야 합니다.

* **그룹 수준 글로벌 승인 프로세스**: 사용자는 다음 항목에 연결할 수 있습니다.

   * 승인 섹션의 승인 프로세스와 연관된 그룹에 속하는 프로젝트, 작업 또는 문제
   * 프로젝트 편집 상자에서 승인 프로세스와 연관된 그룹에 속하는 프로젝트의 태스크 기본 승인 프로세스 영역입니다
   * 프로젝트의 대기열 세부 정보 또는 대기열 항목 섹션에서 기본 승인 프로세스 영역에 있습니다. 프로젝트는 요청 큐로 활성화되어야 하며 승인 프로세스와 연관된 그룹에 속해야 합니다.

   시스템 수준 또는 그룹 수준 승인 프로세스 만들기에 대한 자세한 내용은 [작업 항목에 대한 승인 프로세스 생성](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

* **단일 사용 승인 프로세스**: 단일 프로젝트, 작업, 문제, 템플릿 또는 템플릿 작업에 사용할 수 있습니다. 이 유형의 승인 프로세스는 해당 객체와 연관된 객체에만 영향을 미치며 다른 객체와 연결할 수 없습니다.

   단일 사용 승인 프로세스 만들기에 대한 내용은 [신규 또는 기존 승인 프로세스를 작업물과 연결](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>이 문서에서는 &quot;전역 승인 프로세스&quot;라는 용어를 사용하여 &quot;단일 사용 승인 프로세스&quot;와 구분합니다. 글로벌 승인 프로세스는 반복적으로 사용할 수 있습니다.
>
>그룹 수준 글로벌 승인 프로세스라는 용어는 특정 그룹에만 연관된 상태 및 품목에 대해 반복적으로 사용할 수 있는 승인 프로세스를 의미합니다.

시스템 레벨 승인 프로세스 또는 그룹 레벨 승인 프로세스 생성에 대한 자세한 내용은 [작업 항목에 대한 승인 프로세스 생성](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## 승인 프로세스에 대한 고려 사항

* 승인 프로세스를 연관시키려면 먼저 프로젝트, 작업, 문제, 템플릿 또는 템플릿 작업을 생성해야 합니다.
* 승인 프로세스는 항상 다음의 두 가지 중요한 사항과 연관됩니다.

   * 각 승인 프로세스는 Workfront 시스템의 특정 작업 항목 상태에 해당합니다. 작업 항목의 상태를 변경하면 해당 상태에 대한 첨부된 승인이 해당 항목에 새 상태를 지정하려면 상태 변경을 확인해야 합니다.

      >[!TIP]
      >
      >
      >   
      >   
      >   * 그룹 레벨 승인을 전역 또는 그룹 레벨 상태와 연관시킬 수 있습니다.
      >   * 승인 프로세스를 사용하는 품목의 상태를 승인 프로세스와 연관된 상태 이외의 상태로 변경할 수 없습니다.

         >   
         >   
         >     예를 들어, 진행 중 상태와 연관된 작업 승인이 있는 경우, 승인이 승인되면 해당 상태는 자동으로 진행 중으로 변경됩니다. 상태를 완료됨으로 자동 변경할 수 없거나 승인과 연관되지 않은 다른 상태는 자동으로 변경할 수 없습니다.


   * 승인 프로세스와 연관된 엔티티는 사용자, 작업 역할 또는 팀일 수 있습니다. 사용자는 궁극적으로 승인을 수락하거나 거부할 책임이 있습니다. 프로젝트에서 특정 역할을 수행하는 사용자에게 승인을 할당할 수 있습니다. 예를 들어 프로젝트 소유자 또는 스폰서에 승인을 지정할 수 있습니다. 자세한 내용은 [작업 항목에 대한 승인 프로세스 생성](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

      다음 시나리오가 있습니다.

      * 작업 역할에 승인을 지정하면 작업 역할과 연관된 프로젝트 팀의 모든 사용자가 승인을 결정할 수 있습니다. 승인과 연관된 역할은 기본 역할 또는 기타 역할 중 하나일 수 있습니다.

         프로젝트 팀에 대한 자세한 내용은 [프로젝트 팀 개요](../../manage-work/projects/planning-a-project/project-team-overview.md).

      * 팀에 승인을 지정하면 해당 팀의 모든 구성원이 승인을 결정할 수 있습니다. 승인과 연관된 팀은 홈 팀이나 다른 팀 중 하나일 수 있습니다.

         사용자의 역할 및 팀에 대한 자세한 내용은 [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 작업 항목을 생성할 때 자동으로 승인 프로세스가 첨부되지 않습니다. 사용하려면 수동으로 첨부해야 합니다. 항목에 승인 프로세스 첨부에 대한 자세한 내용은 [신규 또는 기존 승인 프로세스를 작업물과 연결](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
* Workfront 관리자 또는 승인 프로세스에 대한 관리자 액세스 권한이 있는 사용자는 시스템 전체에서 사용할 시스템 수준의 글로벌 승인 프로세스를 만들 수 있습니다. 승인 프로세스에 대한 관리자 권한이 있는 그룹 관리자는 관리하는 특정 그룹에서만 사용할 그룹 수준의 글로벌 승인 프로세스를 생성할 수 있습니다.
* 작업 항목에 대해 사전 정의된 시스템 레벨 또는 그룹 레벨 글로벌 승인 프로세스를 사용하지 않으려면 승인 프로세스를 첨부할 객체에 대한 관리 권한이 있을 때 단일 사용 승인 프로세스를 생성하고 첨부할 수 있습니다.

   >[!NOTE]
   단일 사용 승인 프로세스를 만든 특정 항목에 대해 한 번만 사용할 수 있습니다. 프로젝트, 작업, 문제, 템플릿 및 템플릿 작업에 대한 단일 사용 승인 프로세스에 대해 전역 상태와 그룹 수준 상태를 연결할 수 있습니다.

* 그룹 수준 사용자 지정 상태를 사용하여 항목에 그룹 수준 승인 프로세스를 첨부할 때 프로젝트 그룹을 변경하면 이전 그룹의 승인 상태와 시스템 수준의 기존 승인 상태 간에 충돌이 발생할 수 있습니다. 그룹을 업데이트하기 전에 프로젝트에서 그룹 수준의 승인 프로세스 또는 해당 작업 또는 문제를 제거하는 것이 좋습니다. 그룹 수준 승인 프로세스 생성에 대한 자세한 내용은 [그룹 수준 승인 프로세스](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md). 사용자 지정 그룹 상태 만들기에 대한 자세한 내용은 [그룹 상태 만들기 또는 편집](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md). 프로젝트 그룹 업데이트에 대한 자세한 내용은 [프로젝트 편집](../../manage-work/projects/manage-projects/edit-projects.md).

## 승인 프로세스 워크플로우

이 섹션에서는 작업 항목 승인에 대해 설명합니다.

* [승인 프로세스가 상태에 의존하는 방식](#how-approval-processes-rely-on-statuses)
* [일반적인 워크플로우가 승인 프로세스를 사용하는 방법](#how-a-typical-workflow-uses-an-approval-process)

### 승인 프로세스가 상태에 의존하는 방식 {#how-approval-processes-rely-on-statuses}

승인 프로세스에 상태를 첨부하면 품목이 부서로 이동하여 적절한 순서로 이동됩니다.

**예:** 재무 부서의 승인이 필요한 마케팅 부서 상태에 승인 프로세스를 첨부할 수 있습니다. 그런 다음, 누군가 작업 항목의 상태를 &quot;마케팅 부서&quot;로 변경하면, 재무부가 작업을 시작할 때까지 해당 부서로 이동할 수 없습니다.

작업 항목의 상태에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [시스템 프로젝트 상태 목록에 액세스합니다](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)
* [시스템 작업 상태 목록에 액세스합니다](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)
* [시스템 문제 상태 목록에 액세스합니다](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### 일반적인 워크플로우가 승인 프로세스를 사용하는 방법 {#how-a-typical-workflow-uses-an-approval-process}

다음 시나리오는 Workfront 개체가 이 순서로 여러 단계의 워크플로우를 통해 진행되므로 승인 프로세스를 통해 사용자가 작업을 승인하는 방법을 보여줍니다.

1. 승인 프로세스에 대한 관리자 권한이 있는 Workfront 관리자 또는 사용자는 프로젝트, 작업 또는 문제에 대한 승인 프로세스를 만듭니다.

   >[!NOTE]
   템플릿에 프로젝트 승인 프로세스를 첨부하고 작업 승인 프로세스를 템플릿 작업에 첨부할 수 있습니다. 이 작업을 수행한 후 누군가 템플릿을 사용하여 프로젝트를 만들면 승인 프로세스는 각각 프로젝트 또는 태스크 승인 프로세스가 됩니다. 템플릿 또는 템플릿 작업에 첨부된 단일 사용 승인 프로세스는 프로젝트 및 작업에 대해 단일 사용 승인 프로세스로 유지됩니다.

1. 프로젝트, 작업 또는 발행에 대한 관리 권한이 있는 사용자는 승인 프로세스를 품목에 첨부하거나 항목에 대한 단일 사용 승인을 생성합니다.
1. 작업 품목에 지정된 사용자가 상태를 승인 프로세스를 시작하는 상태로 변경하고 승인 프로세스가 시작됩니다. (승인 프로세스를 생성한 자는 상태와 승인 프로세스 간의 관계를 정의합니다.)
1. 지정된 승인자는 대기 중인 승인 프로세스에 대한 통지를 받고 작업 항목을 검토합니다.
1. 지정된 승인자가 프로세스의 모든 단계를 승인하면 승인 프로세스가 종료됩니다. 또는 단계를 거부하면 상태가 사전 정의된 상태로 재설정되거나 문제가 만들어집니다. (거부 후 발생하는 이러한 자동화된 단계 중 하나를 정의한 승인 프로세스를 만든 사람)

**예:** 광고 팀이 인쇄 준비라는 상태와 이 상태와 연결된 Designer/Copywriter Signoff라는 승인 프로세스를 만들었습니다. 이 승인 프로세스는 다음으로 구성됩니다.

* 팀의 디자이너와 카피라이터의 승인 필요
* 작업 항목의 상태를 인쇄 준비로 변경할 때마다 시작합니다

브로셔 프로젝트 소유자는 디자이너/카피라이터 사인오프 승인 프로세스를 브로셔 프로젝트에 첨부합니다.

프로젝트의 누군가 상태를 인쇄용 준비로 변경하면 카피라이터와 디자이너가 승인하거나 거부하라는 알림을 받습니다. 승인 프로세스 중에 승인 여부를 심의하는 경우 프로젝트의 상태가 인쇄 준비 - 승인 보류 중으로 표시됩니다.

둘 다 Workfront에서 브로셔를 승인하면 프로젝트 상태가 인쇄 준비로 변경됩니다.

## 문서 승인 프로세스

문서 승인은 보다 일반적인 승인을 위해 사용됩니다. 피드백은 업데이트 탭에서 채팅 형식으로 캡처됩니다. 승인 단추를 사용하여 변경 사항을 승인, 거부 또는 승인할 수 있습니다.

Workfront에 업로드한 후 문서에 승인자를 추가하려면 다음을 참조하십시오 [문서 승인 요청](../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## 증명 승인 프로세스

증명 승인은 심층적인 검토에 사용되며 일반적으로 더 복잡한 워크플로우를 포함합니다. 피드백은 교정 뷰어에서 마크업 도구로 캡처됩니다. 승인 단추를 사용하여 변경 사항을 승인, 거부 또는 승인할 수 있습니다.

문서 증명에 자동화된 워크플로우를 추가하고 워크플로우의 특정 사용자를 증명의 승인자로 지정하려면 다음을 참조하십시오 [자동화된 워크플로우를 사용하여 고급 증명 만들기](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## 작업 항목 승인 프로세스에 대한 설정 구성

Workfront 관리자는 시스템에서 작업 항목 승인 프로세스에 대한 전역 설정을 구성할 수 있습니다. 이러한 설정은 승인 결정을 열어 둘 수 있는 기간 또는 시스템에서 승인 위임을 관리하는 방법과 같이 승인 프로세스에 대한 다양한 규칙을 결정합니다. 승인 프로세스 설정에 대한 자세한 내용은 [전역 승인 설정 구성](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).
