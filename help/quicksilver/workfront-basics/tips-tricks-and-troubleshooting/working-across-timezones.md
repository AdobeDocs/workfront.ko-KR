---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 시간대 작업
description: 이렇게 하면 [!DNL Adobe Workfront] 시간대를 사용하여 다음 - EDIT ME를 계산합니다.
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 0%

---

# 시간대 작업

이렇게 하면 [!DNL Adobe Workfront] 시간대를 사용하여 다음을 계산합니다.

* 개체의 시간 필드
* 기타 시간 [!DNL Workfront] 자동화된 Workfront 이메일과 같은 영역

## 의 시간대 [!DNL Workfront]

몇 시에 [!DNL Workfront] 는 조직의 표준 시간대 구성을 기반으로 합니다 [!DNL Workfront] 인스턴스 및 사용자 프로필에 대해 사용할 수 있습니다. 이러한 두 시간대가 서로 다른 경우 에서는 사용하는 다양한 영역과 기능에서 시간 불일치가 표시될 수 있습니다 [!DNL Workfront].

>[!NOTE]
>
><div class="preview">개체에 첨부된 사용자 지정 양식에서는 조직의 인스턴스 및 사용자 프로필에 대해 설정된 시간대 구성이 아니라 계산된 사용자 지정 필드의 날짜 및 시간 문이 UTC(Coordinated Universal Time)로 계산되어 저장됩니다. 사용자 지정 양식의 계산은 각 사용자의 개별 시간대를 기반으로 하여 생성되고 표시됩니다.</div>




