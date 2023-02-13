---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 블루프린트 설치 후 수행할 작업
description: 이 문서에서는 [!DNL Adobe Workfront] 블루프린트를 시스템 사용자에게 완전히 배포하려면
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# 블루프린트 설치 후 수행할 작업

이 문서에서는 [!DNL Adobe Workfront] 블루프린트를 시스템 사용자에게 완전히 배포하려면

* [프로젝트 템플릿 권장 사항](#project-template-recommendations)
* [조직 구조 권장 사항](#organizational-structure-recommendations)
* [대시보드 권장 사항](#dashboard-recommendations)

## 프로젝트 템플릿 권장 사항 {#project-template-recommendations}

이 섹션에는 Blueprint와 함께 설치된 프로젝트 템플릿에 대한 권장 사항이 포함되어 있습니다.

### 새로 만든 역할 및 팀에 사용자 할당 {#assign-users-to-newly-created-roles-and-teams}

블루프린트 설치 프로세스 중에 만든 역할 및/또는 팀에는 사용자와 자동으로 연결된 사용자가 없습니다. 새로 추가된 역할이나 팀에 사용자를 할당하지 않으면 아무도 선택하지 않는 기능에 대한 작업을 만듭니다. 경우에 따라 이러한 역할 및 팀을 채우기 위해 새 사용자를 만들어야 할 수도 있습니다. 새 사용자 만들기에 대한 내용은 [사용자 추가](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### 템플릿 및 템플릿 작업에 사용자 지정 양식 적용 {#apply-a-custom-form-to-the-template-and-the-template-tasks}

설치 프로세스에서 프로젝트 템플릿을 사용자 지정 양식과 연결하지 않습니다. 프로젝트 또는 작업에 보고 일관성을 만들기 위해 특정 양식 또는 필드를 채워야 하거나 디지털 요청 양식에 프로젝트 수준에서 유지해야 하는 필드가 포함되어 있는 경우 템플릿 또는 템플릿 작업을 해당 양식과 연결하는 것이 좋습니다. 자세한 내용은 [개체에 사용자 지정 양식 추가](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### 템플릿 작업 기간 및 작업 예상 업데이트 {#update-template-task-duration-and-effort-estimates}

템플릿의 모든 작업에는 계획된 기간과 계획된 작업량 추정이 포함됩니다. 이러한 추정은 이러한 활동에 대한 지속 시간 및 체류 시간의 시작점 역할을 합니다. 그러나 조직의 기능, 기술 및 속도는 매우 독특합니다. 각 작업의 예상 기간과 노력을 검토하여 조직의 요구 사항을 반영하도록 조정해야 합니다. 자세한 내용은 [의 작업 정보 관리 [!UICONTROL 작업 세부 사항 개요] 영역](../../manage-work/tasks/manage-tasks/task-information-in-overview.md).

### 이정표 경로 및 이정표 연결 {#associate-a-milestone-path-and-milestones}

설치 프로세스에서 프로젝트 템플릿을 이정표 경로와 연결되지 않습니다. 이정표 보고 요구 사항을 지원하기 위해 템플릿에 이정표 경로를 적용하고 템플릿의 주요 작업에 이정표를 적용합니다. 자세한 내용은 [작업과 이정표 연결](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### 팀에 템플릿 롤아웃 {#roll-out-the-template-to-your-team}

이 템플리트를 사용할 작업 관리자와 프로젝트 템플리트 내에서 작업을 실행할 개별 기여자에 대한 교육 자료를 준비합니다.

### 보고서 및 대시보드 만들기 또는 업데이트 {#create-or-update-reports-and-dashboards}

솔루션에서 이전에 조직에서 수행하지 않은 새로운 유형의 작업을 나타내는 경우 [!DNL Workfront]를 채울 수 있도록 새 보고서와 대시보드를 만들어야 할 수도 있습니다. 자세한 내용은 [사용자 지정 보고서 만들기](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) 및 [대시보드 만들기](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

솔루션이 이미 실행 중인 작업과 유사한 경우 [!DNL Workfront]를 채울 경우 작업 시간이 기존 보고서 및 대시보드로 이동하는지 확인해야 합니다. 기존 보고에 피드되지 않는 경우 작업을 수행하여 필터를 업데이트하거나 새 보고서를 만듭니다.

## 조직 구조 권장 사항 {#organizational-structure-recommendations}

이 섹션에는 블루프린트와 함께 설치된 조직 구조 요소에 대한 권장 사항이 포함되어 있습니다.

### 회사

회사를 포함하는 블루프린트를 설치한 후:

* 사용자 지정 양식을 추가하여 유용한 세부 정보로 회사 레코드를 보강합니다(양식 및 세부 정보는 고유한 경우). 자세한 내용은 [개체에 사용자 지정 양식 추가](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* 회사가 클라이언트를 나타내는 경우 회사와 연관된 무효화 비율을 검토합니다. 자세한 내용은 [회사 레벨에서 직무 역할 청구 비율 대체](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* 회사가 클라이언트를 나타내고, 다른 고유한 조직 프로젝트 템플릿이 있는 경우 먼저 프로젝트 템플릿을 새로 추가된 회사와 사전 연결합니다. 자세한 내용은 [프로젝트 템플릿 편집](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* 회사가 클라이언트 또는 공급업체를 나타내는 경우, 이미 사용자 환경에 있을 수 있는 외부 조직의 기존 사용자를 연결합니다. 자세한 내용은 [회사 만들기 및 편집](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* 회사에서 클라이언트나 공급업체를 나타내는 경우 통신, 작업 실행 및 승인을 간소화하기 위해 사용자 환경에서 필요한 외부 조직에 대해 추가 협력자 사용자를 생성합니다. 새 사용자 만들기에 대한 내용은 [사용자 추가](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* 새로 추가된 회사와 연결된 사용자에 대한 조직 차트 관계를 업데이트합니다. 자세한 내용은 [직접 보고서 만들기](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) 및 [조직도 보기](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

회사에 대한 자세한 내용은 [회사 만들기 및 편집](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## 대시보드 권장 사항 {#dashboard-recommendations}

이 섹션에는 블루프린트와 함께 설치된 대시보드 및 보고서에 대한 권장 사항이 포함되어 있습니다.

### 새로 만든 대시보드를 업데이트하여 보고서 추가/제거

블루프린트에서 추가한 대시보드에는 하나 이상의 보고서, 외부 페이지 또는 달력이 있습니다. 모든 보고서 및 기타 대시보드 요소가 필요하지 않거나 기존 보고서, 외부 페이지 및 달력으로 대시보드를 다른 사용자와 공유할 준비가 되기 전에 늘려야 할 것입니다. 자세한 내용은 [대시보드에 보고서 추가](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

### 열 또는 필터 기준을 추가/제거하도록 새로 만든 보고서를 업데이트합니다

대시보드 블루프린트를 통해 배포되는 보고서에는 [!DNL Workfront]. 귀하의 기준에 맞게 보고서를 일부 조정할 것으로 보입니다. 환경의 다른 보고서와 일관성을 유지하기 위해 나열되는 개체의 모든 보고서에 포함하는 열을 추가하거나 특정 프로젝트 유형 또는 사용자 그룹으로 결과를 제한하는 필터 기준을 추가할 수 있습니다. 자세한 내용은 [보기 만들기 또는 편집](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) 및 [필터 만들기 또는 편집](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

### 사용자와 대시보드 또는 보고서 공유

레이아웃 템플릿에 대시보드를 배치하지 않을 경우 대시보드를 유용하게 사용할 수 있는 사용자와 공유해야 합니다. 자세한 내용은 [대시보드 공유](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) 및 [보고서 공유](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### 레이아웃 템플릿에 대시보드 추가

다른 사람이 정보를 사용할 수 있도록 하는 가장 좋은 방법은 레이아웃 템플릿에 대시보드를 추가하는 것입니다. 정기적으로 대시보드를 검토하여 새로 만든 대시보드를 해당 레이아웃 템플릿에 추가하는 것이 가장 도움이 되는 사용자의 레이아웃 템플릿을 식별합니다. 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### 다른 대시보드 및 보고서 업데이트

새 대시보드 및 해당 보고서를 도입하면 기존의 다른 대시보드 및 보고서를 사용 중지 및 조정할 수 있습니다. 기존 보고서를 검토하여 중복되고 모순되는 보고서를 식별하십시오.

### 관련 양식에 사용자 지정 데이터 배포

대시보드 블루프린트에 포함된 일부 보고서에는 보고서의 보기, 필터 또는 그룹화에 있는 사용자 지정 데이터 필드가 있습니다. 경우에 따라 블루프린트에는 이러한 필드가 연결된 양식도 있습니다. 그러나 사용자 지정 필드는 사용자 지정 양식에 적용되지 않는 경우가 많습니다. 열, 필터 또는 그룹화가 올바르게 작동하려면 이러한 필드를 사용자, 프로젝트, 작업 또는 기타 개체 레코드에 연결된 양식과 연결해야 합니다. 자세한 내용은 [사용자 지정 양식에 사용자 지정 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
