---
product-area: projects
navigation-topic: plan-a-project
title: 프로젝트의 작업 분류 구조 결정
description: 프로젝트에 대한 작업 분류 구조(WBS) 정의는 프로젝트 계획을 최종적으로 요약하는 일련의 활동입니다. WBS는 프로젝트의 결과를 관리 가능한 작업 요소로 나눕니다. 이 작업 요소는 이정표를 정의하고 작업 할당을 구성하는 데 사용할 수 있습니다.
author: Alina
feature: Work Management
exl-id: a76c468d-6373-4dab-93ff-a0b3734f368c
source-git-commit: fb1c7ade6622db391e0dac54f37603efe9dc0a58
workflow-type: tm+mt
source-wordcount: '1750'
ht-degree: 1%

---

# 프로젝트의 작업 분류 구조 결정

프로젝트에 대한 작업 분류 구조(WBS) 정의는 프로젝트 계획을 최종적으로 요약하는 일련의 활동입니다. WBS는 프로젝트의 결과를 관리 가능한 작업 요소로 나눕니다. 이 작업 요소는 이정표를 정의하고 작업 할당을 구성하는 데 사용할 수 있습니다.

프로젝트의 작업 분류 구조를 만들려면 프로젝트에 대한 편집 액세스 권한이 있는 플랜 라이선스가 있어야 합니다. WBS를 빌드하는 동안 수행하는 활동 수에 따라 Adobe Workfront의 다른 영역에 대한 추가 액세스가 필요할 수 있습니다.

작업 분류 구조를 변경하는 동안 프로젝트 팀의 사용자에게 트리거되는 알림을 방지하려면 프로젝트를 계획 중 상태로 유지하는 것이 좋습니다.

## 프로젝트 결과물 정의

프로젝트의 목적은 내부 및 외부 이해 관계자에게 유형의 결과물을 제공하는 것입니다. 프로젝트의 결과물은 프로젝트를 완료하여 달성하고자 하는 결과입니다. 결과는 거의 항상 하나 이상의 산출물과 연관되어 있으며 모든 산출물은 프로젝트와 연관되어 있어야 합니다.

프로젝트 결과물은 소비재, 지적 산출물(보고서 등) 또는 서비스일 수 있습니다. 예를 들어, 프로젝트 범위가 집을 짓는 경우 일부 결과물에는 다음이 포함될 수 있습니다.

* 아키텍처 계획 생성
* 배관 공사 완료
* 전기 작업
* 기초를 부어
* 프레이밍 작업
* 그 집의 매매를 마감하다.

프로젝트의 크기와 범위에 따라 프로젝트는 여러 결과물로 구성될 수 있습니다.

결과물을 식별한 후에는 작업별로 분류할 수 있습니다. 작업은 프로젝트에 대한 전반적인 결과를 전달하기 위해 수행하는 결과입니다. 작업을 정의할 때 다음 매개 변수를 고려합니다.

* 완료에 필요한 시간입니다.
* 작업 완료에 필요한 예산.
* 작업을 완료하는 데 필요한 리소스.
* 작업의 논리적 타임라인을 기반으로 리소스 일정 조정.

작업을 정의할 때 하나의 개별 작업에 대해 너무 많은 작업을 계획하지 않도록 하십시오. 작업에 필요한 작업이 40시간(일반적인 주 근무)을 초과하는 경우 하위 작업에서 해당 작업량을 분류해야 할 수 있습니다. 모든 하위 작업이 완료되면 기본 작업이 완료됩니다.

Workfront에서 WBS 결과 및 결과물을 정의하려면 다음 활동을 수행하여 프로젝트 작업의 계층적 보기를 만드는 것이 좋습니다.

* 아직 만들지 않은 경우 새 프로젝트를 만듭니다.\
  프로젝트 만들기에 대한 자세한 내용은 문서 [프로젝트 만들기](../../../manage-work/projects/create-projects/create-project.md)를 참조하십시오.

* 각 결과 및 결과물을 완료하는 데 필요한 모든 작업 항목에 대한 작업을 생성합니다.\
  작업 만들기에 대한 자세한 내용은 문서 [프로젝트에서 작업 만들기](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)를 참조하십시오.

* 방금 생성한 작업에서 주요 결과를 식별하고 이정표와 연결합니다.\
  마일스톤 작업 만들기에 대한 자세한 내용은 문서 [마일스톤 경로 만들기](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) 및 [마일스톤과 작업 연결](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)을 참조하세요.

* 범위가 너무 큰 작업을 하위 작업으로 분류합니다. 결과물을 정의하는 상위 와 연결합니다.\
  하위 작업 만들기에 대한 자세한 내용은 문서 [하위 작업 만들기](../../../manage-work/tasks/create-tasks/create-subtasks.md)를 참조하십시오.