* [조직의 [!DNL Workfront] 인스턴스](#your-organization-s-workfront-instance)
* [사용자 프로필](#your-user-profile)

### 조직의 [!DNL Workfront] 인스턴스 {#your-organization-s-workfront-instance}

조직의 표준 시간대 [!DNL Workfront] 인스턴스는 일반적으로 주 사무실 위치에 대해 설정됩니다. 이에 따라 다음 내용이 결정됩니다.

* 생성된 이메일에 표시된 시간 [!DNL Workfront]
* 새로 추가된 사용자의 시간대입니다(이전). [!DNL Workfront] 관리자는 작업 위치에 따라 다른 시간대를 구성합니다.)

   이 두 예제에 대한 자세한 내용은 [시스템에 대한 기본 정보 구성](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* 프로젝트에 대한 대체 청구 비율의 시작 또는 종료. 자세한 내용은 [프로젝트 레벨에서 작업 역할 청구 비율 대체](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### 사용자 프로필 {#your-user-profile}

사용자 프로필의 시간대는 작업 위치에 대해 구성해야 합니다. 이에 따라 다음 내용이 결정됩니다.

* 보내는 데 표시된 시간 [!DNL Workfront] 이메일 메시지
* 시작 및 종료 시간과 같은 작업 중인 개체의 시간

   여러 시간대의 사용자가 객체에 지정되면 [!DNL Workfront] 각 사용자 프로필에 구성된 시간대를 사용하여 관련된 모든 사용자의 개체 시간을 변환합니다.

   **예:** 작업 중인 동부 표준 시간(EST) 영역에서 오후 4시에 시작하도록 작업을 설정하고 태평양 표준 시간(PST) 영역에서 작업하는 사용자에게 할당합니다. 이러한 사용자의 경우 시작 시간이 오후 1시로 표시됩니다. 오후 4시로 표시하면 3시간 늦게 작업을 시작할 것입니다.

   개체 작성자가 개체 시간을 설정할 때 할당자의 시간대의 차이를 기록해 두지 않고 필요한 조정을 하지 않거나, 할당자가 그 차이를 알지 못하는 경우, 모든 사람이 개체 작업을 수행하는 동안 타이밍을 제대로 가져오기가 어려울 수 있습니다.

   **예:** 1일 작업을 오전 9시에 시작하도록 구성하여 작업의 일부 사용자가 PST 영역에서 작업한다는 것을 잊어버립니다. 그들에게, 시작 시간은 오전 6시입니다. 9시(정오에) 전까지 작업을 시작하지 않기 때문에 작업이 시작되고 3시간 늦게 완료됩니다.

사용자 프로필에서 시간대를 구성하는 방법은 [내 설정 구성](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

자세한 내용은 [!DNL Workfront] 관리자(또는 [!UICONTROL 편집] 사용자에 대한 액세스)는 사용자 프로필에서 시간대를 구성할 수 있습니다. [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 사용자가 시간대에 걸쳐 쉽게 작업할 수 있도록 하는 방법

다음과 같은 여러 가지 방법으로 여러 시간대에 걸쳐 사용자가 보다 쉽게 작업할 수 있도록 지원할 수 있습니다.

* [예약 사용](#use-schedules)
* [사용자 지정 양식에서 계산된 시간 필드 사용](#use-calculated-time-fields-in-a-custom-form)
* [사용자 지정 양식의 날짜 필드 대신 텍스트 필드를 사용하십시오](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### 예약 사용 {#use-schedules}

[!DNL Workfront] 관리자는 조직 내 각 시간대에 대해 별도의 일정을 만들어 작업이 언제 어디서나 모든 사용자에 대해 적절하게 예약되도록 합니다. 관리자가 스케줄을 만들면 이를 특정 프로젝트 및 사용자와 연결할 수 있습니다.

* **[!UICONTROL 프로젝트]**: 프로젝트 생성자는 개별 프로젝트에 대한 일정을 선택할 수 있습니다. 이렇게 하면 지정된 사용자의 시간대로 설정된 작업 시간을 기반으로 프로젝트에서 작업 예약이 결정됩니다.
* **[!UICONTROL 사용자]**: A [!DNL Workfront] 관리자(또는 [!UICONTROL 편집] 사용자 액세스)는 사용자 프로필에서 개별 사용자에 대한 일정을 선택할 수 있습니다.

   이 일정은 프로젝트 일정과 다를 수 있습니다. 예를 들어, 어떤 사람이 프로젝트에서 작업을 만들고 아직 아무도 할당하지 않은 경우, 해당 작업에서는 프로젝트 일정을 사용합니다. 사용자가 작업에 할당되면 해당 사용자의 일정을 사용합니다.

   여러 사용자가 작업에 할당되면 시스템 전체 프로젝트 환경 설정에서 구성한 대로 다음 중 하나를 사용합니다.

   * 작업의 기본 소유자 일정에 대한 시간대
   * 프로젝트 일정에 대한 시간대입니다.

   이로 인해 작업 날짜가 변경될 수 있습니다.

   **예:** EST 사용자는 EST 정오(오전 9시 PST)에 시작하도록 예약된 1일 작업에 할당됩니다. EST 사용자는 2시간 작업만 남아 있기 때문에 작업 완료 일자는 다음 작업일로 약 6시간 연장됩니다.

   에 대한 정보 [!UICONTROL 프로젝트 환경 설정] 영역 [!UICONTROL 설정]를 참조하십시오. [시스템 전체 프로젝트 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   프로젝트 또는 사용자에게 일정을 지정하는 방법에 대한 지침은 [예약 만들기](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   예약에 구성된 시간대가 배포 시 미치는 영향에 대한 자세한 내용은 [!UICONTROL 계획 시간] 에서 [!DNL Workload Balancer]를 참조하십시오. [에서 사용자 할당 관리 [!DNL Workload Balancer]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### 사용자 지정 양식에서 계산된 시간 필드 사용 {#use-calculated-time-fields-in-a-custom-form}

여러 도시에서 시간을 표시하는 공항 시계처럼 조직의 사용자에 대한 현재 시간을 표시하는 사용자 지정 양식에 일련의 계산된 사용자 지정 필드를 사용할 수 있습니다. 각 사용자가 일하는 각 시간대에 대해 필드를 만들어 해당 시간대의 시간을 계산할 수 있습니다.

자세한 내용은 [사용자 지정 양식에 계산된 데이터 추가](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)및 섹션 [날짜 및 시간 계산된 사용자 지정 필드](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) 기사 [계산된 데이터 표현식](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### 사용자 지정 양식의 날짜 필드 대신 텍스트 필드를 사용하십시오 {#use-text-fields-instead-of-date-fields-in-a-custom-form}

원하지 않으면 [!DNL Workfront] 다른 시간대에 있는 사용자에 대해 개체에서 구성한 시간 변환하기 위해 날짜 필드가 아닌 개체에 첨부하는 사용자 지정 양식의 텍스트 필드를 사용할 수 있습니다. 이렇게 하면 시간에 프로젝트의 모든 사용자를 입력하는 시간이 표시됩니다.

이 작업을 수행하는 경우, 작업 시작 및 종료 시기를 결정할 수 있도록 양식 사용자에게 시간대와 사용자의 시간대별 차이를 계산하도록 상기시키는 것이 좋습니다. 사용자 지정 양식에 입력하는 지침이나 해당 필드의 도구 설명에 이 정보를 포함할 수 있습니다. 자세한 내용은 [사용자 지정 양식에 사용자 지정 필드 추가](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
