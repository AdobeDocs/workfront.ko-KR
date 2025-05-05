---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 3 릴리스 활동
description: 이 페이지에서는 2018.1 Beta 3 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 기능은 2018년 1월 7일에 미리보기 환경에서 사용할 수 있습니다. 2018년 초에 프로덕션 환경에서 사용할 수 있습니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 26bbc4a0-e5ed-4b5f-bfc2-f888362c1d22
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 0%

---

# 2018.1 Beta 3 릴리스 활동

이 페이지에서는 2018.1 Beta 3 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 기능은 2018년 1월 7일에 미리보기 환경에서 사용할 수 있습니다. 2018년 초에 프로덕션 환경에서 사용할 수 있습니다.

>[!IMPORTANT]
>
> 이 페이지에 설명된 기능은 프로덕션 환경에서 사용하기 전에 변경될 수 있습니다.

2018.1의 모든 변경 사항 목록은 다음을 참조하십시오.  [2018.1 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

2018.1 Beta 3 릴리스에는 Workfront 관리자와 기타 사용자 모두를 위한 개선 사항이 포함되어 있습니다.

관리자용 **1&rbrace;**

* [그룹 관리자 개선 사항](#group-administrator-improvements)

**모든 사용자용**

* [HTML5 증명 뷰어 개선 사항](#html5-proofing-viewer-improvements)
* [Workfront의 증명 개선 사항](#proofing-improvements-within-workfront)
* [홈 영역 개선](#home-area-improvements) 
* [애자일 개선 사항](#agile-improvements)
* [간트 차트 개선 사항](#gantt-chart-improvements)
* [리소스 플래너 개선 사항](#resource-planner-improvements)

## 그룹 관리자 개선 사항 {#group-administrator-improvements}

* [그룹 관리자에 대해 암호 재설정 UI가 업데이트됨](#reset-password-ui-updated-for-group-administrators)
* [그룹 관리자를 위한 액세스 수준 설정 옵션](#access-level-setup-options-for-group-administrators)
* [그룹에 대한 타임시트 프로필 만들기](#create-timesheet-profiles-for-groups)
* [그룹 관리자로서 사용자에 대한 삭제된 항목 복구](#recover-deleted-items-for-users-as-a-group-administrator)

### 암호 재설정 UI가 그룹 관리자에 대해 업데이트됨 {#reset-password-ui-updated-for-group-administrators}

그룹 관리자는 다른 사용자의 비밀번호를 재설정할 때 자신의 비밀번호를 변경하라는 메시지가 표시됩니다. 이 기능을 반영하도록 UI가 업데이트되었습니다. 이 변경 전에 UI에 Workfront 관리자 암호가 필요하다는 메시지가 표시되었습니다.

다른 사용자의 암호 재설정에 대한 자세한 내용은 [사용자 프로필 편집](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하세요.

그룹 관리자의 기능에 대한 자세한 내용은 [그룹 만들기](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)의 &quot;그룹 관리자의 기능&quot; 섹션을 참조하십시오.

### 그룹 관리자를 위한 액세스 수준 설정 옵션 {#access-level-setup-options-for-group-administrators}

이제 Workfront 관리자는 그룹 관리자가 다른 사용자로 로그인할 수 있는지 여부 또는 다른 사용자의 암호를 재설정할 수 있는지 여부를 제어할 수 있습니다. 이 액세스를 활성화하거나 비활성화하기 위해 액세스 수준에 새 설정을 추가했습니다. 이 변경 이전에는 모든 그룹 관리자가 다른 사용자로 로그인하여 기본적으로 다른 사용자의 암호를 재설정할 수 있었습니다. 이 변경 사항은 플래너 액세스 수준에만 영향을 줍니다.

사용자의 액세스 수준을 구성하는 방법에 대한 자세한 내용은 [사용자에게 액세스 권한 부여](../../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)를 참조하십시오.

그룹 관리자의 기능에 대한 자세한 내용은 [그룹 만들기](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)의 &quot;그룹 관리자의 기능&quot; 섹션을 참조하십시오.

### 그룹에 대한 타임시트 프로필 만들기 {#create-timesheet-profiles-for-groups}

이제 그룹 관리자는 관리하는 그룹에 대한 타임시트 프로필을 만들고 관리하는 그룹 또는 이러한 그룹의 사용자와 연결할 수 있습니다. 타임시트 프로필은 타임시트와 연계된 사용자에 대해 타임시트가 자동으로 생성되도록 합니다.

이 변경 이전에는 Workfront 관리자만 타임시트 프로필을 만들 수 있었습니다.

타임시트 프로필 만들기에 대한 자세한 내용은 [타임시트 프로필 만들기, 편집 및 할당](../../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)을 참조하세요.

그룹 관리자의 기능에 대한 자세한 내용은 [그룹 만들기](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)의 &quot;그룹 관리자의 기능&quot; 섹션을 참조하십시오.

### 그룹 관리자로서 사용자에 대한 삭제된 항목 복구 {#recover-deleted-items-for-users-as-a-group-administrator}

프로젝트가 그룹 관리자인 그룹과 연결되어 있는 경우 프로젝트 또는 삭제된 작업, 문제 또는 문서를 휴지통에서 복구할 수 있습니다. 이 변경 이전에는 Workfront 관리자만 휴지통에서 항목을 복구할 수 있었습니다.

Workfront에서 삭제된 항목을 복구하는 방법에 대한 자세한 내용은 [삭제된 항목 복원](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)을 참조하십시오.

그룹 관리자의 기능에 대한 자세한 내용은 [그룹 만들기](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)의 &quot;그룹 관리자의 기능&quot; 섹션을 참조하십시오. 

## HTML5 증명 뷰어 개선 사항  {#html5-proofing-viewer-improvements}

* [비교 모드](#compare-mode)
* [댓글 목록 필터링](#filter-the-comment-list)
* [첫 번째 문자를 입력한 후 주석 목록이 검색됩니다.](#comment-list-is-searched-after-the-first-character-is-entered)

### 비교 모드 {#compare-mode}

이제 정적 및 비디오 증명을 볼 때 HTML5 증명 뷰어에서 비교 모드를 사용할 수 있습니다. 

HTML5 증명 뷰어의 비교 모드는 기존 증명 뷰어와 다음과 같은 점에서 다릅니다.

* 비교 모드를 실행하면 새 버전이 오른쪽으로 이동하고 비교하려는 버전이 왼쪽에 열립니다.

  이전에는, 새 버전이 오른쪽에 있는 오프닝과 비교하는 버전과 함께 왼쪽으로 이동했습니다.

* 증명 뷰어에서 직접 비교할 증명 버전을 선택할 수 있습니다. 
* 동시 탐색을 입력할 때 증명 뷰어 내에서 증명의 현재 확대/축소 레벨 및 위치가 유지됩니다.
* 동시 탐색 사용 시 새로운 재설정 옵션
* 비교 모드를 종료하는 경우 닫을 증명을 선택할 수 있습니다. 

  이전에는 이전 버전이 항상 닫혀 있었습니다.

* 다양한 모양과 느낌, 사용성이 개선되었습니다.

자세한 내용은 [증명 뷰어에서 증명 비교](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/compare-proofs.md)를 참조하십시오.

### 주석 목록 필터링 {#filter-the-comment-list}

이제 주석 목록에서 주석을 필터링할 수 있습니다. 사용자, 작업, 읽지 않음 등을 기준으로 필터링할 수 있습니다.

### 첫 번째 문자를 입력한 후 주석 목록이 검색됩니다. {#comment-list-is-searched-after-the-first-character-is-entered}

이제 댓글 목록을 검색할 때 첫 번째 문자를 입력한 후 목록이 자동으로 필터링됩니다.

이 변경 이전에는 주석 목록이 필터링되기 전에 검색 필드에 최소 3자를 입력해야 했습니다.

자세한 내용은에서 를 참조하십시오.

## Workfront의 증명 개선 사항 {#proofing-improvements-within-workfront}

* [Workfront Proof에서 Workfront으로 증명 연결](#link-proofs-from-workfront-proof-to-workfront)
* [더 이상 문서에서 증명을 제거할 수 없습니다](#can-no-longer-remove-a-proof-from-a-document)
* [증명을 생성하고 열 때의 모양과 느낌이 업데이트됨](#updated-look-and-feel-when-generating-and-opening-proofs)

### Workfront Proof에서 Workfront으로 증명 연결 {#link-proofs-from-workfront-proof-to-workfront}

이제 Workfront Proof 계정에 이미 존재하는 문서 증명을 Workfront에 연결할 수 있습니다.

이 변경 전에는 Workfront 내의 Workfront Proof에 이미 존재하는 증명에 액세스할 수 없었습니다. 

자세한 내용은 [외부 응용 프로그램에서 문서 연결](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)에서 [외부 응용 프로그램에서 문서 연결](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)을 참조하십시오.

### 더 이상 문서에서 증명을 제거할 수 없음 {#can-no-longer-remove-a-proof-from-a-document}

더 이상 문서에서 증명을 제거할 수 없습니다. 대신 증명을 제거하려면 전체 문서를 삭제해야 합니다.

이 개선 사항을 통해 사용자가 증명 문서의 모든 버전을 실수로 삭제할 위험이 줄어듭니다. 

문서 삭제에 대한 자세한 내용은 [증명 삭제](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md)에서 [증명 삭제](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md)를 참조하십시오.

### 증명을 생성하고 열 때의 모양과 느낌이 업데이트됨 {#updated-look-and-feel-when-generating-and-opening-proofs}

이제 증명이 생성될 때 업데이트된 애니메이션 회전자가 있습니다.

## 홈 영역 개선 {#home-area-improvements}

홈 영역이 다음과 같이 개선되었습니다.

* [홈 영역에서 증명 승인 보기](#view-proof-approvals-from-the-home-area)
* [홈 영역의 항목에 대한 레이아웃 템플릿을 구성할 때 기본 필드가 표시됩니다](#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area)

### 홈 영역에서 증명 승인 보기 {#view-proof-approvals-from-the-home-area}

이제 표준 승인 외에 홈 영역에서 증명 승인을 볼 수 있습니다.

이전에는 Workfront 승인을 볼 수 있었지만 증명에 대한 승인을 볼 수는 없었습니다.  

자세한 내용은 [홈 영역 사용](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md)을 참조하세요.

### 홈 영역의 항목에 대한 레이아웃 템플릿을 구성할 때 기본 필드가 표시됩니다 {#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area}

이전에는 레이아웃 템플릿에서 기본 필드가 표시되지 않았습니다.

자세한 내용은 &quot;레이아웃 템플릿 만들기 및 관리&quot;를 참조하십시오.

## 애자일 개선 사항 {#agile-improvements}

* [작업 또는 문제 세부 정보 페이지에서 직접 반복에 작업 및 문제 추가](#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page)
* [애자일 팀에 대한 스크럼 백로그 및 스토리 보드에 문제 포함](#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team)
* [애자일 팀의 백로그에 그룹화 및 필터 적용](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [빈 반복을 만들고 나중에 업데이트](#create-a-blank-iteration-and-update-it-later)
* [반복을 만들 때 &quot;Focus&quot; 및 &quot;Capacity&quot; 필드가 미리 채워집니다](#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration)

### 작업 또는 문제 세부 정보 페이지에서 직접 반복에 작업 및 문제 추가 {#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page}

이제 애자일 팀에 현재 할당된 작업 및 문제를 작업 또는 문제에서 직접 반복에 추가할 수 있습니다.

이전에는 백로그에서만 반복에 작업을 추가할 수 있었습니다. 

자세한 내용은 [반복 만들기](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)에서 [반복 만들기](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)를 참조하십시오.

### 애자일 팀의 스크럼 백로그 및 스토리 보드에 문제 포함 {#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team}

이제 스크럼 애자일 방법론을 사용할 때 애자일 팀의 백로그에 문제가 기본적으로 포함됩니다(Kanban 방법론을 사용할 때 애자일 팀의 백로그에 문제가 표시되지 않음).

이 변경 이전에는 작업만 백로그에 추가할 수 있었습니다. 문제를 추가하려면 먼저 문제를 작업으로 변환해야 합니다.

백로그에서 문제를 사용하는 방법에 대한 자세한 내용은  [애자일 백로그를 관리합니다](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### 애자일 팀의 백로그에 그룹화 및 필터 적용 {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

이제 애자일 백로그에서 그룹화 및 필터 옵션을 사용할 수 있으므로 그룹화별로 백로그를 구성하고 특정 작업 및 문제를 필터링할 수 있습니다.

이 변경 전에 보기에서 애자일 백로그에 적용할 수 있었습니다.

자세한 내용은  [애자일 백로그 관리](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)  [애자일 백로그를 관리합니다](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### 빈 반복을 만들고 나중에 업데이트 {#create-a-blank-iteration-and-update-it-later}

반복을 만들기 위해 더 이상 작업 또는 문제를 반복에 추가할 필요가 없습니다. 빈 반복을 만들고 나중에 작업 및 문제를 추가할 수 있습니다.

자세한 내용은 [반복 만들기](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)를 참조하십시오.

### 반복을 만들 때 &quot;Focus&quot; 및 &quot;Capacity&quot; 필드가 미리 채워집니다 {#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration}

이제 반복을 만들 때 &quot;포커스&quot; 및 &quot;용량&quot; 필드는 팀이 만든 모든 과거 반복의 평균 값으로 미리 채워집니다. 팀이 과거 반복을 작성하지 않은 경우 이 필드는 0으로 표시됩니다.

이전에는 이러한 필드가 항상 0으로 설정되어 있었습니다.

자세한 내용은 [반복 만들기](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)를 참조하십시오.

## 간트 차트 개선 사항 {#gantt-chart-improvements}

* [간트 차트에서 편집 모드 사용](#enable-edit-mode-in-the-gantt-chart)
* [간트 차트 편집 시 전임 작업 제거](#remove-predecessors-when-editing-the-gantt-chart)

### 간트 차트에서 편집 모드 활성화 {#enable-edit-mode-in-the-gantt-chart}

간트 차트에서 편집 모드를 활성화하면 차트 내의 정보를 변경할 수 있습니다. 이 변경 이전에는 간트 차트에서 정보를 편집할 수 없었습니다. 작업 목록에서 작업 정보만 편집할 수 있습니다.

간트 차트 편집에 대한 자세한 내용은 [작업 목록 간트 차트에서 정보 업데이트](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)를 참조하십시오.

### 간트 차트 편집 시 전임 작업 제거 {#remove-predecessors-when-editing-the-gantt-chart}

이제 간트 차트의 편집 모드를 사용하여 프로젝트의 간트 차트에서 작업 간의 전임 작업 관계를 제거할 수 있습니다. 이 개선 전에 작업 목록 또는 작업 수준에서만 전임 작업 관계를 제거할 수 있습니다.

간트 차트 편집에 대한 자세한 내용은 [작업 목록 간트 차트에서 정보 업데이트](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)를 참조하십시오.

## 리소스 플래너 개선 사항 {#resource-planner-improvements}

* [리소스 플래너에 기간이 없는 예산](#budget-with-zero-duration-in-the-resource-planner)

* [리소스 플래너에 비용별 데이터 표시](#show-data-by-cost-in-the-resource-planner)

### 리소스 플래너의 기간이 0인 예산 {#budget-with-zero-duration-in-the-resource-planner}

>[!NOTE]
>
>이 기능은 미리보기 환경에서 제거되었으며 18.1 릴리스와 함께 릴리스됩니다.

이제 리소스 플래너에서 프로젝트의 기간 내 또는 외부에 있는 모든 날짜에 대한 리소스의 예산을 책정할 수 있습니다. 이 기능이 향상되기 전에는 프로젝트의 시간대 내에 있는 날짜에 대해서만 리소스의 예산을 책정할 수 있었습니다.

리소스 플래너의 리소스 예산 편성에 대한 자세한 내용은 [리소스 플래너 개요](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)의 &quot;리소스 플래너의 리소스 예산 책정&quot; 섹션을 참조하십시오.

### 리소스 플래너에 비용별 데이터 표시 {#show-data-by-cost-in-the-resource-planner}

이제 시간 및 FTE 값 외에도 비용별로 리소스 플래너에 정보를 표시할 수 있습니다. 프로젝트별 보기 또는 역할별 보기에서 리소스 플래너를 볼 때 리소스 플래너에 비용을 표시할 수 있습니다. 사용자별 조회 뷰에서 자원 계획자를 조회할 때 원가를 표시할 수 없습니다.

시간, FTE 또는 비용 값별로 리소스 플래너를 보는 방법에 대한 자세한 내용은 [리소스 플래너 탐색 개요](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md)를 참조하십시오.
