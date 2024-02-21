---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: '2020.2 리소스 관리 개선 사항: 업무 균형자'
description: 이 페이지에서는 프로덕션 환경에 대한 2020.2 릴리스의 모든 리소스 관리 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2020년 5월 11일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00cc1205-5d58-485b-8076-e177f1d931f9
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '1741'
ht-degree: 0%

---

# 2020.2 리소스 관리 개선 사항: 업무 균형자

이 페이지에서는 프로덕션 환경에 대한 2020.2 릴리스의 모든 리소스 관리 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2020년 5월 11일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다.

2020.2 릴리스에서 사용할 수 있는 모든 변경 사항의 목록은 을 참조하십시오. [2020.2 릴리스 개요](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

사용자는 계층 1 자산입니다. 워크로드 밸런서를 통해 번아웃으로부터 보호할 수 있고 핵심 회사 전략에 맞게 조정하면서 최상의 작업을 수행할 수 있도록 할 수 있습니다. 동일한 보기에서 사용자의 워크로드와 수요를 시각화하고 관리할 수 있는 다시 상상된 예약 경험을 소개합니다. 사용자 인터페이스는 초과 및 과소 활용에 대한 명확한 시각적 매핑을 제공하며 모든 이해 당사자에게 투명합니다. 사용자 관리자는 해당 정보를 입력으로 사용할 수 있으며 동일한 화면에서 타임라인을 통해 노력의 균형을 재조정하고 이는 Workfront 플랫폼의 나머지 부분에 반영됩니다.

>[!NOTE]
>
>업무 균형자 가 2019.4 릴리스와 함께 베타 버전으로 릴리스되기 시작했습니다. 모든 업무 균형자 개선 사항은 2020.2 릴리스에서 일반적으로 사용할 수 있습니다. 이 페이지에 설명된 개선 사항은 2020.2 릴리스와 함께 추가되었습니다. 업무 균형자에 대한 개요는 를 참조하십시오. [업무 균형자 개요](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## 업무 균형자에서 일별 및 주별 할당 조정

이제 리소스가 소진되지 않도록 업무 균형자를 사용하여 작업할 사용자의 일별 및 주별 할당을 조정할 수 있습니다.

이 기능이 향상되기 전에는 리소스 예약 도구를 사용해야 이 작업을 수행할 수 있었습니다.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(DO NOT ADD THIS, JUST ADD THE VIDEO FOR NOW: For information about managing allocations in the Workload Balancer, see /Content/Resource Mgmt/Workload Balancer/Manage hours in the Workload Balancer.htm.)</p>
-->

**다음 환경에서 사용할 수 있습니다.**

* Adobe Workfront 클래식
* 새로운 Adobe Workfront 환경

## 업무 균형자 필터

이제 업무 균형자에서 관련 정보를 얻기 위해 업무 균형자의 미할당 작업 및 할당된 작업 영역에 대한 필터를 만들고 나중에 사용할 수 있도록 저장할 수 있습니다. 그런 다음 새 필터로 처음부터 시작하는 대신 저장된 버전을 편집하여 일부 내용을 변경할 수 있습니다.

업무 균형자 의 필터링에 대한 자세한 내용은 [업무 균형자에서 필터 관리](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(or if you are using Adobe Workfront Classic, see )
</MadCap:conditionalText>
-->

.

**다음 환경에서 사용할 수 있습니다.**

* Adobe Workfront 클래식
* 새로운 Adobe Workfront 환경

## 업무 균형자에 남은 시간 표시

이제 새로운 설정을 사용하여 올바른 할당 결정을 내리는 데 도움이 되도록 일정에 따라 사용자가 작업할 수 있는 시간과 사용자가 이미 작업에 할당된 시간(나머지 시간) 간의 시간 차이를 볼 수 있습니다. 이제 업무 균형자에서 새 설정을 사용할 수 있습니다.

업무 균형자에서 정보를 보는 방법에 대한 자세한 내용은 [업무 균형자 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (또는 Adobe Workfront Classic을 사용하는 경우 다음을 참조하십시오.) [업무 균형자 탐색](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648).)

**다음 환경에서 사용할 수 있습니다.**

* 새로운 Adobe Workfront 환경

## 업무 균형자의 미할당 작업 영역에 작업 및 프로젝트에 대한 일별 계획된 시간 표시

작업을 할당하기 전에 사용자의 워크로드에 어떤 영향을 미칠지 이해할 수 있도록 이제 &quot;할당 표시&quot; 설정이 업무 균형자의 미할당 작업 영역에 표시되는 정보를 관리합니다. 이 설정을 활성화하면 작업과 프로젝트 모두에 대해 계획된 시간이 업무 균형자의 미할당 작업 영역에 표시됩니다.

이 변경 이전에는 이 설정이 밸런서의 할당된 작업 영역에 있는 정보만 업데이트했습니다.

업무 균형자 탐색에 대한 자세한 내용은 [업무 균형자 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (또는 Adobe Workfront Classic을 사용하는 경우 다음을 참조하십시오.) [업무 균형자 탐색](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648).).

**다음 환경에서 사용할 수 있습니다.**

* Adobe Workfront 클래식
* 새로운 Adobe Workfront 경험(이전에는 작업에만 사용 가능)

## 업무 균형자에 대한 새 설정 상자

이제 환경을 간소화하기 위해 업무 균형자에서 보기를 업데이트하는 추가 도구를 표시하는 설정 상자를 사용할 수 있습니다. 이 상자에는 다음 설정이 포함됩니다.

* 프로젝트별 그룹
* 작업 및 프로젝트에 대해 할당된 시간 또는 남은 시간을 표시합니다.

업무 균형자에서 정보를 보는 방법에 대한 자세한 내용은 [업무 균형자 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (또는 Adobe Workfront Classic을 사용하는 경우 다음을 참조하십시오.) [업무 균형자 탐색](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648).).

**다음 환경에서 사용할 수 있습니다.**

* Adobe Workfront 클래식
* 새로운 Adobe Workfront 환경

## 링크를 사용하여 업무 균형자 공유

이제 직원들의 업무량을 경영진과 공유하여 직원 채용 요구에 대한 맥락을 파악할 수 있습니다. 이를 위해 이제 다른 사용자와 업무 균형자에 대한 고유 URL을 공유하여 업무 균형자를 공유할 수 있습니다.

업무 균형자 탐색에 대한 자세한 내용은 [업무 균형자 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (또는 Adobe Workfront Classic을 사용하는 경우 다음을 참조하십시오.) [업무 균형자 탐색](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648)).

**다음 환경에서 사용할 수 있습니다.**

* Adobe Workfront 클래식
* 새로운 Adobe Workfront 환경

## 업무 균형자에서 날짜 범위 변경

이제 사용자 요구에 맞게 업무 균형자의 타임라인 기간을 사용자 정의할 수 있도록 사용자 정의 기간을 2, 4 또는 6주로 선택하여 한 번에 표시할 수 있습니다.

이 개선 이전에는 업무 균형자에 항상 현재 주부터 시작되는 정보가 표시되었습니다.

업무 균형자 탐색에 대한 자세한 내용은 [업무 균형자 탐색](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (또는 Adobe Workfront Classic을 사용하는 경우 다음을 참조하십시오.) [업무 균형자 탐색](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648)).

**다음 환경에서 사용할 수 있습니다.**

* Adobe Workfront 클래식
* 새로운 Adobe Workfront 경험(이전에 사용 가능)

## 작업을 다른 프로젝트로 이동하고 복사하면 작업이 프로젝트의 타임라인 내에 맞춰질 수 있을 때 작업 제한이 유지됩니다

작업을 복사하거나 다른 프로젝트로 이동할 때 Workfront에서 작업의 날짜별 작업 제한 사항을 처리하는 방법을 개선했습니다. 날짜별 작업 제한의 예로는 다음과 같아야 함, 다음까지 완료해야 함, 고정 날짜 및 이후에 시작 등이 있습니다.

예를 들어, Must Start On 제약 조건이 있는 작업을 작업의 시작 일자 이전의 계획된 시작 일자가 있는 다른 프로젝트로 이동하거나 복사할 경우 작업은 복사되거나 이동된 후에도 제약 조건을 유지합니다. 작업의 시작 일자 이후 계획된 시작 일자가 있는 프로젝트로 Must Start On 제약 조건이 있는 작업을 이동하거나 복사하면 작업 제한 사항이 가능한 한 빨리 로 변경됩니다.

이 변경 전에 작업 제한 사항은 항상 가능한 한 빨리 로 변경됩니다.

작업 이동에 대한 자세한 내용은 [작업 이동](../../../manage-work/tasks/manage-tasks/move-tasks.md) (또는 Adobe Workfront Classic을 사용하는 경우 다음을 참조하십시오.) [작업 이동](https://one.workfront.com/s/article/Moving-Tasks-2081996259)).

작업 복사에 대한 자세한 내용은 [작업 복사 및 복제](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (또는 Adobe Workfront Classic을 사용하는 경우 다음을 참조하십시오.) [작업 복사 및 복제](https://one.workfront.com/s/article/Copy-and-Duplicate-Tasks-218695605)).

모든 Task Constraints에 대한 개요는 [작업 제한 개요](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (또는 Adobe Workfront Classic을 사용하는 경우 다음을 참조하십시오.) [작업 제한 개요](https://one.workfront.com/s/article/Task-Constraint-Overview-453396848)).

**다음 환경에서 사용할 수 있습니다.**

* Adobe Workfront 클래식
* 새로운 Adobe Workfront 환경

## 세부 정보 탭 또는 작업 목록을 변경하는 동안 데이터 손실 방지

변경 사항을 수동으로 저장할 때 프로젝트 수준의 작업 목록에 있는 객체 또는 작업에 대한 세부 정보 페이지의 정보를 업데이트할 때 데이터 손실을 방지하기 위해 이제 헤더의 정보를 편집하기 전에 저장하지 않은 변경 사항이 있음을 알리는 경고 메시지가 표시됩니다. 변경 사항을 저장하기 전에 허용되는 유일한 작업은 즐겨찾기에 개체를 구독하거나 추가하는 것입니다.

목록에서 작업을 편집하는 방법에 대한 자세한 내용은 [목록에서 작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**다음 환경에서 사용할 수 있습니다.**

* 새로운 Adobe Workfront 환경

## 사용자 지정 상태를 사용하여 그룹에 대한 승인 프로세스 만들기

이제 승인 프로세스에서 그룹별 사용자 지정 상태를 사용하여 그룹이 고유한 워크플로우를 더 쉽게 관리할 수 있습니다.

이전에는 그룹이 그룹별 승인 프로세스에서 자신의 사용자 지정 상태를 사용할 수 없었습니다. 시스템 전체 상태만 사용할 수 있었고 이것이 그룹 승인 프로세스에 항상 맞는 것은 아닙니다.

이제 사용자 지정 상태를 일회용 및 시스템 전체 승인 프로세스 모두에서 사용할 수 있습니다.

* 오브젝트(프로젝트, 작업 또는 문제)에 대한 단일 사용 승인 프로세스를 만들고 해당 오브젝트에서 작업 중인 그룹과 관련된 상태를 기반으로 합니다. 여기에는 그룹과 관련된 모든 사용자 지정 상태가 포함됩니다.
* 글로벌 승인 프로세스를 만들고 그룹 또는 시스템의 모든 사용자에 대해서만 사용할 수 있도록 합니다.

승인 프로세스에 대한 관리 액세스 권한이 있는 사용자는에서 승인 프로세스 구성에 대한 정보를 사용할 수 있습니다. [작업 항목에 대한 승인 프로세스 만들기](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (또는 Adobe Workfront Classic을 사용하는 경우 다음을 참조하십시오.) [승인 프로세스 만들기](https://one.workfront.com/s/article/Creating-Approval-Processes-1001577410)).

사용자의 경우 승인 프로세스를 작업 항목과 연관시키는 방법에 대한 정보는에서 사용할 수 있습니다. [신규 또는 기존 승인 프로세스를 작업과 연결](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (또는 Adobe Workfront Classic을 사용하는 경우 다음을 참조하십시오.) [신규 또는 기존 승인 프로세스를 작업과 연결](https://one.workfront.com/s/article/Associating-a-New-or-Existing-Approval-Process-with-Work-708455630)).

**다음 환경에서 사용할 수 있습니다.**

* Adobe Workfront 클래식
* 새로운 Adobe Workfront 환경

## 업무 균형자에서 할당을 보다 편리하게 업데이트할 수 있는 방법

업무 균형자에서 작업 항목에 대한 사용자의 할당을 보다 편리하게 관리하려면 이제 작업 항목을 두 번 클릭합니다. 기존 할당 편집 메뉴 옵션을 계속 사용할 수도 있습니다. 또한 할당을 업데이트하기 위해 더 이상 할당 표시를 활성화할 필요가 없습니다.

업무 균형자에서 할당을 관리하는 방법에 대한 자세한 내용은 [업무 균형자에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## 업무 균형자에서 작업 계획 시간 업데이트

>[!NOTE]
>
>이 개선 사항은 2020.2 릴리스 직후 프로덕션에서 사용할 수 있습니다.

이제 액세스 수준의 리소스 관리 영역에 있는 새 옵션을 사용하여 이 액세스 권한이 있는 사용자가 업무 균형자에서 계획된 시간을 편집할 수 있습니다. 업무 균형자에서 할당을 조정할 때 일일 할당의 합계는 작업의 계획된 시간 수와 일치하지 않아도 됩니다. 할당을 저장하면 총 할당 시간이 작업의 계획된 시간이 됩니다. 단순 기간 유형이 있는 작업에만 가능합니다.

업무 균형자에서 할당을 관리하는 방법에 대한 자세한 내용은 [업무 균형자에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

리소스 관리에 대한 액세스 권한 부여에 대한 자세한 내용은 [리소스 관리에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## 업무 균형자에서 &quot;베타&quot; 레이블 제거

2020.2 릴리스에서는 업무 균형자 가 더 이상 베타 상태가 아니며 리소스 균형자 를 사용하여 리소스 할당 및 할당을 검토하고 관리할 수 있습니다. &quot;베타&quot; 레이블이 미리보기 환경에서 제거되었습니다. 이 변경 사항은 20.2 프로덕션 릴리스에서도 동일하게 적용됩니다. 업무 균형자에 대한 자세한 내용은 [업무 균형자 개요](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