* 하위 작업과 마일스톤 간의 종속성 관계를 식별합니다.\
  종속성 관계에서 작업의 시작은 다른 작업 또는 작업 그룹의 완료에 따라 달라집니다.\
  작업 종속성에 대한 자세한 내용은 [작업 전임 작업의 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) 및 [작업 목록에서 전임 작업 관계 만들기](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md) 문서를 참조하십시오.

* 프로젝트 수명 중 어느 시점에서든 승인 및 검토가 필요한지 결정합니다. 이 요구 사항을 해결하기 위해 승인 프로세스를 만듭니다.\
  승인에 대한 자세한 내용은 문서 [작업 항목에 대한 승인 프로세스 만들기](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)를 참조하십시오.

## 작업 일정 및 일정 제한 예상

프로젝트의 기본 마일스톤 및 작업 구조를 만든 후에는 작업 제한 및 기간을 정의하여 전체 프로젝트를 완료하는 데 걸리는 시간을 예상할 수 있습니다.

다음 사항을 고려하십시오.

* 작업 제한은 작업에 대한 작업을 시작하거나 종료해야 하는 시점을 정의합니다.

  작업 제한 정의에 대한 자세한 내용은 문서 [작업 제한 개요](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)를 참조하십시오.

* 작업 기간은 작업을 완료하는 데 사용할 수 있는 기간입니다. 기간을 추정할 때 지연 가능성을 고려한 값을 입력할 수 있습니다. 이전에 유사한 프로젝트가 완료된 경우 이 값을 설정할 위치를 알고 있을 수 있습니다.

  기간은 예상 기간이므로 기상, 정전, 공급업체 어려움 또는 기타 예기치 않은 이벤트와 같이 작업에 영향을 줄 수 있는 요소를 고려하도록 낙관적 시간 값을 설정해야 합니다. 또한 연결된 전임 작업 또는 종속성 작업이 있는지 여부와 작업 제한 및 작업 완료에 영향을 줄 수 있는 방법을 고려해야 합니다.

  작업의 기간 유형에 따라 프로젝트 수명 동안 작업 기간을 수정할 수 있지만, 이는 프로젝트의 타임라인에도 영향을 미칩니다. 작업 기간에 대한 자세한 내용은 문서 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)를 참조하십시오.

## 작업 할당

각 작업의 기간 및 제한 사항을 정의한 후 해당 작업을 수행할 시간과 기술을 보유한 사용자를 결정할 수 있습니다. Workfront에서 다음 엔티티에 작업을 할당할 수 있습니다.

* 사용자\
  플래너 또는 작업자 액세스 수준이 있는 사용자만 작업에 할당할 수 있습니다. 요청자 및 검토자에게 작업을 할당할 수 있지만 완료할 수는 없습니다. 이러한 이유로 작업을 할당하지 않는 것이 좋습니다.

  액세스 수준 및 사용자가 Workfront 개체로 수행할 수 있는 작업을 정의하는 방법에 대한 자세한 내용은 [액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)를 참조하십시오.

* 작업 역할
* 팀

작업 할당에 대한 자세한 내용은 [작업 할당](../../../manage-work/tasks/assign-tasks/assign-tasks-1.md) 섹션의 문서를 참조하십시오.

## 리소스 관리

Workfront의 리소스 관리를 사용하면 프로젝트를 완료할 수 있는 충분한 인력이 있는지 여부를 확인할 수 있습니다. 사용자가 프로젝트에 추가되면 Workfront에 각 사용자의 사용률이 표시됩니다. Resource Manager는 프로젝트 기간 동안 사용자가 다른 프로젝트에 할당된 총 시간을 볼 수 있습니다.

>[!NOTE]
>
>프로젝트가 계획 상태인 동안에는 사용자에게 할당된 작업이 작업 목록에 표시되지 않습니다.

회계 연도 또는 분기의 시작에서는 특정 작업 분류 구조에 대한 지식 없이 여러 프로젝트에서 리소스를 더 높은 수준으로 관리할 수 있습니다.\
더 높은 수준의 리소스 사용 계획에 대한 자세한 내용은 문서 [리소스 계획 시작](../../../resource-mgmt/resource-planning/get-started-resource-planning.md)을 참조하세요.

한 프로젝트의 작업 분류 구조를 작성하는 맥락에서 리소스를 관리하고 각 작업이 올바른 리소스에 지정되도록 하면 수행해야 하는 작업에 대한 리소스를 예약할 수 있습니다.\
리소스 예약에 대한 자세한 내용은 [업무 균형자: 문서 인덱스](../../../resource-mgmt/workload-balancer/workload-balancer.md) 섹션에서 문서를 참조하십시오.

## 프로젝트 재무 예상

