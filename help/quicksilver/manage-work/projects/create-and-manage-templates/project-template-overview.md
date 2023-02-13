---
product-area: templates
navigation-topic: templates-navigation-topic
title: 프로젝트 템플릿 개요
description: 프로젝트 템플릿을 사용하여 조직의 프로젝트와 관련된 대부분의 반복 가능한 프로세스, 정보 및 설정을 캡처할 수 있습니다.
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 1%

---

# 프로젝트 템플릿 개요

프로젝트 템플릿을 사용하여 조직의 프로젝트와 관련된 대부분의 반복 가능한 프로세스, 정보 및 설정을 캡처할 수 있습니다.

작업, 대기열 항목, 사용자 정의 양식을 정의하고 템플릿에 문서를 첨부할 수 있습니다.

템플릿을 만든 후 기존 프로젝트에 첨부하거나 템플릿을 사용하여 새 프로젝트를 만들 수 있습니다. 템플릿에 대한 모든 정보는 템플릿을 사용하여 생성된 프로젝트로 전송됩니다.

## Adobe Workfront에서 템플릿 사용에 대한 이점

다음은 템플릿을 사용하여 프로젝트를 만들 때 얻을 수 있는 몇 가지 이점 중 일부입니다.

* 반복적인 새 프로젝트를 만들 때 시간과 노력을 절약할 수 있습니다.
* 범위가 비슷한 프로젝트 간에 일관된 정보가 있습니다.
* 이 기능은 프로젝트에 대해 보고할 때 유용합니다. 예를 들어, 동일한 템플릿을 공유하는 프로젝트에 대해 보고하고 진행 상황을 비교하며 진행 상황을 개선할 수 있는 방법을 찾을 수 있습니다.
* 향후 프로젝트 설정을 정의할 수 있을 뿐만 아니라 템플릿에 향후 프로젝트에 대한 다음 정보를 추가할 수 있습니다.

   * 작업
   * 문서
   * 승인
   * 대기열 세부 정보
   * 대기열 주제
   * 주제 그룹
   * 라우팅 규칙
   * 사용자 지정 Forms
   * 회사 및 그룹 정보

## 템플릿 만들기 우수 사례

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

템플릿을 만들 때 다음 사항을 고려하십시오.

* 템플릿 작업에 사용자를 할당하지 마십시오. 작업을 할당되지 않은 상태로 둘 수 있지만 작업에 작업 역할을 할당하는 것이 좋습니다. 이 경우 템플릿을 사용하여 프로젝트를 만들 때 사용자에게 작업에 할당할 수 있는 항목을 알 수 있습니다.
* 항상 템플릿 작업에 기간 및 계획 시간 값을 지정합니다. 프로젝트의 모든 작업은 작업이 열려 있을 수 있는 기간 및 작업이 실제로 완료되는 데 걸리는 시간에 대한 계획 시간 값과 연관되어야 합니다. 이 정보가 없는 작업은 Workfront에서 리소스 관리 도구를 사용할 때 리소스에 대해 적절한 예산책정될 수 없습니다.

   기간에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [프로젝트 기간 개요](../../../manage-work/projects/planning-a-project/project-duration.md)

   계획된 시간에 대한 자세한 내용은 [계획 시간 개요](../../../manage-work/tasks/task-information/planned-hours.md).

* 향후 프로젝트 계획을 완전히 이해한 경우 최종 단계에서 작업 간의 이전 관계를 추가합니다. 템플릿 작업에 선행 작업을 추가하는 것은 프로젝트의 작업에 선행 작업을 추가하는 것과 비슷합니다.

   작업에 선행 작업을 추가하는 방법에 대한 자세한 내용은 [작업 선행 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* 나중에 사용할 수 있도록 템플릿을 공유할 사용자와 템플릿에서 만들 프로젝트를 공유할 사용자를 지정합니다. 템플릿 공유에 대한 자세한 내용은 [프로젝트 템플릿 공유](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* 글로벌 승인 프로세스를 사용하고 가능한 경우 템플릿 및 템플릿 작업에 추가합니다. 이렇게 하면 작업이나 향후 프로젝트에서 동일한 승인을 통과해야 하는 시간이 절약됩니다.

   승인 만들기에 대한 자세한 내용은 [작업 항목에 대한 승인 프로세스 생성](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   승인 프로세스를 작업 항목에 연관시키는 방법에 대한 자세한 내용은 [신규 또는 기존 승인 프로세스를 작업물과 연결](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 템플릿을 만드는 방법

다음과 같은 방법으로 새 템플릿을 만들 수 있습니다.

* 처음부터\
   처음부터 새 템플릿을 만드는 방법에 대한 자세한 내용은 [프로젝트 템플릿 만들기](../../../manage-work/projects/create-and-manage-templates/create-template.md).

* 기존 프로젝트에서 프로젝트를 템플릿으로 저장하여\
   기존 프로젝트에서 템플릿을 만드는 방법에 대한 자세한 내용은 [프로젝트에서 템플릿 만들기](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md).

* 다른 템플릿에서 복사하여\
   기존 템플릿 복사에 대한 자세한 내용은 [프로젝트 템플릿 복사](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* 예제 템플릿을 사용합니다.\
   예제 템플릿을 사용하여 템플릿 만들기에 대한 자세한 내용은 [예에서 프로젝트 템플릿 만들기](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md).
