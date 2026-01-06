---
product-area: templates
navigation-topic: templates-navigation-topic
title: 프로젝트 템플릿 개요
description: 프로젝트 템플릿을 사용하여 조직의 프로젝트와 관련된 대부분의 반복 가능한 프로세스, 정보 및 설정을 캡처할 수 있습니다.
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 2%

---

# 프로젝트 템플릿 개요

<!-- Audited: 12/2023 -->

프로젝트 템플릿을 사용하여 조직의 프로젝트와 관련된 대부분의 반복 가능한 프로세스, 정보 및 설정을 캡처할 수 있습니다.

작업, 대기열 주제, 사용자 정의 양식을 정의하고 템플릿에 문서를 첨부할 수 있습니다.

템플릿을 만든 후 기존 프로젝트에 첨부하거나 이를 사용하여 새 프로젝트를 빌드할 수 있습니다. 템플릿에 대한 모든 정보는 템플릿을 사용하여 생성된 프로젝트로 전송됩니다.

## Adobe Workfront에서 템플릿 사용에 대한 이점

다음은 템플릿을 사용하여 프로젝트를 만들 때 얻을 수 있는 몇 가지 이점입니다.

* 반복적인 새 프로젝트를 만들 때 시간과 노력을 절약할 수 있습니다.
* 범위가 유사한 프로젝트에서 일관된 정보가 있습니다.
* 프로젝트에 대해 보고할 때 유용합니다. 예를 들어 동일한 템플릿을 공유하는 프로젝트에 대해 보고하여 진행 상황을 비교하고 완료 방법에 대한 개선 사항을 찾을 수 있습니다.
* 향후 프로젝트 설정을 정의하는 것 외에도 템플릿에 향후 프로젝트에 대한 다음 정보를 추가할 수 있습니다.

   * 작업
   * 문서
   * 승인
   * 대기열 세부 정보
   * 대기열 주제
   * 주제 그룹
   * 라우팅 규칙
   * 사용자 정의 양식
   * 회사 및 그룹 정보

## 템플릿 만들기에 대한 우수 사례

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

템플릿을 만들 때 다음 사항을 고려하십시오.

* 템플릿 작업에 사용자를 할당하지 마십시오. 작업을 할당 해제한 상태로 둘 수 있지만 작업에 작업 역할을 할당하는 것이 좋습니다. 템플릿을 사용하여 프로젝트를 만들 때 사용자에게 작업을 할당할 수 있는 방법을 알려 줍니다.
* 항상 템플릿 작업에 기간 및 계획된 시간 값을 제공합니다. 프로젝트의 모든 작업은 작업을 진행 중인 상태로 유지할 수 있는 기간 및 작업을 완료하는 데 실제로 걸리는 시간에 대한 계획된 시간 값과 연결되어야 합니다. Workfront에서 리소스 관리 도구를 사용할 때 이 정보가 없는 작업은 리소스 예산을 제대로 책정할 수 없습니다.

  기간에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [프로젝트 기간 개요](../../../manage-work/projects/planning-a-project/project-duration.md)

  계획된 시간에 대한 자세한 내용은 [계획된 시간 개요](../../../manage-work/tasks/task-information/planned-hours.md)를 참조하십시오.

* 향후 프로젝트 계획 전체를 명확하게 이해할 수 있는 경우 맨 끝에서 작업 간에 전임 작업 관계를 추가합니다. 템플릿 작업에 전임 작업을 추가하는 것은 프로젝트의 작업에 전임 작업을 추가하는 것과 비슷합니다.

  작업에 전임 작업을 추가하는 방법에 대한 자세한 내용은 [작업 전임 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)를 참조하십시오.

* 나중에 사용하기 위해 템플릿을 공유할 사용자 및 템플릿에서 만들 프로젝트를 공유할 사용자를 지정합니다. 템플릿 공유에 대한 자세한 내용은 [프로젝트 템플릿 공유](../../../manage-work/projects/create-and-manage-templates/share-project-template.md)를 참조하십시오.
* 글로벌 승인 프로세스를 사용하고 가능한 경우 템플릿 및 템플릿 작업에 추가합니다. 이를 통해 작업 또는 향후 프로젝트가 동일한 승인을 거쳐야 하는 시간을 절약할 수 있습니다.

  승인 만들기에 대한 자세한 내용은 [작업 항목에 대한 승인 프로세스 만들기](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)를 참조하십시오.

  승인 프로세스를 작업 항목에 연결하는 방법에 대한 자세한 내용은 [새 승인 프로세스 또는 기존 승인 프로세스를 작업과 연결](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)을 참조하십시오.

## 템플릿을 만드는 방법

다음과 같은 방법으로 새 템플릿을 만들 수 있습니다.

* 처음부터.\
  처음부터 새 템플릿을 만드는 방법에 대한 자세한 내용은 [프로젝트 템플릿 만들기](../../../manage-work/projects/create-and-manage-templates/create-template.md)를 참조하십시오.

* 기존 프로젝트에서 프로젝트를 템플릿으로 저장\
  기존 프로젝트에서 템플릿을 만드는 방법에 대한 자세한 내용은 [프로젝트에서 템플릿 만들기](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md)를 참조하십시오.

* 다른 템플릿에서 복사하여\
  기존 템플릿을 복사하는 방법에 대한 자세한 내용은 [프로젝트 템플릿 복사](../../../manage-work/projects/create-and-manage-templates/copy-template.md)를 참조하십시오.

* 예제 템플릿을 사용합니다.\
  예제 템플릿을 사용하여 템플릿을 만드는 방법에 대한 자세한 내용은 [예제에서 프로젝트 템플릿 만들기](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md)를 참조하십시오.