Workfront은 각 작업의 계획된 비용과 프로젝트의 전체 비용을 계산합니다. 작업에 대한 계획된 비용에는 작업의 모든 비용과 작업에 할당된 직원 또는 역할의 비용이 포함됩니다. 작업, 역할 및 직원의 시간당 요금은 작업, 역할 및 사용자를 만드는 동안 할당됩니다.

프로젝트 재무 정보에 대한 자세한 내용은 [프로젝트 재무: 문서 인덱스](../../../manage-work/projects/project-finances/project-finances-overview.md) 섹션을 참조하십시오.

## 프로젝트에 대한 승인 지점 결정

Workfront에서 승인 프로세스를 생성하여 프로젝트에 대한 검토 지점을 설정하여 진행 상황과 잠재적인 문제 영역을 모니터링할 수 있습니다. 프로젝트 소유자는 승인 프로세스를 통해 지연 및 조기 작업을 식별하고 작업 상태를 변경한 사용자를 나열하는 감사 추적을 보고 문제 해결 방법 및 종료 시기 등 문제 기록을 볼 수 있습니다. 프로젝트 소유자는 프로젝트를 검토한 후 필요한 경우 프로젝트 계획을 수행하고 업데이트할 단계를 결정할 수 있습니다.

승인에 대한 자세한 내용은 문서 [작업 항목에 대한 승인 프로세스 만들기](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)를 참조하십시오.

## WBS 보기

프로젝트의 WBS를 이해하기 위해 다음 작업 요소를 볼 수 있습니다.

* 작업 순서 및 타임라인(계획된 시작 및 완료 일자, 작업 기간)
* 전임 작업 종속성
* 하위 및 상위 관계
* 할당

WBS를 완료하면 프로젝트 수준의 작업 목록 또는 보고서에서 볼 수 있습니다.

* [작업 목록에서 WBS 보기](#view-the-wbs-in-a-task-list)
* [작업 보고서에서 WBS 보기](#view-the-wbs-in-a-task-report)

### 작업 목록에서 WBS 보기 {#view-the-wbs-in-a-task-list}

프로젝트 수준에서 작업 목록을 볼 수 있습니다.

1. 작업 분류 구조를 보려는 프로젝트로 이동합니다.
1. **작업** 탭을 선택합니다.
1. (선택 사항) **그룹화** 드롭다운 메뉴에서 **없음**&#x200B;을 선택합니다.

   작업 분류 구조에는 WBS에 있는 작업의 들여쓰기가 표시되지 않습니다.

1. **보기** 드롭다운 메뉴에서 **작업 분류** 보기를 선택합니다.

   작업 분류 구조가 선택한 뷰의 두 번째 열에 표시됩니다.

   ![작업 목록의 작업 분류 구조](assets/work-breakdown-structure.png)

### 작업 보고서에서 WBS 보기 {#view-the-wbs-in-a-task-report}

다음 중 하나를 수행하여 작업 보고서를 작성하고 작업의 WBS를 표시할 수 있습니다.

* 보고서에 기존 작업 분류 구조 보기를 적용합니다.
* 사용자 지정 보고서에 작업 분류 구조 열을 추가합니다.

>[!TIP]
>
>작업이 속한 프로젝트에 명확성을 추가하기 위해 프로젝트 그룹을 추가하는 것이 좋습니다. 작업의 들여쓰기는 작업 보고서에 표시되지 않습니다.

보고서 작성에 대한 자세한 내용은 문서 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.

## 프로젝트의 WBS를 템플릿으로 저장

방금 만든 WBS와 유사한 작업 일정을 따르는 다른 프로젝트에서 작업하는 경우 프로젝트를 템플릿으로 저장할 수 있습니다. 템플릿은 향후 관련 프로젝트를 만들 때 시간과 노력을 절약합니다.

조직에 이직률이 거의 없는 경우 템플릿을 저장하기 위해 사용자 할당이 수행된 후까지 기다리는 것이 좋습니다. 프로젝트를 템플릿으로 저장하는 시기에 관계없이 템플릿을 새 프로젝트에 첨부하는 동안 사용자 할당 또는 특정 작업을 제거할 수 있습니다.

작업 분류 구조의 다음 요소는 나중에 다른 프로젝트에서 사용할 수 있도록 템플릿에 저장할 수 있습니다.

* 전임 작업 종속성
* 할당(프로젝트 소유자, 스폰서 및 리소스 관리자 포함)
* 승인 프로세스
* 작업 제한
* 문서
* 경비 및 기타 재무 정보
* 목표
* 시간 유형
* 요청 대기열 구조
* 미리 알림
* 위험
* 청구 요금
* 정보 공유
* 사용자 정의 양식

프로젝트를 템플릿으로 저장하는 방법에 대한 자세한 내용은 문서 [프로젝트에서 템플릿 만들기](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md)를 참조하십시오.
