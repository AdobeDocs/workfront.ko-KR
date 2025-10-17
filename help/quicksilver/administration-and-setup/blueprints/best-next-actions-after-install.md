---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 블루프린트 설치 후 수행할 작업
description: 이 문서에서는  [!DNL Adobe Workfront] 에 블루프린트를 설치한 후 시스템 사용자에게 블루프린트를 완전히 배포하기 위해 수행해야 하는 작업에 대해 간략히 설명합니다.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 0%

---

# 블루프린트 설치 후 수행할 작업

이 문서에서는 [!DNL Adobe Workfront]에 블루프린트를 설치한 후 시스템 사용자에게 블루프린트를 완전히 배포해야 하는 작업에 대해 간략하게 설명합니다.

* [프로젝트 템플릿 권장 사항](#project-template-recommendations)
* [조직 구조 권장 사항](#organizational-structure-recommendations)
* [대시보드 추천](#dashboard-recommendations)

## 프로젝트 템플릿 권장 사항 {#project-template-recommendations}

이 섹션에는 블루프린트와 함께 설치된 프로젝트 템플릿에 대한 권장 사항이 포함되어 있습니다.

### 새로 생성된 역할 및 팀에 사용자 할당 {#assign-users-to-newly-created-roles-and-teams}

블루프린트 설치 프로세스 중에 생성된 역할 및/또는 팀에는 자동으로 연결된 사용자가 없습니다. 새로 추가된 역할이나 팀에 사용자를 할당하지 않으면 아무도 선택하지 않는 기능에 대한 작업을 만듭니다. 경우에 따라 이러한 역할과 팀을 채우기 위해 새 사용자를 만들어야 할 수 있습니다. 새 사용자를 만드는 방법에 대한 자세한 내용은 [사용자 추가](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)를 참조하십시오.

### 템플릿 및 템플릿 작업에 사용자 정의 양식 적용 {#apply-a-custom-form-to-the-template-and-the-template-tasks}

설치 프로세스는 프로젝트 템플릿을 사용자 정의 양식과 연결하지 않습니다. 프로젝트 또는 작업에서 보고 일관성을 만들기 위해 특정 양식이나 필드를 채워야 하거나, 디지털 요청 양식에 프로젝트 수준에서 유지해야 하는 필드가 포함된 경우, 템플릿 또는 템플릿 작업을 해당 양식에 연결하는 것이 좋습니다. 자세한 내용은 [개체에 사용자 정의 양식 추가](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)를 참조하십시오.

### 템플릿 작업 기간 및 작업량 추정치 업데이트 {#update-template-task-duration-and-effort-estimates}

템플릿의 모든 작업에는 계획된 기간 및 계획된 작업량 예측이 포함됩니다. 이러한 예상은 이러한 활동에 대한 기간 및 체류 시간의 시작점 역할을 합니다. 하지만 조직의 기능, 기술 및 속도는 독특합니다. 각 작업의 예상 기간과 노력을 검토하여 조직의 요구 사항을 반영하도록 조정해야 합니다. 자세한 내용은 [작업 세부 정보 개요[!UICONTROL  영역의 ]작업 정보 관리](../../manage-work/tasks/manage-tasks/task-information-in-overview.md)를 참조하십시오.

### 마일스톤 경로 및 마일스톤 연결 {#associate-a-milestone-path-and-milestones}

설치 프로세스는 프로젝트 템플릿을 마일스톤 경로와 연결하지 않습니다. 템플릿에 마일스톤 경로를 적용하고 템플릿의 주요 작업에 마일스톤을 적용하여 마일스톤 보고 요구 사항을 지원합니다. 자세한 내용은 [작업과 마일스톤 연결](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)을 참조하세요.

### 템플릿을 내 팀에 롤아웃 {#roll-out-the-template-to-your-team}

이 템플릿을 사용할 작업 관리자와 프로젝트 템플릿 내에서 작업을 실행할 개별 기여자를 위한 교육 자료를 준비합니다.

### 보고서 및 대시보드 만들기 또는 업데이트 {#create-or-update-reports-and-dashboards}

솔루션이 조직이 이전에 [!DNL Workfront]에서 수행하지 않은 새로운 작업 유형을 나타내는 경우 작업을 지원하기 위해 새 보고서와 대시보드를 만들어야 할 수 있습니다. 자세한 내용은 [사용자 지정 보고서 만들기](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) 및 [대시보드 만들기](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)를 참조하세요.

솔루션이 [!DNL Workfront]에서 이미 실행 중인 작업과 유사한 경우 작업이 예상대로 기존 보고서 및 대시보드에 공급되는지 확인해야 합니다. 기존 보고에 피드되지 않는 경우 필터를 업데이트하거나 새 보고서를 만드는 작업을 수행하십시오.

## 조직 구조 권장 사항 {#organizational-structure-recommendations}

이 섹션에는 블루프린트와 함께 설치된 조직 구조 요소에 대한 권장 사항이 포함되어 있습니다.

### 회사

회사가 포함된 블루프린트를 설치한 후:

* 사용자 정의 양식을 추가하여 유용한 세부 정보로 회사 레코드를 보강합니다(양식과 해당 세부 정보는 귀하에게 고유함). 자세한 내용은 [개체에 사용자 정의 양식 추가](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)를 참조하십시오.
* 회사가 고객을 대표하는 경우 회사와 연결된 재정의 비율을 검토하십시오. 자세한 내용은 [회사 수준에서 작업 역할 청구 요금 재정의](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)를 참조하십시오.
* 회사가 고객을 대표하고 해당 조직에 고유한 다른 프로젝트 템플릿이 있는 경우 먼저 프로젝트 템플릿을 새로 추가된 회사와 미리 연결합니다. 자세한 내용은 [프로젝트 템플릿 편집](../../manage-work/projects/create-and-manage-templates/edit-templates.md)을 참조하십시오.
* 회사가 고객이나 공급업체를 대표하는 경우 해당 환경에 이미 속해 있을 수 있는 외부 조직의 기존 사용자를 연결합니다. 자세한 내용은 [회사 만들기 및 편집](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)을 참조하세요.
* 회사가 고객이나 공급업체를 대표하는 경우 커뮤니케이션, 작업 실행 및 승인을 간소화하는 데 필요한 외부 조직을 위한 추가 공동 작업자 사용자를 만듭니다. 새 사용자를 만드는 방법에 대한 자세한 내용은 [사용자 추가](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)를 참조하십시오.
* 새로 추가된 회사와 연결된 사용자의 조직 차트 관계를 업데이트합니다. 자세한 내용은 [부하 직원 만들기](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) 및 [조직도 보기](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md)를 참조하세요.

회사에 대한 자세한 내용은 [회사 만들기 및 편집](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)을 참조하세요.

## 대시보드 추천 {#dashboard-recommendations}

이 섹션에는 블루프린트와 함께 설치된 대시보드 및 보고서에 대한 권장 사항이 포함되어 있습니다.

### 새로 생성된 대시보드를 업데이트하여 보고서 추가/제거

블루프린트에서 추가된 대시보드에는 하나 이상의 보고서, 외부 페이지 또는 달력이 있습니다. 모든 보고서 및 기타 대시보드 요소가 필요하지 않거나 대시보드를 다른 사용자와 공유할 준비를 하기 전에 기존 보고서, 외부 페이지 및 달력으로 보강해야 할 수 있습니다. 자세한 내용은 [대시보드에 보고서 추가](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md)를 참조하십시오.

### 새로 생성된 보고서를 업데이트하여 열 또는 필터 조건 추가/제거

대시보드 블루프린트를 통해 배포된 보고서에 [!DNL Workfront]의 구성을 지원하는 일부 열 또는 필터 기준이 없습니다. 귀하의 표준에 맞게 보고서를 조정할 것으로 예상됩니다. 환경의 다른 보고서와의 일관성을 구축하기 위해 나열되는 개체의 모든 보고서에 포함하는 열을 추가하거나 결과를 특정 프로젝트 유형 또는 사용자 그룹으로 제한하는 일부 필터 기준을 추가할 수 있습니다. 자세한 내용은 [보기 만들기 또는 편집](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) 및 [필터 만들기 또는 편집](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md)을 참조하세요.

### 사용자와 대시보드 또는 보고서 공유

레이아웃 템플릿에 대시보드를 배치할 계획이 없는 경우 대시보드를 유용하게 사용할 수 있는 사용자와 공유해야 합니다. 자세한 내용은 [대시보드 공유](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) 및 [보고서 공유](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)를 참조하세요.

### 레이아웃 템플릿에 대시보드 추가

다른 사람이 정보를 사용할 수 있도록 하는 가장 좋은 방법은 레이아웃 템플릿에 대시보드를 추가하는 것입니다. 정기적으로 대시보드를 검토함으로써 가장 많은 이점을 얻을 수 있는 사람의 레이아웃 템플릿을 식별하고 새로 만든 대시보드를 해당 레이아웃 템플릿에 추가합니다. 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)를 참조하십시오.

### 다른 대시보드 및 보고서 업데이트

새 대시보드 및 해당 보고서를 도입하면 사용 중단 및 기존의 다른 대시보드 및 보고서를 조정할 수 있습니다. 시간을 내어 기존 보고서를 검토하여 중복되고 모순되는 보고서를 식별하십시오.

### 관련 양식에 사용자 정의 데이터 배포

대시보드 블루프린트에 포함된 일부 보고서에는 보고서의 보기, 필터 또는 그룹화에 사용자 정의 데이터 필드가 있습니다. 경우에 따라 블루프린트는 이러한 필드와 연결된 양식도 갖습니다. 하지만 대부분의 경우 사용자 정의 필드는 사용자 정의 양식에 적용되지 않습니다. 열, 필터 또는 그룹화가 올바르게 작동하려면 이러한 필드를 사용자, 프로젝트, 작업 또는 기타 개체 레코드에 연결된 양식과 연결해야 합니다. 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.
