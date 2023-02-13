---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 프로젝트 실제 완료 일자 개요
description: 프로젝트, 작업 및 문제에 Adobe Workfront의 실제 완료 날짜가 있습니다. 프로젝트, 작업 또는 문제가 완료된 것으로 표시된 날짜입니다.
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
source-git-commit: 3a3dc541219706e3f6a4700889db344c110838bb
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# 프로젝트 실제 완료 일자 개요

프로젝트, 작업 및 문제에 Adobe Workfront의 실제 완료 날짜가 있습니다. 프로젝트, 작업 또는 문제가 완료된 것으로 표시된 날짜입니다.

## 실제 완료 날짜

실제 완료 일자는 작업이 완료되는 실제 날짜와 시간을 나타냅니다. 작업 또는 문제가 완료 또는 완료로 표시되면 Workfront에서는 항목의 상태 변경 날짜를 자동으로 작업 또는 문제의 실제 완료 날짜로 설정합니다. 해당 날짜가 작업 또는 문제가 실제로 완료된 시기를 정확하게 반영하지 않은 경우 실제 완료 날짜를 수동으로 편집할 수 있습니다.

예를 들어, 월요일에 수행한 작업이나 문제를 표시할 수 있지만, 이전 금요일에 작업이 완료되었음을 알 수 있습니다. 작업 또는 문제를 완료 로 표시한 후 실제 완료 날짜를 수동으로 업데이트하거나 실제 완료 날짜를 반영하도록 이전 금요일 날짜로 출고할 수 있습니다.

프로젝트의 실제 완료 일자를 수동으로 편집할 수는 없지만 실제 완료 날짜로 변경을 트리거할 수 있는 프로젝트의 상태를 수동으로 변경할 수 있습니다.

프로젝트의 실제 완료 일자는 다음과 같은 방법으로 설정됩니다.

* 프로젝트의 상태를 수동으로 업데이트하여 다음을 수행합니다. 프로젝트의 완료 모드가 수동으로 설정되고 프로젝트의 상태를 완료로 수동으로 변경하면 프로젝트의 실제 완료 날짜가 상태가 변경될 때 날짜 및 시간으로 업데이트됩니다.
* 프로젝트의 마지막 작업이 완료되면 자동으로 다음을 수행합니다. 프로젝트의 완료 모드가 자동으로 설정되어 있고 마지막 작업을 완료로 표시하거나 마지막 작업의 실제 완료 날짜를 갱신하는 경우 프로젝트의 실제 완료 날짜도 해당 날짜로 업데이트됩니다.

   프로젝트의 완료 모드 설정에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

   >[!NOTE]
   >
   >Workfront에서는 전체 프로젝트에 대한 실제 완료 날짜로 마지막으로 완료된 프로젝트의 태스크의 실제 완료 날짜를 사용합니다.

Workfront 또는 그룹 관리자는 Workfront이 오늘 날짜나 작업의 계획된 완료 날짜를 사용하는지 또는 작업이 완료 또는 종료됨으로 설정될 때 문제를 사용하는지 여부를 결정합니다. 작업 및 문제 환경 설정 설정에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## 실제 완료 일자 찾기

실제 완료 날짜는 Workfront의 다음 영역에 있습니다.

* 프로젝트, 작업 및 문제 세부 정보 영역
* 프로젝트, 작업 및 문제 상자 편집
* 프로젝트, 작업 및 문제 업데이트 영역을 시스템 업데이트로 업데이트합니다.
* 프로젝트, 작업, 문제 목록 또는 보고서

보고서 만들기에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
