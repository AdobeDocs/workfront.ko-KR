---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 베타 3 릴리스 활동
description: 2017.3 릴리스는 2017년 11월 초에 프로덕션 환경에서 사용할 수 있습니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: dc0cada8-4b9e-40cb-89a5-16f15268b513
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 6%

---

# 2017.3 베타 3 릴리스 활동

2017.3 릴리스는 2017년 11월 초에 프로덕션 환경에서 사용할 수 있습니다.

>[!IMPORTANT]
>
> 이 페이지에 설명된 기능은 프로덕션 환경에서 사용하기 전에 변경될 수 있습니다.

2017.3의 모든 변경 사항 목록은 다음을 참조하십시오.  [2017.3 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

2017.3 베타 3 릴리스에는 모든 사용자를 위한 개선 사항이 포함되어 있습니다.

* [차트 색상 사용자 정의](#customize-chart-colors)
* [프로젝트 복사 시 추가 옵션](#additional-options-when-copying-projects)
* [리소스 플래너 개선 사항: 필터](#resource-planner-improvement-filters)
* [리소스 플래너 개선 사항: &quot;설정&quot; 영역에 문제 시간 표시](#resource-planner-improvement-show-issue-hours-in-the-settings-area)
* [사용자 정의 새로 고침 및 미리보기 샌드박스에 대한 SSO 정보가 새로 고쳐지지 않음](#sso-information-for-the-custom-refresh-and-preview-sandboxes-do-not-refresh)
* [Workfront Proof에 대한 브라우저 지원 요구 사항 업데이트됨](#updated-browser-support-requirements-for-workfront-proof)

## 차트 색상 사용자 정의 {#customize-chart-colors}

이제 차트 요소의 색상을 사용자 정의할 수 있습니다. 이는 보고서의 모든 차트 유형에 적용됩니다. 간트 차트에는 적용되지 않습니다.

이 변경 이전에는 모든 차트의 요소 색상이 기본적으로 Workfront에 의해 선택되었습니다. 차트 색상 사용자 정의에 대한 자세한 내용은 의 &quot;차트 색상 사용자 정의&quot; 섹션을 참조하십시오. [보고서에 차트 추가](../../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

## 프로젝트 복사 시 추가 옵션 {#additional-options-when-copying-projects}

이제 프로젝트를 복사할 때 작업 또는 문제를 복사할 때 사용할 수 있는 옵션과 이제 일치합니다. 복사하는 동안 복사된 프로젝트의 상태를 변경할 수도 있습니다.

이 업데이트 이전에는 복사한 프로젝트를 복사하는 동안 프로젝트의 상태를 변경할 수 없었고, 프로젝트를 복사할 때에는 두 가지 옵션만 사용할 수 있었습니다.

* 작업 및 프로젝트에 대한 할당을 유지하려면
* 작업 및 프로젝트에 대한 진행 상태를 유지하려면

새 기능을 사용하여 이전 옵션이 제거되었으며 프로젝트를 복사할 때 다음과 같은 옵션이 추가되었습니다.

* 할당 지우기
* 재무 정보 지우기
* 진행 상황 지우기
* 승인 프로세스 지우기
* 사용자 정의 데이터 지우기
* 미리 알림 지우기
* 문서 지우기
* 경비 지우기
* 모든 전임 작업 지우기
* 권한 지우기
* 모두 선택

프로젝트 복사와 관련된 새로운 기능에 대한 자세한 내용은 의 &quot;미리보기 환경에서 프로젝트 복사&quot; 섹션을 참조하십시오.   [프로젝트 복사](../../../../manage-work/projects/manage-projects/copy-project.md).

## 리소스 플래너 개선 사항: 필터 {#resource-planner-improvement-filters}

이제 다음 개체를 사용하여 리소스 플래너에 표시되는 정보를 필터링할 수 있습니다.

* Portfolio
* 프로젝트 상태
* 팀
* 작업 역할
* 리소스 풀

이러한 개체를 기반으로 사용자 지정 필터를 추가할 수도 있습니다.

리소스 플래너 사용에 대한 자세한 내용은 [리소스 플래너 개요](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md). 

## 리소스 플래너 개선 사항: &quot;설정&quot; 영역에 문제 시간 표시 {#resource-planner-improvement-show-issue-hours-in-the-settings-area}

리소스 플래너에는 리소스 플래너를 사용자 지정하는 몇 가지 옵션이 표시되는 새 설정 영역이 있습니다. 이번 릴리스에서는 리소스 플래너의 계획된 시간 열에 문제의 계획된 시간을 포함하는 첫 번째 옵션을 추가했습니다.

리소스 플래너 사용에 대한 자세한 내용은 [리소스 플래너 개요](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## 사용자 정의 새로 고침 및 미리보기 샌드박스에 대한 SSO 정보가 새로 고쳐지지 않음 {#sso-information-for-the-custom-refresh-and-preview-sandboxes-do-not-refresh}

이 릴리스부터 사용자 정의 새로 고침 및 미리보기 샌드박스를 새로 고칠 때 SSO 정보가 프로덕션 환경에서 복사되거나 비활성화되지 않습니다. 이 변경 이전에는 사용자 정의 새로 고침 및 미리보기 샌드박스의 SSO 정보가 비활성화되어 &quot;없음&quot;으로 설정되었습니다.

사용자 지정 새로 고침 샌드박스 환경에 대한 자세한 내용은 [Adobe Workfront 사용자 지정 새로 고침 샌드박스 환경](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

미리보기 샌드박스 환경에 대한 자세한 내용은 [Adobe Workfront 미리보기 샌드박스 환경](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

## Workfront Proof에 대한 브라우저 지원 요구 사항 업데이트됨 {#updated-browser-support-requirements-for-workfront-proof}

Workfront Proof에 대한 브라우저 지원 요구 사항이 업데이트되었습니다. 자세한 내용은 [Adobe Workfront 브라우저 요구 사항](../../../../workfront-basics/workfront-browser-requirements.md).
