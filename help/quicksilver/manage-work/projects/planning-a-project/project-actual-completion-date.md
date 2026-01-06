---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 프로젝트 실제 완료 일자 개요
description: 프로젝트, 작업 및 문제의 Adobe Workfront 실제 완료 일자는 다음과 같습니다. 프로젝트, 작업 또는 문제가 완료된 것으로 표시된 날짜입니다.
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# 프로젝트 실제 완료 일자 개요

프로젝트, 작업 및 문제의 Adobe Workfront 실제 완료 일자는 다음과 같습니다. 프로젝트, 작업 또는 문제가 완료된 것으로 표시된 날짜입니다.

## 실제 완료 일자

실제 완료 일자는 작업이 완료된 실제 일자와 시간을 나타냅니다. 작업 또는 문제가 완료 또는 완료로 표시되면 Workfront은 항목의 상태 변경 일자를 작업 또는 문제의 실제 완료 일자로 자동 설정합니다. 작업 또는 문제가 실제로 완료된 날짜가 해당 날짜에 정확하게 반영되지 않은 경우 실제 완료 날짜를 수동으로 편집할 수 있습니다.

예를 들어 작업 또는 문제를 월요일에 완료됨으로 표시할 수 있지만 작업이 이전 금요일에 완료된 것으로 알고 있습니다. 작업 또는 문제를 완료로 표시한 후 실제 완료를 반영하기 위해 작업 또는 문제의 실제 완료 일자를 이전 금요일의 일자로 수동으로 업데이트할 수 있습니다.

프로젝트의 실제 완료 일자를 수동으로 편집할 수는 없지만, 실제 완료 일자에 대한 변경을 트리거할 수 있는 프로젝트의 상태를 수동으로 변경할 수는 있습니다.

프로젝트의 실제 완료 일자는 다음과 같은 방법으로 설정됩니다.

* 프로젝트 상태 수동 업데이트: 프로젝트의 완료 모드가 수동으로 설정되어 있고 프로젝트의 상태를 완료로 수동으로 변경하면 프로젝트의 실제 완료 일자가 마지막으로 완료된 작업의 날짜 및 시간으로 업데이트됩니다.
* 자동으로, 프로젝트의 마지막 작업이 완료될 때: 프로젝트의 완료 모드가 자동으로 설정되어 있고 마지막 작업을 완료로 표시하거나 마지막 작업의 실제 완료 일자를 갱신할 경우 프로젝트의 실제 완료 일자도 해당 일자로 업데이트됩니다.

  프로젝트의 완료 모드 설정에 대한 자세한 내용은 문서 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md)을 참조하세요.

  >[!NOTE]
  >
  >Workfront은 마지막으로 완료된 프로젝트 작업의 실제 완료 일자를 전체 프로젝트의 실제 완료 일자로 사용합니다.

Workfront 또는 그룹 관리자는 작업 또는 문제가 완료 또는 마감으로 설정된 경우 Workfront에서 오늘 일자를 사용할지 또는 계획된 완료 일자를 사용할지 여부를 결정합니다. 작업 및 문제 환경 설정 지정에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)을 참조하십시오.

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## 실제 완료 일자 찾기

실제 완료 일자는 Workfront의 다음 영역에 있습니다.

* 프로젝트, 작업 및 문제 세부 정보 영역
* 프로젝트, 작업 및 문제 상자 편집
* 시스템 업데이트로 프로젝트, 작업 및 문제 업데이트 영역.
* 프로젝트, 작업 또는 문제 목록이나 보고서.

보고서 만들기에 대한 자세한 내용은 문서 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.
